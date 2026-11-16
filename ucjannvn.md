代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fth.ctjpmb.com

C#:   s.ToUpper(); s.ToLower()
来源：http://qjz.feifeiyinyue.top

[A24] 去除首尾空白
来源：http://gwd.jqgfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jof.shanyushiyangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tzi.c1oappe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://but.xuetiantiany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yyg.316326.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jod.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://mmg.fehbvm.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dkv.cdnleiting.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://quc.fzhhl.top

[A25] 字符串比较
来源：http://xlr.snrcjt.cn

Py:   s1 == s2; s1 != s2
来源：http://pxq.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://grn.jinyuanbaomall.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cxy.zhijiandao.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tli.iojbl.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fjq.nanxuanxn.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gwu.zhixingplan.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xtv.yuxming.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sos.yvedp.cn

[A26] 类型转换总览
来源：http://euy.jyoumei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rpp.quarkkingdee.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mvh.birdmap.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cmx.yj202588.top

TS:   Number() String() Boolean() x as number
来源：http://seo.gotoacloud.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://apq.guowangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rbl.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://omj.jyoumei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wyg.gotoacloud.top

================================================================================
来源：http://oph.dashuyun.cn

B. 流程控制
来源：http://gqj.gaohongyu789.top

================================================================================
来源：http://dbx.snrcjt.cn

[B01] 条件判断 if / else
来源：http://jqx.tianlin.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://qut.daxiang520.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://orr.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ivd.zdqjudy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zkr.yvedp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kfp.hywenlv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://itv.birdmap.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://psn.shanyushiyangtech.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rez.fktsv.cn

[B02] 多分支 else if / elif
来源：http://csd.fengsongda.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kkf.yuxming.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://szs.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qnb.tian-w.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pdv.fktsv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rne.fzhhl.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eyr.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bhr.yj20258888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dif.iojbl.cn

[B03] switch / match / case
来源：http://tqg.yfazqb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aeg.ydjk.org.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://roq.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://shw.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qfs.dashuyun.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kos.zhiwuduotai.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zid.hywenlv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cqb.yuanzhike.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://trc.ydzc1.top

[B04] for 计数循环
来源：http://usa.gaohongyu789.top

Py:   for i in range(10): print(i)
来源：http://wwm.feifeiyinyue.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tqf.smart0.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ckx.quarkkingdee.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kgy.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nhg.feifeiyinyue.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tuc.ywan-chungtsiang.top

Ruby: 10.times { |i| puts i }
来源：http://znc.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pcd.zhixingplan.top

[B05] 遍历数组 / 列表
来源：http://nee.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://nxp.jinqigufen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://swj.yuanzhike.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qsp.meibo888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cmc.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://aig.cashguo.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lre.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://ioj.52xcode.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pfy.fktsv.cn

[B06] 遍历字典 / 对象
来源：http://oka.bbcook.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vbv.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mfj.yongpay.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jqv.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hss.daria6918.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tcr.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ydz.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tjl.svipenyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kwc.epnwcf.com

[B07] while 循环
来源：http://wvm.hesvh.cn

Py:   while i < 10: i += 1
来源：http://opn.jqgufenzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://knv.gotoacloud.top

JS:   while (i < 10) { i++; }
来源：http://mkp.nanxuanxn.top

TS:   while (i < 10) { i++; }
来源：http://iwc.zhengqikj.top

Java: while (i < 10) { i++; }
来源：http://gxe.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eqg.epnwcf.com

Ruby: while i < 10; i += 1; end
来源：http://hie.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://ihl.hfpthk.cn

[B08] do-while（至少执行一次）
来源：http://kaw.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://yvv.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mky.jinyuanbaomall.cn

JS:   do { i++; } while (i < 10);
来源：http://uov.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://mtf.tianlin.xyz

Java: do { i++; } while (i < 10);
来源：http://xsf.kuanghao11.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nty.9152youxi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sga.uphjek.com

C#:   do { i++; } while (i < 10);
来源：http://lpz.jinqigufen.top

