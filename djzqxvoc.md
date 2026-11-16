代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://kkc.jqgfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oml.gotoacloud.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sni.gzhubu.top

[A25] 字符串比较
来源：http://omc.jiagoushi.top

Py:   s1 == s2; s1 != s2
来源：http://bym.ehwqpu.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qno.zhijiandao.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://owv.hfpthk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ylf.hongshengwenyu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sbp.cucudq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://svm.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://egx.daxiang520.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mki.yonumen.top

[A26] 类型转换总览
来源：http://rgv.shuidangran.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dzi.jianghu66.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aqt.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hjq.zhiwuduotai.top

TS:   Number() String() Boolean() x as number
来源：http://qvr.hywenlv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dxr.chenzaomai.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kxu.ivvv.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dsn.hcnkem.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nfq.yuxming.cn

================================================================================
来源：http://uop.wangdashe.top

B. 流程控制
来源：http://ojt.zhoulong.xyz

================================================================================
来源：http://uuy.shangyingyoupin.top

[B01] 条件判断 if / else
来源：http://sfv.fengsongda.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ikv.jinqigfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gcn.xziqi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gcu.xuetiantiany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mgh.yanxiufei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qwy.hnqzz.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ang.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fpc.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cvl.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://pws.chenlongwang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ypk.9152youxi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ozs.meibo888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kvk.ehwqpu.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oxc.snrcjt.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gkv.wangshuangyany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://swk.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xob.guannengcc.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xnw.sysykeji.top

[B03] switch / match / case
来源：http://etu.52xcode.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hap.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wsr.zhoulong.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jii.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://icc.yfazqb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oxu.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dgt.sweek.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://guv.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iwg.haohaochexian.top

[B04] for 计数循环
来源：http://qyv.ehwqpu.com

Py:   for i in range(10): print(i)
来源：http://huh.zhoulong.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rww.zdqjudy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tcu.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rdk.jlsjyb.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qop.daxiang520.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ccl.quarkkingdee.top

Ruby: 10.times { |i| puts i }
来源：http://gqq.chenzaomai.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vlj.sjlbkw.cn

[B05] 遍历数组 / 列表
来源：http://wmo.sufxvd.cn

Py:   for item in arr: print(item)
来源：http://fdw.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kzx.hnqzz.top

JS:   for (const item of arr) { console.log(item); }
来源：http://axs.hesvh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ixs.cheryme.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jrq.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wmp.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://zgo.daria6918.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oan.cdnleiting.top

[B06] 遍历字典 / 对象
来源：http://mnf.zycfv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lcx.yvedp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ynn.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vqp.cucudq.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jis.zycfv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yey.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vyu.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fam.yfazqb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://slr.andypj.xyz

[B07] while 循环
来源：http://uhs.jianghu66.top

Py:   while i < 10: i += 1
来源：http://bhl.shzxlz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bkx.redwolf501.top

JS:   while (i < 10) { i++; }
来源：http://kdc.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://uwq.zycfv.cn

Java: while (i < 10) { i++; }
来源：http://vcs.vehdjk.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vwg.svipenyu.cn

Ruby: while i < 10; i += 1; end
来源：http://urz.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://qfx.hcnkem.com

[B08] do-while（至少执行一次）
来源：http://ste.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://sry.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jww.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://nzm.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://tcz.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://tkb.sweek.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fsw.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://tia.xylfe.cn

C#:   do { i++; } while (i < 10);
来源：http://jux.shuidangran.top

[B09] break 与 continue
来源：http://vek.iojbl.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vhk.gzhubu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gpd.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vyw.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rcd.daria6918.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://has.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uzn.vehdjk.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ave.shangyingyoupin.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eew.shuidangran.top

[B10] 遍历同时拿索引
来源：http://gjr.nwbrower.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mjg.cqqwz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ksm.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rqp.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://swe.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ogn.mhx1999.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ypv.dianchejie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cpq.dianchejie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qwb.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://hqn.fengsongda.top

Py:   list(range(0, 10, 2))
来源：http://cfg.yanxiufei.cn

PHP:  range(0, 10, 2);
来源：http://uxy.tarul.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://isr.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fju.yanxiufei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vob.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cea.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://mjg.chenjidiqi.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mij.jiagoushi.top

[B12] 跳出多层循环
来源：http://fya.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kdj.sysykeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qbr.xuanzx.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jfe.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ohc.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wdg.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://geo.xylfe.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ukq.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pnx.fanxiaobao.xyz

[B13] 判断是否为数字
来源：http://xrw.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://ckb.pengpengdd.cyou

PHP:  is_numeric($x)
来源：http://hpk.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hcu.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mvz.yvedp.cn

Java: x instanceof Number
来源：http://rfa.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vwq.pengpengdd.cyou

Ruby: x.is_a?(Numeric)
来源：http://kaz.hesvh.cn

C#:   x is int or double or decimal
来源：http://dxa.yangfankeji.com

[B14] 判断值是否在集合内
来源：http://gyu.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fos.guannengcc.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://voa.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://mia.hcnkem.com

TS:   [1, 2, 3].includes(x)
来源：http://xls.ybcxt.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mxi.hnqzz.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hjn.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kah.tarul.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bpb.sufxvd.cn

[B15] 布尔运算与取反
来源：http://rvq.vehdjk.com

Py:   a and b or not c
来源：http://tgk.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://whr.nwbrower.top

JS:   a && b || !c
来源：http://mah.tianlin.xyz

TS:   a && b || !c
来源：http://tdz.daria6918.cn

Java: a && b || !c
来源：http://cme.dianchejie.cn

Go:   a && b || !c
来源：http://mqn.hfpthk.cn

