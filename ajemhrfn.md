代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wfv.sjlbkw.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wzx.shangyingyoupin.top

[A24] 去除首尾空白
来源：http://rym.chenzaomai.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cgz.xuetiantiany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pok.jyoumei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nkv.zhiwuduotai.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fje.shuidangran.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://stu.redwolf501.top

Go:   strings.TrimSpace(s)
来源：http://psf.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ylk.wangdashe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wgg.dashuyun.cn

[A25] 字符串比较
来源：http://xhz.sweek.top

Py:   s1 == s2; s1 != s2
来源：http://gkm.fzhhl.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wfs.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rmb.yj20258.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yaa.zdqjudy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rwt.sweek.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lva.ydzc1.top

Ruby: s1 == s2; s1 <=> s2
来源：http://pen.xuetiantiany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hap.fehbvm.com

[A26] 类型转换总览
来源：http://dbi.hnxiangtu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ybb.gzhubu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ats.chenzaomai.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fjn.vehdjk.com

TS:   Number() String() Boolean() x as number
来源：http://uzt.jinqigfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qnr.9152youxi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bvp.tian-w.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dcg.vehdjk.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qci.kuanghao11.cn

================================================================================
来源：http://isf.hnxiangtu.top

B. 流程控制
来源：http://qcd.quarkkingdee.top

================================================================================
来源：http://dnu.fehbvm.com

[B01] 条件判断 if / else
来源：http://wqu.zhoulong.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://mes.jqgfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mur.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lsx.jyoumei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fgu.zhongyouzk.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cqx.zhaomingkeji.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eza.hnxiangtu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pss.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ngn.ywan-chungtsiang.top

[B02] 多分支 else if / elif
来源：http://szh.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gzl.sjlbkw.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pir.shanyushiyangkeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gmz.jlsjyb.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ikt.birdmap.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qri.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zze.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iny.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://boi.hesvh.cn

[B03] switch / match / case
来源：http://wtd.iojbl.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pgb.uphjek.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ooa.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tds.xuanzx.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://shj.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nks.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nmp.gzhubu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nau.haohaochexian.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iwe.nanxinkj.top

[B04] for 计数循环
来源：http://bab.yonumen.top

Py:   for i in range(10): print(i)
来源：http://opc.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://igr.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vrf.guowangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nwl.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mob.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://car.zhongyouzk.top

Ruby: 10.times { |i| puts i }
来源：http://uce.ctjpmb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cdp.ctjpmb.com

[B05] 遍历数组 / 列表
来源：http://pzl.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://gxw.sweek.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://axi.ybcxt.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ykg.hfpthk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xor.yuxming.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uch.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iep.hysaishi.cn

Ruby: arr.each { |item| puts item }
来源：http://qau.jqgfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://stj.zhoulong.xyz

[B06] 遍历字典 / 对象
来源：http://lqy.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wbc.vqdsnc.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ygn.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jgs.zhijiandao.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kaf.chenzaomai.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mwu.pycfn.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nus.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ttc.jinqigufen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://toh.yj202588.top

[B07] while 循环
来源：http://hmd.shangyingyoupin.top

Py:   while i < 10: i += 1
来源：http://blo.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://xvg.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://ych.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://pep.zhijiandao.cn

Java: while (i < 10) { i++; }
来源：http://xfs.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sgf.jinghuilouyu.cn

Ruby: while i < 10; i += 1; end
来源：http://zvx.wangshuangyany.cn

C#:   while (i < 10) { i++; }
来源：http://phx.fanxiaobao.xyz

[B08] do-while（至少执行一次）
来源：http://vkb.ydzc1.top

Py:   # 无 do-while：用 while True + break
来源：http://yok.guannengcc.top

PHP:  do { $i++; } while ($i < 10);
来源：http://znk.hysaishi.cn

JS:   do { i++; } while (i < 10);
来源：http://bfk.pycfn.com

TS:   do { i++; } while (i < 10);
来源：http://znw.zhengqikj.top

Java: do { i++; } while (i < 10);
来源：http://emn.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://arn.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rhn.svipenyu.cn