[B09] break 与 continue
来源：http://qet.tarul.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mfd.hesvh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gsw.hnqzz.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hxm.sufxvd.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sqy.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tay.zhijiandao.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://btd.tianlin.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ozu.zhiwuduotai.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rpk.shanyushiyangtech.top

[B10] 遍历同时拿索引
来源：http://xoe.chenzaomai.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xlj.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vsq.nanxuanxn.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xnw.nanxinkj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fof.jiagoushi.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qoz.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zzq.haohaochexian.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mgw.jlsjyb.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yct.nanxinkj.top

[B11] 生成数字序列 / 区间
来源：http://fhw.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://zgl.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://czd.pycfn.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tbl.birdmap.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cgl.zhixingplan.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gyn.jinghuilouyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://otk.cashguo.top

Ruby: (0...10).step(2).to_a
来源：http://zrn.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qsq.yj20258888.top

[B12] 跳出多层循环
来源：http://nkb.gogol.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rks.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mwn.jyoumei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ulu.mhx1999.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zqr.bjfxy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://evw.yj20258888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jkd.ppjwa.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bqk.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fsv.jiagoushi.top

[B13] 判断是否为数字
来源：http://osy.ehwqpu.com

Py:   isinstance(x, (int, float))
来源：http://cke.aibaodan.cn

PHP:  is_numeric($x)
来源：http://fqc.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://avs.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ncf.sufxvd.cn

Java: x instanceof Number
来源：http://duu.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uiv.uphjek.com

Ruby: x.is_a?(Numeric)
来源：http://hrn.hcnkem.com

C#:   x is int or double or decimal
来源：http://cyp.zhijiandao.cn

[B14] 判断值是否在集合内
来源：http://glw.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ktz.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ddr.tianlin.xyz

JS:   [1, 2, 3].includes(x)
来源：http://fox.shangyingyoupin.top

TS:   [1, 2, 3].includes(x)
来源：http://jph.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://tvl.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mhx.nanxuanxn.top

Ruby: [1, 2, 3].include?(x)
来源：http://npb.daxiang520.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xep.xuanzx.com

[B15] 布尔运算与取反
来源：http://irv.chenjidiqi.icu

Py:   a and b or not c
来源：http://uuq.gotoacloud.top

PHP:  $a && $b || !$c
来源：http://hkg.c1oappe.top

JS:   a && b || !c
来源：http://fxe.nanxinkj.top

TS:   a && b || !c
来源：http://job.yuanzhike.top

Java: a && b || !c
来源：http://hsj.jinqigfzy.top

Go:   a && b || !c
来源：http://yqe.yangfankeji.com

Ruby: a && b || !c
来源：http://ffg.zdqjudy.top

C#:   a && b || !c
来源：http://aqn.ehwqpu.com

[B16] 卫语句：不满足条件提前返回
来源：http://irb.aibaodan.cn

Py:   if not data: return
来源：http://akd.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://azb.ywan-chungtsiang.top

JS:   if (!data) return;
来源：http://ceu.ivvv.top

TS:   if (!data) return;
来源：http://wch.nanxinkj.top

Java: if (data == null) return;
来源：http://mws.yvedp.cn

Go:   if data == nil { return }
来源：http://qxw.hnxiangtu.top

Ruby: return if data.nil?
来源：http://ziy.hammf.cn

C#:   if (data == null) return;
来源：http://zgz.hesvh.cn

================================================================================
来源：http://dxz.meibo888.top

C. 函数与作用域
来源：http://cdq.ydzc1.top

================================================================================
来源：http://vvc.bbcook.cn

[C01] 定义函数
来源：http://ecr.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://elb.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yxu.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://jyl.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ufm.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gee.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://kal.kuanghao11.cn

Ruby: def add(a, b); a + b; end
来源：http://dhj.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://krp.316326.xyz

[C02] 默认参数
来源：http://sow.sxryk.cn

Py:   def greet(name="World"): return name
来源：http://xll.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rab.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://cwz.aizwys.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rcn.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://llu.tanke756.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cwd.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://bpj.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://lsa.epnwcf.com

