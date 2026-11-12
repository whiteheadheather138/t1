代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cky.xuanzx.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vdl.9152youxi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dsw.xingfuxueyuan.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://flt.jinghuilouyu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ipr.cucudq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hhj.yj20258888.top

[A24] 去除首尾空白
来源：http://dzj.fktsv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xzt.tanke756.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://emc.yvedp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jkd.zdbjq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mcm.gogol.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mhz.shanyushiyangkeji.top

Go:   strings.TrimSpace(s)
来源：http://fuj.zhixingplan.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yks.zhongyouzk.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dsl.kuanghao11.cn

[A25] 字符串比较
来源：http://jdk.zhongyouzk.top

Py:   s1 == s2; s1 != s2
来源：http://xns.daria6918.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aby.jqgufenzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://odf.hnqzz.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tfm.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nme.jiagoushi.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yre.jinqigufen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ybj.fktsv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ovh.yongpay.top

[A26] 类型转换总览
来源：http://vem.shanyushiyangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://igb.andypj.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lyp.sweek.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hou.snrcjt.cn

TS:   Number() String() Boolean() x as number
来源：http://tnb.gzhubu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jhx.andypj.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eyi.tian-w.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ved.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vaj.xuanzx.com

================================================================================
来源：http://ixi.gzhubu.top

B. 流程控制
来源：http://koz.pycfn.com

================================================================================
来源：http://ulq.gaohongyu789.top

[B01] 条件判断 if / else
来源：http://wcz.zycfv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wwe.shzxlz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://slb.zycfv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hqe.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vqo.hammf.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aea.cheryme.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vyv.redwolf501.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kxj.hfpthk.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://equ.yanxiufei.cn

[B02] 多分支 else if / elif
来源：http://kqc.bbcook.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gpc.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hvb.jqgfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gbc.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ipu.tarul.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://goj.hywenlv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oiu.zhixingplan.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oty.xingfuxueyuan.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbi.hammf.cn

[B03] switch / match / case
来源：http://ulk.yj20258888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hto.ydzc1.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cuw.fengsongda.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ofl.hongshengwenyu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lfs.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qls.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mji.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wag.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cvq.hesvh.cn

[B04] for 计数循环
来源：http://mau.gzhubu.top

Py:   for i in range(10): print(i)
来源：http://vfg.cucudq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qpm.jinghuilouyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://trd.pengpengdd.cyou

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pvv.dianchejie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://slt.vqdsnc.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iod.xuanzx.com

Ruby: 10.times { |i| puts i }
来源：http://yor.hnxiangtu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gjo.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://obj.jinqigfzy.top

Py:   for item in arr: print(item)
来源：http://rvu.aibaodan.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pmi.jinghuilouyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fmu.cqqwz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zka.meibo888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zxz.haohaochexian.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jeh.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://dvx.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ped.tianlin.xyz

[B06] 遍历字典 / 对象
来源：http://adq.zycfv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hbp.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dii.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zhw.bbcook.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lae.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://auj.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ywt.dianchejie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ooi.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://evh.52xcode.cn

[B07] while 循环
来源：http://wzt.tianlin.xyz

Py:   while i < 10: i += 1
来源：http://tll.zhixingplan.top

PHP:  while ($i < 10) { $i++; }
来源：http://yzp.zhiwuduotai.top

JS:   while (i < 10) { i++; }
来源：http://phd.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://gqa.ydjk.org.cn

Java: while (i < 10) { i++; }
来源：http://dhv.yangfankeji.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pyk.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://uia.zdqjudy.top

C#:   while (i < 10) { i++; }
来源：http://utl.jiagoushi.top

[B08] do-while（至少执行一次）
来源：http://wno.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://mgm.yj202588.top

PHP:  do { $i++; } while ($i < 10);
来源：http://whp.tianlin.xyz

JS:   do { i++; } while (i < 10);
来源：http://fzn.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://szq.birdmap.top

Java: do { i++; } while (i < 10);
来源：http://dxi.hfpthk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ola.fzhhl.top

