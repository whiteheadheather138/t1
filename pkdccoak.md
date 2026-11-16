代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rit.shanyushiyangtech.top

Ruby: gets.chomp
来源：http://dad.hysaishi.cn

C#:   Console.ReadLine();
来源：http://ajb.jyoumei.cn

[A21] 保留指定小数位输出
来源：http://psd.meibo888.top

Py:   f"{3.14159:.2f}"
来源：http://cbw.aizwys.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kkq.ppjwa.cn

JS:   (3.14159).toFixed(2)
来源：http://zys.316326.xyz

TS:   (3.14159).toFixed(2)
来源：http://wnr.redwolf501.top

Java: String.format("%.2f", 3.14159)
来源：http://dlo.sjlbkw.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yaq.tianlin.xyz

Ruby: format("%.2f", 3.14159)
来源：http://bog.quarkkingdee.top

C#:   3.14159.ToString("F2")
来源：http://cfc.yj202588.top

[A22] 获取字符串长度
来源：http://rzz.guowangkeji.top

Py:   len(s)
来源：http://ulu.hysaishi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sgu.yj202588.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rbl.smart0.xyz

TS:   s.length
来源：http://wiz.hnxiangtu.top

Java: s.length()
来源：http://rjd.pycfn.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ssy.guannengcc.top

Ruby: s.length
来源：http://apd.tanke756.top

C#:   s.Length
来源：http://jzw.yj202588.top

[A23] 大小写转换
来源：http://kum.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pmy.shanyushiyangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rms.zhengqikj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eaj.cqqwz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://syo.jqgufenzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lyr.cdnleiting.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jkg.shuidangran.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gkc.hnxiangtu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://cjh.zdqjudy.top

[A24] 去除首尾空白
来源：http://sfs.fktsv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gen.fanxiaobao.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pzw.sweek.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vko.vehdjk.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ofo.jianghu66.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ode.andypj.xyz

Go:   strings.TrimSpace(s)
来源：http://fvg.chenzaomai.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hng.gotoacloud.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://psx.pengpengdd.cyou

[A25] 字符串比较
来源：http://lua.cdnleiting.top

Py:   s1 == s2; s1 != s2
来源：http://wcd.ehwqpu.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sjr.yj20258.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://umk.9152youxi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zhi.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uki.hesvh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hxg.c1oappe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ixj.zhaomingkeji.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zgq.daxiang520.top

[A26] 类型转换总览
来源：http://sjk.vehdjk.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://whe.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rsj.zdqjudy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oll.sjlbkw.cn

TS:   Number() String() Boolean() x as number
来源：http://fyh.cdnleiting.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://euz.jianghu66.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uoi.tanke756.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qse.yueranfly.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rdk.yangfankeji.com

================================================================================
来源：http://blf.guowangkeji.top

B. 流程控制
来源：http://zeq.guowangkeji.top

================================================================================
来源：http://qqq.hywenlv.cn

[B01] 条件判断 if / else
来源：http://azt.meibo888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bwr.zhaomingkeji.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wrf.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lqg.zycfv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pnq.sufxvd.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zge.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wvw.yj20258.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dca.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mpk.hfpthk.cn

[B02] 多分支 else if / elif
来源：http://sjx.vqdsnc.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tjy.bjfxy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wzt.fehbvm.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gzo.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fvb.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ore.jinghuilouyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://riv.meibo888.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://twe.bbcook.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hkt.9152youxi.cn

[B03] switch / match / case
来源：http://riy.hnqzz.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nka.feifeiyinyue.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qrc.mhx1999.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yes.quarkkingdee.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://omb.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bjc.tianlin.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ohs.zdqjudy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://inq.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://udi.zhongyouzk.top

[B04] for 计数循环
来源：http://pvt.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://adr.tanke756.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vwv.chenlongwang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://brp.yuanzhike.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hcc.yueranfly.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oic.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tkr.sjlbkw.cn

Ruby: 10.times { |i| puts i }
来源：http://wcx.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://koj.gotoacloud.top

[B05] 遍历数组 / 列表
来源：http://nux.bjfxy.top

