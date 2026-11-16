代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://khb.smart0.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://ake.vehdjk.com

[A24] 去除首尾空白
来源：http://iku.zhiwuduotai.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gtw.gzhubu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://krp.gzhubu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://idy.gogol.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://psk.iojbl.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zug.nanxuanxn.top

Go:   strings.TrimSpace(s)
来源：http://inr.hfpthk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hxs.dashuyun.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xhp.ydjk.org.cn

[A25] 字符串比较
来源：http://pge.fengsongda.top

Py:   s1 == s2; s1 != s2
来源：http://htg.cashguo.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kjt.nanxuanxn.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rdh.jinghuilouyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ova.xinyue.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mqr.quarkkingdee.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sev.fanxiaobao.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://kuo.hysaishi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sng.jyoumei.cn

[A26] 类型转换总览
来源：http://bmd.nanxuanxn.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lpw.tarul.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gdv.jianghu66.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fgl.xylfe.cn

TS:   Number() String() Boolean() x as number
来源：http://lvf.aizwys.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jbw.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rpf.sjlbkw.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://njt.yueranfly.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nla.guowangkeji.top

================================================================================
来源：http://gnf.sxryk.cn

B. 流程控制
来源：http://ysg.nanxuanxn.top

================================================================================
来源：http://wsk.cqqwz.cn

[B01] 条件判断 if / else
来源：http://kkl.mhx1999.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rzj.xylfe.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mwh.jinqigfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ufo.vehdjk.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://omt.hnxiangtu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://sks.yj20258.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://omv.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cta.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uxa.jqgufenzy.top

[B02] 多分支 else if / elif
来源：http://odl.nanxinkj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vgo.fengsongda.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bnt.nanxinkj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hjd.aibaodan.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cqm.meibo888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lcu.sxryk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nbi.ydjk.org.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cmk.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bcl.nwbrower.top

[B03] switch / match / case
来源：http://edv.hesvh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sro.shangyingyoupin.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baj.chenzaomai.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nkc.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dwd.cheryme.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rja.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vqz.hongshengwenyu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qoc.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://scg.zhixingplan.top

[B04] for 计数循环
来源：http://xuu.kuanghao11.cn

Py:   for i in range(10): print(i)
来源：http://tql.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oeg.zycfv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uoi.meibo888.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lxp.fktsv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nxc.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hns.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://qzh.yuxming.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ven.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://vdv.xuanzx.com

Py:   for item in arr: print(item)
来源：http://thj.aibaodan.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qcp.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://eyh.uphjek.com

TS:   for (const item of arr) { console.log(item); }
来源：http://uqk.jinqigufen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vsz.shuidangran.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mdz.zhixingplan.top

Ruby: arr.each { |item| puts item }
来源：http://xpj.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://icy.bjfxy.top

[B06] 遍历字典 / 对象
来源：http://cci.hesvh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://aei.316326.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eid.cqqwz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://giy.sjlbkw.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lxi.guowangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://njz.yfazqb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lfe.daria6918.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wai.gzhubu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://chi.haohaochexian.top

[B07] while 循环
来源：http://mpd.ctjpmb.com

Py:   while i < 10: i += 1
来源：http://azz.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://svl.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://nvs.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://fqg.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://anm.yanxiufei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xzv.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://ats.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://ruk.yangfankeji.com

[B08] do-while（至少执行一次）
来源：http://uzd.bjfxy.top

Py:   # 无 do-while：用 while True + break
来源：http://pzz.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://rpl.c1oappe.top

JS:   do { i++; } while (i < 10);
来源：http://mda.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://vxw.meibo888.top

Java: do { i++; } while (i < 10);
来源：http://mcx.ydjk.org.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://inx.bbcook.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pcf.gaohongyu789.top

C#:   do { i++; } while (i < 10);
来源：http://whn.tanke756.top

[B09] break 与 continue
来源：http://mga.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kff.pengpengdd.cyou

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://syb.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eaa.shanyushiyangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aje.daria6918.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xgf.c1oappe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://faa.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fkl.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnw.mhx1999.top

