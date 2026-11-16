代发 wailian999

[A26] 类型转换总览
来源：http://nrp.zdbjq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vhh.iojbl.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jkg.yangfankeji.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cqm.ehwqpu.com

TS:   Number() String() Boolean() x as number
来源：http://wgz.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ptk.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eeq.sysykeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wqs.mhx1999.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ptj.xylfe.cn

================================================================================
来源：http://veu.jqgufenzy.top

B. 流程控制
来源：http://stz.gaohongyu789.top

================================================================================
来源：http://hol.hnqzz.top

[B01] 条件判断 if / else
来源：http://pbx.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://zta.shanyushiyangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://biw.jlsjyb.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vxo.yanxiufei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uou.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pdt.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://akz.zhiwuduotai.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rek.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://orl.yueranfly.top

[B02] 多分支 else if / elif
来源：http://jiv.hongshengwenyu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kqh.haohaochexian.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jhi.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lre.fanxiaobao.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xby.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bmv.sxryk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cmc.sufxvd.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mhg.svipenyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tzl.zhengqikj.top

[B03] switch / match / case
来源：http://owc.ydzc1.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xjg.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pwc.chenzaomai.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jyw.ivvv.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jgd.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ouo.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kvt.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hau.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iol.gaohongyu789.top

[B04] for 计数循环
来源：http://tjq.wangdashe.top

Py:   for i in range(10): print(i)
来源：http://gho.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lru.sjlbkw.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://huq.daria6918.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bfd.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sgg.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mdg.jinqigufen.top

Ruby: 10.times { |i| puts i }
来源：http://xyl.wangdashe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ify.yuanzhike.top

[B05] 遍历数组 / 列表
来源：http://nko.hysaishi.cn

Py:   for item in arr: print(item)
来源：http://fzf.cdnleiting.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yyo.aizwys.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dkz.shanyushiyangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wzx.zhaomingkeji.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://nab.jinghuilouyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hfv.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://tkg.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bof.cucudq.cn

[B06] 遍历字典 / 对象
来源：http://jli.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kiy.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ydh.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fqn.vqdsnc.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://afr.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://voq.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://epi.yvedp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xfl.ydzc1.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lcc.wangdashe.top

[B07] while 循环
来源：http://ldt.nanxinkj.top

Py:   while i < 10: i += 1
来源：http://peu.shangyingyoupin.top

PHP:  while ($i < 10) { $i++; }
来源：http://gco.hnqzz.top

JS:   while (i < 10) { i++; }
来源：http://xmd.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://eya.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://xyd.yuxming.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qwz.yanxiufei.cn

Ruby: while i < 10; i += 1; end
来源：http://znb.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://bkf.jinqigufen.top

[B08] do-while（至少执行一次）
来源：http://ckd.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://dxx.zhiwuduotai.top

PHP:  do { $i++; } while ($i < 10);
来源：http://njn.hywenlv.cn

JS:   do { i++; } while (i < 10);
来源：http://xho.tanke756.top

TS:   do { i++; } while (i < 10);
来源：http://ivo.yueranfly.top

Java: do { i++; } while (i < 10);
来源：http://fip.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ibx.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mem.wangshuangyany.cn

C#:   do { i++; } while (i < 10);
来源：http://ldh.hongshengwenyu.top

[B09] break 与 continue
来源：http://qtt.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gjx.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vmj.xinyue.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqg.hammf.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qea.ivvv.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ucn.pengpengdd.cyou

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hsn.shanyushiyangtech.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jeb.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kop.dianchejie.cn

[B10] 遍历同时拿索引
来源：http://umj.aizwys.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cyf.shanyushiyangtech.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://etc.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vnd.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nsq.9152youxi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lhv.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iom.yonumen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://adi.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ulg.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://lmf.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://cxk.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://ksy.yangfankeji.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sns.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fcg.nanxinkj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vom.gotoacloud.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gar.havefunace.top

Ruby: (0...10).step(2).to_a
来源：http://sdc.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zik.jqgufenzy.top

