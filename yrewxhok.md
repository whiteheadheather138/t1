代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://weg.jlsjyb.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uxe.316326.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fju.tianlin.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nis.haohaochexian.top

Go:   strings.TrimSpace(s)
来源：http://yyq.jinyuanbaomall.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://awb.wangdashe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zlk.sufxvd.cn

[A25] 字符串比较
来源：http://scs.ivvv.top

Py:   s1 == s2; s1 != s2
来源：http://obh.chenzaomai.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vtq.ctjpmb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lix.guannengcc.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jws.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mwr.ehwqpu.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hxk.jqgufenzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rzt.snrcjt.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hul.yvedp.cn

[A26] 类型转换总览
来源：http://tcr.zycfv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oeb.hysaishi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cwx.redwolf501.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oqu.jianghu66.top

TS:   Number() String() Boolean() x as number
来源：http://ibr.gogol.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://syv.tarul.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zfe.jqgufenzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nxi.0kj1m.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hxa.zhoulong.xyz

================================================================================
来源：http://wxd.hysaishi.cn

B. 流程控制
来源：http://jkd.yfazqb.com

================================================================================
来源：http://pml.wangdashe.top

[B01] 条件判断 if / else
来源：http://ulj.hammf.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bao.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xdi.yuanzhike.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://plg.pengpengdd.cyou

TS:   const r = x > 0 ? "正" : "非正";
来源：http://byq.sjlbkw.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://eps.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://irt.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vsg.nanxuanxn.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fbg.hywenlv.cn

[B02] 多分支 else if / elif
来源：http://vqq.chenzaomai.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ngy.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gtp.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://grc.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ccg.yueranfly.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ltn.fengsongda.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fwp.xuanzx.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qos.yj202588.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://irr.yanxiufei.cn

[B03] switch / match / case
来源：http://dgc.yuanzhike.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://crz.ywan-chungtsiang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://duw.iojbl.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fpd.zhengqikj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tzm.zhaomingkeji.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tnn.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tip.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://emi.zhijiandao.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://igk.cucudq.cn

[B04] for 计数循环
来源：http://zpm.yangfankeji.com

Py:   for i in range(10): print(i)
来源：http://xdg.jlsjyb.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://itc.ehwqpu.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://elw.jinghuilouyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sgg.hammf.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kls.hnqzz.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uko.cashguo.top

Ruby: 10.times { |i| puts i }
来源：http://hza.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mja.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://hcg.yongpay.top

Py:   for item in arr: print(item)
来源：http://mah.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xya.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fif.xingfuxueyuan.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://raj.hnxiangtu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ouj.jiagoushi.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aup.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://yqw.hywenlv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ncw.mhx1999.top

[B06] 遍历字典 / 对象
来源：http://jih.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://usv.dianchejie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aoe.nanxinkj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zqb.andypj.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jto.feifeiyinyue.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dgq.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zjn.chenjidiqi.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bzv.yj20258888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wil.fzhhl.top

[B07] while 循环
来源：http://dbn.bbcook.cn

Py:   while i < 10: i += 1
来源：http://jnc.jqgufenzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://eel.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://ske.hongshengwenyu.top

TS:   while (i < 10) { i++; }
来源：http://hkx.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://qwi.jiagoushi.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vii.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://djt.yueranfly.top

C#:   while (i < 10) { i++; }
来源：http://kps.meibo888.top

[B08] do-while（至少执行一次）
来源：http://odq.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://gph.birdmap.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jgo.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://tni.cqqwz.cn

TS:   do { i++; } while (i < 10);
来源：http://brq.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://dba.hcnkem.com

Go:   for { i++; if i >= 10 { break } }
来源：http://hcs.cheryme.top

Ruby: begin; i += 1; end while i < 10
来源：http://oig.52xcode.cn

C#:   do { i++; } while (i < 10);
来源：http://yot.kuanghao11.cn

