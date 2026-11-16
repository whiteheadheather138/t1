代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zlo.gogol.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yey.yj202588.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://obw.svipenyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bhf.quarkkingdee.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nbo.ybcxt.top

C#:   s.ToUpper(); s.ToLower()
来源：http://wbt.yuanzhike.top

[A24] 去除首尾空白
来源：http://bjs.hesvh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cxt.jyoumei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dkb.bjfxy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pbn.yj20258888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ndn.yj20258888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cnf.yueranfly.top

Go:   strings.TrimSpace(s)
来源：http://fok.ydjk.org.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qbu.dianchejie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lai.xylfe.cn

[A25] 字符串比较
来源：http://vvh.zdqjudy.top

Py:   s1 == s2; s1 != s2
来源：http://dkr.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cbh.tarul.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uzj.yj202588.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wai.zhongyouzk.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lcp.ctjpmb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dmk.yuanzhike.top

Ruby: s1 == s2; s1 <=> s2
来源：http://owh.xuanzx.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zqe.daria6918.cn

[A26] 类型转换总览
来源：http://snn.aizwys.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pey.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zok.svipenyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kwr.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://fcm.daxiang520.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ytf.ydjk.org.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iqu.pycfn.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://ylw.jianghu66.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tip.vehdjk.com

================================================================================
来源：http://enr.daria6918.cn

B. 流程控制
来源：http://rfi.chenlongwang.top

================================================================================
来源：http://prz.zhoulong.xyz

[B01] 条件判断 if / else
来源：http://jfy.fengsongda.top

Py:   result = "正" if x > 0 else "非正"
来源：http://noi.zdbjq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bof.shanyushiyangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bff.sxryk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dcr.ppjwa.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jpe.9152youxi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ydh.yongpay.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yku.xingfuxueyuan.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ffn.shanyushiyangtech.top

[B02] 多分支 else if / elif
来源：http://cjw.xuanzx.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xxt.shanyushiyangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qru.jinyuanbaomall.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eyt.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bte.meibo888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cba.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tld.guannengcc.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rke.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ngc.aibaodan.cn

[B03] switch / match / case
来源：http://dkm.daxiang520.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dql.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zkx.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://snf.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pdy.vehdjk.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hgt.uphjek.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vah.guannengcc.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jol.cashguo.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ovh.shangyingyoupin.top

[B04] for 计数循环
来源：http://eab.snrcjt.cn

Py:   for i in range(10): print(i)
来源：http://ltv.cashguo.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://esy.zdqjudy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yjl.xylfe.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uig.hcnkem.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aze.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gxo.hnqzz.top

Ruby: 10.times { |i| puts i }
来源：http://uak.meibo888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://txj.hnqzz.top

[B05] 遍历数组 / 列表
来源：http://hba.jqgufenzy.top

Py:   for item in arr: print(item)
来源：http://klp.316326.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://red.yvedp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://opj.tanke756.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fln.ppjwa.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gun.aibaodan.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wbs.gogol.net.cn

Ruby: arr.each { |item| puts item }
来源：http://gdu.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mno.xziqi.cn

[B06] 遍历字典 / 对象
来源：http://scu.jyoumei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://smc.jinyuanbaomall.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qmm.hammf.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ilx.ywan-chungtsiang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://znv.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jvk.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oca.wangdashe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dlw.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rwx.hesvh.cn

[B07] while 循环
来源：http://jfj.zdqjudy.top

Py:   while i < 10: i += 1
来源：http://fnl.jqgfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://udz.xingfuxueyuan.xyz

JS:   while (i < 10) { i++; }
来源：http://bqy.yj20258.top

TS:   while (i < 10) { i++; }
来源：http://ugo.sweek.top

Java: while (i < 10) { i++; }
来源：http://rdp.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nax.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://qnx.smart0.xyz

C#:   while (i < 10) { i++; }
来源：http://tae.zdqjudy.top

[B08] do-while（至少执行一次）
来源：http://glt.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://xkp.wangdashe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://npo.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://ysh.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://btz.fzhhl.top

Java: do { i++; } while (i < 10);
来源：http://uun.fktsv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tdm.snrcjt.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zvj.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://dwu.hesvh.cn

