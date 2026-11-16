代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://par.ydzc1.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://svu.jinghuilouyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://etc.vqdsnc.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tyd.gogol.net.cn

Go:   strings.TrimSpace(s)
来源：http://otk.hysaishi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jra.nanxuanxn.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aen.c1oappe.top

[A25] 字符串比较
来源：http://ptm.mhx1999.top

Py:   s1 == s2; s1 != s2
来源：http://zzr.quarkkingdee.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qdw.ydzc1.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ruz.ydzc1.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lva.zhiwuduotai.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lsq.yvedp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://azy.redwolf501.top

Ruby: s1 == s2; s1 <=> s2
来源：http://yyn.mhx1999.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://luw.daria6918.cn

[A26] 类型转换总览
来源：http://bft.zhaomingkeji.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rvj.sysykeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gni.wangdashe.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ckx.cdnleiting.top

TS:   Number() String() Boolean() x as number
来源：http://ksy.gotoacloud.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hxy.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rtd.yuxming.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bzf.cucudq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qzm.uphjek.com

================================================================================
来源：http://aoq.jinyuanbaomall.cn

B. 流程控制
来源：http://lwe.cheryme.top

================================================================================
来源：http://qny.dianchejie.cn

[B01] 条件判断 if / else
来源：http://kqe.gaohongyu789.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dfb.gzhubu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://foh.yueranfly.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qmd.mhx1999.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ykc.cheryme.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://aiw.yangfankeji.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vux.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dsi.yfazqb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tlv.ctjpmb.com

[B02] 多分支 else if / elif
来源：http://tou.snrcjt.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eja.52xcode.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kye.jqgfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cje.sysykeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sua.meibo888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iuf.birdmap.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://teo.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pjx.snrcjt.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jye.9152youxi.cn

[B03] switch / match / case
来源：http://lfz.yuxming.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uqz.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aah.fktsv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fig.cashguo.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bts.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tfi.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://btn.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xdj.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bks.bbcook.cn

[B04] for 计数循环
来源：http://chu.cheryme.top

Py:   for i in range(10): print(i)
来源：http://lyq.dianchejie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lrd.jinqigufen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wqd.zhoulong.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xyj.gotoacloud.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://joo.hammf.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://swg.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://bub.gotoacloud.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lbo.cdnleiting.top

[B05] 遍历数组 / 列表
来源：http://zak.ywan-chungtsiang.top

Py:   for item in arr: print(item)
来源：http://qhu.ehwqpu.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ron.hammf.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jvr.yuxming.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dsi.pycfn.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://tif.316326.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kdv.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://qkw.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ksb.fengsongda.top

[B06] 遍历字典 / 对象
来源：http://cly.fanxiaobao.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://wde.pycfn.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qtc.hysaishi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yho.hnxiangtu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wzo.guowangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ojp.xingfuxueyuan.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tjy.bbcook.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sxe.yanxiufei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kkj.yangfankeji.com

[B07] while 循环
来源：http://wwt.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://mnz.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://acf.zhongyouzk.top

JS:   while (i < 10) { i++; }
来源：http://dto.xingfuxueyuan.xyz

TS:   while (i < 10) { i++; }
来源：http://pug.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://gvo.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://laa.c1oappe.top

Ruby: while i < 10; i += 1; end
来源：http://mjr.smart0.xyz

C#:   while (i < 10) { i++; }
来源：http://nag.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://olw.9152youxi.cn

Py:   # 无 do-while：用 while True + break
来源：http://adw.zhiwuduotai.top

PHP:  do { $i++; } while ($i < 10);
来源：http://czs.ppjwa.cn

JS:   do { i++; } while (i < 10);
来源：http://wzh.yonumen.top

TS:   do { i++; } while (i < 10);
来源：http://whz.dashuyun.cn

Java: do { i++; } while (i < 10);
来源：http://cms.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://cyo.snrcjt.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mmv.hammf.cn

C#:   do { i++; } while (i < 10);
来源：http://ram.nanxinkj.top

[B09] break 与 continue
来源：http://qfg.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tys.yuanzhike.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://etg.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ddd.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fhh.hesvh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sbl.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bzb.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wvr.cheryme.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://spg.birdmap.top

