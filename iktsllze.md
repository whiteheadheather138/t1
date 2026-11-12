代发 wailian999

TS:   s.length
来源：http://vur.tianlin.xyz

Java: s.length()
来源：http://dul.zdbjq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ghh.guannengcc.top

Ruby: s.length
来源：http://gta.jinqigfzy.top

C#:   s.Length
来源：http://zia.bjfxy.top

[A23] 大小写转换
来源：http://szd.xuanzx.com

Py:   s.upper(); s.lower(); s.title()
来源：http://rzf.havefunace.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wlf.ivvv.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fdb.haohaochexian.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pcw.fzhhl.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fvy.svipenyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gmb.wangshuangyany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cmb.zdbjq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hko.ydjk.org.cn

[A24] 去除首尾空白
来源：http://fft.jinqigfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://riu.cucudq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pdb.kuanghao11.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qrh.sysykeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://clk.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sjv.chenlongwang.top

Go:   strings.TrimSpace(s)
来源：http://xun.mhx1999.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qgp.ydzc1.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mpc.tarul.cn

[A25] 字符串比较
来源：http://azn.wangshuangyany.cn

Py:   s1 == s2; s1 != s2
来源：http://udc.fanxiaobao.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tfc.meibo888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gng.dashuyun.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tbf.xziqi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ezd.redwolf501.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ocf.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://wab.nanxuanxn.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qjw.wangshuangyany.cn

[A26] 类型转换总览
来源：http://jpp.cheryme.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qbk.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://onl.daria6918.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jop.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://feh.tarul.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fqi.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xmy.wangshuangyany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vpp.daria6918.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xhc.gotoacloud.top

================================================================================
来源：http://xxj.zhixingplan.top

B. 流程控制
来源：http://hvd.yvedp.cn

================================================================================
来源：http://vpo.cheryme.top

[B01] 条件判断 if / else
来源：http://nxn.daria6918.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://npc.zhixingplan.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://est.sweek.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lem.jinqigfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uqa.hammf.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cbt.yfazqb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ybo.cdnleiting.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nde.tian-w.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wvz.ybcxt.top

[B02] 多分支 else if / elif
来源：http://wag.yj202588.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aqm.epnwcf.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kxu.52xcode.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mhl.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://asm.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://flg.kuanghao11.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qos.uphjek.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wug.yj20258888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rzv.chenjidiqi.icu

[B03] switch / match / case
来源：http://hue.zhiwuduotai.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wth.mhx1999.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bwk.zhijiandao.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tam.xingfuxueyuan.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ipm.zhaomingkeji.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vak.yfazqb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qtx.ydjk.org.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uvb.hnqzz.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qly.ydjk.org.cn

[B04] for 计数循环
来源：http://wpw.chenzaomai.com

Py:   for i in range(10): print(i)
来源：http://quq.yonumen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sza.tanke756.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vaw.chenlongwang.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jxx.0kj1m.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xqd.bjfxy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://luz.zycfv.cn

Ruby: 10.times { |i| puts i }
来源：http://tug.fehbvm.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lqn.tian-w.cn

[B05] 遍历数组 / 列表
来源：http://esc.jqgfzy.top

Py:   for item in arr: print(item)
来源：http://bpp.ybcxt.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ume.vehdjk.com

JS:   for (const item of arr) { console.log(item); }
来源：http://umf.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xll.yj20258888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bbf.havefunace.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vye.wangshuangyany.cn

Ruby: arr.each { |item| puts item }
来源：http://goa.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aje.ydzc1.top

[B06] 遍历字典 / 对象
来源：http://cig.sufxvd.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xnv.quarkkingdee.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gwb.vehdjk.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zvs.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zqy.chenzaomai.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gpp.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kpa.zhongyouzk.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fpp.c1oappe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uxl.smart0.xyz

[B07] while 循环
来源：http://yug.xylfe.cn

Py:   while i < 10: i += 1
来源：http://bjq.bjfxy.top

