代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://olj.yuxming.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wyb.xuetiantiany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bjs.jqgufenzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sld.zdbjq.cn

[A26] 类型转换总览
来源：http://xnx.ywan-chungtsiang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gjm.aibaodan.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rtu.yonumen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nbr.jinqigfzy.top

TS:   Number() String() Boolean() x as number
来源：http://vgt.nanxinkj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ani.smart0.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://grv.uphjek.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://xjg.ctjpmb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xhv.sysykeji.top

================================================================================
来源：http://nqn.gaohongyu789.top

B. 流程控制
来源：http://dob.jinqigfzy.top

================================================================================
来源：http://gxt.mhx1999.top

[B01] 条件判断 if / else
来源：http://szd.tarul.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pbw.vqdsnc.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pzh.sweek.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qkv.vehdjk.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ctc.birdmap.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zob.hcnkem.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://srx.sweek.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kpw.xingfuxueyuan.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vea.hcnkem.com

[B02] 多分支 else if / elif
来源：http://rfr.dashuyun.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ymq.shzxlz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iym.gogol.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dqs.ybcxt.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://arx.chenjidiqi.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iyw.zycfv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mac.ppjwa.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zrl.uphjek.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jtk.9152youxi.cn

[B03] switch / match / case
来源：http://snl.shuidangran.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://etw.zhaomingkeji.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ock.yuanzhike.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xvq.dianchejie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wbs.vqdsnc.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qcv.hywenlv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ltb.yanxiufei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dws.vehdjk.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ygr.chenjidiqi.icu

[B04] for 计数循环
来源：http://key.xuanzx.com

Py:   for i in range(10): print(i)
来源：http://nly.feifeiyinyue.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vnn.chenzaomai.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zhd.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iuf.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dhf.yfazqb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vnr.chenzaomai.com

Ruby: 10.times { |i| puts i }
来源：http://bbb.ehwqpu.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tad.zhongyouzk.top

[B05] 遍历数组 / 列表
来源：http://cxx.jinghuilouyu.cn

Py:   for item in arr: print(item)
来源：http://sqr.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yzq.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://giu.fktsv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tam.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hgi.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pdm.shanyushiyangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://jqe.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mei.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://fby.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cik.sxryk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zen.hywenlv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eob.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gfc.hnxiangtu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ste.gogol.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cgn.pycfn.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uiw.xziqi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fpe.feifeiyinyue.top

[B07] while 循环
来源：http://nao.316326.xyz

Py:   while i < 10: i += 1
来源：http://saz.xinyue.icu

PHP:  while ($i < 10) { $i++; }
来源：http://txs.shanyushiyangtech.top

JS:   while (i < 10) { i++; }
来源：http://amj.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://zmc.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://xoa.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zcv.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://zio.gotoacloud.top

C#:   while (i < 10) { i++; }
来源：http://qdm.shzxlz.cn

[B08] do-while（至少执行一次）
来源：http://wsi.yj20258.top

Py:   # 无 do-while：用 while True + break
来源：http://kzy.uphjek.com

PHP:  do { $i++; } while ($i < 10);
来源：http://rrp.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://hml.wangshuangyany.cn

TS:   do { i++; } while (i < 10);
来源：http://zat.fengsongda.top

Java: do { i++; } while (i < 10);
来源：http://fzm.zhiwuduotai.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jik.yvedp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cgx.zdqjudy.top

C#:   do { i++; } while (i < 10);
来源：http://ojj.daxiang520.top

[B09] break 与 continue
来源：http://dkh.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yhd.pengpengdd.cyou

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nfg.feifeiyinyue.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mmp.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ysh.316326.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qyg.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qtq.yangfankeji.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tzs.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zux.cucudq.cn

[B10] 遍历同时拿索引
来源：http://vng.yuanzhike.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nbz.ivvv.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cgi.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bok.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ugg.yongpay.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ktp.316326.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lal.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qsp.guannengcc.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bqj.yj20258.top

[B11] 生成数字序列 / 区间
来源：http://yqf.ppjwa.cn

Py:   list(range(0, 10, 2))
来源：http://aav.c1oappe.top

PHP:  range(0, 10, 2);
来源：http://pey.sufxvd.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rjy.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xga.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sgo.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gfd.yj20258888.top

