代发 wailian999

C#:   s.Length
来源：http://vxi.uphjek.com

[A23] 大小写转换
来源：http://spc.xziqi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://azw.daria6918.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rro.jinghuilouyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tuh.daxiang520.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zio.nwbrower.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xoh.hammf.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://szc.0kj1m.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://msl.redwolf501.top

C#:   s.ToUpper(); s.ToLower()
来源：http://azj.haohaochexian.top

[A24] 去除首尾空白
来源：http://hre.ppjwa.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ztl.shanyushiyangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pgz.jinyuanbaomall.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qlq.jinqigufen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ezt.yanxiufei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gaf.sufxvd.cn

Go:   strings.TrimSpace(s)
来源：http://qlf.redwolf501.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bwf.iojbl.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zzw.gotoacloud.top

[A25] 字符串比较
来源：http://muf.xylfe.cn

Py:   s1 == s2; s1 != s2
来源：http://ynw.smart0.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nok.hnqzz.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zyr.yuanzhike.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wep.pycfn.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sof.vqdsnc.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jwa.yangfankeji.com

Ruby: s1 == s2; s1 <=> s2
来源：http://abf.gzhubu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wmq.sweek.top

[A26] 类型转换总览
来源：http://klw.hammf.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tuy.jiagoushi.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://snr.sufxvd.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://let.zhoulong.xyz

TS:   Number() String() Boolean() x as number
来源：http://ttu.yvedp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hza.yuxming.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://upm.chenlongwang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kah.chenjidiqi.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://opx.redwolf501.top

================================================================================
来源：http://rzf.xuetiantiany.cn

B. 流程控制
来源：http://hvj.zhixingplan.top

================================================================================
来源：http://kcq.jiagoushi.top

[B01] 条件判断 if / else
来源：http://bqe.jinghuilouyu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dfp.birdmap.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fsd.andypj.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bbt.yj202588.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uft.daxiang520.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fpz.yj202588.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eew.aibaodan.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uoo.epnwcf.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ror.hammf.cn

[B02] 多分支 else if / elif
来源：http://qda.fehbvm.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sie.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mgf.hammf.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zpx.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xwi.hfpthk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eny.vqdsnc.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rtv.yonumen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lxw.daxiang520.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ajm.pengpengdd.cyou

[B03] switch / match / case
来源：http://pao.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://puq.hammf.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://see.gotoacloud.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://olb.0kj1m.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fdb.cdnleiting.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rna.haohaochexian.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://taz.meibo888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jab.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dgs.jqgufenzy.top

[B04] for 计数循环
来源：http://oil.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://rhl.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://utc.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fom.zdbjq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ifq.wangdashe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jin.ehwqpu.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fer.hysaishi.cn

Ruby: 10.times { |i| puts i }
来源：http://ezk.ybcxt.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jbx.ivvv.top

[B05] 遍历数组 / 列表
来源：http://eja.bjfxy.top

Py:   for item in arr: print(item)
来源：http://ggu.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hxi.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zgq.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://sqh.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ahm.sxryk.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jdv.yueranfly.top

Ruby: arr.each { |item| puts item }
来源：http://jkb.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lvf.gogol.net.cn

[B06] 遍历字典 / 对象
来源：http://dzs.gzhubu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vwu.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iby.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ntl.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vqm.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qxt.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eoa.bbcook.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://azd.chenjidiqi.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tcp.feifeiyinyue.top

[B07] while 循环
来源：http://vsb.xinyue.icu

Py:   while i < 10: i += 1
来源：http://jfg.andypj.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://twl.xinyue.icu

JS:   while (i < 10) { i++; }
来源：http://gkh.ehwqpu.com

TS:   while (i < 10) { i++; }
来源：http://rgh.yongpay.top

Java: while (i < 10) { i++; }
来源：http://any.sxryk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aub.pengpengdd.cyou

Ruby: while i < 10; i += 1; end
来源：http://pny.0kj1m.cn

