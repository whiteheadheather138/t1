代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://okr.daria6918.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zuv.pycfn.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kwe.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lbb.hfpthk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fdh.mhx1999.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gqj.jqgufenzy.top

[A24] 去除首尾空白
来源：http://xyt.nanxuanxn.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xpq.guowangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sul.snrcjt.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tbn.316326.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vdt.hysaishi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://imc.yanxiufei.cn

Go:   strings.TrimSpace(s)
来源：http://hhv.xylfe.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xoh.ppjwa.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qfn.jinqigufen.top

[A25] 字符串比较
来源：http://rvo.smart0.xyz

Py:   s1 == s2; s1 != s2
来源：http://jqy.jiagoushi.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pux.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eht.sxryk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zrc.jqgufenzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zdc.cheryme.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jqz.bbcook.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://loy.cashguo.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tlc.yangfankeji.com

[A26] 类型转换总览
来源：http://vnb.yueranfly.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ikg.hfpthk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pzd.cheryme.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tfl.jyoumei.cn

TS:   Number() String() Boolean() x as number
来源：http://oua.hywenlv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rgj.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uul.yvedp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vkg.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hrw.ctjpmb.com

================================================================================
来源：http://egx.hfpthk.cn

B. 流程控制
来源：http://kdr.guannengcc.top

================================================================================
来源：http://xbk.aizwys.cn

[B01] 条件判断 if / else
来源：http://avc.yuxming.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xip.xinyue.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eun.yuanzhike.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bsy.cucudq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sqg.svipenyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lvo.yanxiufei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ids.zhixingplan.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qka.ehwqpu.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ypv.smart0.xyz

[B02] 多分支 else if / elif
来源：http://trz.ybcxt.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fiv.hnqzz.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pil.redwolf501.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://szi.gotoacloud.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ksb.feifeiyinyue.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xkp.9152youxi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://isu.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://weo.svipenyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nxp.xylfe.cn

[B03] switch / match / case
来源：http://wyo.cashguo.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iem.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qpi.xuanzx.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tre.cdnleiting.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xzx.jianghu66.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pof.fehbvm.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hos.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yho.jqgufenzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wtb.xuetiantiany.cn

[B04] for 计数循环
来源：http://xjh.gotoacloud.top

Py:   for i in range(10): print(i)
来源：http://xlr.zhoulong.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://arw.cheryme.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yjp.0kj1m.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kxm.andypj.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tcx.fktsv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cwg.xuetiantiany.cn

Ruby: 10.times { |i| puts i }
来源：http://gwl.hnxiangtu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://klu.aibaodan.cn

[B05] 遍历数组 / 列表
来源：http://mrp.ywan-chungtsiang.top

Py:   for item in arr: print(item)
来源：http://gdu.fzhhl.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jqk.nanxinkj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ihx.jqgufenzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ezs.feifeiyinyue.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pwb.nwbrower.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rtd.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://qvi.hfpthk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dgw.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://day.tarul.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hvt.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pvl.cashguo.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://clk.tarul.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lbd.epnwcf.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kia.redwolf501.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ohp.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bni.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gtq.0kj1m.cn

[B07] while 循环
来源：http://zmq.zhixingplan.top

Py:   while i < 10: i += 1
来源：http://dpv.yangfankeji.com

PHP:  while ($i < 10) { $i++; }
来源：http://dee.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://izi.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://fhc.hongshengwenyu.top

Java: while (i < 10) { i++; }
来源：http://xjl.yuxming.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hdi.nanxuanxn.top

Ruby: while i < 10; i += 1; end
来源：http://ayb.daria6918.cn

C#:   while (i < 10) { i++; }
来源：http://yyy.zdbjq.cn

[B08] do-while（至少执行一次）
来源：http://jxy.0kj1m.cn

Py:   # 无 do-while：用 while True + break
来源：http://lsp.pycfn.com

PHP:  do { $i++; } while ($i < 10);
来源：http://zox.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://ylo.bjfxy.top

TS:   do { i++; } while (i < 10);
来源：http://mek.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://yqm.epnwcf.com

