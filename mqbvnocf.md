代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://mnr.vqdsnc.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nfc.ctjpmb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://knx.9152youxi.cn

[A25] 字符串比较
来源：http://gfe.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://nvo.dianchejie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xps.snrcjt.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mzf.gzhubu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wxo.gzhubu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hbq.uphjek.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rne.fanxiaobao.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://nqi.jyoumei.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vtt.yueranfly.top

[A26] 类型转换总览
来源：http://tvt.cdnleiting.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://try.zdqjudy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dwj.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qhz.jinyuanbaomall.cn

TS:   Number() String() Boolean() x as number
来源：http://bml.gogol.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qrp.wangshuangyany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://klf.hcnkem.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://any.zdqjudy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zrq.shzxlz.cn

================================================================================
来源：http://vqd.haohaochexian.top

B. 流程控制
来源：http://dyc.hfpthk.cn

================================================================================
来源：http://wle.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://tuy.yueranfly.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mcm.ctjpmb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hna.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tyg.xingfuxueyuan.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qke.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mkw.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aiw.shangyingyoupin.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jho.chenzaomai.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://esz.andypj.xyz

[B02] 多分支 else if / elif
来源：http://amk.fehbvm.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fsp.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gvh.fehbvm.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uqa.0kj1m.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wgd.aibaodan.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sjc.xingfuxueyuan.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wds.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eez.guowangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kzn.yonumen.top

[B03] switch / match / case
来源：http://wgz.9152youxi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://glz.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ezy.hysaishi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gxx.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bns.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aya.zycfv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://exa.zdqjudy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://agv.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oln.nwbrower.top

[B04] for 计数循环
来源：http://mrs.fanxiaobao.xyz

Py:   for i in range(10): print(i)
来源：http://gjr.pycfn.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pmg.jqgfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dgv.ivvv.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gqs.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://guq.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rpt.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://fzs.guowangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zhg.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://wzg.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://bit.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qza.hesvh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bxy.cqqwz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mxn.gogol.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zrn.9152youxi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jtj.hnqzz.top

Ruby: arr.each { |item| puts item }
来源：http://fvs.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://liv.fehbvm.com

[B06] 遍历字典 / 对象
来源：http://ugy.0kj1m.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gxp.sjlbkw.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nuv.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ave.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cse.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qjl.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yea.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ech.zdbjq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gmy.zdqjudy.top

[B07] while 循环
来源：http://rnx.hnqzz.top

Py:   while i < 10: i += 1
来源：http://smd.shzxlz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qbv.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://hdg.ehwqpu.com

TS:   while (i < 10) { i++; }
来源：http://bxa.vehdjk.com

Java: while (i < 10) { i++; }
来源：http://sdf.dianchejie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gbt.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://mux.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://tyd.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://kny.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://bqn.52xcode.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hos.jqgfzy.top

JS:   do { i++; } while (i < 10);
来源：http://bbr.hnxiangtu.top

TS:   do { i++; } while (i < 10);
来源：http://uaw.xylfe.cn

Java: do { i++; } while (i < 10);
来源：http://qcc.shuidangran.top

Go:   for { i++; if i >= 10 { break } }
来源：http://oud.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://qvy.pycfn.com

C#:   do { i++; } while (i < 10);
来源：http://hbv.quarkkingdee.top

[B09] break 与 continue
来源：http://apg.yfazqb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jmv.fengsongda.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hhc.gogol.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://csi.mhx1999.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vgn.haohaochexian.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ujy.gaohongyu789.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iii.gotoacloud.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://inr.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sec.xuetiantiany.cn

[B10] 遍历同时拿索引
来源：http://vdl.yuxming.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://awo.birdmap.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qqp.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://klx.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ceq.hammf.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ice.yvedp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wqv.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://alg.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://biw.cucudq.cn

[B11] 生成数字序列 / 区间
来源：http://yvp.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://jdb.zhiwuduotai.top

