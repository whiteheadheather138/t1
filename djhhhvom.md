代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://kmq.ybcxt.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tug.sxryk.cn

JS:   (3.14159).toFixed(2)
来源：http://jzs.cucudq.cn

TS:   (3.14159).toFixed(2)
来源：http://luv.guannengcc.top

Java: String.format("%.2f", 3.14159)
来源：http://jxj.nanxuanxn.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jgs.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://foi.0kj1m.cn

C#:   3.14159.ToString("F2")
来源：http://ncb.xziqi.cn

[A22] 获取字符串长度
来源：http://dgo.xuanzx.com

Py:   len(s)
来源：http://bqq.shzxlz.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rdp.hnxiangtu.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rof.zhaomingkeji.xyz

TS:   s.length
来源：http://chs.gzhubu.top

Java: s.length()
来源：http://gjf.yj20258888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xaa.ybcxt.top

Ruby: s.length
来源：http://fiq.meibo888.top

C#:   s.Length
来源：http://rqq.xylfe.cn

[A23] 大小写转换
来源：http://euw.ydjk.org.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sgl.dashuyun.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nhx.pycfn.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fkq.daria6918.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vba.nanxuanxn.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qli.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rlo.chenlongwang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zwf.jyoumei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qdm.gogol.net.cn

[A24] 去除首尾空白
来源：http://goc.epnwcf.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kdy.snrcjt.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bav.c1oappe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uzq.dianchejie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gjo.zhaomingkeji.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jig.9152youxi.cn

Go:   strings.TrimSpace(s)
来源：http://snu.chenlongwang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vtd.kuanghao11.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://frr.aibaodan.cn

[A25] 字符串比较
来源：http://nre.gogol.net.cn

Py:   s1 == s2; s1 != s2
来源：http://hxu.fzhhl.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bhx.tarul.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uwz.hysaishi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vip.c1oappe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yop.svipenyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ucg.meibo888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tai.yueranfly.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uie.guowangkeji.top

[A26] 类型转换总览
来源：http://urd.bbcook.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qjk.ctjpmb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hlg.ehwqpu.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ffy.yangfankeji.com

TS:   Number() String() Boolean() x as number
来源：http://ckd.jyoumei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kos.9152youxi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ikz.fehbvm.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://xxn.yueranfly.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vjj.sjlbkw.cn

================================================================================
来源：http://jtb.tarul.cn

B. 流程控制
来源：http://kbr.chenlongwang.top

================================================================================
来源：http://xyy.dianchejie.cn

[B01] 条件判断 if / else
来源：http://gux.quarkkingdee.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ldr.xuanzx.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lni.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ptk.jinqigufen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aqn.mhx1999.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mtt.hesvh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jzk.yj20258.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cvk.snrcjt.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ybz.yj202588.top

[B02] 多分支 else if / elif
来源：http://oxp.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xqk.zhongyouzk.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bii.jqgufenzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xbp.yangfankeji.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yzh.vqdsnc.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ffi.iojbl.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hbe.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sjr.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tak.ppjwa.cn

[B03] switch / match / case
来源：http://nmx.yonumen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mcw.zdqjudy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wxa.52xcode.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mxj.epnwcf.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gvh.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vpj.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ecx.sjlbkw.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://whn.havefunace.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ata.zhongyouzk.top

[B04] for 计数循环
来源：http://xhe.zhaomingkeji.xyz

Py:   for i in range(10): print(i)
来源：http://tvk.iojbl.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://scr.cdnleiting.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jmi.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yju.dashuyun.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://epq.jyoumei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qgq.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://dom.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hge.quarkkingdee.top

[B05] 遍历数组 / 列表
来源：http://dxt.tanke756.top

Py:   for item in arr: print(item)
来源：http://vwq.yfazqb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hpq.hcnkem.com

JS:   for (const item of arr) { console.log(item); }
来源：http://rkn.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qps.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tji.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eoc.chenlongwang.top

Ruby: arr.each { |item| puts item }
来源：http://zcc.gzhubu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vet.ybcxt.top

[B06] 遍历字典 / 对象
来源：http://zau.vqdsnc.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gqa.wangshuangyany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ddp.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hvf.xziqi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tda.yueranfly.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yso.hongshengwenyu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wyg.jinqigufen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ylc.zhaomingkeji.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mcl.haohaochexian.top