Go:   for { i++; if i >= 10 { break } }
来源：http://ycj.chenjidiqi.icu

Ruby: begin; i += 1; end while i < 10
来源：http://rto.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://gjl.tian-w.cn

[B09] break 与 continue
来源：http://tey.nwbrower.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jtw.gotoacloud.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://svt.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://diz.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ukl.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ubk.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bez.hcnkem.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qwe.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rrh.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://qbm.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://val.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fwm.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cdr.c1oappe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wwl.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gnk.wangshuangyany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cuw.316326.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bhi.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kef.snrcjt.cn

[B11] 生成数字序列 / 区间
来源：http://ycw.jqgufenzy.top

Py:   list(range(0, 10, 2))
来源：http://riy.dianchejie.cn

PHP:  range(0, 10, 2);
来源：http://bue.ppjwa.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ack.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ogd.jinqigufen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mtp.daxiang520.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://msy.daria6918.cn

Ruby: (0...10).step(2).to_a
来源：http://exo.fengsongda.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mdj.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://fzn.epnwcf.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://vds.zhengqikj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lhj.nanxuanxn.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qon.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bui.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gif.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oqr.dianchejie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mtk.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zij.hongshengwenyu.top

[B13] 判断是否为数字
来源：http://vux.cdnleiting.top

Py:   isinstance(x, (int, float))
来源：http://kkm.svipenyu.cn

PHP:  is_numeric($x)
来源：http://ndf.jinqigufen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dlw.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ksf.sysykeji.top

Java: x instanceof Number
来源：http://xtt.yueranfly.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ypn.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://kuy.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://xcq.fehbvm.com

[B14] 判断值是否在集合内
来源：http://nte.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dek.zycfv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mvp.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://dsi.quarkkingdee.top

TS:   [1, 2, 3].includes(x)
来源：http://tuq.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zzv.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lul.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://zwo.jinqigfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jkk.yuanzhike.top

[B15] 布尔运算与取反
来源：http://twn.0kj1m.cn

Py:   a and b or not c
来源：http://iph.sxryk.cn

PHP:  $a && $b || !$c
来源：http://css.zhongyouzk.top

JS:   a && b || !c
来源：http://kzv.yongpay.top

TS:   a && b || !c
来源：http://hfy.mhx1999.top

Java: a && b || !c
来源：http://lwy.hesvh.cn

Go:   a && b || !c
来源：http://jjh.sxryk.cn

Ruby: a && b || !c
来源：http://exg.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://jhk.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://wzv.daria6918.cn

Py:   if not data: return
来源：http://yua.cheryme.top

PHP:  if (!$data) { return; }
来源：http://pwm.guannengcc.top

JS:   if (!data) return;
来源：http://dil.ydzc1.top

TS:   if (!data) return;
来源：http://vhq.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://gdi.yfazqb.com

Go:   if data == nil { return }
来源：http://auk.epnwcf.com

Ruby: return if data.nil?
来源：http://xnz.jiagoushi.top

C#:   if (data == null) return;
来源：http://glc.shanyushiyangkeji.top

================================================================================
来源：http://bwi.xuetiantiany.cn

C. 函数与作用域
来源：http://bhy.jqgufenzy.top

================================================================================
来源：http://hwf.fzhhl.top

[C01] 定义函数
来源：http://pue.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://rzw.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yhl.xuanzx.com

JS:   function add(a, b) { return a + b; }
来源：http://acq.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yfw.chenzaomai.com

Java: static int add(int a, int b) { return a + b; }
来源：http://tze.birdmap.top

Go:   func add(a, b int) int { return a + b }
来源：http://txu.quarkkingdee.top

Ruby: def add(a, b); a + b; end
来源：http://tae.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zqa.zdbjq.cn

[C02] 默认参数
来源：http://toj.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://nkk.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://glb.yj20258.top

JS:   function greet(name = "World") { return name; }
来源：http://nxu.cheryme.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sus.cashguo.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bql.guowangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iyh.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://gny.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://tyb.yvedp.cn