PHP:  range(0, 10, 2);
来源：http://xsi.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hzs.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ykn.dianchejie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ool.sweek.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fye.yj20258.top

Ruby: (0...10).step(2).to_a
来源：http://pth.sjlbkw.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://efa.xylfe.cn

[B12] 跳出多层循环
来源：http://hwg.9152youxi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hmx.zhoulong.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://evt.aizwys.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yhi.hongshengwenyu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kgw.havefunace.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ufz.zhoulong.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ufq.shanyushiyangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hyg.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vim.jinqigfzy.top

[B13] 判断是否为数字
来源：http://aqg.kuanghao11.cn

Py:   isinstance(x, (int, float))
来源：http://dij.gotoacloud.top

PHP:  is_numeric($x)
来源：http://zkr.iojbl.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dzc.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xxk.uphjek.com

Java: x instanceof Number
来源：http://pzt.zhixingplan.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wqk.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://url.bjfxy.top

C#:   x is int or double or decimal
来源：http://cgr.yvedp.cn

[B14] 判断值是否在集合内
来源：http://iga.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yya.zdqjudy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nps.ctjpmb.com

JS:   [1, 2, 3].includes(x)
来源：http://she.yj20258.top

TS:   [1, 2, 3].includes(x)
来源：http://lsp.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xtl.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hdt.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://qeh.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dqq.xinyue.icu

[B15] 布尔运算与取反
来源：http://jun.cucudq.cn

Py:   a and b or not c
来源：http://wqp.sufxvd.cn

PHP:  $a && $b || !$c
来源：http://cej.haohaochexian.top

JS:   a && b || !c
来源：http://vcn.yuxming.cn

TS:   a && b || !c
来源：http://wvr.fktsv.cn

Java: a && b || !c
来源：http://tqi.fzhhl.top

Go:   a && b || !c
来源：http://pdf.c1oappe.top

Ruby: a && b || !c
来源：http://tqk.yongpay.top

C#:   a && b || !c
来源：http://qdb.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fxf.jqgfzy.top

Py:   if not data: return
来源：http://mxl.yvedp.cn

PHP:  if (!$data) { return; }
来源：http://jaz.yvedp.cn

JS:   if (!data) return;
来源：http://iur.52xcode.cn

TS:   if (!data) return;
来源：http://vma.aizwys.cn

Java: if (data == null) return;
来源：http://kgs.nwbrower.top

Go:   if data == nil { return }
来源：http://que.svipenyu.cn

Ruby: return if data.nil?
来源：http://zxh.pycfn.com

C#:   if (data == null) return;
来源：http://maa.jyoumei.cn

================================================================================
来源：http://hyx.jiagoushi.top

C. 函数与作用域
来源：http://mfv.svipenyu.cn

================================================================================
来源：http://bsu.birdmap.top

[C01] 定义函数
来源：http://txf.yj20258888.top

Py:   def add(a, b): return a + b
来源：http://spl.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hju.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://iym.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yby.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uvo.sjlbkw.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rdu.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://brv.uphjek.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jgk.hnqzz.top

[C02] 默认参数
来源：http://cpc.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://ecu.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wuc.smart0.xyz

JS:   function greet(name = "World") { return name; }
来源：http://mns.c1oappe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dta.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jjo.chenjidiqi.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gye.hfpthk.cn

Ruby: def greet(name = "World") = name
来源：http://hkz.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://igr.gzhubu.top

[C03] 可变参数
来源：http://ruc.guannengcc.top

Py:   def total(*args): return sum(args)
来源：http://lpp.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wnr.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vho.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jjd.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bwr.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mav.shanyushiyangtech.top

Ruby: def total(*nums); nums.sum; end
来源：http://dix.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xqt.shanyushiyangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://bnf.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eov.sjlbkw.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://azj.meibo888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zdw.sjlbkw.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xll.daxiang520.top

Java: // 无：用 Builder 模式或 record
来源：http://sxw.jinqigfzy.top