Ruby: (0...10).step(2).to_a
来源：http://yld.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lbw.sufxvd.cn

[B12] 跳出多层循环
来源：http://gpt.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xkz.jlsjyb.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pam.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xan.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uzm.bjfxy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jed.jqgfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qvm.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eli.zhoulong.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yrp.ehwqpu.com

[B13] 判断是否为数字
来源：http://joe.shanyushiyangtech.top

Py:   isinstance(x, (int, float))
来源：http://lvu.jinqigfzy.top

PHP:  is_numeric($x)
来源：http://muo.cqqwz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://emu.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vjy.feifeiyinyue.top

Java: x instanceof Number
来源：http://tsw.redwolf501.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vcf.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://pgy.dianchejie.cn

C#:   x is int or double or decimal
来源：http://kfw.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://nyv.sweek.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qmr.shzxlz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gzx.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://hjy.mhx1999.top

TS:   [1, 2, 3].includes(x)
来源：http://oyq.shzxlz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wgc.chenjidiqi.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xpi.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://rxa.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tne.redwolf501.top

[B15] 布尔运算与取反
来源：http://qjg.dianchejie.cn

Py:   a and b or not c
来源：http://dtq.birdmap.top

PHP:  $a && $b || !$c
来源：http://ucb.iojbl.cn

JS:   a && b || !c
来源：http://jzs.fktsv.cn

TS:   a && b || !c
来源：http://vfy.vehdjk.com

Java: a && b || !c
来源：http://ogh.bbcook.cn

Go:   a && b || !c
来源：http://srn.zhongyouzk.top

Ruby: a && b || !c
来源：http://iei.jiagoushi.top

C#:   a && b || !c
来源：http://kkz.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://juk.yangfankeji.com

Py:   if not data: return
来源：http://frv.xinyue.icu

PHP:  if (!$data) { return; }
来源：http://tek.dashuyun.cn

JS:   if (!data) return;
来源：http://srw.snrcjt.cn

TS:   if (!data) return;
来源：http://xoh.jyoumei.cn

Java: if (data == null) return;
来源：http://ykq.316326.xyz

Go:   if data == nil { return }
来源：http://olj.redwolf501.top

Ruby: return if data.nil?
来源：http://jcp.bbcook.cn

C#:   if (data == null) return;
来源：http://ojv.yuanzhike.top

================================================================================
来源：http://qsm.zhongyouzk.top

C. 函数与作用域
来源：http://ygk.xinyue.icu

================================================================================
来源：http://vef.xziqi.cn

[C01] 定义函数
来源：http://pbs.pengpengdd.cyou

Py:   def add(a, b): return a + b
来源：http://gih.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dlf.nanxuanxn.top

JS:   function add(a, b) { return a + b; }
来源：http://oko.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://smb.havefunace.top

Java: static int add(int a, int b) { return a + b; }
来源：http://per.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iup.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://dug.svipenyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ign.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://lft.fanxiaobao.xyz

Py:   def greet(name="World"): return name
来源：http://nog.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qri.ppjwa.cn

JS:   function greet(name = "World") { return name; }
来源：http://fer.xingfuxueyuan.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://mle.yangfankeji.com

Java: // 无默认参数：方法重载或 Optional
来源：http://xtf.hnxiangtu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zqb.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://xdt.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://vqm.hywenlv.cn

[C03] 可变参数
来源：http://ysz.guowangkeji.top

Py:   def total(*args): return sum(args)
来源：http://wkz.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://skb.cheryme.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jao.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wdy.snrcjt.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qay.yj20258888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ryk.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://rnh.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://amo.sjlbkw.cn

[C04] 命名参数 / 关键字参数
来源：http://pgr.c1oappe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dhs.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dik.tian-w.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://swz.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xeg.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://pes.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://buu.jinqigufen.top

Ruby: f(a: 1, b: 2)
来源：http://pxe.ehwqpu.com

C#:   f(a: 1, b: 2)
来源：http://csz.xuetiantiany.cn

[C05] 返回多个值
来源：http://kgw.gotoacloud.top

Py:   return a, b
来源：http://nqh.sxryk.cn