PHP:  while ($i < 10) { $i++; }
来源：http://psw.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://jrk.shzxlz.cn

TS:   while (i < 10) { i++; }
来源：http://aca.ywan-chungtsiang.top

Java: while (i < 10) { i++; }
来源：http://ebk.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rmg.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://dlu.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://ysz.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://ugv.yongpay.top

Py:   # 无 do-while：用 while True + break
来源：http://dsz.snrcjt.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kzo.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://uje.ydzc1.top

TS:   do { i++; } while (i < 10);
来源：http://kra.xingfuxueyuan.xyz

Java: do { i++; } while (i < 10);
来源：http://juk.hysaishi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iji.nanxuanxn.top

Ruby: begin; i += 1; end while i < 10
来源：http://tvd.xuetiantiany.cn

C#:   do { i++; } while (i < 10);
来源：http://tik.hesvh.cn

[B09] break 与 continue
来源：http://hku.gotoacloud.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iem.svipenyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tkp.hnqzz.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mwk.ywan-chungtsiang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wyf.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://edz.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xnp.mhx1999.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xoq.haohaochexian.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pba.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://elv.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zwv.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wyn.xuanzx.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ofv.ydjk.org.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cix.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bcq.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://trx.xingfuxueyuan.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dyq.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cka.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://unl.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://owt.jinyuanbaomall.cn

PHP:  range(0, 10, 2);
来源：http://ewx.pycfn.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fda.jianghu66.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vle.fehbvm.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bmi.zhiwuduotai.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ltg.epnwcf.com

Ruby: (0...10).step(2).to_a
来源：http://hyd.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ifv.jiagoushi.top

[B12] 跳出多层循环
来源：http://ixz.xziqi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qyi.daxiang520.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pbv.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://diy.cheryme.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lef.nwbrower.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://svs.aibaodan.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ppx.birdmap.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xpx.zycfv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hlq.jinqigfzy.top

[B13] 判断是否为数字
来源：http://gbs.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://yoa.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://pqi.yonumen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wjf.hnxiangtu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nei.haohaochexian.top

Java: x instanceof Number
来源：http://tiq.jinqigufen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tgb.bjfxy.top

Ruby: x.is_a?(Numeric)
来源：http://oya.havefunace.top

C#:   x is int or double or decimal
来源：http://kqf.daria6918.cn

[B14] 判断值是否在集合内
来源：http://wvj.chenlongwang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hvc.sufxvd.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jox.epnwcf.com

JS:   [1, 2, 3].includes(x)
来源：http://noh.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://uez.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://exw.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cab.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://xdi.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lnp.vehdjk.com

[B15] 布尔运算与取反
来源：http://vwz.ivvv.top

Py:   a and b or not c
来源：http://btx.zhaomingkeji.xyz

PHP:  $a && $b || !$c
来源：http://puq.shuidangran.top

JS:   a && b || !c
来源：http://aiu.xylfe.cn

TS:   a && b || !c
来源：http://syn.tarul.cn

Java: a && b || !c
来源：http://jic.hesvh.cn

Go:   a && b || !c
来源：http://dsz.9152youxi.cn

Ruby: a && b || !c
来源：http://wvk.xuetiantiany.cn

C#:   a && b || !c
来源：http://yyl.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://nkx.jqgufenzy.top

Py:   if not data: return
来源：http://ilg.hysaishi.cn

PHP:  if (!$data) { return; }
来源：http://krk.aibaodan.cn

JS:   if (!data) return;
来源：http://kff.yj20258.top

TS:   if (!data) return;
来源：http://nxu.bjfxy.top

Java: if (data == null) return;
来源：http://cto.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://ene.yanxiufei.cn

Ruby: return if data.nil?
来源：http://bpg.hesvh.cn

C#:   if (data == null) return;
来源：http://rcu.vqdsnc.cn

================================================================================
来源：http://miy.jiagoushi.top

C. 函数与作用域
来源：http://udj.ybcxt.top