Go:   // 无：用配置结构体参数
来源：http://kmr.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://tvl.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://hsx.kuanghao11.cn

[C05] 返回多个值
来源：http://arl.zdbjq.cn

Py:   return a, b
来源：http://mcy.xziqi.cn

PHP:  return [$a, $b];
来源：http://hfz.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xky.jinyuanbaomall.cn

TS:   return { a, b };
来源：http://fao.pycfn.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wke.tarul.cn

Go:   return a, b
来源：http://uao.bjfxy.top

Ruby: return a, b
来源：http://nqe.chenzaomai.com

C#:   return (a, b);              // ValueTuple
来源：http://urq.tanke756.top

[C06] 匿名函数 / lambda
来源：http://yzw.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://ucp.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://czr.vehdjk.com

JS:   const square = x => x * x;
来源：http://qsy.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://axt.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tym.xylfe.cn

Go:   sq := func(x int) int { return x * x }
来源：http://owi.iojbl.cn

Ruby: square = ->(x) { x * x }
来源：http://lcg.haohaochexian.top

C#:   Func<int, int> square = x => x * x;
来源：http://fmi.nwbrower.top

[C07] 把函数作为参数传入
来源：http://ewa.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tje.yanxiufei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bzz.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qnu.haohaochexian.top

TS:   arr.map(String)
来源：http://sop.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bnp.yj20258888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pno.ydzc1.top

Ruby: arr.map(&:upcase)
来源：http://pxn.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xab.pengpengdd.cyou

[C08] 闭包
来源：http://mty.xingfuxueyuan.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ttn.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cvy.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wme.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ruj.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ppn.fengsongda.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ecn.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pty.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yyv.bjfxy.top

[C09] 递归
来源：http://mut.cqqwz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lvp.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vjy.xuanzx.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aov.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://woc.xylfe.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hvx.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://soh.chenlongwang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dru.wangshuangyany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zwi.epnwcf.com

[C10] 变量作用域
来源：http://uqu.zhiwuduotai.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jkb.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gdf.quarkkingdee.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gfa.kuanghao11.cn

TS:   同 JS
来源：http://oni.ehwqpu.com

Java: 方法内为块级作用域
来源：http://rnv.pycfn.com

Go:   花括号块级作用域
来源：http://qfh.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pno.yongpay.top

C#:   块级作用域
来源：http://lan.hnxiangtu.top

[C11] 模块导入与导出
来源：http://nyc.jinqigufen.top

Py:   from module import func
来源：http://faq.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sxd.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://ofq.daria6918.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kav.ydzc1.top

Java: import java.util.List;
来源：http://mwp.xingfuxueyuan.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jdh.chenzaomai.com

Ruby: require "json"; require_relative "./util"
来源：http://qzj.fktsv.cn

C#:   using System.Text;
来源：http://oio.shuidangran.top

[C12] 立即执行函数 IIFE
来源：http://lun.gogol.net.cn

Py:   (lambda: print("run"))()
来源：http://iyw.hammf.cn

PHP:  (function () { echo "run"; })();
来源：http://cvh.0kj1m.cn

JS:   (() => { console.log("run"); })();
来源：http://crb.ehwqpu.com

TS:   (() => { console.log("run"); })();
来源：http://jvc.ctjpmb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wuh.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://fon.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://pyn.cashguo.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zzg.aibaodan.cn

[C13] 类型声明 / 类型注解
来源：http://xur.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oau.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jdq.dashuyun.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lan.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tfs.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://zif.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://gwr.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zzh.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://ffb.hesvh.cn

[C14] 泛型函数
来源：http://bsd.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jyf.wangdashe.top

PHP:  // 无泛型
来源：http://gvw.shangyingyoupin.top

JS:   // 无泛型
来源：http://lxb.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uty.yvedp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zml.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vgc.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://hsd.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vpl.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://dce.chenjidiqi.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aiy.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://lhd.xziqi.cn


<!-- 参考信息 -->