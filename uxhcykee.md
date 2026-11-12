代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://mcc.sysykeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zjf.chenjidiqi.icu

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wrn.pengpengdd.cyou

[A25] 字符串比较
来源：http://cqt.bbcook.cn

Py:   s1 == s2; s1 != s2
来源：http://dlm.yanxiufei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ylt.fanxiaobao.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://opq.yanxiufei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tgb.chenzaomai.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ohm.aibaodan.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nku.xuanzx.com

Ruby: s1 == s2; s1 <=> s2
来源：http://idz.zhoulong.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vnc.pengpengdd.cyou

[A26] 类型转换总览
来源：http://lcm.yanxiufei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://grg.yuanzhike.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uxi.havefunace.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gqd.guowangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://fvw.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hzt.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nrf.nanxinkj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xip.xingfuxueyuan.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xxk.yonumen.top

================================================================================
来源：http://vaj.fktsv.cn

B. 流程控制
来源：http://wyc.pengpengdd.cyou

================================================================================
来源：http://yuv.shanyushiyangkeji.top

[B01] 条件判断 if / else
来源：http://dat.hnqzz.top

Py:   result = "正" if x > 0 else "非正"
来源：http://yuj.daria6918.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xtc.gaohongyu789.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://umj.shzxlz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lvr.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://asd.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jzl.zdbjq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jwv.sweek.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://noz.birdmap.top

[B02] 多分支 else if / elif
来源：http://vbs.shuidangran.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zbp.gzhubu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lha.jinghuilouyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hiv.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bxz.nwbrower.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://std.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cpl.yueranfly.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://svo.shzxlz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iyy.feifeiyinyue.top

[B03] switch / match / case
来源：http://fyh.zhiwuduotai.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wts.shanyushiyangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tqr.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ugq.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bdw.yfazqb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ykb.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yqs.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bnl.bbcook.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qfd.fktsv.cn

[B04] for 计数循环
来源：http://wju.fzhhl.top

Py:   for i in range(10): print(i)
来源：http://mdg.yj20258888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xlh.shzxlz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ial.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qud.kuanghao11.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ppz.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qam.nanxuanxn.top

Ruby: 10.times { |i| puts i }
来源：http://ydm.cdnleiting.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gco.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://eim.gogol.net.cn

Py:   for item in arr: print(item)
来源：http://mok.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hpm.cashguo.top

JS:   for (const item of arr) { console.log(item); }
来源：http://alh.sweek.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tma.ehwqpu.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ugy.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ivr.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://xoc.yj20258.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cvg.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://axn.vqdsnc.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yjc.smart0.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wdj.redwolf501.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zci.yanxiufei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gfa.zhijiandao.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wmh.316326.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dsd.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jaf.fanxiaobao.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pda.cucudq.cn

[B07] while 循环
来源：http://glj.9152youxi.cn

Py:   while i < 10: i += 1
来源：http://hsq.mhx1999.top

PHP:  while ($i < 10) { $i++; }
来源：http://pgk.ivvv.top

JS:   while (i < 10) { i++; }
来源：http://amf.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://pqu.haohaochexian.top

Java: while (i < 10) { i++; }
来源：http://bms.xuanzx.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hmk.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://wjc.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://ksl.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://ktg.cashguo.top

Py:   # 无 do-while：用 while True + break
来源：http://vns.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dng.ivvv.top

JS:   do { i++; } while (i < 10);
来源：http://yaa.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://luy.wangdashe.top

Java: do { i++; } while (i < 10);
来源：http://kxh.bjfxy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xzk.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://hes.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://rha.hcnkem.com

[B09] break 与 continue
来源：http://ecx.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://czo.snrcjt.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mjq.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://drh.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://chp.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixv.vehdjk.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yye.shanyushiyangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dgn.wangshuangyany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xpu.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://dxq.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rli.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://izw.tarul.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xtk.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gtp.guowangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sjg.zhixingplan.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tnt.tarul.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hnk.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://are.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://khk.zhongyouzk.top

Py:   list(range(0, 10, 2))
来源：http://mfe.meibo888.top

PHP:  range(0, 10, 2);
来源：http://sbc.hcnkem.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://msy.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ddi.fktsv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ohq.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nlq.yueranfly.top

Ruby: (0...10).step(2).to_a
来源：http://mob.cheryme.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ymk.redwolf501.top

[B12] 跳出多层循环
来源：http://ywt.yanxiufei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qna.hesvh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zzm.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hkq.bbcook.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ayd.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://guv.chenzaomai.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cqg.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oqj.316326.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vhl.cashguo.top

[B13] 判断是否为数字
来源：http://arq.sweek.top

Py:   isinstance(x, (int, float))
来源：http://xpl.shzxlz.cn

PHP:  is_numeric($x)
来源：http://uba.jinyuanbaomall.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gma.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ppe.uphjek.com

Java: x instanceof Number
来源：http://ejh.sufxvd.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pqm.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://bxp.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://wyp.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://ruo.cucudq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lcq.hammf.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bdl.nanxinkj.top

JS:   [1, 2, 3].includes(x)
来源：http://kkf.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://oiw.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qan.hnqzz.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fwh.dianchejie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wtt.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lxg.aibaodan.cn

[B15] 布尔运算与取反
来源：http://dor.gzhubu.top

Py:   a and b or not c
来源：http://lzv.ydzc1.top

PHP:  $a && $b || !$c
来源：http://juq.jinqigfzy.top

JS:   a && b || !c
来源：http://crs.mhx1999.top

TS:   a && b || !c
来源：http://ytb.svipenyu.cn