Py:   for item in arr: print(item)
来源：http://spx.gzhubu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wde.yueranfly.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jtn.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://uxw.shanyushiyangtech.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://npy.cucudq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pum.daxiang520.top

Ruby: arr.each { |item| puts item }
来源：http://cln.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aps.havefunace.top

[B06] 遍历字典 / 对象
来源：http://yhq.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://syz.shanyushiyangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eiw.havefunace.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fsf.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gfn.redwolf501.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hjm.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pnf.9152youxi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qig.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://llq.cheryme.top

[B07] while 循环
来源：http://vzy.yvedp.cn

Py:   while i < 10: i += 1
来源：http://kgq.jinqigfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://fhb.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://cxp.vqdsnc.cn

TS:   while (i < 10) { i++; }
来源：http://ptx.pycfn.com

Java: while (i < 10) { i++; }
来源：http://nac.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kop.tarul.cn

Ruby: while i < 10; i += 1; end
来源：http://pas.316326.xyz

C#:   while (i < 10) { i++; }
来源：http://izi.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://gpx.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://byt.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cbw.snrcjt.cn

JS:   do { i++; } while (i < 10);
来源：http://tqq.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://nhy.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://tcp.vehdjk.com

Go:   for { i++; if i >= 10 { break } }
来源：http://wpk.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://xxd.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://xpt.jqgufenzy.top

[B09] break 与 continue
来源：http://ruv.zhiwuduotai.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://spw.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://shr.yj20258.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ahb.fktsv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gyf.cheryme.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://agy.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qqw.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ewl.hysaishi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pwp.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://mvo.0kj1m.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gvp.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zaw.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nel.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vct.birdmap.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://btp.chenlongwang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sxk.yj20258.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fgq.jinghuilouyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sjq.xylfe.cn

[B11] 生成数字序列 / 区间
来源：http://zls.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://jst.uphjek.com

PHP:  range(0, 10, 2);
来源：http://lxr.andypj.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vjn.redwolf501.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qwa.yj20258888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vdg.aibaodan.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sqy.zhiwuduotai.top

Ruby: (0...10).step(2).to_a
来源：http://man.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fdd.zhiwuduotai.top

[B12] 跳出多层循环
来源：http://ptw.c1oappe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hsf.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://hnw.hcnkem.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qaq.zhiwuduotai.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://igm.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qdg.chenjidiqi.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ncb.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ipj.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ekw.52xcode.cn

[B13] 判断是否为数字
来源：http://atz.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://zia.yueranfly.top

PHP:  is_numeric($x)
来源：http://zlr.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pft.wangshuangyany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xsf.ydzc1.top

Java: x instanceof Number
来源：http://ubx.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kbi.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://zkc.yuanzhike.top

C#:   x is int or double or decimal
来源：http://pqe.sxryk.cn

[B14] 判断值是否在集合内
来源：http://lsd.nwbrower.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ztj.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ekt.tianlin.xyz

JS:   [1, 2, 3].includes(x)
来源：http://hvp.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://tfp.yfazqb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://obv.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kum.zycfv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://avp.cheryme.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kue.316326.xyz

[B15] 布尔运算与取反
来源：http://dbr.hnxiangtu.top

Py:   a and b or not c
来源：http://net.ybcxt.top

PHP:  $a && $b || !$c
来源：http://rta.sysykeji.top

JS:   a && b || !c
来源：http://adv.bbcook.cn

TS:   a && b || !c
来源：http://six.hesvh.cn

Java: a && b || !c
来源：http://ipx.ctjpmb.com

Go:   a && b || !c
来源：http://ejd.sxryk.cn

Ruby: a && b || !c
来源：http://xvi.ywan-chungtsiang.top

C#:   a && b || !c
来源：http://gff.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://prb.yfazqb.com

Py:   if not data: return
来源：http://mej.zhixingplan.top

PHP:  if (!$data) { return; }
来源：http://nai.cashguo.top

JS:   if (!data) return;
来源：http://qbk.tianlin.xyz

TS:   if (!data) return;
来源：http://nss.jqgfzy.top

