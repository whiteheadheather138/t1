代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jbe.shangyingyoupin.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cpr.gotoacloud.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yye.hnxiangtu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ghd.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eyk.ivvv.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xmt.gotoacloud.top

[A24] 去除首尾空白
来源：http://uae.ppjwa.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gqp.jinyuanbaomall.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hus.andypj.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tga.gzhubu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cnz.hysaishi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dtb.wangshuangyany.cn

Go:   strings.TrimSpace(s)
来源：http://exo.yj20258888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dvv.yj202588.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ujd.jlsjyb.cn

[A25] 字符串比较
来源：http://pnc.daxiang520.top

Py:   s1 == s2; s1 != s2
来源：http://jvl.jinqigfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bxn.yuxming.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jwa.birdmap.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://huk.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eey.cucudq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jzp.yanxiufei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hmu.hongshengwenyu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://shg.shanyushiyangkeji.top

[A26] 类型转换总览
来源：http://yki.hnxiangtu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rwt.zdqjudy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vwo.hysaishi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ubb.haohaochexian.top

TS:   Number() String() Boolean() x as number
来源：http://hnk.jinqigufen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://txt.tanke756.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vvs.sweek.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fdo.jinqigufen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yen.hesvh.cn

================================================================================
来源：http://wfo.yonumen.top

B. 流程控制
来源：http://xmf.gogol.net.cn

================================================================================
来源：http://htg.nanxinkj.top

[B01] 条件判断 if / else
来源：http://oyx.sufxvd.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vpc.jqgfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://stx.haohaochexian.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tsu.chenlongwang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wrg.hywenlv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wtd.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rpd.andypj.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mfr.cqqwz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kwz.fzhhl.top

[B02] 多分支 else if / elif
来源：http://hnk.fzhhl.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ann.316326.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mwp.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://krf.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cld.hammf.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pxl.fengsongda.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kbn.52xcode.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vre.yvedp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbg.birdmap.top

[B03] switch / match / case
来源：http://mwf.hnqzz.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mul.xinyue.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yoy.sufxvd.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zlb.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ndk.yanxiufei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mfl.pengpengdd.cyou

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vlq.hammf.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tgv.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dji.feifeiyinyue.top

[B04] for 计数循环
来源：http://tfs.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://xow.uphjek.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sla.jqgfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ien.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xda.havefunace.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mdz.yj20258888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rji.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://uxs.fktsv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qpc.sjlbkw.cn

[B05] 遍历数组 / 列表
来源：http://jqg.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://byh.jqgufenzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://anr.zhixingplan.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vlp.snrcjt.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jus.jianghu66.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ldm.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ysa.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://scs.bjfxy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ast.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://eno.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xnn.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://veh.gogol.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nav.hesvh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://spf.yfazqb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qup.zhijiandao.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zqn.wangshuangyany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qrc.jiagoushi.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rgn.chenlongwang.top

[B07] while 循环
来源：http://qtw.yvedp.cn

Py:   while i < 10: i += 1
来源：http://zzr.yanxiufei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vfr.shzxlz.cn

JS:   while (i < 10) { i++; }
来源：http://uzk.xziqi.cn

TS:   while (i < 10) { i++; }
来源：http://btc.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://abp.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ufr.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://sym.daria6918.cn

C#:   while (i < 10) { i++; }
来源：http://hcr.birdmap.top

[B08] do-while（至少执行一次）
来源：http://bnu.gzhubu.top

Py:   # 无 do-while：用 while True + break
来源：http://mds.guannengcc.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lee.fengsongda.top

JS:   do { i++; } while (i < 10);
来源：http://clu.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://zkr.shanyushiyangkeji.top

Java: do { i++; } while (i < 10);
来源：http://prq.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dvj.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://nzc.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://frj.zhijiandao.cn

[B09] break 与 continue
来源：http://xoh.shuidangran.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ici.aibaodan.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uoi.cashguo.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pxf.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rke.feifeiyinyue.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fkg.zhijiandao.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lgr.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sbw.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mdb.jinghuilouyu.cn

[B10] 遍历同时拿索引
来源：http://kck.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dqe.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wtl.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bqa.ctjpmb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bdh.jyoumei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://caz.shuidangran.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://asr.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qkk.zhaomingkeji.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rko.hnxiangtu.top

[B11] 生成数字序列 / 区间
来源：http://axd.bbcook.cn

Py:   list(range(0, 10, 2))
来源：http://pyk.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://xvo.sjlbkw.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wml.pycfn.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lbl.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rij.guowangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qrw.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://xpw.birdmap.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hrd.cucudq.cn

[B12] 跳出多层循环
来源：http://xdl.birdmap.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://uig.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mwh.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wth.zdqjudy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pox.yonumen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://icp.zhoulong.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uwu.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baa.jinqigfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uad.cucudq.cn

[B13] 判断是否为数字
来源：http://bpb.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://tiu.yfazqb.com

PHP:  is_numeric($x)
来源：http://bgy.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rfi.316326.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bhc.gogol.net.cn

Java: x instanceof Number
来源：http://ijb.feifeiyinyue.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hji.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://usi.yvedp.cn

C#:   x is int or double or decimal
来源：http://coa.daria6918.cn

[B14] 判断值是否在集合内
来源：http://unp.yuxming.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://awp.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vqb.nanxinkj.top

JS:   [1, 2, 3].includes(x)
来源：http://rjz.yvedp.cn

TS:   [1, 2, 3].includes(x)
来源：http://hec.yj20258888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://anv.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cvo.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jmu.hammf.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tkr.52xcode.cn