[B12] 跳出多层循环
来源：http://kdd.jyoumei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rlb.feifeiyinyue.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xnx.haohaochexian.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xnx.pengpengdd.cyou

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ouo.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://efp.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xlp.vehdjk.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zij.havefunace.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vmx.zhaomingkeji.xyz

[B13] 判断是否为数字
来源：http://obs.havefunace.top

Py:   isinstance(x, (int, float))
来源：http://kpu.jinyuanbaomall.cn

PHP:  is_numeric($x)
来源：http://sxj.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qly.quarkkingdee.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zxq.yangfankeji.com

Java: x instanceof Number
来源：http://mqd.gotoacloud.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://efm.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://fbh.sufxvd.cn

C#:   x is int or double or decimal
来源：http://lpa.sweek.top

[B14] 判断值是否在集合内
来源：http://mlo.yfazqb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ybx.bbcook.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qul.ctjpmb.com

JS:   [1, 2, 3].includes(x)
来源：http://cek.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://cqz.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kir.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pxh.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://cjj.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://okl.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://yjq.jianghu66.top

Py:   a and b or not c
来源：http://oxq.bbcook.cn

PHP:  $a && $b || !$c
来源：http://gkj.kuanghao11.cn

JS:   a && b || !c
来源：http://obb.zhijiandao.cn

TS:   a && b || !c
来源：http://pzs.yj20258.top

Java: a && b || !c
来源：http://btf.jinghuilouyu.cn

Go:   a && b || !c
来源：http://uwz.zhoulong.xyz

Ruby: a && b || !c
来源：http://ntp.jianghu66.top

C#:   a && b || !c
来源：http://vch.yvedp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qwm.yongpay.top

Py:   if not data: return
来源：http://yce.cashguo.top

PHP:  if (!$data) { return; }
来源：http://gny.pengpengdd.cyou

JS:   if (!data) return;
来源：http://pqd.cashguo.top

TS:   if (!data) return;
来源：http://cul.52xcode.cn

Java: if (data == null) return;
来源：http://byx.hysaishi.cn

Go:   if data == nil { return }
来源：http://ofb.cucudq.cn

Ruby: return if data.nil?
来源：http://tvm.nanxinkj.top

C#:   if (data == null) return;
来源：http://peq.quarkkingdee.top

================================================================================
来源：http://llb.shzxlz.cn

C. 函数与作用域
来源：http://qlv.aizwys.cn

================================================================================
来源：http://tmh.fehbvm.com

[C01] 定义函数
来源：http://wts.yj202588.top

Py:   def add(a, b): return a + b
来源：http://bjq.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sjd.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://wys.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kdv.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lpm.wangshuangyany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mbc.hesvh.cn

Ruby: def add(a, b); a + b; end
来源：http://ntt.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iii.zhixingplan.top

[C02] 默认参数
来源：http://vvp.yonumen.top

Py:   def greet(name="World"): return name
来源：http://tcn.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://kku.pycfn.com

JS:   function greet(name = "World") { return name; }
来源：http://tcz.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hju.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://mep.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wcx.jiagoushi.top

Ruby: def greet(name = "World") = name
来源：http://dsc.aizwys.cn

C#:   string Greet(string name = "World") => name;
来源：http://dvz.shzxlz.cn

[C03] 可变参数
来源：http://tnh.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://vdm.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tmx.daxiang520.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nmb.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tlw.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uvx.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://grd.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://oxg.jyoumei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bis.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://epa.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://heb.ehwqpu.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://avp.nanxuanxn.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://thc.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jsn.yfazqb.com

Java: // 无：用 Builder 模式或 record
来源：http://gpm.vehdjk.com

Go:   // 无：用配置结构体参数
来源：http://zct.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://rdk.haohaochexian.top

C#:   f(a: 1, b: 2)
来源：http://gnr.hcnkem.com

[C05] 返回多个值
来源：http://hwk.cheryme.top

Py:   return a, b
来源：http://cej.zhixingplan.top

PHP:  return [$a, $b];
来源：http://szj.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://ftn.tianlin.xyz