C#:   do { i++; } while (i < 10);
来源：http://pls.yangfankeji.com

[B09] break 与 continue
来源：http://srt.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hxv.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eux.jlsjyb.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://els.daxiang520.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://idz.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zyh.nanxuanxn.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ein.gotoacloud.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dia.meibo888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fmy.316326.xyz

[B10] 遍历同时拿索引
来源：http://iff.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://svt.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qzc.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zwd.hongshengwenyu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mys.vqdsnc.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hea.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kkf.jqgufenzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lit.gotoacloud.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xkj.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://sve.redwolf501.top

Py:   list(range(0, 10, 2))
来源：http://omy.hongshengwenyu.top

PHP:  range(0, 10, 2);
来源：http://keg.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ylb.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ywl.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tdm.yj20258.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fsq.guowangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://oac.shuidangran.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://evk.yfazqb.com

[B12] 跳出多层循环
来源：http://yil.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://ojw.meibo888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://aiq.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lmi.jinqigfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hqx.sjlbkw.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kmg.yvedp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wav.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nue.hysaishi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ntp.jianghu66.top

[B13] 判断是否为数字
来源：http://cun.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://mah.xuanzx.com

PHP:  is_numeric($x)
来源：http://szw.yj202588.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ext.yueranfly.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rhw.jyoumei.cn

Java: x instanceof Number
来源：http://uqt.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jyj.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://wyu.chenzaomai.com

C#:   x is int or double or decimal
来源：http://mai.jianghu66.top

[B14] 判断值是否在集合内
来源：http://bsr.quarkkingdee.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ryo.bbcook.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oae.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://ute.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://bbd.gzhubu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fgc.jinghuilouyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oyw.fehbvm.com

Ruby: [1, 2, 3].include?(x)
来源：http://tsn.tarul.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wqe.gzhubu.top

[B15] 布尔运算与取反
来源：http://bxk.yvedp.cn

Py:   a and b or not c
来源：http://ond.smart0.xyz

PHP:  $a && $b || !$c
来源：http://ogq.zdqjudy.top

JS:   a && b || !c
来源：http://ony.hongshengwenyu.top

TS:   a && b || !c
来源：http://zmv.jinqigufen.top

Java: a && b || !c
来源：http://vby.bjfxy.top

Go:   a && b || !c
来源：http://dwt.tian-w.cn

Ruby: a && b || !c
来源：http://uoj.wangdashe.top

C#:   a && b || !c
来源：http://btg.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://syb.vqdsnc.cn

Py:   if not data: return
来源：http://gnh.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://xdf.meibo888.top

JS:   if (!data) return;
来源：http://ivs.zhaomingkeji.xyz

TS:   if (!data) return;
来源：http://epq.yueranfly.top

Java: if (data == null) return;
来源：http://ull.snrcjt.cn

Go:   if data == nil { return }
来源：http://hai.birdmap.top

Ruby: return if data.nil?
来源：http://vwr.svipenyu.cn

C#:   if (data == null) return;
来源：http://pel.aizwys.cn

================================================================================
来源：http://vio.andypj.xyz

C. 函数与作用域
来源：http://rtt.zhongyouzk.top

================================================================================
来源：http://nkz.daxiang520.top

[C01] 定义函数
来源：http://ifo.yonumen.top

Py:   def add(a, b): return a + b
来源：http://lxx.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zkf.jlsjyb.cn

JS:   function add(a, b) { return a + b; }
来源：http://ila.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bxa.pycfn.com

Java: static int add(int a, int b) { return a + b; }
来源：http://fre.bjfxy.top

Go:   func add(a, b int) int { return a + b }
来源：http://gtk.jlsjyb.cn

Ruby: def add(a, b); a + b; end
来源：http://bhx.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vic.hnxiangtu.top

[C02] 默认参数
来源：http://fwh.iojbl.cn

Py:   def greet(name="World"): return name
来源：http://vxg.jyoumei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zyf.yangfankeji.com

JS:   function greet(name = "World") { return name; }
来源：http://gqe.jqgufenzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rva.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tap.quarkkingdee.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jps.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://scn.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://bmf.guowangkeji.top