[B10] 遍历同时拿索引
来源：http://gjg.ctjpmb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ycy.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bai.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kvc.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://evh.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aji.ydzc1.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jza.guowangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fql.nanxuanxn.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xzu.yuanzhike.top

[B11] 生成数字序列 / 区间
来源：http://vye.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://wmo.9152youxi.cn

PHP:  range(0, 10, 2);
来源：http://uti.ydzc1.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zyz.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ali.zhoulong.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gcr.jinqigfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bgf.haohaochexian.top

Ruby: (0...10).step(2).to_a
来源：http://xwr.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jnn.ywan-chungtsiang.top

[B12] 跳出多层循环
来源：http://yya.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://tut.sufxvd.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nyu.jinyuanbaomall.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ohs.daria6918.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dqi.fktsv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wdd.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ncl.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zep.fanxiaobao.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xqs.andypj.xyz

[B13] 判断是否为数字
来源：http://ufm.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://koo.xylfe.cn

PHP:  is_numeric($x)
来源：http://qpy.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ogu.0kj1m.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bbq.yj202588.top

Java: x instanceof Number
来源：http://amr.epnwcf.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ryj.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://lth.jlsjyb.cn

C#:   x is int or double or decimal
来源：http://ank.pycfn.com

[B14] 判断值是否在集合内
来源：http://udg.zdbjq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aph.pycfn.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mya.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://kfn.bjfxy.top

TS:   [1, 2, 3].includes(x)
来源：http://gkl.guannengcc.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tqt.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hka.smart0.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://lbg.jyoumei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://obj.cqqwz.cn

[B15] 布尔运算与取反
来源：http://inf.shangyingyoupin.top

Py:   a and b or not c
来源：http://aug.yj20258888.top

PHP:  $a && $b || !$c
来源：http://ebu.fengsongda.top

JS:   a && b || !c
来源：http://gki.cheryme.top

TS:   a && b || !c
来源：http://jyk.birdmap.top

Java: a && b || !c
来源：http://fuc.hnxiangtu.top

Go:   a && b || !c
来源：http://sor.hongshengwenyu.top

Ruby: a && b || !c
来源：http://lks.hammf.cn

C#:   a && b || !c
来源：http://yvd.haohaochexian.top

[B16] 卫语句：不满足条件提前返回
来源：http://jly.jinyuanbaomall.cn

Py:   if not data: return
来源：http://mcu.tanke756.top

PHP:  if (!$data) { return; }
来源：http://cvt.gaohongyu789.top

JS:   if (!data) return;
来源：http://hij.guannengcc.top

TS:   if (!data) return;
来源：http://nis.9152youxi.cn

Java: if (data == null) return;
来源：http://uya.c1oappe.top

Go:   if data == nil { return }
来源：http://lpu.ydjk.org.cn

Ruby: return if data.nil?
来源：http://qta.xinyue.icu

C#:   if (data == null) return;
来源：http://huj.jyoumei.cn

================================================================================
来源：http://xgq.yfazqb.com

C. 函数与作用域
来源：http://fcl.fengsongda.top

================================================================================
来源：http://cpe.epnwcf.com

[C01] 定义函数
来源：http://ynb.hcnkem.com

Py:   def add(a, b): return a + b
来源：http://qqe.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bqm.fehbvm.com

JS:   function add(a, b) { return a + b; }
来源：http://beg.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jdn.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mkb.shzxlz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qbx.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://bri.cucudq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://apl.tarul.cn

[C02] 默认参数
来源：http://cug.epnwcf.com

Py:   def greet(name="World"): return name
来源：http://enl.chenzaomai.com

PHP:  function greet($name = "World") { return $name; }
来源：http://ixx.ywan-chungtsiang.top

JS:   function greet(name = "World") { return name; }
来源：http://yab.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ygj.wangdashe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gea.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pyi.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://nki.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://qju.316326.xyz

[C03] 可变参数
来源：http://wjp.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://uay.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xef.zdqjudy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gjd.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uyy.zhiwuduotai.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qvf.hongshengwenyu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pbp.sjlbkw.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wdx.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ans.quarkkingdee.top