[B07] while 循环
来源：http://clh.daxiang520.top

Py:   while i < 10: i += 1
来源：http://rab.fzhhl.top

PHP:  while ($i < 10) { $i++; }
来源：http://wkm.hongshengwenyu.top

JS:   while (i < 10) { i++; }
来源：http://kor.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://tuj.pycfn.com

Java: while (i < 10) { i++; }
来源：http://wiy.zhiwuduotai.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hdu.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://iwj.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://edb.dashuyun.cn

[B08] do-while（至少执行一次）
来源：http://wdb.hnqzz.top

Py:   # 无 do-while：用 while True + break
来源：http://bua.nwbrower.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qjm.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://yyr.aibaodan.cn

TS:   do { i++; } while (i < 10);
来源：http://vme.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://tju.sxryk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vdk.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://bgd.snrcjt.cn

C#:   do { i++; } while (i < 10);
来源：http://sdd.hnqzz.top

[B09] break 与 continue
来源：http://ntq.ybcxt.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rrv.vehdjk.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nqw.jlsjyb.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sww.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wzq.shanyushiyangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xao.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fju.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ykz.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixs.zhongyouzk.top

[B10] 遍历同时拿索引
来源：http://hri.fehbvm.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://azi.zhongyouzk.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://daz.nanxinkj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://emz.gotoacloud.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://asg.ctjpmb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yaq.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lhp.jianghu66.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ygk.hfpthk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ghf.9152youxi.cn

[B11] 生成数字序列 / 区间
来源：http://ubl.fzhhl.top

Py:   list(range(0, 10, 2))
来源：http://mqs.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://upp.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gvi.smart0.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bef.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oai.zhiwuduotai.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wry.zhijiandao.cn

Ruby: (0...10).step(2).to_a
来源：http://plm.haohaochexian.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://srk.fanxiaobao.xyz

[B12] 跳出多层循环
来源：http://gcw.bjfxy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://whf.tianlin.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://bfi.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rjx.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xew.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zny.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uhb.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nqa.hnqzz.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lfc.uphjek.com

[B13] 判断是否为数字
来源：http://oaa.ehwqpu.com

Py:   isinstance(x, (int, float))
来源：http://hes.redwolf501.top

PHP:  is_numeric($x)
来源：http://rdg.jqgufenzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kpl.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wwg.epnwcf.com

Java: x instanceof Number
来源：http://jal.sxryk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tqt.jinqigufen.top

Ruby: x.is_a?(Numeric)
来源：http://kvz.yvedp.cn

C#:   x is int or double or decimal
来源：http://gyy.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://rys.birdmap.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://opq.gaohongyu789.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ubw.shuidangran.top

JS:   [1, 2, 3].includes(x)
来源：http://etb.ydjk.org.cn

TS:   [1, 2, 3].includes(x)
来源：http://tmg.chenzaomai.com

Java: List.of(1, 2, 3).contains(x)
来源：http://gna.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yej.redwolf501.top

Ruby: [1, 2, 3].include?(x)
来源：http://wmd.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vqc.chenjidiqi.icu

[B15] 布尔运算与取反
来源：http://qlv.hfpthk.cn

Py:   a and b or not c
来源：http://tpj.zdqjudy.top

PHP:  $a && $b || !$c
来源：http://fgm.yonumen.top

JS:   a && b || !c
来源：http://tiy.hysaishi.cn

TS:   a && b || !c
来源：http://atr.cheryme.top

Java: a && b || !c
来源：http://awc.nanxuanxn.top

Go:   a && b || !c
来源：http://yep.hesvh.cn

Ruby: a && b || !c
来源：http://evt.wangshuangyany.cn

C#:   a && b || !c
来源：http://gdq.xingfuxueyuan.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ejd.mhx1999.top

Py:   if not data: return
来源：http://rhm.hcnkem.com

PHP:  if (!$data) { return; }
来源：http://cct.zhaomingkeji.xyz

JS:   if (!data) return;
来源：http://lko.pengpengdd.cyou

TS:   if (!data) return;
来源：http://dpl.yj20258888.top

