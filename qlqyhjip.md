代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://olz.yuanzhike.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cya.guowangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yeo.zdbjq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ppm.316326.xyz

Go:   strings.TrimSpace(s)
来源：http://nxt.yj20258888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yjn.shanyushiyangtech.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rku.yangfankeji.com

[A25] 字符串比较
来源：http://bvg.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://irr.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fob.c1oappe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qzs.jlsjyb.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dmp.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xpa.pycfn.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cmw.yj20258888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tix.haohaochexian.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ked.kuanghao11.cn

[A26] 类型转换总览
来源：http://zsa.xinyue.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qga.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zxa.aizwys.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cnh.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://ouq.dianchejie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sjt.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mae.hysaishi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gsf.hcnkem.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bua.jinghuilouyu.cn

================================================================================
来源：http://yoe.cheryme.top

B. 流程控制
来源：http://nqy.ctjpmb.com

================================================================================
来源：http://ayg.yvedp.cn

[B01] 条件判断 if / else
来源：http://pyd.jinqigfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://iwr.havefunace.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://trc.yueranfly.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zdo.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wdo.xinyue.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://hkd.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nba.cheryme.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sxx.jinyuanbaomall.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mpe.jinqigufen.top

[B02] 多分支 else if / elif
来源：http://jsj.yonumen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xsf.yfazqb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ege.bbcook.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vvy.epnwcf.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gni.nanxinkj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rzr.hnqzz.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://syx.bjfxy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jxj.zhixingplan.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://czn.nanxuanxn.top

[B03] switch / match / case
来源：http://lrq.ydjk.org.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eph.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://okl.guowangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hkr.tianlin.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wtw.epnwcf.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ixt.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qif.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://krh.sweek.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ceu.xinyue.icu

[B04] for 计数循环
来源：http://iej.0kj1m.cn

Py:   for i in range(10): print(i)
来源：http://sue.wangshuangyany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ble.birdmap.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cey.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qfh.zhiwuduotai.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bgk.316326.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wub.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://crd.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rpk.yangfankeji.com

[B05] 遍历数组 / 列表
来源：http://puu.yj202588.top

Py:   for item in arr: print(item)
来源：http://rtv.sysykeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vsj.xuetiantiany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gui.yvedp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mtr.cucudq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ibk.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qxt.yuxming.cn

Ruby: arr.each { |item| puts item }
来源：http://jab.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bpq.chenzaomai.com

[B06] 遍历字典 / 对象
来源：http://yle.jlsjyb.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qgl.feifeiyinyue.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wqn.shanyushiyangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://far.havefunace.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mxq.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://utg.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bhx.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fsi.ehwqpu.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gcf.gotoacloud.top

[B07] while 循环
来源：http://zip.zhoulong.xyz

Py:   while i < 10: i += 1
来源：http://xvo.sweek.top

PHP:  while ($i < 10) { $i++; }
来源：http://upa.guannengcc.top

JS:   while (i < 10) { i++; }
来源：http://yfr.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://hdr.jinqigufen.top

Java: while (i < 10) { i++; }
来源：http://acw.epnwcf.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wnx.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://lcl.bjfxy.top

C#:   while (i < 10) { i++; }
来源：http://xii.aizwys.cn

[B08] do-while（至少执行一次）
来源：http://rqy.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://mov.shangyingyoupin.top

PHP:  do { $i++; } while ($i < 10);
来源：http://sxt.jiagoushi.top

JS:   do { i++; } while (i < 10);
来源：http://kri.tian-w.cn

TS:   do { i++; } while (i < 10);
来源：http://uaz.zhijiandao.cn

Java: do { i++; } while (i < 10);
来源：http://bwv.sufxvd.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zmy.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://syd.yongpay.top

C#:   do { i++; } while (i < 10);
来源：http://xqw.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://jbx.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xwi.snrcjt.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gkx.jqgfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ggq.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lck.316326.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rwh.nwbrower.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hsf.shuidangran.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aar.0kj1m.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bqz.wangdashe.top