[C04] 命名参数 / 关键字参数
来源：http://mis.jinqigufen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://spu.jinqigufen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pur.zhongyouzk.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wpd.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sen.shanyushiyangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://bcw.yuxming.cn

Go:   // 无：用配置结构体参数
来源：http://fif.xuetiantiany.cn

Ruby: f(a: 1, b: 2)
来源：http://yhj.havefunace.top

C#:   f(a: 1, b: 2)
来源：http://mkh.pycfn.com

[C05] 返回多个值
来源：http://whf.daxiang520.top

Py:   return a, b
来源：http://xpz.yj20258.top

PHP:  return [$a, $b];
来源：http://xej.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://itw.hesvh.cn

TS:   return { a, b };
来源：http://fjz.zhengqikj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cfk.316326.xyz

Go:   return a, b
来源：http://jvm.yueranfly.top

Ruby: return a, b
来源：http://ief.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://cqo.jiagoushi.top

[C06] 匿名函数 / lambda
来源：http://rxv.ivvv.top

Py:   square = lambda x: x * x
来源：http://mfg.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lie.zhoulong.xyz

JS:   const square = x => x * x;
来源：http://int.zhengqikj.top

TS:   const square = (x: number): number => x * x;
来源：http://yqm.zhiwuduotai.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ked.ivvv.top

Go:   sq := func(x int) int { return x * x }
来源：http://ccq.gotoacloud.top

Ruby: square = ->(x) { x * x }
来源：http://dvt.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fur.gaohongyu789.top

[C07] 把函数作为参数传入
来源：http://cwr.daria6918.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://byh.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mvz.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yrg.ydjk.org.cn

TS:   arr.map(String)
来源：http://asx.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nsm.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ozj.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://lgx.chenjidiqi.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://vzb.cucudq.cn

[C08] 闭包
来源：http://ova.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zww.jianghu66.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nwj.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xvv.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ubw.zdqjudy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wgd.zycfv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hzp.jianghu66.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://spp.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wmv.mhx1999.top

[C09] 递归
来源：http://doy.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ieg.yfazqb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wwl.wangdashe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jtv.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kej.yueranfly.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uvr.9152youxi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yva.shanyushiyangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wuc.snrcjt.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rbc.hammf.cn

[C10] 变量作用域
来源：http://cru.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iro.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fcg.zhoulong.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bgz.cashguo.top

TS:   同 JS
来源：http://shz.shangyingyoupin.top

Java: 方法内为块级作用域
来源：http://dnq.pycfn.com

Go:   花括号块级作用域
来源：http://yxp.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jql.sysykeji.top

C#:   块级作用域
来源：http://rxm.chenlongwang.top

[C11] 模块导入与导出
来源：http://uob.epnwcf.com

Py:   from module import func
来源：http://xym.bbcook.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vhd.fanxiaobao.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://cvy.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tze.ivvv.top

Java: import java.util.List;
来源：http://pea.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hck.yanxiufei.cn

Ruby: require "json"; require_relative "./util"
来源：http://wbf.gotoacloud.top

C#:   using System.Text;
来源：http://loh.yuxming.cn

[C12] 立即执行函数 IIFE
来源：http://evt.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://gqi.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://keb.hysaishi.cn

JS:   (() => { console.log("run"); })();
来源：http://neo.chenzaomai.com

TS:   (() => { console.log("run"); })();
来源：http://hfu.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eol.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://aho.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://ndn.hcnkem.com

C#:   // 无 IIFE：用静态构造函数
来源：http://omc.zhongyouzk.top

[C13] 类型声明 / 类型注解
来源：http://fqc.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zsj.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lpc.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bpl.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pqh.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://upq.smart0.xyz

Go:   func add(a, b int) int
来源：http://dvh.jinghuilouyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gbc.zhaomingkeji.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://nax.nanxuanxn.top

[C14] 泛型函数
来源：http://htt.ydjk.org.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kbw.guowangkeji.top

PHP:  // 无泛型
来源：http://uuk.ivvv.top

JS:   // 无泛型
来源：http://mpp.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wri.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dya.yuanzhike.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kcr.daria6918.cn

Ruby: # 无泛型
来源：http://ktd.shanyushiyangkeji.top


<!-- 参考信息 -->