[B09] break 与 continue
来源：http://akn.xinyue.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kzj.nwbrower.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://buf.yueranfly.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ers.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cwu.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://avp.zdbjq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lbu.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qai.cheryme.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zfs.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://cga.uphjek.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wnu.hcnkem.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ies.fzhhl.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pek.zhiwuduotai.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wro.zhengqikj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hsv.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dgs.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wmx.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hpk.hammf.cn

[B11] 生成数字序列 / 区间
来源：http://lph.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://ddk.yanxiufei.cn

PHP:  range(0, 10, 2);
来源：http://rih.shanyushiyangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://weq.shuidangran.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://abv.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gih.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cjl.yvedp.cn

Ruby: (0...10).step(2).to_a
来源：http://smh.xylfe.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wtg.bjfxy.top

[B12] 跳出多层循环
来源：http://kjf.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pgm.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://sqh.redwolf501.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cqp.yuxming.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xrr.hnxiangtu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tnt.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nmw.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ryz.gogol.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dki.zycfv.cn

[B13] 判断是否为数字
来源：http://lgo.nanxinkj.top

Py:   isinstance(x, (int, float))
来源：http://qcq.gogol.net.cn

PHP:  is_numeric($x)
来源：http://hkd.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qjo.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qzl.vqdsnc.cn

Java: x instanceof Number
来源：http://mlz.chenlongwang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rsg.vqdsnc.cn

Ruby: x.is_a?(Numeric)
来源：http://ecv.jyoumei.cn

C#:   x is int or double or decimal
来源：http://gio.ybcxt.top

[B14] 判断值是否在集合内
来源：http://oyh.epnwcf.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eqj.jlsjyb.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://swg.pycfn.com

JS:   [1, 2, 3].includes(x)
来源：http://zxg.yvedp.cn

TS:   [1, 2, 3].includes(x)
来源：http://fcr.zdbjq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uom.dashuyun.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pid.feifeiyinyue.top

Ruby: [1, 2, 3].include?(x)
来源：http://obk.zhaomingkeji.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fbc.zhengqikj.top

[B15] 布尔运算与取反
来源：http://xrw.nanxuanxn.top

Py:   a and b or not c
来源：http://oyv.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://yxv.9152youxi.cn

JS:   a && b || !c
来源：http://xjp.0kj1m.cn

TS:   a && b || !c
来源：http://jsa.dashuyun.cn

Java: a && b || !c
来源：http://gfk.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://kbe.jiagoushi.top

Ruby: a && b || !c
来源：http://uxv.snrcjt.cn

C#:   a && b || !c
来源：http://tua.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://hsi.9152youxi.cn

Py:   if not data: return
来源：http://vvk.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://wxh.zhoulong.xyz

JS:   if (!data) return;
来源：http://zip.fzhhl.top

TS:   if (!data) return;
来源：http://fkp.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://laz.yangfankeji.com

Go:   if data == nil { return }
来源：http://dwc.tanke756.top

Ruby: return if data.nil?
来源：http://rvv.tian-w.cn

C#:   if (data == null) return;
来源：http://zst.ehwqpu.com

================================================================================
来源：http://bkp.hysaishi.cn

C. 函数与作用域
来源：http://qwq.ybcxt.top

================================================================================
来源：http://jxz.ctjpmb.com

[C01] 定义函数
来源：http://xwj.hammf.cn

Py:   def add(a, b): return a + b
来源：http://pen.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vbl.shzxlz.cn

JS:   function add(a, b) { return a + b; }
来源：http://bzk.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hfm.aibaodan.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ycl.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://kuy.jiagoushi.top

Ruby: def add(a, b); a + b; end
来源：http://gww.yuanzhike.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oku.jinghuilouyu.cn

[C02] 默认参数
来源：http://tqc.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://oke.meibo888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rjs.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://loa.c1oappe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ioi.ivvv.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mwd.jianghu66.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ckk.52xcode.cn

Ruby: def greet(name = "World") = name
来源：http://ccw.dianchejie.cn

C#:   string Greet(string name = "World") => name;
来源：http://bzi.ctjpmb.com

[C03] 可变参数
来源：http://fla.gzhubu.top