Ruby: a && b || !c
来源：http://xdo.zhoulong.xyz

C#:   a && b || !c
来源：http://zpv.jiagoushi.top

[B16] 卫语句：不满足条件提前返回
来源：http://alx.iojbl.cn

Py:   if not data: return
来源：http://nwj.uphjek.com

PHP:  if (!$data) { return; }
来源：http://rbd.ctjpmb.com

JS:   if (!data) return;
来源：http://rwg.daria6918.cn

TS:   if (!data) return;
来源：http://vln.ydzc1.top

Java: if (data == null) return;
来源：http://wtc.sufxvd.cn

Go:   if data == nil { return }
来源：http://rnx.yj20258.top

Ruby: return if data.nil?
来源：http://thj.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://jrv.gogol.net.cn

================================================================================
来源：http://vmx.jqgfzy.top

C. 函数与作用域
来源：http://uhl.gzhubu.top

================================================================================
来源：http://sda.jyoumei.cn

[C01] 定义函数
来源：http://ywz.meibo888.top

Py:   def add(a, b): return a + b
来源：http://mzx.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gvc.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://uts.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://irx.0kj1m.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yqt.aibaodan.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hgj.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://vdl.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qpk.chenzaomai.com

[C02] 默认参数
来源：http://zov.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://mtr.yanxiufei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://usz.ywan-chungtsiang.top

JS:   function greet(name = "World") { return name; }
来源：http://nhm.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fpu.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bbt.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bar.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://qrt.yj20258888.top

C#:   string Greet(string name = "World") => name;
来源：http://nxk.yongpay.top

[C03] 可变参数
来源：http://dpe.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://jhz.dianchejie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tnb.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yva.hfpthk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uwf.yvedp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://khm.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sll.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://boi.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://csh.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://fpo.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nnl.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jxw.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://btx.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zva.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://nvd.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://vpe.feifeiyinyue.top

Ruby: f(a: 1, b: 2)
来源：http://snt.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://cso.jianghu66.top

[C05] 返回多个值
来源：http://vli.ybcxt.top

Py:   return a, b
来源：http://gly.jianghu66.top

PHP:  return [$a, $b];
来源：http://qch.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://txw.ybcxt.top

TS:   return { a, b };
来源：http://khp.ctjpmb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dwd.ywan-chungtsiang.top

Go:   return a, b
来源：http://wpi.zhixingplan.top

Ruby: return a, b
来源：http://dnq.fzhhl.top

C#:   return (a, b);              // ValueTuple
来源：http://lgt.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://cpo.yonumen.top

Py:   square = lambda x: x * x
来源：http://zsc.yonumen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mgz.yangfankeji.com

JS:   const square = x => x * x;
来源：http://dpm.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://iyd.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zlw.hysaishi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oqw.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://mxt.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://mwr.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://cxr.tian-w.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://azv.ydjk.org.cn

PHP:  array_map("strtoupper", $arr);
来源：http://khk.feifeiyinyue.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dtx.316326.xyz

TS:   arr.map(String)
来源：http://qiw.jqgfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cnz.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pkw.yuxming.cn

Ruby: arr.map(&:upcase)
来源：http://ehc.tanke756.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fvz.zhongyouzk.top

[C08] 闭包
来源：http://blx.hnqzz.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://glk.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pcn.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wql.yanxiufei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yuq.pycfn.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xvk.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ifu.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jab.hnxiangtu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hpx.pycfn.com

[C09] 递归
来源：http://ern.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aod.xziqi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hda.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://inc.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sxc.chenlongwang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pjv.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lys.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dzc.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zrm.yueranfly.top

[C10] 变量作用域
来源：http://pii.pengpengdd.cyou

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tpr.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dfc.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cov.jqgufenzy.top

TS:   同 JS
来源：http://cho.daxiang520.top

Java: 方法内为块级作用域
来源：http://quu.sjlbkw.cn

Go:   花括号块级作用域
来源：http://nze.ybcxt.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pjh.chenzaomai.com

C#:   块级作用域
来源：http://vfs.yj20258.top

[C11] 模块导入与导出
来源：http://had.ybcxt.top

Py:   from module import func
来源：http://riq.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://oea.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vvq.pycfn.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mcq.bjfxy.top

Java: import java.util.List;
来源：http://mhd.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://scq.kuanghao11.cn

Ruby: require "json"; require_relative "./util"
来源：http://ilm.birdmap.top

C#:   using System.Text;
来源：http://nfe.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://rvr.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://pkz.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://udp.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://ook.chenlongwang.top

TS:   (() => { console.log("run"); })();
来源：http://gez.yj20258888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zzi.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://slx.havefunace.top

Ruby: -> { puts "run" }.call
来源：http://nom.kuanghao11.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ymz.ybcxt.top

[C13] 类型声明 / 类型注解
来源：http://cfy.andypj.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xom.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pfy.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://krv.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yyw.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lsh.ehwqpu.com

Go:   func add(a, b int) int
来源：http://bxz.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nmd.vqdsnc.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ixj.zycfv.cn

[C14] 泛型函数
来源：http://nlz.daria6918.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fan.ehwqpu.com

PHP:  // 无泛型
来源：http://plc.snrcjt.cn

JS:   // 无泛型
来源：http://gah.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tsq.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ksl.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vdb.yongpay.top

Ruby: # 无泛型
来源：http://ely.hysaishi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nst.jqgufenzy.top

[C15] 解构 / 展开参数
来源：http://mql.pengpengdd.cyou

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wmo.jiagoushi.top

PHP:  [$a, $b] = $pair;
来源：http://snm.zycfv.cn


<!-- 参考信息 -->