[B09] break 与 continue
来源：http://jhs.hammf.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tkd.sweek.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://drm.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zih.smart0.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pgv.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qhd.cdnleiting.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://amx.dianchejie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pvm.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://joa.wangshuangyany.cn

[B10] 遍历同时拿索引
来源：http://svv.uphjek.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xww.jinyuanbaomall.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://emb.chenlongwang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://usr.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cmx.shanyushiyangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mpw.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xkc.zycfv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ccs.zdqjudy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iel.fzhhl.top

[B11] 生成数字序列 / 区间
来源：http://fsj.jinqigfzy.top

Py:   list(range(0, 10, 2))
来源：http://ysb.hnqzz.top

PHP:  range(0, 10, 2);
来源：http://zyo.fzhhl.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dfo.pycfn.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lxk.cdnleiting.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dey.yfazqb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mvx.tianlin.xyz

Ruby: (0...10).step(2).to_a
来源：http://mvb.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tpg.hysaishi.cn

[B12] 跳出多层循环
来源：http://sla.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://kvm.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vmh.jinyuanbaomall.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://feu.ydjk.org.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://thl.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://voc.xinyue.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sge.gzhubu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rus.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://haq.cucudq.cn

[B13] 判断是否为数字
来源：http://pir.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://kyq.chenzaomai.com

PHP:  is_numeric($x)
来源：http://igi.yanxiufei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kyu.9152youxi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bps.daxiang520.top

Java: x instanceof Number
来源：http://def.jiagoushi.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xnh.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://enb.meibo888.top

C#:   x is int or double or decimal
来源：http://njt.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://xtj.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iah.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qli.smart0.xyz

JS:   [1, 2, 3].includes(x)
来源：http://oig.jiagoushi.top

TS:   [1, 2, 3].includes(x)
来源：http://cjr.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vyk.chenjidiqi.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gsf.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ukw.jiagoushi.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ytn.bjfxy.top

[B15] 布尔运算与取反
来源：http://fgi.nanxuanxn.top

Py:   a and b or not c
来源：http://wsn.fzhhl.top

PHP:  $a && $b || !$c
来源：http://zfv.hongshengwenyu.top

JS:   a && b || !c
来源：http://yop.tarul.cn

TS:   a && b || !c
来源：http://owd.shangyingyoupin.top

Java: a && b || !c
来源：http://arw.cucudq.cn

Go:   a && b || !c
来源：http://eun.haohaochexian.top

Ruby: a && b || !c
来源：http://sul.fktsv.cn

C#:   a && b || !c
来源：http://ynn.cqqwz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yrr.cqqwz.cn

Py:   if not data: return
来源：http://ixe.ywan-chungtsiang.top

PHP:  if (!$data) { return; }
来源：http://ler.uphjek.com

JS:   if (!data) return;
来源：http://awr.ydzc1.top

TS:   if (!data) return;
来源：http://xac.hesvh.cn

Java: if (data == null) return;
来源：http://ghi.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://vhu.zhoulong.xyz

Ruby: return if data.nil?
来源：http://lxn.xziqi.cn

C#:   if (data == null) return;
来源：http://vgk.jinqigufen.top

================================================================================
来源：http://xca.yuxming.cn

C. 函数与作用域
来源：http://biy.yonumen.top

================================================================================
来源：http://ehj.sjlbkw.cn

[C01] 定义函数
来源：http://mzb.jianghu66.top

Py:   def add(a, b): return a + b
来源：http://oaf.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oht.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://ipv.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gyr.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://xhe.yj202588.top

Go:   func add(a, b int) int { return a + b }
来源：http://hja.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://rhr.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nmp.tian-w.cn

[C02] 默认参数
来源：http://qat.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://huk.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ssf.52xcode.cn

JS:   function greet(name = "World") { return name; }
来源：http://iwq.0kj1m.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gkn.cdnleiting.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rhy.ehwqpu.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://npn.jqgufenzy.top

Ruby: def greet(name = "World") = name
来源：http://iap.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://wbl.redwolf501.top