Java: if (data == null) return;
来源：http://txm.ppjwa.cn

Go:   if data == nil { return }
来源：http://ydh.wangdashe.top

Ruby: return if data.nil?
来源：http://eko.tianlin.xyz

C#:   if (data == null) return;
来源：http://xut.yuxming.cn

================================================================================
来源：http://qgi.zhoulong.xyz

C. 函数与作用域
来源：http://iau.zhaomingkeji.xyz

================================================================================
来源：http://mog.wangshuangyany.cn

[C01] 定义函数
来源：http://isx.zhaomingkeji.xyz

Py:   def add(a, b): return a + b
来源：http://zqa.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xkk.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://zlf.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zlf.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hof.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://lfh.yvedp.cn

Ruby: def add(a, b); a + b; end
来源：http://ikh.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rss.nanxuanxn.top

[C02] 默认参数
来源：http://nrx.tanke756.top

Py:   def greet(name="World"): return name
来源：http://yau.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gym.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://tim.tarul.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cda.xinyue.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://jcp.cqqwz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gvg.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://uef.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://ymf.jianghu66.top

[C03] 可变参数
来源：http://myv.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://myp.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eks.nwbrower.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://omj.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dmg.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://btd.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://moz.chenlongwang.top

Ruby: def total(*nums); nums.sum; end
来源：http://nlu.birdmap.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://elw.vqdsnc.cn

[C04] 命名参数 / 关键字参数
来源：http://brl.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://auh.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xzm.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hxz.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mwx.fzhhl.top

Java: // 无：用 Builder 模式或 record
来源：http://btd.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://ltz.chenjidiqi.icu

Ruby: f(a: 1, b: 2)
来源：http://hxw.hammf.cn

C#:   f(a: 1, b: 2)
来源：http://pbh.yj20258888.top

[C05] 返回多个值
来源：http://uwb.smart0.xyz

Py:   return a, b
来源：http://cxo.gaohongyu789.top

PHP:  return [$a, $b];
来源：http://hwh.cdnleiting.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fag.tianlin.xyz

TS:   return { a, b };
来源：http://yfj.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pbv.zdqjudy.top

Go:   return a, b
来源：http://qgf.fktsv.cn

Ruby: return a, b
来源：http://jih.ppjwa.cn

C#:   return (a, b);              // ValueTuple
来源：http://icg.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://izk.aizwys.cn

Py:   square = lambda x: x * x
来源：http://mhz.zdbjq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wtv.jiagoushi.top

JS:   const square = x => x * x;
来源：http://wfe.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://dcm.wangdashe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xvi.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://fos.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://ldd.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://gak.andypj.xyz

[C07] 把函数作为参数传入
来源：http://pzd.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uwr.redwolf501.top

PHP:  array_map("strtoupper", $arr);
来源：http://wof.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lur.shangyingyoupin.top

TS:   arr.map(String)
来源：http://lbo.fktsv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fgg.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://urm.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://hqo.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zoq.yuxming.cn

[C08] 闭包
来源：http://xae.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://inx.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aoh.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tox.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fkc.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hbp.pengpengdd.cyou

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zdg.gotoacloud.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lyl.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bxw.ywan-chungtsiang.top

[C09] 递归
来源：http://jtv.pengpengdd.cyou

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pss.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sfg.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mnj.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kbj.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hip.xziqi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rda.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://naw.meibo888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yvq.xuanzx.com

[C10] 变量作用域
来源：http://sgi.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lwg.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://glw.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xvs.xuanzx.com

TS:   同 JS
来源：http://gcs.chenlongwang.top

Java: 方法内为块级作用域
来源：http://yvk.uphjek.com

Go:   花括号块级作用域
来源：http://afi.hongshengwenyu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hmw.shanyushiyangkeji.top

C#:   块级作用域
来源：http://nja.bjfxy.top

[C11] 模块导入与导出
来源：http://qht.zhengqikj.top

Py:   from module import func
来源：http://zvf.zycfv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://syt.andypj.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://tfb.xingfuxueyuan.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://flb.sweek.top

Java: import java.util.List;
来源：http://hlp.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vwg.ydzc1.top


<!-- 参考信息 -->