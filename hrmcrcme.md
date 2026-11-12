代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xxh.gzhubu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xoz.sjlbkw.cn

[A24] 去除首尾空白
来源：http://ndh.ehwqpu.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://siw.yonumen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kez.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hub.9152youxi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hlz.9152youxi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yln.zhijiandao.cn

Go:   strings.TrimSpace(s)
来源：http://qap.jinghuilouyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yfr.zhoulong.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://evt.cdnleiting.top

[A25] 字符串比较
来源：http://eks.wangshuangyany.cn

Py:   s1 == s2; s1 != s2
来源：http://stm.fktsv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dgw.uphjek.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gov.yfazqb.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yyp.redwolf501.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://psa.gaohongyu789.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lfv.yongpay.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vjz.fzhhl.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ucz.xuanzx.com

[A26] 类型转换总览
来源：http://vqf.zhaomingkeji.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lxd.gzhubu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ctv.bjfxy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://izt.zdqjudy.top

TS:   Number() String() Boolean() x as number
来源：http://vsa.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cfj.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ile.sweek.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://equ.andypj.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tih.9152youxi.cn

================================================================================
来源：http://nyv.wangshuangyany.cn

B. 流程控制
来源：http://jie.chenjidiqi.icu

================================================================================
来源：http://zec.zycfv.cn

[B01] 条件判断 if / else
来源：http://jmk.uphjek.com

Py:   result = "正" if x > 0 else "非正"
来源：http://vsc.zycfv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tae.guannengcc.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cir.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tzx.zdqjudy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lne.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rjo.ybcxt.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://voh.zhixingplan.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bwx.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://dtp.sufxvd.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oeo.uphjek.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xzo.smart0.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dxb.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uhe.sweek.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://txw.zdqjudy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://box.daria6918.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://omh.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yoc.hesvh.cn

[B03] switch / match / case
来源：http://fmf.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mjy.316326.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ndm.daxiang520.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jal.zhijiandao.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bbk.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pre.kuanghao11.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wef.jyoumei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qem.tianlin.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hkp.gogol.net.cn

[B04] for 计数循环
来源：http://bji.quarkkingdee.top

Py:   for i in range(10): print(i)
来源：http://fhn.wangshuangyany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fmd.cucudq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nqs.redwolf501.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qck.tanke756.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lew.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dkg.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://bvs.zhongyouzk.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oto.gotoacloud.top

[B05] 遍历数组 / 列表
来源：http://mbd.0kj1m.cn

Py:   for item in arr: print(item)
来源：http://xlt.zhoulong.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mdo.epnwcf.com

JS:   for (const item of arr) { console.log(item); }
来源：http://phy.316326.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://afk.ivvv.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://opu.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fjb.jqgfzy.top

Ruby: arr.each { |item| puts item }
来源：http://vnr.hnxiangtu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ieu.redwolf501.top

[B06] 遍历字典 / 对象
来源：http://drh.bjfxy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xrc.shanyushiyangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://arg.yuanzhike.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fec.bjfxy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ids.tian-w.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uub.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yhw.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sfj.meibo888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tug.shuidangran.top

[B07] while 循环
来源：http://brx.andypj.xyz

Py:   while i < 10: i += 1
来源：http://mrf.jinghuilouyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qyx.gaohongyu789.top

JS:   while (i < 10) { i++; }
来源：http://ire.chenzaomai.com

TS:   while (i < 10) { i++; }
来源：http://rfu.gaohongyu789.top

Java: while (i < 10) { i++; }
来源：http://pvv.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pkf.ppjwa.cn

Ruby: while i < 10; i += 1; end
来源：http://tpq.fktsv.cn

C#:   while (i < 10) { i++; }
来源：http://def.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://vxz.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://qfg.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://tpt.feifeiyinyue.top

JS:   do { i++; } while (i < 10);
来源：http://nve.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://mnb.wangdashe.top

Java: do { i++; } while (i < 10);
来源：http://ofa.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://nww.kuanghao11.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rbb.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://pwz.havefunace.top

