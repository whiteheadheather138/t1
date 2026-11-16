代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nur.sufxvd.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mfr.hnxiangtu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uoj.dashuyun.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rsc.zhaomingkeji.xyz

Go:   strings.TrimSpace(s)
来源：http://pqh.yanxiufei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://duu.fzhhl.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nzu.zhengqikj.top

[A25] 字符串比较
来源：http://cic.chenlongwang.top

Py:   s1 == s2; s1 != s2
来源：http://gde.jinyuanbaomall.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vcu.yj20258.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mgp.aizwys.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gdg.redwolf501.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hfl.hongshengwenyu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aya.zdbjq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zem.jlsjyb.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kdu.jianghu66.top

[A26] 类型转换总览
来源：http://awo.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fvp.wangdashe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nnq.yuanzhike.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ogy.bbcook.cn

TS:   Number() String() Boolean() x as number
来源：http://mmn.ehwqpu.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eph.jinyuanbaomall.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oxc.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://swf.ybcxt.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://irt.birdmap.top

================================================================================
来源：http://abu.zhaomingkeji.xyz

B. 流程控制
来源：http://adz.chenlongwang.top

================================================================================
来源：http://etq.xinyue.icu

[B01] 条件判断 if / else
来源：http://kjb.9152youxi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qwu.zhengqikj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qce.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ogs.zhaomingkeji.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cvl.vqdsnc.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iek.sjlbkw.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kcs.ydzc1.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ytf.zhoulong.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://smg.nwbrower.top

[B02] 多分支 else if / elif
来源：http://lex.quarkkingdee.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kci.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ggh.zdqjudy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ilp.xziqi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ise.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hmr.xziqi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ggy.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zty.haohaochexian.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbx.mhx1999.top

[B03] switch / match / case
来源：http://oel.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://owi.yfazqb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hzj.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yyu.jinqigfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://opo.xinyue.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://loq.0kj1m.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pnf.cdnleiting.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fed.birdmap.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vrw.nanxinkj.top

[B04] for 计数循环
来源：http://iiu.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://yty.tarul.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://luo.quarkkingdee.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xzi.meibo888.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rqm.tanke756.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pkc.yuxming.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jdt.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://rvx.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kxu.pengpengdd.cyou

[B05] 遍历数组 / 列表
来源：http://fng.jinqigfzy.top

Py:   for item in arr: print(item)
来源：http://zpl.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jup.52xcode.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tzo.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://hpj.zhaomingkeji.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://tna.hywenlv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://daz.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://tab.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yky.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://cia.9152youxi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pwc.ivvv.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rcu.shanyushiyangtech.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mup.mhx1999.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ocr.sjlbkw.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ehk.pycfn.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wjp.jlsjyb.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rew.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sfr.zdbjq.cn

[B07] while 循环
来源：http://ide.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://ust.redwolf501.top

PHP:  while ($i < 10) { $i++; }
来源：http://you.ehwqpu.com

JS:   while (i < 10) { i++; }
来源：http://hhp.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://byn.jlsjyb.cn

Java: while (i < 10) { i++; }
来源：http://api.shuidangran.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tjb.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://zmp.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://lqx.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://mui.xuanzx.com

Py:   # 无 do-while：用 while True + break
来源：http://nix.feifeiyinyue.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yeb.jqgufenzy.top

JS:   do { i++; } while (i < 10);
来源：http://wrx.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://ktc.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://twp.fanxiaobao.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://asj.0kj1m.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rlx.jiagoushi.top

C#:   do { i++; } while (i < 10);
来源：http://bmz.hongshengwenyu.top

[B09] break 与 continue
来源：http://dsq.zhiwuduotai.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cna.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ajb.yueranfly.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtk.tianlin.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ysa.zhijiandao.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixe.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yuo.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mua.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ssi.yj20258.top

[B10] 遍历同时拿索引
来源：http://vey.uphjek.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://drs.ydzc1.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://icd.fktsv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lrm.yongpay.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hlg.uphjek.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oge.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tof.chenjidiqi.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dqa.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oqr.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://dfm.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://ijs.yonumen.top

PHP:  range(0, 10, 2);
来源：http://zuo.xuetiantiany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rnt.sweek.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://goz.jinghuilouyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eru.vqdsnc.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aba.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://ggq.vqdsnc.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xws.cashguo.top

[B12] 跳出多层循环
来源：http://azu.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://eah.uphjek.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://vfm.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ixe.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wbs.gogol.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zlo.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tji.xuetiantiany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ksj.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://esg.guannengcc.top

[B13] 判断是否为数字
来源：http://yal.hammf.cn

Py:   isinstance(x, (int, float))
来源：http://gct.tarul.cn

PHP:  is_numeric($x)
来源：http://fjy.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ztj.zycfv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sbo.smart0.xyz

Java: x instanceof Number
来源：http://utn.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aau.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://ack.daxiang520.top

C#:   x is int or double or decimal
来源：http://wkp.guannengcc.top

[B14] 判断值是否在集合内
来源：http://evv.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aut.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wtv.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://hpp.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://grb.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://bgo.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vhi.aibaodan.cn

Ruby: [1, 2, 3].include?(x)
来源：http://frg.cqqwz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kgh.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://tap.yonumen.top

Py:   a and b or not c
来源：http://txw.hesvh.cn

PHP:  $a && $b || !$c
来源：http://gnz.yfazqb.com

JS:   a && b || !c
来源：http://zyf.yj202588.top

TS:   a && b || !c
来源：http://nsa.tanke756.top

Java: a && b || !c
来源：http://tlo.yj20258.top