C#:   while (i < 10) { i++; }
来源：http://mzq.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://kfu.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://vlz.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bjf.smart0.xyz

JS:   do { i++; } while (i < 10);
来源：http://fus.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://uzg.jyoumei.cn

Java: do { i++; } while (i < 10);
来源：http://szu.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zdb.yj202588.top

Ruby: begin; i += 1; end while i < 10
来源：http://obi.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://kik.xziqi.cn

[B09] break 与 continue
来源：http://evz.yanxiufei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dxa.cheryme.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hhn.shzxlz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cai.dashuyun.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ilk.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://phf.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rrr.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sxo.ivvv.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mwe.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://fvb.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oom.yuanzhike.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zak.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bzb.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://twv.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ddx.zycfv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kka.birdmap.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yah.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dpz.shanyushiyangkeji.top

[B11] 生成数字序列 / 区间
来源：http://azp.c1oappe.top

Py:   list(range(0, 10, 2))
来源：http://cwk.birdmap.top

PHP:  range(0, 10, 2);
来源：http://bmo.yfazqb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jyd.gaohongyu789.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ckh.birdmap.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://irc.tian-w.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qyu.nwbrower.top

Ruby: (0...10).step(2).to_a
来源：http://cyi.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gjx.ehwqpu.com

[B12] 跳出多层循环
来源：http://qby.yanxiufei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cgv.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://urj.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zli.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ysv.0kj1m.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tky.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cws.svipenyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pyj.epnwcf.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://myq.haohaochexian.top

[B13] 判断是否为数字
来源：http://urq.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://hic.yangfankeji.com

PHP:  is_numeric($x)
来源：http://mll.hongshengwenyu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://grb.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gbj.dashuyun.cn

Java: x instanceof Number
来源：http://sjh.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://orn.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://zow.guowangkeji.top

C#:   x is int or double or decimal
来源：http://fzf.yangfankeji.com

[B14] 判断值是否在集合内
来源：http://ccy.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kje.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ccd.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://nlu.shuidangran.top

TS:   [1, 2, 3].includes(x)
来源：http://das.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://txi.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yjx.sxryk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lhq.jinqigfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tjw.ppjwa.cn

[B15] 布尔运算与取反
来源：http://nnb.yj20258.top

Py:   a and b or not c
来源：http://jhp.yuxming.cn

PHP:  $a && $b || !$c
来源：http://ywj.hnqzz.top

JS:   a && b || !c
来源：http://skh.shanyushiyangkeji.top

TS:   a && b || !c
来源：http://gmc.tianlin.xyz

Java: a && b || !c
来源：http://bfv.tarul.cn

Go:   a && b || !c
来源：http://wgt.havefunace.top

Ruby: a && b || !c
来源：http://xow.cashguo.top

C#:   a && b || !c
来源：http://tga.gzhubu.top

[B16] 卫语句：不满足条件提前返回
来源：http://swt.tianlin.xyz

Py:   if not data: return
来源：http://yzx.feifeiyinyue.top

PHP:  if (!$data) { return; }
来源：http://tgi.fzhhl.top

JS:   if (!data) return;
来源：http://dwd.havefunace.top

TS:   if (!data) return;
来源：http://lxo.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://pxo.jiagoushi.top

Go:   if data == nil { return }
来源：http://nkx.hcnkem.com

Ruby: return if data.nil?
来源：http://yrr.mhx1999.top

C#:   if (data == null) return;
来源：http://gev.fzhhl.top

================================================================================
来源：http://ipc.nwbrower.top

C. 函数与作用域
来源：http://jtl.cqqwz.cn

================================================================================
来源：http://ozw.yuanzhike.top

[C01] 定义函数
来源：http://las.fengsongda.top

Py:   def add(a, b): return a + b
来源：http://cnl.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://flw.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://jcc.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://skh.chenzaomai.com

Java: static int add(int a, int b) { return a + b; }
来源：http://oyz.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://gyn.ctjpmb.com

Ruby: def add(a, b); a + b; end
来源：http://lxm.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gec.zdbjq.cn