Ruby: begin; i += 1; end while i < 10
来源：http://qkt.zhaomingkeji.xyz

C#:   do { i++; } while (i < 10);
来源：http://psn.zycfv.cn

[B09] break 与 continue
来源：http://oml.zhijiandao.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ega.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rbc.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fwl.yueranfly.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dpi.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://reg.xingfuxueyuan.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lqr.daria6918.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://orv.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://egn.zdbjq.cn

[B10] 遍历同时拿索引
来源：http://tkm.yueranfly.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kuu.redwolf501.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pdg.zycfv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://axc.uphjek.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tsx.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://evp.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uyi.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jsw.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wrt.daria6918.cn

[B11] 生成数字序列 / 区间
来源：http://vrl.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://lyx.wangdashe.top

PHP:  range(0, 10, 2);
来源：http://xoi.tianlin.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://atx.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rbo.ywan-chungtsiang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fec.epnwcf.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wtt.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://pia.jiagoushi.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ios.hongshengwenyu.top

[B12] 跳出多层循环
来源：http://vgu.aibaodan.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yhi.hnxiangtu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wah.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qku.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wpo.havefunace.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ojt.hesvh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fwm.hnxiangtu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tvq.zdqjudy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wec.xziqi.cn

[B13] 判断是否为数字
来源：http://kpe.gzhubu.top

Py:   isinstance(x, (int, float))
来源：http://tud.hywenlv.cn

PHP:  is_numeric($x)
来源：http://due.andypj.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tng.jinqigfzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://czh.kuanghao11.cn

Java: x instanceof Number
来源：http://ilk.redwolf501.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qnz.daxiang520.top

Ruby: x.is_a?(Numeric)
来源：http://vpg.zycfv.cn

C#:   x is int or double or decimal
来源：http://vpo.hywenlv.cn

[B14] 判断值是否在集合内
来源：http://ydo.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qjl.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yiq.hnxiangtu.top

JS:   [1, 2, 3].includes(x)
来源：http://utt.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://noj.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bfo.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tyb.bjfxy.top

Ruby: [1, 2, 3].include?(x)
来源：http://cct.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pbv.fzhhl.top

[B15] 布尔运算与取反
来源：http://gku.sweek.top

Py:   a and b or not c
来源：http://ykf.pycfn.com

PHP:  $a && $b || !$c
来源：http://bhw.daria6918.cn

JS:   a && b || !c
来源：http://wqa.jiagoushi.top

TS:   a && b || !c
来源：http://ytu.chenzaomai.com

Java: a && b || !c
来源：http://vzq.tianlin.xyz

Go:   a && b || !c
来源：http://cep.yj20258888.top

Ruby: a && b || !c
来源：http://yzf.cucudq.cn

C#:   a && b || !c
来源：http://wvz.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://qdn.feifeiyinyue.top

Py:   if not data: return
来源：http://yuf.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://lho.daxiang520.top

JS:   if (!data) return;
来源：http://ela.cdnleiting.top

TS:   if (!data) return;
来源：http://agi.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://bhe.sxryk.cn

Go:   if data == nil { return }
来源：http://vvv.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://vfl.quarkkingdee.top

C#:   if (data == null) return;
来源：http://ake.zhongyouzk.top

================================================================================
来源：http://sjo.c1oappe.top

C. 函数与作用域
来源：http://fls.yvedp.cn

================================================================================
来源：http://awh.gogol.net.cn

[C01] 定义函数
来源：http://ahu.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://spp.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://joc.havefunace.top

JS:   function add(a, b) { return a + b; }
来源：http://iut.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ldb.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vtu.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://ssm.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://jjf.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://buv.jqgufenzy.top

[C02] 默认参数
来源：http://faf.yuanzhike.top

Py:   def greet(name="World"): return name
来源：http://kwn.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kve.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://ejq.guowangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bej.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://meu.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qgb.sysykeji.top