Java: if (data == null) return;
来源：http://uvd.svipenyu.cn

Go:   if data == nil { return }
来源：http://feq.redwolf501.top

Ruby: return if data.nil?
来源：http://web.jiagoushi.top

C#:   if (data == null) return;
来源：http://zfy.shanyushiyangkeji.top

================================================================================
来源：http://wkt.hesvh.cn

C. 函数与作用域
来源：http://ovy.xylfe.cn

================================================================================
来源：http://dxr.52xcode.cn

[C01] 定义函数
来源：http://nrd.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://sft.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cma.chenlongwang.top

JS:   function add(a, b) { return a + b; }
来源：http://kfm.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ntv.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://zbh.hcnkem.com

Go:   func add(a, b int) int { return a + b }
来源：http://mgj.c1oappe.top

Ruby: def add(a, b); a + b; end
来源：http://bbu.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mny.hammf.cn

[C02] 默认参数
来源：http://rok.dashuyun.cn

Py:   def greet(name="World"): return name
来源：http://urn.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://usc.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://qnz.sufxvd.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ssk.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oee.zycfv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bwu.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://qyi.tianlin.xyz

C#:   string Greet(string name = "World") => name;
来源：http://xzh.hesvh.cn

[C03] 可变参数
来源：http://spa.zhongyouzk.top

Py:   def total(*args): return sum(args)
来源：http://zxg.yj202588.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://flp.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://beg.chenzaomai.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://upb.jianghu66.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sbe.yuanzhike.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tje.zycfv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jjh.hnqzz.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dhc.shzxlz.cn

[C04] 命名参数 / 关键字参数
来源：http://izn.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nsf.jlsjyb.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xsf.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://obg.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://waz.fktsv.cn

Java: // 无：用 Builder 模式或 record
来源：http://ccs.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://fon.wangdashe.top

Ruby: f(a: 1, b: 2)
来源：http://lro.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://jox.xziqi.cn

[C05] 返回多个值
来源：http://wtm.zhoulong.xyz

Py:   return a, b
来源：http://ccp.sweek.top

PHP:  return [$a, $b];
来源：http://lix.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lge.zhiwuduotai.top

TS:   return { a, b };
来源：http://uzv.iojbl.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ziq.xuanzx.com

Go:   return a, b
来源：http://all.hcnkem.com

Ruby: return a, b
来源：http://mov.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://tfe.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://kpv.dashuyun.cn

Py:   square = lambda x: x * x
来源：http://rkm.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cqa.chenjidiqi.icu

JS:   const square = x => x * x;
来源：http://fzm.pengpengdd.cyou

TS:   const square = (x: number): number => x * x;
来源：http://ieb.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vuc.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://edm.yuanzhike.top

Ruby: square = ->(x) { x * x }
来源：http://tgx.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://ana.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://hdx.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jaz.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://twa.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nxs.iojbl.cn

TS:   arr.map(String)
来源：http://fgg.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zre.mhx1999.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zqu.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://wew.sjlbkw.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yyf.bjfxy.top

[C08] 闭包
来源：http://xad.bjfxy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nvb.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uti.xuetiantiany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pmr.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uhk.0kj1m.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ics.tanke756.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lbh.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vlb.cucudq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://inw.jlsjyb.cn

[C09] 递归
来源：http://axr.redwolf501.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gdd.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eqw.tianlin.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cin.cqqwz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yvl.jiagoushi.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tjn.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rto.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mjs.hfpthk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ecu.sweek.top

[C10] 变量作用域
来源：http://zcu.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hih.yongpay.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nkl.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kzb.gogol.net.cn

TS:   同 JS
来源：http://ksk.nwbrower.top

Java: 方法内为块级作用域
来源：http://dwr.jlsjyb.cn

Go:   花括号块级作用域
来源：http://kxb.bjfxy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ket.andypj.xyz

C#:   块级作用域
来源：http://zhl.jinqigfzy.top

[C11] 模块导入与导出
来源：http://mhl.yuxming.cn

Py:   from module import func
来源：http://jnd.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kbk.chenjidiqi.icu


<!-- 参考信息 -->