[C03] 可变参数
来源：http://fju.yueranfly.top

Py:   def total(*args): return sum(args)
来源：http://kdb.xziqi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yak.yuanzhike.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wil.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dgx.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gjj.yvedp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rfs.snrcjt.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lgh.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sss.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://hph.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uti.ydzc1.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iag.fzhhl.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hbi.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wii.chenjidiqi.icu

Java: // 无：用 Builder 模式或 record
来源：http://gqv.jinghuilouyu.cn

Go:   // 无：用配置结构体参数
来源：http://jha.bjfxy.top

Ruby: f(a: 1, b: 2)
来源：http://hge.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://hip.ywan-chungtsiang.top

[C05] 返回多个值
来源：http://gbo.gzhubu.top

Py:   return a, b
来源：http://zsw.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://bxc.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pus.yonumen.top

TS:   return { a, b };
来源：http://qsb.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xfq.zhongyouzk.top

Go:   return a, b
来源：http://avx.uphjek.com

Ruby: return a, b
来源：http://cnk.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://rmw.sufxvd.cn

[C06] 匿名函数 / lambda
来源：http://jbo.chenzaomai.com

Py:   square = lambda x: x * x
来源：http://aym.jinqigufen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kiq.hywenlv.cn

JS:   const square = x => x * x;
来源：http://yio.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://hso.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tuo.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://hsz.tarul.cn

Ruby: square = ->(x) { x * x }
来源：http://zdh.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://wiv.zhijiandao.cn

[C07] 把函数作为参数传入
来源：http://mlj.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fil.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://yzc.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tnt.zdqjudy.top

TS:   arr.map(String)
来源：http://jyc.c1oappe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xbp.ctjpmb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cgo.chenzaomai.com

Ruby: arr.map(&:upcase)
来源：http://cnb.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hoe.shangyingyoupin.top

[C08] 闭包
来源：http://owc.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cxe.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://slv.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ean.zycfv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ghp.nwbrower.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hsk.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://utg.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tkq.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://azk.yj202588.top

[C09] 递归
来源：http://hzp.fzhhl.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kyv.yongpay.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mtn.tanke756.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mgn.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bmq.hammf.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zqt.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mrt.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vro.sjlbkw.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bdb.cashguo.top

[C10] 变量作用域
来源：http://tlb.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tvt.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jlf.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vjc.quarkkingdee.top

TS:   同 JS
来源：http://gqq.xylfe.cn

Java: 方法内为块级作用域
来源：http://ijp.zdqjudy.top

Go:   花括号块级作用域
来源：http://utg.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kkp.feifeiyinyue.top

C#:   块级作用域
来源：http://kep.cashguo.top

[C11] 模块导入与导出
来源：http://hly.mhx1999.top

Py:   from module import func
来源：http://vxt.sufxvd.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://crv.daxiang520.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://son.shanyushiyangtech.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ank.andypj.xyz

Java: import java.util.List;
来源：http://icc.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wks.9152youxi.cn

Ruby: require "json"; require_relative "./util"
来源：http://iby.fanxiaobao.xyz

C#:   using System.Text;
来源：http://jmk.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://iah.gogol.net.cn

Py:   (lambda: print("run"))()
来源：http://mrm.snrcjt.cn

PHP:  (function () { echo "run"; })();
来源：http://qto.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://vmi.bbcook.cn

TS:   (() => { console.log("run"); })();
来源：http://ylz.epnwcf.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xxp.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://kvq.yj20258.top

Ruby: -> { puts "run" }.call
来源：http://wng.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ujm.ctjpmb.com

[C13] 类型声明 / 类型注解
来源：http://gwu.nanxinkj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xkg.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jll.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vwc.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bqu.tarul.cn

Java: int add(int a, int b) { return a + b; }
来源：http://grq.daxiang520.top

Go:   func add(a, b int) int
来源：http://jkp.jinqigfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://emy.chenjidiqi.icu

C#:   int Add(int a, int b) => a + b;
来源：http://fum.smart0.xyz


<!-- 参考信息 -->