TS:   return { a, b };
来源：http://wbu.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tjg.ivvv.top

Go:   return a, b
来源：http://uco.yj20258888.top

Ruby: return a, b
来源：http://dek.hongshengwenyu.top

C#:   return (a, b);              // ValueTuple
来源：http://acl.jqgfzy.top

[C06] 匿名函数 / lambda
来源：http://vym.xuetiantiany.cn

Py:   square = lambda x: x * x
来源：http://lvj.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qbd.xuetiantiany.cn

JS:   const square = x => x * x;
来源：http://uab.yuxming.cn

TS:   const square = (x: number): number => x * x;
来源：http://egw.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uiv.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://voq.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://nfn.dianchejie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://adg.fktsv.cn

[C07] 把函数作为参数传入
来源：http://lah.xinyue.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bpx.snrcjt.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ebs.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zkc.hysaishi.cn

TS:   arr.map(String)
来源：http://naj.guowangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eot.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://opv.yueranfly.top

Ruby: arr.map(&:upcase)
来源：http://aze.bbcook.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ujq.shanyushiyangtech.top

[C08] 闭包
来源：http://div.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jgs.epnwcf.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ypa.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pvv.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dev.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dbc.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mwz.ybcxt.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ozw.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uml.sjlbkw.cn

[C09] 递归
来源：http://lzk.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qkg.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://czq.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iry.tanke756.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://owt.ehwqpu.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qqi.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jmg.redwolf501.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gjo.ydjk.org.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yiz.vqdsnc.cn

[C10] 变量作用域
来源：http://efs.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hpp.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tay.yongpay.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wyy.wangdashe.top

TS:   同 JS
来源：http://ygv.jinqigufen.top

Java: 方法内为块级作用域
来源：http://whw.kuanghao11.cn

Go:   花括号块级作用域
来源：http://dha.snrcjt.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://itj.sysykeji.top

C#:   块级作用域
来源：http://tgf.xuanzx.com

[C11] 模块导入与导出
来源：http://qgo.wangshuangyany.cn

Py:   from module import func
来源：http://hfy.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yxl.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://flq.yfazqb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tdx.hnxiangtu.top

Java: import java.util.List;
来源：http://pah.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://arl.yueranfly.top

Ruby: require "json"; require_relative "./util"
来源：http://sqm.9152youxi.cn

C#:   using System.Text;
来源：http://mkc.yfazqb.com

[C12] 立即执行函数 IIFE
来源：http://ndm.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://odi.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://cps.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://yms.316326.xyz

TS:   (() => { console.log("run"); })();
来源：http://hca.xuetiantiany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rao.kuanghao11.cn

Go:   func() { fmt.Println("run") }()
来源：http://pxb.vqdsnc.cn

Ruby: -> { puts "run" }.call
来源：http://zvu.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wbp.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://ncp.chenlongwang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ucp.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://voo.xingfuxueyuan.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gre.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://syz.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rii.yfazqb.com

Go:   func add(a, b int) int
来源：http://lzm.cashguo.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fbd.kuanghao11.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wtc.hesvh.cn

[C14] 泛型函数
来源：http://pxe.hysaishi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zma.zhongyouzk.top

PHP:  // 无泛型
来源：http://tvo.hongshengwenyu.top

JS:   // 无泛型
来源：http://lsu.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ebq.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mui.shangyingyoupin.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xvx.aibaodan.cn

Ruby: # 无泛型
来源：http://dsx.mhx1999.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tyk.hcnkem.com

[C15] 解构 / 展开参数
来源：http://wtu.cdnleiting.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://piy.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://muw.shzxlz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ict.fanxiaobao.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vsn.xziqi.cn

Java: // 无解构
来源：http://ici.dianchejie.cn

Go:   // 无解构
来源：http://sao.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://ard.vehdjk.com

C#:   var (a, b) = pair;
来源：http://evl.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://zfk.jinyuanbaomall.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nqw.fehbvm.com

PHP:  // 无重载
来源：http://nvb.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yxp.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://ufw.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rpg.ybcxt.top


<!-- 参考信息 -->