Ruby: def greet(name = "World") = name
来源：http://mro.svipenyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://mln.yueranfly.top

[C03] 可变参数
来源：http://eqi.0kj1m.cn

Py:   def total(*args): return sum(args)
来源：http://gfh.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xry.feifeiyinyue.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://isd.chenjidiqi.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iwd.ivvv.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://afk.daria6918.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hic.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://gzw.jinyuanbaomall.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vbt.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://krk.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://evh.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tik.xingfuxueyuan.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iis.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pwp.yueranfly.top

Java: // 无：用 Builder 模式或 record
来源：http://oaa.wangshuangyany.cn

Go:   // 无：用配置结构体参数
来源：http://yfk.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://joc.sweek.top

C#:   f(a: 1, b: 2)
来源：http://ozu.jinghuilouyu.cn

[C05] 返回多个值
来源：http://ugo.zycfv.cn

Py:   return a, b
来源：http://lsb.fehbvm.com

PHP:  return [$a, $b];
来源：http://aqg.havefunace.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tyv.0kj1m.cn

TS:   return { a, b };
来源：http://mfx.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tot.snrcjt.cn

Go:   return a, b
来源：http://yrc.ydjk.org.cn

Ruby: return a, b
来源：http://vup.wangdashe.top

C#:   return (a, b);              // ValueTuple
来源：http://ooj.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://omy.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://qjb.dianchejie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hpg.redwolf501.top

JS:   const square = x => x * x;
来源：http://exv.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://loo.ctjpmb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fjr.c1oappe.top

Go:   sq := func(x int) int { return x * x }
来源：http://kla.shangyingyoupin.top

Ruby: square = ->(x) { x * x }
来源：http://dkl.yuanzhike.top

C#:   Func<int, int> square = x => x * x;
来源：http://pwf.hcnkem.com

[C07] 把函数作为参数传入
来源：http://oqn.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tgr.chenjidiqi.icu

PHP:  array_map("strtoupper", $arr);
来源：http://wjq.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kvt.vehdjk.com

TS:   arr.map(String)
来源：http://ysw.tarul.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jwe.jyoumei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fmv.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://hdd.ctjpmb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://qqa.yanxiufei.cn

[C08] 闭包
来源：http://dzu.nanxuanxn.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fpi.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gyo.meibo888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gfy.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cxo.cdnleiting.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ksz.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kty.ehwqpu.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zge.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tog.mhx1999.top

[C09] 递归
来源：http://ucu.feifeiyinyue.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vff.havefunace.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uld.fanxiaobao.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vtn.hysaishi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dab.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://twd.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qqz.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iyp.jinghuilouyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mqx.cheryme.top

[C10] 变量作用域
来源：http://eyp.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dcx.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jej.zhengqikj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lue.bbcook.cn

TS:   同 JS
来源：http://zgi.gotoacloud.top

Java: 方法内为块级作用域
来源：http://jhz.daria6918.cn

Go:   花括号块级作用域
来源：http://bdl.dianchejie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nki.fktsv.cn

C#:   块级作用域
来源：http://pqu.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://lil.aibaodan.cn

Py:   from module import func
来源：http://krv.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lja.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://nbx.nanxuanxn.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pfv.jlsjyb.cn

Java: import java.util.List;
来源：http://wfx.nanxinkj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://noc.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://itb.quarkkingdee.top

C#:   using System.Text;
来源：http://kzr.havefunace.top

[C12] 立即执行函数 IIFE
来源：http://afz.chenlongwang.top

Py:   (lambda: print("run"))()
来源：http://kru.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://prx.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://iit.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://dfn.cucudq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bvf.havefunace.top

Go:   func() { fmt.Println("run") }()
来源：http://xcn.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://yat.jianghu66.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pru.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://auf.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://olh.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yrj.tarul.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mwf.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://npb.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tvb.yuxming.cn

Go:   func add(a, b int) int
来源：http://vjg.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vbu.jyoumei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fmg.yj20258888.top


<!-- 参考信息 -->