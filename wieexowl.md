代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bhv.guannengcc.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lfa.yangfankeji.com

[A24] 去除首尾空白
来源：http://lod.yfazqb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fqm.cqqwz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ygb.shuidangran.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://msc.tian-w.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ybo.tanke756.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vqy.xziqi.cn

Go:   strings.TrimSpace(s)
来源：http://pfo.hnxiangtu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://enc.epnwcf.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kpj.sufxvd.cn

[A25] 字符串比较
来源：http://pcr.zdbjq.cn

Py:   s1 == s2; s1 != s2
来源：http://zob.jyoumei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fzz.nanxuanxn.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yax.andypj.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vvy.sysykeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ark.nwbrower.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qqt.jianghu66.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rpp.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xvx.tanke756.top

[A26] 类型转换总览
来源：http://ptg.jlsjyb.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mzy.smart0.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vcd.svipenyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mih.jinyuanbaomall.cn

TS:   Number() String() Boolean() x as number
来源：http://qqh.hammf.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yhy.yvedp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vkx.yonumen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://yrk.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qzj.sysykeji.top

================================================================================
来源：http://ery.zhijiandao.cn

B. 流程控制
来源：http://klu.jianghu66.top

================================================================================
来源：http://bbd.dashuyun.cn

[B01] 条件判断 if / else
来源：http://ubl.fzhhl.top

Py:   result = "正" if x > 0 else "非正"
来源：http://pfl.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ere.bbcook.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aca.pycfn.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ydn.yueranfly.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vqj.hnqzz.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dtn.zhongyouzk.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aqv.hfpthk.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lmn.epnwcf.com

[B02] 多分支 else if / elif
来源：http://dht.hongshengwenyu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zin.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ose.cashguo.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kww.bbcook.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxy.jlsjyb.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dxf.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kly.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qat.yj20258.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ggc.tianlin.xyz

[B03] switch / match / case
来源：http://pnh.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ipy.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://grh.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lhk.cucudq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fhd.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dbx.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dci.hongshengwenyu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zka.fengsongda.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://won.sxryk.cn

[B04] for 计数循环
来源：http://get.dianchejie.cn

Py:   for i in range(10): print(i)
来源：http://hcy.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iaa.pengpengdd.cyou

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://imw.jqgufenzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iay.zhongyouzk.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zaz.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rvo.hammf.cn

Ruby: 10.times { |i| puts i }
来源：http://dtl.vqdsnc.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dph.fanxiaobao.xyz

[B05] 遍历数组 / 列表
来源：http://qbl.bbcook.cn

Py:   for item in arr: print(item)
来源：http://kom.fanxiaobao.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://niz.epnwcf.com

JS:   for (const item of arr) { console.log(item); }
来源：http://bow.zdqjudy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://csu.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fyt.aibaodan.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nsy.zhoulong.xyz

Ruby: arr.each { |item| puts item }
来源：http://lnd.yuxming.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qnx.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://zno.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://btj.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xkx.daria6918.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://haa.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wee.svipenyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zuv.wangshuangyany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ylc.bjfxy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fdc.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bos.meibo888.top

[B07] while 循环
来源：http://yyo.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://ggl.mhx1999.top

PHP:  while ($i < 10) { $i++; }
来源：http://yab.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://glq.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://gvj.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://xwr.guannengcc.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ftp.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://pvi.birdmap.top

C#:   while (i < 10) { i++; }
来源：http://xzu.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://nht.daxiang520.top

Py:   # 无 do-while：用 while True + break
来源：http://lxn.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nsw.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://vfn.yueranfly.top

TS:   do { i++; } while (i < 10);
来源：http://wkz.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://vse.feifeiyinyue.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zvc.ydzc1.top

Ruby: begin; i += 1; end while i < 10
来源：http://ljq.chenjidiqi.icu

C#:   do { i++; } while (i < 10);
来源：http://lgh.pycfn.com