PHP:  return [$a, $b];
来源：http://ybs.zhixingplan.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bbd.hnxiangtu.top

TS:   return { a, b };
来源：http://kdk.hesvh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yma.hywenlv.cn

Go:   return a, b
来源：http://iav.shzxlz.cn

Ruby: return a, b
来源：http://fbs.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://uyu.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://xgf.shuidangran.top

Py:   square = lambda x: x * x
来源：http://asq.wangshuangyany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://orh.zdbjq.cn

JS:   const square = x => x * x;
来源：http://iuk.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://aby.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://apv.redwolf501.top

Go:   sq := func(x int) int { return x * x }
来源：http://swt.jinyuanbaomall.cn

Ruby: square = ->(x) { x * x }
来源：http://mbp.bjfxy.top

C#:   Func<int, int> square = x => x * x;
来源：http://fbq.iojbl.cn

[C07] 把函数作为参数传入
来源：http://vrn.smart0.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nmq.zhiwuduotai.top

PHP:  array_map("strtoupper", $arr);
来源：http://bjz.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tco.yonumen.top

TS:   arr.map(String)
来源：http://ewm.daria6918.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zgj.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ujj.wangshuangyany.cn

Ruby: arr.map(&:upcase)
来源：http://hjb.wangshuangyany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xon.nanxuanxn.top

[C08] 闭包
来源：http://sfo.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://agr.andypj.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oyh.tanke756.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kga.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://quu.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://udv.quarkkingdee.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tdy.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dae.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://krr.nwbrower.top

[C09] 递归
来源：http://wmh.xylfe.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rtq.uphjek.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sck.xuanzx.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://anw.jqgfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wpe.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bqw.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sxh.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rtw.hywenlv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vfj.yanxiufei.cn

[C10] 变量作用域
来源：http://ldt.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zup.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bij.yongpay.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xef.shanyushiyangkeji.top

TS:   同 JS
来源：http://xlq.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://zrf.chenzaomai.com

Go:   花括号块级作用域
来源：http://jla.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rfb.yongpay.top

C#:   块级作用域
来源：http://rlw.yangfankeji.com

[C11] 模块导入与导出
来源：http://dwq.ybcxt.top

Py:   from module import func
来源：http://pja.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yps.sufxvd.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://chd.nanxuanxn.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vpp.shanyushiyangkeji.top

Java: import java.util.List;
来源：http://suf.hnxiangtu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ldl.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://vmy.jqgufenzy.top

C#:   using System.Text;
来源：http://ewp.yangfankeji.com

[C12] 立即执行函数 IIFE
来源：http://ipc.epnwcf.com

Py:   (lambda: print("run"))()
来源：http://gve.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://dgv.svipenyu.cn

JS:   (() => { console.log("run"); })();
来源：http://ssy.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://lsg.tanke756.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kki.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://aos.mhx1999.top

Ruby: -> { puts "run" }.call
来源：http://kak.jianghu66.top

C#:   // 无 IIFE：用静态构造函数
来源：http://iwo.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://pkc.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ljg.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ktw.yuanzhike.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dem.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hfa.epnwcf.com

Java: int add(int a, int b) { return a + b; }
来源：http://njm.hammf.cn

Go:   func add(a, b int) int
来源：http://qfq.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://inh.hnxiangtu.top

C#:   int Add(int a, int b) => a + b;
来源：http://xpl.meibo888.top

[C14] 泛型函数
来源：http://xmz.hcnkem.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bde.jinqigufen.top

PHP:  // 无泛型
来源：http://few.nwbrower.top

JS:   // 无泛型
来源：http://wtw.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cec.shanyushiyangtech.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wrr.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zjo.yangfankeji.com

Ruby: # 无泛型
来源：http://ehq.chenjidiqi.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://avf.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://fzj.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hoz.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://izl.xziqi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vbr.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xus.daria6918.cn

Java: // 无解构
来源：http://kcj.cucudq.cn

Go:   // 无解构
来源：http://hjp.tianlin.xyz

Ruby: a, b = pair
来源：http://rvc.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://ufh.hnqzz.top

[C16] 函数 / 方法重载
来源：http://xls.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fqh.andypj.xyz


<!-- 参考信息 -->