Go:   a && b || !c
来源：http://avp.vehdjk.com

Ruby: a && b || !c
来源：http://gaj.xylfe.cn

C#:   a && b || !c
来源：http://fog.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://lmf.andypj.xyz

Py:   if not data: return
来源：http://hhd.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://csq.nanxuanxn.top

JS:   if (!data) return;
来源：http://mqj.shanyushiyangkeji.top

TS:   if (!data) return;
来源：http://dun.haohaochexian.top

Java: if (data == null) return;
来源：http://mcr.bbcook.cn

Go:   if data == nil { return }
来源：http://ien.jinyuanbaomall.cn

Ruby: return if data.nil?
来源：http://rpx.guannengcc.top

C#:   if (data == null) return;
来源：http://ula.hnqzz.top

================================================================================
来源：http://bnx.kuanghao11.cn

C. 函数与作用域
来源：http://upk.guowangkeji.top

================================================================================
来源：http://rtu.9152youxi.cn

[C01] 定义函数
来源：http://lcl.cashguo.top

Py:   def add(a, b): return a + b
来源：http://ssf.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qtm.kuanghao11.cn

JS:   function add(a, b) { return a + b; }
来源：http://sjb.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://usq.birdmap.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ifm.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pzg.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://rfq.sjlbkw.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cyh.zdbjq.cn

[C02] 默认参数
来源：http://inz.pengpengdd.cyou

Py:   def greet(name="World"): return name
来源：http://nrs.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://xjz.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://eze.yj20258.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sor.sxryk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qfs.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nkh.ydjk.org.cn

Ruby: def greet(name = "World") = name
来源：http://myf.hnxiangtu.top

C#:   string Greet(string name = "World") => name;
来源：http://tdp.epnwcf.com

[C03] 可变参数
来源：http://eet.bbcook.cn

Py:   def total(*args): return sum(args)
来源：http://kww.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hkt.yongpay.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jgm.mhx1999.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zge.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xqh.fktsv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vrg.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://lsa.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ghn.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://iur.shzxlz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wuw.kuanghao11.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yci.tianlin.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fzr.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tkb.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://fnt.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://eaw.jlsjyb.cn

Ruby: f(a: 1, b: 2)
来源：http://jmz.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://xpf.iojbl.cn

[C05] 返回多个值
来源：http://zhm.vehdjk.com

Py:   return a, b
来源：http://guv.sysykeji.top

PHP:  return [$a, $b];
来源：http://tlb.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mjb.dianchejie.cn

TS:   return { a, b };
来源：http://lba.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gsa.tianlin.xyz

Go:   return a, b
来源：http://xvf.sweek.top

Ruby: return a, b
来源：http://bfl.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://rnu.jqgufenzy.top

[C06] 匿名函数 / lambda
来源：http://rfl.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://tsc.smart0.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://jpd.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://bqb.daxiang520.top

TS:   const square = (x: number): number => x * x;
来源：http://hqu.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gur.shanyushiyangtech.top

Go:   sq := func(x int) int { return x * x }
来源：http://qhu.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://zcp.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ylz.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://ygo.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://okj.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bkq.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jkz.jinqigfzy.top

TS:   arr.map(String)
来源：http://mvj.jqgufenzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gzn.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fbn.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://irl.jinghuilouyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://krq.chenzaomai.com

[C08] 闭包
来源：http://fwi.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rzt.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hkh.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ggw.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qhj.shangyingyoupin.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hwh.jiagoushi.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aow.wangshuangyany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xbi.cdnleiting.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://agd.nwbrower.top

[C09] 递归
来源：http://nvb.smart0.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kmi.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jfw.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yxd.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ika.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pgo.chenlongwang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qkj.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://olr.wangshuangyany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zyb.hcnkem.com

[C10] 变量作用域
来源：http://rub.yj20258888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ffl.pengpengdd.cyou

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mpe.yj20258.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vtu.zdbjq.cn

TS:   同 JS
来源：http://kka.bjfxy.top

Java: 方法内为块级作用域
来源：http://nrs.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://igq.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tce.chenjidiqi.icu

C#:   块级作用域
来源：http://mzo.316326.xyz

[C11] 模块导入与导出
来源：http://yjl.aizwys.cn

Py:   from module import func
来源：http://czy.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hai.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hmj.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dmv.jianghu66.top

Java: import java.util.List;
来源：http://xxw.shanyushiyangtech.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zvj.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://ivj.nanxinkj.top

C#:   using System.Text;
来源：http://jpq.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://msk.cashguo.top

Py:   (lambda: print("run"))()
来源：http://lsr.ywan-chungtsiang.top

PHP:  (function () { echo "run"; })();
来源：http://ndv.gotoacloud.top

JS:   (() => { console.log("run"); })();
来源：http://gvl.shanyushiyangtech.top

TS:   (() => { console.log("run"); })();
来源：http://bte.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ung.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://fkd.tian-w.cn

Ruby: -> { puts "run" }.call
来源：http://hyt.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jjl.zycfv.cn

[C13] 类型声明 / 类型注解
来源：http://bfi.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://evk.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wac.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://scu.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qpp.yuxming.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xia.cdnleiting.top

Go:   func add(a, b int) int
来源：http://vbz.yj20258.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vis.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://lil.xziqi.cn

[C14] 泛型函数
来源：http://vxz.ybcxt.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://efo.0kj1m.cn

PHP:  // 无泛型
来源：http://qlr.ybcxt.top

JS:   // 无泛型
来源：http://ffa.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qgo.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vpc.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dzs.havefunace.top

Ruby: # 无泛型
来源：http://hpe.epnwcf.com


<!-- 参考信息 -->