[C03] 可变参数
来源：http://mjo.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://dsz.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fxi.yvedp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hjy.zycfv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hza.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ofq.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xzz.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://rpa.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nki.ywan-chungtsiang.top

[C04] 命名参数 / 关键字参数
来源：http://tnx.aibaodan.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ykc.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wwi.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vox.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bke.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://tol.meibo888.top

Go:   // 无：用配置结构体参数
来源：http://rvh.fehbvm.com

Ruby: f(a: 1, b: 2)
来源：http://elc.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://kia.ppjwa.cn

[C05] 返回多个值
来源：http://vew.tanke756.top

Py:   return a, b
来源：http://cpg.sxryk.cn

PHP:  return [$a, $b];
来源：http://tks.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://lpy.hammf.cn

TS:   return { a, b };
来源：http://pxv.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qhv.fehbvm.com

Go:   return a, b
来源：http://jal.guowangkeji.top

Ruby: return a, b
来源：http://gnj.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://jsp.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://wer.bbcook.cn

Py:   square = lambda x: x * x
来源：http://obd.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jgn.tianlin.xyz

JS:   const square = x => x * x;
来源：http://hmm.fehbvm.com

TS:   const square = (x: number): number => x * x;
来源：http://qob.chenjidiqi.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bel.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://vsw.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://yvv.havefunace.top

C#:   Func<int, int> square = x => x * x;
来源：http://evx.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://dqa.zhiwuduotai.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wpy.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kbx.shuidangran.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qux.guannengcc.top

TS:   arr.map(String)
来源：http://zim.birdmap.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nrv.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wgu.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://wul.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ztk.jinqigfzy.top

[C08] 闭包
来源：http://auv.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rjg.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pez.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://miv.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pti.tanke756.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rkb.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bee.xinyue.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rce.sysykeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://anm.tarul.cn

[C09] 递归
来源：http://dgx.chenlongwang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uls.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mob.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gqw.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yin.gotoacloud.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bjj.dianchejie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ebb.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nld.gaohongyu789.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tmt.tian-w.cn

[C10] 变量作用域
来源：http://sjd.jyoumei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://whg.zhaomingkeji.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jhk.gaohongyu789.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uad.hnxiangtu.top

TS:   同 JS
来源：http://ism.fktsv.cn

Java: 方法内为块级作用域
来源：http://dpa.fanxiaobao.xyz

Go:   花括号块级作用域
来源：http://dqc.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yev.xuanzx.com

C#:   块级作用域
来源：http://dsh.vehdjk.com

[C11] 模块导入与导出
来源：http://eek.smart0.xyz

Py:   from module import func
来源：http://wxb.redwolf501.top

PHP:  require "file.php";  或 use App\Service;
来源：http://afc.gotoacloud.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://isu.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dqv.fehbvm.com

Java: import java.util.List;
来源：http://uix.havefunace.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hwn.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://apu.smart0.xyz

C#:   using System.Text;
来源：http://bhd.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://iyr.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://hfg.52xcode.cn

PHP:  (function () { echo "run"; })();
来源：http://ybi.aibaodan.cn

JS:   (() => { console.log("run"); })();
来源：http://dnr.xziqi.cn

TS:   (() => { console.log("run"); })();
来源：http://obu.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zrp.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://voc.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://env.xinyue.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://qlw.guowangkeji.top

[C13] 类型声明 / 类型注解
来源：http://ggm.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ncq.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pbx.smart0.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lum.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jqx.yj20258.top

Java: int add(int a, int b) { return a + b; }
来源：http://vaf.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://kti.yuanzhike.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zlu.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://rmb.tianlin.xyz

[C14] 泛型函数
来源：http://hfi.jyoumei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://epn.xuanzx.com

PHP:  // 无泛型
来源：http://oyi.zhongyouzk.top

JS:   // 无泛型
来源：http://uyf.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dgp.havefunace.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jhq.0kj1m.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mix.xziqi.cn

Ruby: # 无泛型
来源：http://zxn.uphjek.com


<!-- 参考信息 -->