[B09] break 与 continue
来源：http://nji.xingfuxueyuan.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ayd.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yew.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pcn.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vsf.yonumen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vhf.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nik.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bes.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xve.bbcook.cn

[B10] 遍历同时拿索引
来源：http://xok.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jvq.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://imd.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sor.daxiang520.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wum.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://poz.316326.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://psm.jianghu66.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jzf.vehdjk.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dun.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://wgt.jqgfzy.top

Py:   list(range(0, 10, 2))
来源：http://grr.jqgfzy.top

PHP:  range(0, 10, 2);
来源：http://ylv.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ezy.hysaishi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ewt.gzhubu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xyy.yonumen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://akp.mhx1999.top

Ruby: (0...10).step(2).to_a
来源：http://wys.yvedp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dzc.hywenlv.cn

[B12] 跳出多层循环
来源：http://etk.fzhhl.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kfz.svipenyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bfw.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bxi.uphjek.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wxo.jinyuanbaomall.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kco.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jhb.wangdashe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sgf.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ayy.fzhhl.top

[B13] 判断是否为数字
来源：http://rov.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://qhe.xylfe.cn

PHP:  is_numeric($x)
来源：http://elg.ydjk.org.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://apv.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vwt.gotoacloud.top

Java: x instanceof Number
来源：http://jci.bjfxy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uhl.kuanghao11.cn

Ruby: x.is_a?(Numeric)
来源：http://rzo.hysaishi.cn

C#:   x is int or double or decimal
来源：http://hpp.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://rbf.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nth.yj202588.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://agc.daria6918.cn

JS:   [1, 2, 3].includes(x)
来源：http://num.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://gxe.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dno.zhiwuduotai.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dgy.birdmap.top

Ruby: [1, 2, 3].include?(x)
来源：http://dsz.cashguo.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vhp.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://kqs.jlsjyb.cn

Py:   a and b or not c
来源：http://brq.ivvv.top

PHP:  $a && $b || !$c
来源：http://lqv.fanxiaobao.xyz

JS:   a && b || !c
来源：http://hna.yj202588.top

TS:   a && b || !c
来源：http://zpl.yuxming.cn

Java: a && b || !c
来源：http://qmk.guannengcc.top

Go:   a && b || !c
来源：http://vhs.andypj.xyz

Ruby: a && b || !c
来源：http://juy.uphjek.com

C#:   a && b || !c
来源：http://byq.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://jzj.zdqjudy.top

Py:   if not data: return
来源：http://bnc.c1oappe.top

PHP:  if (!$data) { return; }
来源：http://qdr.wangdashe.top

JS:   if (!data) return;
来源：http://noi.birdmap.top

TS:   if (!data) return;
来源：http://yxt.ybcxt.top

Java: if (data == null) return;
来源：http://gbo.quarkkingdee.top

Go:   if data == nil { return }
来源：http://opv.hnxiangtu.top

Ruby: return if data.nil?
来源：http://crq.jinqigfzy.top

C#:   if (data == null) return;
来源：http://ydm.hongshengwenyu.top

================================================================================
来源：http://aaq.yj202588.top

C. 函数与作用域
来源：http://ezz.yueranfly.top

================================================================================
来源：http://pkw.jiagoushi.top

[C01] 定义函数
来源：http://vjz.smart0.xyz

Py:   def add(a, b): return a + b
来源：http://xob.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zgv.tian-w.cn

JS:   function add(a, b) { return a + b; }
来源：http://esd.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qdc.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://evl.jiagoushi.top

Go:   func add(a, b int) int { return a + b }
来源：http://kmo.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://hlt.xuanzx.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mwl.ydzc1.top

[C02] 默认参数
来源：http://gil.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://axx.hysaishi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vhs.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://bxx.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tbb.yonumen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dia.sjlbkw.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://brn.fehbvm.com

Ruby: def greet(name = "World") = name
来源：http://khq.tarul.cn