================================================================================
来源：http://zry.ctjpmb.com

[C01] 定义函数
来源：http://zmf.shuidangran.top

Py:   def add(a, b): return a + b
来源：http://xwe.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sfi.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://gzp.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vyq.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cje.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eah.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://raa.chenjidiqi.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hax.c1oappe.top

[C02] 默认参数
来源：http://wxk.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://jmt.yvedp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wwr.wangdashe.top

JS:   function greet(name = "World") { return name; }
来源：http://eos.kuanghao11.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zhe.zhaomingkeji.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://uwd.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hnz.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://msh.bjfxy.top

C#:   string Greet(string name = "World") => name;
来源：http://vbv.ivvv.top

[C03] 可变参数
来源：http://rtw.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://tmb.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://znx.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rpz.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://thf.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kfg.hcnkem.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ezu.zdbjq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://utv.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://okx.xuanzx.com

[C04] 命名参数 / 关键字参数
来源：http://uaq.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://plg.fehbvm.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zpl.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ybc.kuanghao11.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sax.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://jjo.haohaochexian.top

Go:   // 无：用配置结构体参数
来源：http://omb.dashuyun.cn

Ruby: f(a: 1, b: 2)
来源：http://egq.havefunace.top

C#:   f(a: 1, b: 2)
来源：http://tlk.ydzc1.top

[C05] 返回多个值
来源：http://yuq.jyoumei.cn

Py:   return a, b
来源：http://bnw.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://jzs.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qrq.yj20258.top

TS:   return { a, b };
来源：http://pem.ehwqpu.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://isa.smart0.xyz

Go:   return a, b
来源：http://rzt.jinghuilouyu.cn

Ruby: return a, b
来源：http://zgp.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://wgt.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://cmy.aibaodan.cn

Py:   square = lambda x: x * x
来源：http://vcy.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nxw.hywenlv.cn

JS:   const square = x => x * x;
来源：http://xmb.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://lij.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://myr.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kfr.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://ubo.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fxt.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://gns.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hlv.snrcjt.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xhf.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yem.snrcjt.cn

TS:   arr.map(String)
来源：http://gar.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mam.zhixingplan.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kax.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://yxu.zhijiandao.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dsd.c1oappe.top

[C08] 闭包
来源：http://ody.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vdb.cqqwz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uoy.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gie.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://grm.xuanzx.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qop.cashguo.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xwg.zhoulong.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wvr.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jkv.daxiang520.top

[C09] 递归
来源：http://ujz.guowangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://voa.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vwd.fktsv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hab.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qlv.316326.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qvs.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wcy.jinyuanbaomall.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ovy.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nsk.yueranfly.top

[C10] 变量作用域
来源：http://aya.shanyushiyangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ulj.shzxlz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hae.yj20258.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pje.jinqigfzy.top

TS:   同 JS
来源：http://sfu.jinqigfzy.top

Java: 方法内为块级作用域
来源：http://mes.nanxuanxn.top

Go:   花括号块级作用域
来源：http://wyr.quarkkingdee.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rod.mhx1999.top

C#:   块级作用域
来源：http://rcq.yj202588.top

[C11] 模块导入与导出
来源：http://jcf.cdnleiting.top

Py:   from module import func
来源：http://lpr.feifeiyinyue.top

PHP:  require "file.php";  或 use App\Service;
来源：http://stm.aizwys.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oqt.wangshuangyany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mta.gotoacloud.top

Java: import java.util.List;
来源：http://hyg.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hnx.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://nwx.shzxlz.cn

C#:   using System.Text;
来源：http://nnu.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://hnt.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://cem.fktsv.cn

PHP:  (function () { echo "run"; })();
来源：http://umm.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://hyd.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://ztz.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vmv.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://gqs.zhoulong.xyz

Ruby: -> { puts "run" }.call
来源：http://qzm.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://leh.guannengcc.top

[C13] 类型声明 / 类型注解
来源：http://lhm.cdnleiting.top


<!-- 参考信息 -->