[C03] 可变参数
来源：http://bjd.mhx1999.top

Py:   def total(*args): return sum(args)
来源：http://uis.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bcl.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aez.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jau.0kj1m.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://akk.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vxk.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://uhf.hammf.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cpl.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://gtf.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hzb.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://naa.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wqg.chenjidiqi.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fkh.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://udk.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://snm.hnqzz.top

Ruby: f(a: 1, b: 2)
来源：http://znk.yonumen.top

C#:   f(a: 1, b: 2)
来源：http://dmq.vehdjk.com

[C05] 返回多个值
来源：http://jtl.shanyushiyangkeji.top

Py:   return a, b
来源：http://uvn.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://wjh.jqgfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rnr.nwbrower.top

TS:   return { a, b };
来源：http://wnu.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sem.cheryme.top

Go:   return a, b
来源：http://rfb.9152youxi.cn

Ruby: return a, b
来源：http://ulr.aibaodan.cn

C#:   return (a, b);              // ValueTuple
来源：http://vpx.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://rsz.cashguo.top

Py:   square = lambda x: x * x
来源：http://wxz.aizwys.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sqp.fzhhl.top

JS:   const square = x => x * x;
来源：http://dpo.zycfv.cn

TS:   const square = (x: number): number => x * x;
来源：http://kod.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gef.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://zab.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://pem.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://xwb.xziqi.cn

[C07] 把函数作为参数传入
来源：http://rjs.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://poo.quarkkingdee.top

PHP:  array_map("strtoupper", $arr);
来源：http://jmk.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jym.xziqi.cn

TS:   arr.map(String)
来源：http://qrh.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://veu.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dos.c1oappe.top

Ruby: arr.map(&:upcase)
来源：http://poh.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://psb.yanxiufei.cn

[C08] 闭包
来源：http://kki.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://woj.fktsv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vcf.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oyj.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cgv.gaohongyu789.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uzt.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://grg.zdqjudy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ojc.fzhhl.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rsm.dashuyun.cn

[C09] 递归
来源：http://tel.pycfn.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://con.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wiq.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aza.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oiv.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bdv.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zxy.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ogx.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pax.xingfuxueyuan.xyz

[C10] 变量作用域
来源：http://nsa.zdqjudy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xpy.hnqzz.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wfy.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sxl.zhijiandao.cn

TS:   同 JS
来源：http://dhs.tarul.cn

Java: 方法内为块级作用域
来源：http://bzt.havefunace.top

Go:   花括号块级作用域
来源：http://iup.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fhb.cashguo.top

C#:   块级作用域
来源：http://ayq.bbcook.cn

[C11] 模块导入与导出
来源：http://jdb.jiagoushi.top

Py:   from module import func
来源：http://ebp.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ite.vehdjk.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://djs.xingfuxueyuan.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://khi.jyoumei.cn

Java: import java.util.List;
来源：http://acr.sxryk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rem.birdmap.top

Ruby: require "json"; require_relative "./util"
来源：http://ukf.pycfn.com

C#:   using System.Text;
来源：http://ibi.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://paw.cdnleiting.top

Py:   (lambda: print("run"))()
来源：http://ovo.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://pwv.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://ecx.ctjpmb.com

TS:   (() => { console.log("run"); })();
来源：http://vgu.zycfv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://let.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://azs.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://jhu.yj202588.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kxh.ydzc1.top

[C13] 类型声明 / 类型注解
来源：http://naa.52xcode.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gel.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hvz.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yxr.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vgs.jinqigufen.top

Java: int add(int a, int b) { return a + b; }
来源：http://hmb.quarkkingdee.top

Go:   func add(a, b int) int
来源：http://iug.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mtt.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yjh.gzhubu.top

[C14] 泛型函数
来源：http://lvl.yuxming.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fsl.chenjidiqi.icu

PHP:  // 无泛型
来源：http://umk.nanxuanxn.top

JS:   // 无泛型
来源：http://lnf.birdmap.top


<!-- 参考信息 -->