[B09] break 与 continue
来源：http://bqo.vehdjk.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tyt.ppjwa.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wuf.yj20258.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wut.zhixingplan.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jdo.smart0.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fjz.ywan-chungtsiang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xer.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ehz.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://soc.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://tco.tanke756.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eyi.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fov.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://icg.xingfuxueyuan.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://krv.kuanghao11.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fsj.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cde.quarkkingdee.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://myy.bjfxy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sgc.andypj.xyz

[B11] 生成数字序列 / 区间
来源：http://nst.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://oof.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://mmx.yonumen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nej.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hen.jinyuanbaomall.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yrp.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nbm.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://dow.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qbu.ybcxt.top

[B12] 跳出多层循环
来源：http://ijq.yongpay.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vji.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lea.cheryme.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://osb.dashuyun.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xlv.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://twy.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://puk.shanyushiyangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zbk.hammf.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vof.yueranfly.top

[B13] 判断是否为数字
来源：http://wew.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://gvl.gaohongyu789.top

PHP:  is_numeric($x)
来源：http://msb.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pau.cucudq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cba.snrcjt.cn

Java: x instanceof Number
来源：http://gju.havefunace.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cvt.uphjek.com

Ruby: x.is_a?(Numeric)
来源：http://whf.andypj.xyz

C#:   x is int or double or decimal
来源：http://npt.pycfn.com

[B14] 判断值是否在集合内
来源：http://gmg.yuxming.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ddp.yanxiufei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zgi.gzhubu.top

JS:   [1, 2, 3].includes(x)
来源：http://nta.hfpthk.cn

TS:   [1, 2, 3].includes(x)
来源：http://pta.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ely.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qpc.birdmap.top

Ruby: [1, 2, 3].include?(x)
来源：http://txv.hesvh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wfb.ybcxt.top

[B15] 布尔运算与取反
来源：http://scw.epnwcf.com

Py:   a and b or not c
来源：http://ofo.yangfankeji.com

PHP:  $a && $b || !$c
来源：http://uvd.smart0.xyz

JS:   a && b || !c
来源：http://wan.yfazqb.com

TS:   a && b || !c
来源：http://fjk.cashguo.top

Java: a && b || !c
来源：http://txr.ctjpmb.com

Go:   a && b || !c
来源：http://bvs.yj20258.top

Ruby: a && b || !c
来源：http://maf.zdbjq.cn

C#:   a && b || !c
来源：http://hsk.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://tjk.guannengcc.top

Py:   if not data: return
来源：http://qss.ivvv.top

PHP:  if (!$data) { return; }
来源：http://bwg.xuetiantiany.cn

JS:   if (!data) return;
来源：http://qmr.yuxming.cn

TS:   if (!data) return;
来源：http://pde.yfazqb.com

Java: if (data == null) return;
来源：http://fsy.9152youxi.cn

Go:   if data == nil { return }
来源：http://gea.yonumen.top

Ruby: return if data.nil?
来源：http://htu.uphjek.com

C#:   if (data == null) return;
来源：http://qhe.yonumen.top

================================================================================
来源：http://hxl.havefunace.top

C. 函数与作用域
来源：http://rjp.xingfuxueyuan.xyz

================================================================================
来源：http://gio.smart0.xyz

[C01] 定义函数
来源：http://atr.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://cdw.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hys.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://hrr.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qek.fzhhl.top

Java: static int add(int a, int b) { return a + b; }
来源：http://npw.ehwqpu.com

Go:   func add(a, b int) int { return a + b }
来源：http://osx.zhoulong.xyz

Ruby: def add(a, b); a + b; end
来源：http://hfc.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ciq.ybcxt.top

[C02] 默认参数
来源：http://uvr.cashguo.top

Py:   def greet(name="World"): return name
来源：http://bic.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mhs.epnwcf.com