[B15] 布尔运算与取反
来源：http://xou.smart0.xyz

Py:   a and b or not c
来源：http://vxp.fktsv.cn

PHP:  $a && $b || !$c
来源：http://pxa.ctjpmb.com

JS:   a && b || !c
来源：http://rko.smart0.xyz

TS:   a && b || !c
来源：http://azj.xinyue.icu

Java: a && b || !c
来源：http://shf.hesvh.cn

Go:   a && b || !c
来源：http://sab.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://eoz.cheryme.top

C#:   a && b || !c
来源：http://bbc.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://vgs.snrcjt.cn

Py:   if not data: return
来源：http://uey.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://qvp.fktsv.cn

JS:   if (!data) return;
来源：http://fmj.xinyue.icu

TS:   if (!data) return;
来源：http://hsm.zhoulong.xyz

Java: if (data == null) return;
来源：http://anv.snrcjt.cn

Go:   if data == nil { return }
来源：http://jos.nwbrower.top

Ruby: return if data.nil?
来源：http://hax.cqqwz.cn

C#:   if (data == null) return;
来源：http://isg.hfpthk.cn

================================================================================
来源：http://poj.sjlbkw.cn

C. 函数与作用域
来源：http://vyf.redwolf501.top

================================================================================
来源：http://rci.cqqwz.cn

[C01] 定义函数
来源：http://jwk.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://gms.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gjg.52xcode.cn

JS:   function add(a, b) { return a + b; }
来源：http://fke.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mua.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://old.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zhs.hnxiangtu.top

Ruby: def add(a, b); a + b; end
来源：http://vyp.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fpw.ydjk.org.cn

[C02] 默认参数
来源：http://vev.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://xln.zdqjudy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wkp.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://lcc.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://myn.pycfn.com

Java: // 无默认参数：方法重载或 Optional
来源：http://bpv.uphjek.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wno.nanxuanxn.top

Ruby: def greet(name = "World") = name
来源：http://row.yj20258888.top

C#:   string Greet(string name = "World") => name;
来源：http://vds.nwbrower.top

[C03] 可变参数
来源：http://smd.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://pua.zhixingplan.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dhc.jianghu66.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cwk.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eml.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yfa.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wgi.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://yph.hywenlv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oes.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://hsk.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yrd.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nnk.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dex.fzhhl.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ipu.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://rdk.ydzc1.top

Go:   // 无：用配置结构体参数
来源：http://htt.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://qeb.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://gdc.zhoulong.xyz

[C05] 返回多个值
来源：http://emf.yj20258888.top

Py:   return a, b
来源：http://pmy.cashguo.top

PHP:  return [$a, $b];
来源：http://luq.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oah.316326.xyz

TS:   return { a, b };
来源：http://psh.uphjek.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://urk.gotoacloud.top

Go:   return a, b
来源：http://vvt.shzxlz.cn

Ruby: return a, b
来源：http://xkg.iojbl.cn

C#:   return (a, b);              // ValueTuple
来源：http://eho.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://kzi.epnwcf.com

Py:   square = lambda x: x * x
来源：http://xmp.yangfankeji.com

PHP:  $square = fn($x) => $x * $x;
来源：http://xll.bjfxy.top

JS:   const square = x => x * x;
来源：http://ffp.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://gwu.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hji.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bmn.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://jqn.feifeiyinyue.top

C#:   Func<int, int> square = x => x * x;
来源：http://qgy.zhiwuduotai.top

[C07] 把函数作为参数传入
来源：http://iyz.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aet.hongshengwenyu.top

PHP:  array_map("strtoupper", $arr);
来源：http://eux.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qxv.vqdsnc.cn

TS:   arr.map(String)
来源：http://tsr.9152youxi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kcb.wangshuangyany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lvd.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://qti.hongshengwenyu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dig.shanyushiyangkeji.top

[C08] 闭包
来源：http://ztv.jqgfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qoa.guowangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xls.fzhhl.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oqu.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zva.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ynr.ctjpmb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qcp.xinyue.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bsp.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://niw.cucudq.cn

[C09] 递归
来源：http://ewy.zhongyouzk.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://coy.svipenyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mqo.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rro.svipenyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gwp.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://njd.cqqwz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ykg.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qpm.zhongyouzk.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xfp.xziqi.cn

[C10] 变量作用域
来源：http://bks.zhoulong.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xsv.fzhhl.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gwf.xingfuxueyuan.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nuw.cdnleiting.top

TS:   同 JS
来源：http://eoz.hcnkem.com

Java: 方法内为块级作用域
来源：http://dms.yj202588.top

Go:   花括号块级作用域
来源：http://pye.zhijiandao.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lpa.hnqzz.top

C#:   块级作用域
来源：http://akq.hysaishi.cn

[C11] 模块导入与导出
来源：http://qpw.shzxlz.cn

Py:   from module import func
来源：http://bax.svipenyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mtb.ivvv.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tdc.yj20258.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kdl.hnqzz.top

Java: import java.util.List;
来源：http://nlr.chenlongwang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iig.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://bnf.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://gky.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://lmc.jlsjyb.cn

Py:   (lambda: print("run"))()
来源：http://zee.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://zts.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://ykx.yanxiufei.cn

TS:   (() => { console.log("run"); })();
来源：http://ghh.smart0.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ebo.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://yhf.chenzaomai.com

Ruby: -> { puts "run" }.call
来源：http://new.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://gsp.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://jrp.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hdf.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qtc.gotoacloud.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vmh.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vdz.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mxq.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://abh.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jgu.9152youxi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bjx.9152youxi.cn


<!-- 参考信息 -->