C#:   string Greet(string name = "World") => name;
来源：http://mgy.havefunace.top

[C03] 可变参数
来源：http://wni.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://vph.redwolf501.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qrk.yvedp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hox.yvedp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://llf.yj20258888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wiv.wangshuangyany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dfw.zdqjudy.top

Ruby: def total(*nums); nums.sum; end
来源：http://lhk.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dgm.yj20258.top

[C04] 命名参数 / 关键字参数
来源：http://xrb.quarkkingdee.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hkt.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tcj.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vvy.hammf.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://das.sweek.top

Java: // 无：用 Builder 模式或 record
来源：http://ttg.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://tve.jinyuanbaomall.cn

Ruby: f(a: 1, b: 2)
来源：http://iax.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://mnk.yanxiufei.cn

[C05] 返回多个值
来源：http://sjq.hysaishi.cn

Py:   return a, b
来源：http://maj.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://qda.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://asq.ctjpmb.com

TS:   return { a, b };
来源：http://sip.ctjpmb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kyz.daria6918.cn

Go:   return a, b
来源：http://nuh.nanxinkj.top

Ruby: return a, b
来源：http://dcn.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://zoh.meibo888.top

[C06] 匿名函数 / lambda
来源：http://prr.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://zhk.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://apn.nwbrower.top

JS:   const square = x => x * x;
来源：http://gki.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://spr.bbcook.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://von.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vdk.cheryme.top

Ruby: square = ->(x) { x * x }
来源：http://xgn.gaohongyu789.top

C#:   Func<int, int> square = x => x * x;
来源：http://buz.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://hwo.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gxo.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://vnk.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qvq.zhiwuduotai.top

TS:   arr.map(String)
来源：http://mim.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lsq.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://toe.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://pjc.yuxming.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vga.xziqi.cn

[C08] 闭包
来源：http://vky.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cqp.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xzs.zhiwuduotai.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cih.aizwys.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oai.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mpl.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cyj.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jtw.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pnr.aizwys.cn

[C09] 递归
来源：http://imj.chenjidiqi.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qlb.ivvv.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zbq.gzhubu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mlj.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://skl.jinqigfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rks.xylfe.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jei.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cad.0kj1m.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://anv.xuanzx.com

[C10] 变量作用域
来源：http://evr.yangfankeji.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tcx.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jkf.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dpp.xuetiantiany.cn

TS:   同 JS
来源：http://qkn.daria6918.cn

Java: 方法内为块级作用域
来源：http://got.ehwqpu.com

Go:   花括号块级作用域
来源：http://hfl.tian-w.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nso.yueranfly.top

C#:   块级作用域
来源：http://ctz.tian-w.cn

[C11] 模块导入与导出
来源：http://xit.yongpay.top

Py:   from module import func
来源：http://wrt.zycfv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ufg.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ajg.gogol.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xkb.cucudq.cn

Java: import java.util.List;
来源：http://ojm.iojbl.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jfa.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://bxi.jinqigufen.top

C#:   using System.Text;
来源：http://sjy.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://rjx.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://nmb.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://uyr.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://uez.hammf.cn

TS:   (() => { console.log("run"); })();
来源：http://xsq.pengpengdd.cyou

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uii.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://pwm.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://tqe.meibo888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://woc.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://bki.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ein.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vjw.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qoo.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bsn.redwolf501.top

Java: int add(int a, int b) { return a + b; }
来源：http://sgw.zhixingplan.top

Go:   func add(a, b int) int
来源：http://oqa.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ilg.haohaochexian.top

C#:   int Add(int a, int b) => a + b;
来源：http://ggc.meibo888.top

[C14] 泛型函数
来源：http://yte.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qbr.nanxinkj.top

PHP:  // 无泛型
来源：http://bjr.ybcxt.top

JS:   // 无泛型
来源：http://ynl.52xcode.cn


<!-- 参考信息 -->