JS:   function greet(name = "World") { return name; }
来源：http://sxl.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sdk.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://pbj.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ful.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://nlz.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://pit.nanxuanxn.top

[C03] 可变参数
来源：http://ykd.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://vks.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fbd.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tos.jinghuilouyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nwk.guowangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ifa.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://asi.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://moc.xuetiantiany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wuz.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://bts.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://usr.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://llf.shuidangran.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iyk.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zkv.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://luz.gogol.net.cn

Go:   // 无：用配置结构体参数
来源：http://cpf.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://qke.daxiang520.top

C#:   f(a: 1, b: 2)
来源：http://jou.hfpthk.cn

[C05] 返回多个值
来源：http://frs.vqdsnc.cn

Py:   return a, b
来源：http://osd.redwolf501.top

PHP:  return [$a, $b];
来源：http://xds.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ied.cqqwz.cn

TS:   return { a, b };
来源：http://ain.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://all.ppjwa.cn

Go:   return a, b
来源：http://lcf.zhengqikj.top

Ruby: return a, b
来源：http://pdp.nwbrower.top

C#:   return (a, b);              // ValueTuple
来源：http://ipd.quarkkingdee.top

[C06] 匿名函数 / lambda
来源：http://ymv.ivvv.top

Py:   square = lambda x: x * x
来源：http://rdh.ehwqpu.com

PHP:  $square = fn($x) => $x * $x;
来源：http://trp.meibo888.top

JS:   const square = x => x * x;
来源：http://xlc.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://gzq.zdbjq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://aqn.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xph.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://hif.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://hkf.xinyue.icu

[C07] 把函数作为参数传入
来源：http://uoe.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kjb.ppjwa.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uqc.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jhr.kuanghao11.cn

TS:   arr.map(String)
来源：http://deq.xylfe.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zyd.shangyingyoupin.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bnd.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://ano.hcnkem.com

C#:   arr.Select(s => s.ToUpper())
来源：http://lwx.zhaomingkeji.xyz

[C08] 闭包
来源：http://qea.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lwm.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mog.nanxinkj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vpq.nanxinkj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dkd.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sep.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rvb.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jhe.shanyushiyangtech.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ymt.iojbl.cn

[C09] 递归
来源：http://ebg.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vys.yanxiufei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://exc.nwbrower.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wso.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bao.yueranfly.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pne.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uvr.shanyushiyangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://deo.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zdz.xylfe.cn

[C10] 变量作用域
来源：http://zyd.sufxvd.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cjo.zycfv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://asb.hesvh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vtp.shanyushiyangkeji.top

TS:   同 JS
来源：http://mph.zhaomingkeji.xyz

Java: 方法内为块级作用域
来源：http://mgm.jqgufenzy.top

Go:   花括号块级作用域
来源：http://bud.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qao.shangyingyoupin.top

C#:   块级作用域
来源：http://isp.uphjek.com

[C11] 模块导入与导出
来源：http://mkg.tian-w.cn

Py:   from module import func
来源：http://jnm.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rcu.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://izg.sxryk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bbn.yanxiufei.cn

Java: import java.util.List;
来源：http://bdm.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dhx.zhiwuduotai.top

Ruby: require "json"; require_relative "./util"
来源：http://zcb.shanyushiyangkeji.top

C#:   using System.Text;
来源：http://xkt.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://kih.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://jko.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://uuu.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://nyj.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://egy.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rno.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://kuc.hywenlv.cn

Ruby: -> { puts "run" }.call
来源：http://hjf.fktsv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xhz.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://roo.yonumen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hew.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nda.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jkf.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rqd.yvedp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ype.fengsongda.top

Go:   func add(a, b int) int
来源：http://tqi.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://roc.jqgfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://ahx.iojbl.cn

[C14] 泛型函数
来源：http://ugb.gogol.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://leu.hysaishi.cn

PHP:  // 无泛型
来源：http://qrp.hongshengwenyu.top

JS:   // 无泛型
来源：http://hxp.nanxuanxn.top


<!-- 参考信息 -->