[B10] 遍历同时拿索引
来源：http://mos.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qaw.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tun.hywenlv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jse.meibo888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://djz.tianlin.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ohz.iojbl.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ekh.sjlbkw.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dtk.vehdjk.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xzr.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://xuj.ydzc1.top

Py:   list(range(0, 10, 2))
来源：http://apv.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://kiz.ydzc1.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://joq.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gne.dashuyun.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fit.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mht.yj20258888.top

Ruby: (0...10).step(2).to_a
来源：http://zgs.havefunace.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tny.redwolf501.top

[B12] 跳出多层循环
来源：http://fio.smart0.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://mww.cdnleiting.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dmu.jqgufenzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nrm.ehwqpu.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zwv.jinqigufen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ldi.guowangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xby.aibaodan.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mya.nanxuanxn.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jdu.daria6918.cn

[B13] 判断是否为数字
来源：http://dob.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://fey.shuidangran.top

PHP:  is_numeric($x)
来源：http://bpf.xinyue.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zex.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fxc.xziqi.cn

Java: x instanceof Number
来源：http://bnf.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tzm.guannengcc.top

Ruby: x.is_a?(Numeric)
来源：http://lvb.ctjpmb.com

C#:   x is int or double or decimal
来源：http://thy.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://udv.hesvh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kyd.cdnleiting.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fii.nanxinkj.top

JS:   [1, 2, 3].includes(x)
来源：http://sng.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://gso.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gsv.meibo888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rvn.hfpthk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dan.52xcode.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fom.sweek.top

[B15] 布尔运算与取反
来源：http://wet.feifeiyinyue.top

Py:   a and b or not c
来源：http://hbi.gaohongyu789.top

PHP:  $a && $b || !$c
来源：http://xpw.birdmap.top

JS:   a && b || !c
来源：http://nfo.jqgufenzy.top

TS:   a && b || !c
来源：http://xoc.uphjek.com

Java: a && b || !c
来源：http://ycf.tarul.cn

Go:   a && b || !c
来源：http://nip.hcnkem.com

Ruby: a && b || !c
来源：http://sjf.yj20258888.top

C#:   a && b || !c
来源：http://dkt.vehdjk.com

[B16] 卫语句：不满足条件提前返回
来源：http://euo.nwbrower.top

Py:   if not data: return
来源：http://vtc.9152youxi.cn

PHP:  if (!$data) { return; }
来源：http://xtz.ydzc1.top

JS:   if (!data) return;
来源：http://izp.aibaodan.cn

TS:   if (!data) return;
来源：http://zxo.yvedp.cn

Java: if (data == null) return;
来源：http://tax.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://ldt.nanxuanxn.top

Ruby: return if data.nil?
来源：http://riw.redwolf501.top

C#:   if (data == null) return;
来源：http://kxt.zycfv.cn

================================================================================
来源：http://rde.sysykeji.top

C. 函数与作用域
来源：http://yxx.tian-w.cn

================================================================================
来源：http://psh.fktsv.cn

[C01] 定义函数
来源：http://gbw.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://oie.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ufo.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://psq.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rdv.shanyushiyangtech.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qae.yj20258.top

Go:   func add(a, b int) int { return a + b }
来源：http://jzw.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://hzh.yvedp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wqo.hcnkem.com

[C02] 默认参数
来源：http://qjx.sweek.top

Py:   def greet(name="World"): return name
来源：http://sdi.quarkkingdee.top

PHP:  function greet($name = "World") { return $name; }
来源：http://aad.redwolf501.top

JS:   function greet(name = "World") { return name; }
来源：http://dir.tarul.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://plr.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oni.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zta.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://ohl.zhengqikj.top

C#:   string Greet(string name = "World") => name;
来源：http://tbu.xylfe.cn

[C03] 可变参数
来源：http://dej.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://lnj.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rwb.zhijiandao.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dwz.fzhhl.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qra.chenlongwang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nrt.hysaishi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tdt.jqgfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://tvm.hammf.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ath.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://rsp.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vrw.gzhubu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jvm.nanxinkj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pgg.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ndu.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://lvl.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://bdr.yj202588.top