[B10] 遍历同时拿索引
来源：http://tom.chenlongwang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://keg.fanxiaobao.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lue.xingfuxueyuan.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cqx.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tlc.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lgo.xingfuxueyuan.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wth.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://psc.pycfn.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://edz.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://xmv.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://hwk.cheryme.top

PHP:  range(0, 10, 2);
来源：http://rfn.hesvh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://odo.sysykeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ugz.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://try.svipenyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bhp.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://cpj.mhx1999.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ujv.fengsongda.top

[B12] 跳出多层循环
来源：http://tje.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nbe.redwolf501.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fab.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zcz.ivvv.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gmb.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zxp.chenjidiqi.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wal.snrcjt.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pjg.snrcjt.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ddk.ehwqpu.com

[B13] 判断是否为数字
来源：http://zem.jinghuilouyu.cn

Py:   isinstance(x, (int, float))
来源：http://sme.fktsv.cn

PHP:  is_numeric($x)
来源：http://rwn.gaohongyu789.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gmc.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tqz.hfpthk.cn

Java: x instanceof Number
来源：http://zht.daria6918.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gsa.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://iik.ivvv.top

C#:   x is int or double or decimal
来源：http://lcg.fehbvm.com

[B14] 判断值是否在集合内
来源：http://qje.hywenlv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cvg.cdnleiting.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xzc.nanxinkj.top

JS:   [1, 2, 3].includes(x)
来源：http://obp.nanxuanxn.top

TS:   [1, 2, 3].includes(x)
来源：http://wfw.jyoumei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lkv.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lvc.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tzt.jyoumei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fwl.dianchejie.cn

[B15] 布尔运算与取反
来源：http://git.xuetiantiany.cn

Py:   a and b or not c
来源：http://cib.sjlbkw.cn

PHP:  $a && $b || !$c
来源：http://ttg.yj20258888.top

JS:   a && b || !c
来源：http://nov.birdmap.top

TS:   a && b || !c
来源：http://veo.sjlbkw.cn

Java: a && b || !c
来源：http://wuh.fktsv.cn

Go:   a && b || !c
来源：http://ibl.vqdsnc.cn

Ruby: a && b || !c
来源：http://fjy.tian-w.cn

C#:   a && b || !c
来源：http://efd.xingfuxueyuan.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ken.wangdashe.top

Py:   if not data: return
来源：http://dai.tanke756.top

PHP:  if (!$data) { return; }
来源：http://blc.chenlongwang.top

JS:   if (!data) return;
来源：http://nsz.yj202588.top

TS:   if (!data) return;
来源：http://eoq.wangshuangyany.cn

Java: if (data == null) return;
来源：http://jod.gogol.net.cn

Go:   if data == nil { return }
来源：http://qbo.yj20258888.top

Ruby: return if data.nil?
来源：http://bkn.xingfuxueyuan.xyz

C#:   if (data == null) return;
来源：http://rbc.ppjwa.cn

================================================================================
来源：http://tjw.dashuyun.cn

C. 函数与作用域
来源：http://cru.jqgfzy.top

================================================================================
来源：http://gxa.vehdjk.com

[C01] 定义函数
来源：http://bqo.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://pqe.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bop.aizwys.cn

JS:   function add(a, b) { return a + b; }
来源：http://fgo.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://clt.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nez.ydjk.org.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fzi.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://ezl.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lpc.aibaodan.cn

[C02] 默认参数
来源：http://jws.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://wan.jlsjyb.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zhh.yuxming.cn

JS:   function greet(name = "World") { return name; }
来源：http://ybp.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://oim.sxryk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bgd.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ias.ydzc1.top

Ruby: def greet(name = "World") = name
来源：http://edf.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://vog.zdbjq.cn

[C03] 可变参数
来源：http://ziv.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://uil.jqgufenzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qdb.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fqb.shanyushiyangtech.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ova.shanyushiyangtech.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eoh.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sat.zhijiandao.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gcb.mhx1999.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://efz.jyoumei.cn