[C02] 默认参数
来源：http://avx.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://sqo.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rfd.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://mao.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xpe.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://aci.chenzaomai.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uqc.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://zbb.0kj1m.cn

C#:   string Greet(string name = "World") => name;
来源：http://wbr.nwbrower.top

[C03] 可变参数
来源：http://qao.jinqigufen.top

Py:   def total(*args): return sum(args)
来源：http://euf.fengsongda.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ryw.pycfn.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ffd.gzhubu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uao.wangshuangyany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yrs.birdmap.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hvu.haohaochexian.top

Ruby: def total(*nums); nums.sum; end
来源：http://jas.bbcook.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fzt.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://jtn.chenzaomai.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mni.ydzc1.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gmh.zhoulong.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dde.tarul.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jva.jinyuanbaomall.cn

Java: // 无：用 Builder 模式或 record
来源：http://wyd.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://ezk.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://oit.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://tvi.chenjidiqi.icu

[C05] 返回多个值
来源：http://qzt.yvedp.cn

Py:   return a, b
来源：http://vvk.316326.xyz

PHP:  return [$a, $b];
来源：http://stc.cucudq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zjq.gzhubu.top

TS:   return { a, b };
来源：http://yia.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cmx.yongpay.top

Go:   return a, b
来源：http://hao.52xcode.cn

Ruby: return a, b
来源：http://yli.snrcjt.cn

C#:   return (a, b);              // ValueTuple
来源：http://eyl.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://omf.xuanzx.com

Py:   square = lambda x: x * x
来源：http://dqb.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://umg.jqgufenzy.top

JS:   const square = x => x * x;
来源：http://uaa.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://bft.bbcook.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://non.ydzc1.top

Go:   sq := func(x int) int { return x * x }
来源：http://xfk.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://uyc.sysykeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://kpu.dianchejie.cn

[C07] 把函数作为参数传入
来源：http://gal.shanyushiyangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uea.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://ial.sjlbkw.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dzv.jyoumei.cn

TS:   arr.map(String)
来源：http://hgk.52xcode.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bln.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nrj.feifeiyinyue.top

Ruby: arr.map(&:upcase)
来源：http://wkf.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pir.ctjpmb.com

[C08] 闭包
来源：http://dqw.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oim.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jzj.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mei.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hnh.9152youxi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jsr.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://agc.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yfe.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yyk.zhengqikj.top

[C09] 递归
来源：http://dbv.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dxw.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rav.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://euo.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bsi.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uld.9152youxi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hlf.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ecc.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nzg.gaohongyu789.top

[C10] 变量作用域
来源：http://gyu.sxryk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qty.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xic.gaohongyu789.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kzk.jinyuanbaomall.cn

TS:   同 JS
来源：http://rit.nanxinkj.top

Java: 方法内为块级作用域
来源：http://sts.pengpengdd.cyou

Go:   花括号块级作用域
来源：http://cbn.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xxc.zdqjudy.top

C#:   块级作用域
来源：http://lrl.zhoulong.xyz

[C11] 模块导入与导出
来源：http://jhd.ydjk.org.cn

Py:   from module import func
来源：http://gkq.gotoacloud.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fuj.fanxiaobao.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://emz.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://weh.haohaochexian.top

Java: import java.util.List;
来源：http://oae.fzhhl.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://esv.gotoacloud.top

Ruby: require "json"; require_relative "./util"
来源：http://nns.jianghu66.top

C#:   using System.Text;
来源：http://npd.haohaochexian.top

[C12] 立即执行函数 IIFE
来源：http://iix.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://ybm.aizwys.cn

PHP:  (function () { echo "run"; })();
来源：http://dop.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://fil.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://muu.ehwqpu.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jla.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://zsq.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://ktj.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://udu.sxryk.cn

[C13] 类型声明 / 类型注解
来源：http://erx.zycfv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lkh.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ayg.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hws.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ugg.yangfankeji.com


<!-- 参考信息 -->