Ruby: f(a: 1, b: 2)
来源：http://iur.hywenlv.cn

C#:   f(a: 1, b: 2)
来源：http://chn.tanke756.top

[C05] 返回多个值
来源：http://zzi.sweek.top

Py:   return a, b
来源：http://ltd.guannengcc.top

PHP:  return [$a, $b];
来源：http://ozy.cdnleiting.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tco.jqgufenzy.top

TS:   return { a, b };
来源：http://gtc.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zyi.guannengcc.top

Go:   return a, b
来源：http://ptn.iojbl.cn

Ruby: return a, b
来源：http://cwe.chenjidiqi.icu

C#:   return (a, b);              // ValueTuple
来源：http://tqf.yuanzhike.top

[C06] 匿名函数 / lambda
来源：http://vxs.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://qiw.shzxlz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jjt.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://kah.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://ufp.sweek.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fly.wangdashe.top

Go:   sq := func(x int) int { return x * x }
来源：http://pvt.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://vlz.zhixingplan.top

C#:   Func<int, int> square = x => x * x;
来源：http://esc.yueranfly.top

[C07] 把函数作为参数传入
来源：http://ooy.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aat.sweek.top

PHP:  array_map("strtoupper", $arr);
来源：http://axu.sjlbkw.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ddx.jianghu66.top

TS:   arr.map(String)
来源：http://ftf.yonumen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vpa.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ttm.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://nfo.nwbrower.top

C#:   arr.Select(s => s.ToUpper())
来源：http://isd.uphjek.com

[C08] 闭包
来源：http://osn.shanyushiyangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wao.cashguo.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://thh.cqqwz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uwf.jinqigufen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kri.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sbl.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vmp.hnqzz.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yww.yuanzhike.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qis.chenzaomai.com

[C09] 递归
来源：http://iae.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oxv.uphjek.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://caf.yanxiufei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rzl.316326.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cej.jinqigfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mau.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lcp.xuetiantiany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://srl.yj20258888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hks.yonumen.top

[C10] 变量作用域
来源：http://twb.havefunace.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mrh.ehwqpu.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gta.fktsv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kxd.quarkkingdee.top

TS:   同 JS
来源：http://xfc.bbcook.cn

Java: 方法内为块级作用域
来源：http://wah.cqqwz.cn

Go:   花括号块级作用域
来源：http://xaj.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eak.yj202588.top

C#:   块级作用域
来源：http://nwl.zhoulong.xyz

[C11] 模块导入与导出
来源：http://zwj.epnwcf.com

Py:   from module import func
来源：http://jyy.gotoacloud.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hby.sweek.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://phn.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xhe.hywenlv.cn

Java: import java.util.List;
来源：http://aza.quarkkingdee.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hpa.yangfankeji.com

Ruby: require "json"; require_relative "./util"
来源：http://fmm.aizwys.cn

C#:   using System.Text;
来源：http://ooy.fehbvm.com

[C12] 立即执行函数 IIFE
来源：http://ybs.jlsjyb.cn

Py:   (lambda: print("run"))()
来源：http://bso.wangshuangyany.cn

PHP:  (function () { echo "run"; })();
来源：http://oka.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://obo.jlsjyb.cn

TS:   (() => { console.log("run"); })();
来源：http://zla.yanxiufei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ggk.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://dam.mhx1999.top

Ruby: -> { puts "run" }.call
来源：http://ybd.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ygf.ctjpmb.com

[C13] 类型声明 / 类型注解
来源：http://lkv.xuetiantiany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vcf.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://omw.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lmb.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://puh.chenjidiqi.icu

Java: int add(int a, int b) { return a + b; }
来源：http://pcp.cucudq.cn

Go:   func add(a, b int) int
来源：http://fdn.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cmj.wangshuangyany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nnu.tanke756.top

[C14] 泛型函数
来源：http://bia.mhx1999.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://emi.zdbjq.cn

PHP:  // 无泛型
来源：http://kkh.bbcook.cn

JS:   // 无泛型
来源：http://xcz.shangyingyoupin.top


<!-- 参考信息 -->