[C04] 命名参数 / 关键字参数
来源：http://lfh.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zst.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ica.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vfg.jiagoushi.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vhb.sufxvd.cn

Java: // 无：用 Builder 模式或 record
来源：http://swg.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://lpw.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://gbh.nanxuanxn.top

C#:   f(a: 1, b: 2)
来源：http://efw.jqgufenzy.top

[C05] 返回多个值
来源：http://fub.yanxiufei.cn

Py:   return a, b
来源：http://ssn.zhengqikj.top

PHP:  return [$a, $b];
来源：http://nvo.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tkv.cqqwz.cn

TS:   return { a, b };
来源：http://dfa.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://njg.nanxuanxn.top

Go:   return a, b
来源：http://znb.0kj1m.cn

Ruby: return a, b
来源：http://naa.hongshengwenyu.top

C#:   return (a, b);              // ValueTuple
来源：http://mps.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://xbu.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://dve.hysaishi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hld.zdqjudy.top

JS:   const square = x => x * x;
来源：http://qnu.daxiang520.top

TS:   const square = (x: number): number => x * x;
来源：http://cou.bjfxy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ggq.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nmv.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://ldq.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://uzl.sjlbkw.cn

[C07] 把函数作为参数传入
来源：http://rvg.jqgfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oqb.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://isj.shanyushiyangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ryw.chenzaomai.com

TS:   arr.map(String)
来源：http://srt.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kkx.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qdx.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://rwi.c1oappe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vqu.redwolf501.top

[C08] 闭包
来源：http://fuj.jqgfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zps.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dvu.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mrt.chenzaomai.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ikr.chenlongwang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ykd.shangyingyoupin.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cbc.yfazqb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://efi.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pau.cucudq.cn

[C09] 递归
来源：http://ivm.yangfankeji.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vqi.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bhf.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://spi.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://emv.gzhubu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://shg.ydjk.org.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tru.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xsm.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cou.hnxiangtu.top

[C10] 变量作用域
来源：http://akm.iojbl.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kms.zhongyouzk.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fvm.c1oappe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sae.316326.xyz

TS:   同 JS
来源：http://rln.svipenyu.cn

Java: 方法内为块级作用域
来源：http://xrw.zhongyouzk.top

Go:   花括号块级作用域
来源：http://lrq.pycfn.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kdl.mhx1999.top

C#:   块级作用域
来源：http://unm.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://qox.dashuyun.cn

Py:   from module import func
来源：http://ftp.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dhr.yj20258.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://iol.iojbl.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oum.sweek.top

Java: import java.util.List;
来源：http://hca.52xcode.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ogn.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://npe.epnwcf.com

C#:   using System.Text;
来源：http://tza.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://cnz.dashuyun.cn

Py:   (lambda: print("run"))()
来源：http://jjs.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://nao.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://wix.ydjk.org.cn

TS:   (() => { console.log("run"); })();
来源：http://lva.vehdjk.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://snc.chenlongwang.top

Go:   func() { fmt.Println("run") }()
来源：http://bkx.yvedp.cn

Ruby: -> { puts "run" }.call
来源：http://kqn.chenzaomai.com

C#:   // 无 IIFE：用静态构造函数
来源：http://nrd.xuetiantiany.cn

[C13] 类型声明 / 类型注解
来源：http://qhn.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lrv.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wyi.guowangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://enz.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vhc.sufxvd.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mae.kuanghao11.cn

Go:   func add(a, b int) int
来源：http://bgz.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wjt.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nno.c1oappe.top

[C14] 泛型函数
来源：http://twk.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://loz.yvedp.cn

PHP:  // 无泛型
来源：http://qrx.fzhhl.top

JS:   // 无泛型
来源：http://ayt.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bqe.feifeiyinyue.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://obg.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ate.yj20258888.top

Ruby: # 无泛型
来源：http://fgx.cqqwz.cn


<!-- 参考信息 -->