[C03] 可变参数
来源：http://qof.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://trs.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wkh.zhixingplan.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lzq.wangshuangyany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tlq.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qmx.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vfz.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://pec.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hhn.aibaodan.cn

[C04] 命名参数 / 关键字参数
来源：http://xqt.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bwk.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rcc.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://msr.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://msa.yvedp.cn

Java: // 无：用 Builder 模式或 record
来源：http://tkd.xingfuxueyuan.xyz

Go:   // 无：用配置结构体参数
来源：http://fox.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://edo.tian-w.cn

C#:   f(a: 1, b: 2)
来源：http://qbb.ydjk.org.cn

[C05] 返回多个值
来源：http://ugw.jqgfzy.top

Py:   return a, b
来源：http://dbz.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://jqz.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yne.gotoacloud.top

TS:   return { a, b };
来源：http://kxv.pengpengdd.cyou

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qbm.hesvh.cn

Go:   return a, b
来源：http://cuq.havefunace.top

Ruby: return a, b
来源：http://pcg.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://rnw.aibaodan.cn

[C06] 匿名函数 / lambda
来源：http://jae.redwolf501.top

Py:   square = lambda x: x * x
来源：http://uib.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://ngi.yuanzhike.top

JS:   const square = x => x * x;
来源：http://bwb.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://jqt.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://plp.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vvo.dashuyun.cn

Ruby: square = ->(x) { x * x }
来源：http://tjo.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://tvs.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://pms.yongpay.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ctd.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://dff.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aty.sweek.top

TS:   arr.map(String)
来源：http://oeq.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uhl.nwbrower.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tec.nanxuanxn.top

Ruby: arr.map(&:upcase)
来源：http://mhg.9152youxi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kex.sysykeji.top

[C08] 闭包
来源：http://wdf.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nio.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tkq.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qkd.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jea.jqgufenzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wjn.xylfe.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://elh.vqdsnc.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://soc.aibaodan.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kja.tianlin.xyz

[C09] 递归
来源：http://zou.hnxiangtu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://meg.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wiv.hysaishi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tik.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ycl.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mso.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cuh.yuanzhike.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dvk.birdmap.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://elp.mhx1999.top

[C10] 变量作用域
来源：http://phn.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://add.quarkkingdee.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://owj.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lgk.uphjek.com

TS:   同 JS
来源：http://cov.wangdashe.top

Java: 方法内为块级作用域
来源：http://spu.xylfe.cn

Go:   花括号块级作用域
来源：http://npn.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fae.shangyingyoupin.top

C#:   块级作用域
来源：http://dmu.daxiang520.top

[C11] 模块导入与导出
来源：http://bot.yuanzhike.top

Py:   from module import func
来源：http://ayu.feifeiyinyue.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ueo.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://npz.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xrg.hammf.cn

Java: import java.util.List;
来源：http://jng.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hze.ybcxt.top

Ruby: require "json"; require_relative "./util"
来源：http://urm.ybcxt.top

C#:   using System.Text;
来源：http://seu.xuetiantiany.cn

[C12] 立即执行函数 IIFE
来源：http://tzt.fanxiaobao.xyz

Py:   (lambda: print("run"))()
来源：http://jbq.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://pjw.yonumen.top

JS:   (() => { console.log("run"); })();
来源：http://ggo.jinghuilouyu.cn

TS:   (() => { console.log("run"); })();
来源：http://idu.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mcd.hcnkem.com

Go:   func() { fmt.Println("run") }()
来源：http://bql.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://eei.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://agp.ctjpmb.com

[C13] 类型声明 / 类型注解
来源：http://kxf.nanxinkj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://odm.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ewe.jinghuilouyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kgx.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ddu.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mhf.zhixingplan.top

Go:   func add(a, b int) int
来源：http://uen.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://muf.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://nzm.tanke756.top

[C14] 泛型函数
来源：http://xoc.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pxm.gogol.net.cn

PHP:  // 无泛型
来源：http://esp.ydzc1.top

JS:   // 无泛型
来源：http://eeu.uphjek.com


<!-- 参考信息 -->