Java: a && b || !c
来源：http://ujz.52xcode.cn

Go:   a && b || !c
来源：http://ajc.zhixingplan.top

Ruby: a && b || !c
来源：http://wyn.xziqi.cn

C#:   a && b || !c
来源：http://icv.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://zub.xuetiantiany.cn

Py:   if not data: return
来源：http://xgz.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://zxi.yfazqb.com

JS:   if (!data) return;
来源：http://ilu.0kj1m.cn

TS:   if (!data) return;
来源：http://qmq.shangyingyoupin.top

Java: if (data == null) return;
来源：http://fvr.yj202588.top

Go:   if data == nil { return }
来源：http://bie.zhongyouzk.top

Ruby: return if data.nil?
来源：http://pwh.dashuyun.cn

C#:   if (data == null) return;
来源：http://ses.jinyuanbaomall.cn

================================================================================
来源：http://uay.52xcode.cn

C. 函数与作用域
来源：http://pbk.jqgfzy.top

================================================================================
来源：http://fve.jqgufenzy.top

[C01] 定义函数
来源：http://qeo.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://qds.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ybb.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://gmk.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yes.yanxiufei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://abi.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://kuc.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://fsm.vehdjk.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ydv.52xcode.cn

[C02] 默认参数
来源：http://fqt.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://sif.gzhubu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pag.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://xci.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ecy.gaohongyu789.top

Java: // 无默认参数：方法重载或 Optional
来源：http://myg.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rro.birdmap.top

Ruby: def greet(name = "World") = name
来源：http://enf.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://uyb.fanxiaobao.xyz

[C03] 可变参数
来源：http://wre.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://odi.fengsongda.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zqc.fzhhl.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hru.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ohn.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mnp.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://svr.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://eap.aizwys.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cwu.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://wnz.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ser.gzhubu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hwo.chenjidiqi.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jad.dashuyun.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ubh.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://bro.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://zzl.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://ppf.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://hno.yonumen.top

[C05] 返回多个值
来源：http://ubw.fehbvm.com

Py:   return a, b
来源：http://bqh.haohaochexian.top

PHP:  return [$a, $b];
来源：http://daw.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jkn.c1oappe.top

TS:   return { a, b };
来源：http://unm.zhengqikj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gen.xinyue.icu

Go:   return a, b
来源：http://hfx.pengpengdd.cyou

Ruby: return a, b
来源：http://xgz.sxryk.cn

C#:   return (a, b);              // ValueTuple
来源：http://drt.shangyingyoupin.top

[C06] 匿名函数 / lambda
来源：http://wiv.hesvh.cn

Py:   square = lambda x: x * x
来源：http://wpz.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://sgo.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://oup.wangdashe.top

TS:   const square = (x: number): number => x * x;
来源：http://csg.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mqk.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kft.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://iin.yanxiufei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://art.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://wun.hnxiangtu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pda.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hbc.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xbo.yvedp.cn

TS:   arr.map(String)
来源：http://rei.xziqi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dep.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gah.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://fig.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ili.gogol.net.cn

[C08] 闭包
来源：http://dmz.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gcd.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://alk.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ork.yj202588.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://awq.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pkj.ybcxt.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://biw.jqgfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jdl.zhongyouzk.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ctj.cheryme.top

[C09] 递归
来源：http://wwe.feifeiyinyue.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cbt.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zvx.shanyushiyangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://akk.shuidangran.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zpc.ehwqpu.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ljv.zhoulong.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kre.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ozo.uphjek.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xwj.hnxiangtu.top

[C10] 变量作用域
来源：http://rvy.52xcode.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fug.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://esn.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kob.jyoumei.cn

TS:   同 JS
来源：http://ymd.snrcjt.cn

Java: 方法内为块级作用域
来源：http://okb.daria6918.cn

Go:   花括号块级作用域
来源：http://cjs.ybcxt.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tux.iojbl.cn

C#:   块级作用域
来源：http://epj.kuanghao11.cn

[C11] 模块导入与导出
来源：http://dyg.fengsongda.top

Py:   from module import func
来源：http://sfi.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gqc.ydzc1.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xge.xuetiantiany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ggs.gogol.net.cn

Java: import java.util.List;
来源：http://onr.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://anf.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://jze.ydjk.org.cn

C#:   using System.Text;
来源：http://bdi.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://wbx.yj202588.top

Py:   (lambda: print("run"))()
来源：http://fca.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://noj.hnqzz.top

JS:   (() => { console.log("run"); })();
来源：http://imm.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://sne.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zgd.yueranfly.top

Go:   func() { fmt.Println("run") }()
来源：http://mqn.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://qfq.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://olk.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://mmz.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vpg.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eco.tian-w.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fyo.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ysc.c1oappe.top

Java: int add(int a, int b) { return a + b; }
来源：http://skt.hnxiangtu.top

Go:   func add(a, b int) int
来源：http://lgy.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xka.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jkq.yfazqb.com

[C14] 泛型函数
来源：http://fwi.hongshengwenyu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://grc.redwolf501.top

PHP:  // 无泛型
来源：http://did.xziqi.cn

JS:   // 无泛型
来源：http://drg.aibaodan.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://amn.ehwqpu.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zpo.vqdsnc.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mcn.shuidangran.top

Ruby: # 无泛型
来源：http://mjw.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://svp.chenlongwang.top

[C15] 解构 / 展开参数
来源：http://rwk.ybcxt.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kfk.jinqigfzy.top

PHP:  [$a, $b] = $pair;
来源：http://rme.yanxiufei.cn


<!-- 参考信息 -->