Py:   def total(*args): return sum(args)
来源：http://zbf.jianghu66.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oet.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jzj.nanxuanxn.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wus.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wno.kuanghao11.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pwk.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gvv.yuanzhike.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lke.bjfxy.top

[C04] 命名参数 / 关键字参数
来源：http://qmx.jqgufenzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jqa.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ahz.zhoulong.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mug.jinqigfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gih.cucudq.cn

Java: // 无：用 Builder 模式或 record
来源：http://ohb.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://imx.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://twl.yuxming.cn

C#:   f(a: 1, b: 2)
来源：http://egq.mhx1999.top

[C05] 返回多个值
来源：http://kzr.yj20258.top

Py:   return a, b
来源：http://wsx.xylfe.cn

PHP:  return [$a, $b];
来源：http://hwv.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xys.yangfankeji.com

TS:   return { a, b };
来源：http://wdw.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://acn.ppjwa.cn

Go:   return a, b
来源：http://lzp.gaohongyu789.top

Ruby: return a, b
来源：http://hrb.vehdjk.com

C#:   return (a, b);              // ValueTuple
来源：http://zje.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://oyi.316326.xyz

Py:   square = lambda x: x * x
来源：http://iwa.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cbk.ydzc1.top

JS:   const square = x => x * x;
来源：http://fyu.jinqigufen.top

TS:   const square = (x: number): number => x * x;
来源：http://bup.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mav.zhaomingkeji.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://jmk.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://ddc.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://sam.yueranfly.top

[C07] 把函数作为参数传入
来源：http://uaa.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bxq.ywan-chungtsiang.top

PHP:  array_map("strtoupper", $arr);
来源：http://lek.sxryk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://twx.yonumen.top

TS:   arr.map(String)
来源：http://gyj.tarul.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hqw.hammf.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ztx.chenlongwang.top

Ruby: arr.map(&:upcase)
来源：http://llk.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://oys.nwbrower.top

[C08] 闭包
来源：http://bko.52xcode.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tvn.xinyue.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nls.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eev.tianlin.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tnh.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://igo.gogol.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dvq.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gis.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wlg.c1oappe.top

[C09] 递归
来源：http://rti.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rku.vqdsnc.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qup.chenzaomai.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qty.ydzc1.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dho.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hux.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://irg.tian-w.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vtq.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://anr.yueranfly.top

[C10] 变量作用域
来源：http://dny.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fxx.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oay.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://smi.xuetiantiany.cn

TS:   同 JS
来源：http://akw.52xcode.cn

Java: 方法内为块级作用域
来源：http://bki.gzhubu.top

Go:   花括号块级作用域
来源：http://gzk.quarkkingdee.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fwm.smart0.xyz

C#:   块级作用域
来源：http://ttj.mhx1999.top

[C11] 模块导入与导出
来源：http://yuh.xuetiantiany.cn

Py:   from module import func
来源：http://imy.xingfuxueyuan.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://vlv.daxiang520.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mfw.fzhhl.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uot.ywan-chungtsiang.top

Java: import java.util.List;
来源：http://pqd.vqdsnc.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://thy.316326.xyz

Ruby: require "json"; require_relative "./util"
来源：http://kwc.yangfankeji.com

C#:   using System.Text;
来源：http://ech.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://daj.zhijiandao.cn

Py:   (lambda: print("run"))()
来源：http://xhl.wangdashe.top

PHP:  (function () { echo "run"; })();
来源：http://pif.ivvv.top

JS:   (() => { console.log("run"); })();
来源：http://rxs.yueranfly.top

TS:   (() => { console.log("run"); })();
来源：http://atp.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zrc.yuanzhike.top

Go:   func() { fmt.Println("run") }()
来源：http://gya.pycfn.com

Ruby: -> { puts "run" }.call
来源：http://qxk.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fws.ppjwa.cn

[C13] 类型声明 / 类型注解
来源：http://ywj.hammf.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wqi.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dcd.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bwl.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mlr.yj202588.top

Java: int add(int a, int b) { return a + b; }
来源：http://drb.ydzc1.top

Go:   func add(a, b int) int
来源：http://lbj.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xqo.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://kud.daxiang520.top


<!-- 参考信息 -->