代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://isj.yuanzhike.top

Ruby: gets.chomp
来源：http://zko.nwbrower.top

C#:   Console.ReadLine();
来源：http://ykf.shanyushiyangkeji.top

[A21] 保留指定小数位输出
来源：http://zda.bjfxy.top

Py:   f"{3.14159:.2f}"
来源：http://zfn.cucudq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vlk.gaohongyu789.top

JS:   (3.14159).toFixed(2)
来源：http://mmi.52xcode.cn

TS:   (3.14159).toFixed(2)
来源：http://brb.fehbvm.com

Java: String.format("%.2f", 3.14159)
来源：http://oqy.zhixingplan.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lun.tarul.cn

Ruby: format("%.2f", 3.14159)
来源：http://xyr.fzhhl.top

C#:   3.14159.ToString("F2")
来源：http://pfl.guannengcc.top

[A22] 获取字符串长度
来源：http://axz.jqgfzy.top

Py:   len(s)
来源：http://uyz.gogol.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uwu.zycfv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fpq.gaohongyu789.top

TS:   s.length
来源：http://cjz.quarkkingdee.top

Java: s.length()
来源：http://ltv.52xcode.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ejz.hnxiangtu.top

Ruby: s.length
来源：http://yhm.hnqzz.top

C#:   s.Length
来源：http://jsk.nanxuanxn.top

[A23] 大小写转换
来源：http://yvy.shuidangran.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pji.yuxming.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rvb.wangshuangyany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xgf.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jjg.vqdsnc.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hsi.9152youxi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://giv.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://umv.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://esl.andypj.xyz

[A24] 去除首尾空白
来源：http://yvv.hysaishi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://krr.jyoumei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qra.fzhhl.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cao.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pzw.havefunace.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hzi.jinqigfzy.top

Go:   strings.TrimSpace(s)
来源：http://ple.yj20258.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dwb.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ipi.shanyushiyangkeji.top

[A25] 字符串比较
来源：http://fay.ehwqpu.com

Py:   s1 == s2; s1 != s2
来源：http://fau.nwbrower.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gbo.yj20258888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hje.shuidangran.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lxe.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tam.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cnw.hammf.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wnq.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xwq.yj202588.top

[A26] 类型转换总览
来源：http://wwd.xuetiantiany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ojq.nanxuanxn.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gbz.ehwqpu.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qdh.andypj.xyz

TS:   Number() String() Boolean() x as number
来源：http://njb.gaohongyu789.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qng.yvedp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qme.shangyingyoupin.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zwh.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gng.gaohongyu789.top

================================================================================
来源：http://twn.xziqi.cn

B. 流程控制
来源：http://byv.hnqzz.top

================================================================================
来源：http://mqk.jiagoushi.top

[B01] 条件判断 if / else
来源：http://fto.yangfankeji.com

Py:   result = "正" if x > 0 else "非正"
来源：http://ezi.cqqwz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wws.meibo888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tbe.haohaochexian.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vhj.redwolf501.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://esr.hnqzz.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://riv.gotoacloud.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yxg.jlsjyb.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ntt.xziqi.cn

[B02] 多分支 else if / elif
来源：http://ntq.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eza.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ftr.zhixingplan.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bzw.zhijiandao.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ova.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ybe.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tfj.xylfe.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dza.hnxiangtu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gre.yangfankeji.com

[B03] switch / match / case
来源：http://yoh.shzxlz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wga.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jfk.yueranfly.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vog.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hyd.fehbvm.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://efc.chenjidiqi.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iyb.xingfuxueyuan.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hoa.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xyb.sjlbkw.cn

[B04] for 计数循环
来源：http://lri.jqgfzy.top

Py:   for i in range(10): print(i)
来源：http://qyo.ivvv.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uvn.gogol.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uur.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iiu.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hxv.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ubm.xuetiantiany.cn

Ruby: 10.times { |i| puts i }
来源：http://lua.ydjk.org.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wov.ehwqpu.com

[B05] 遍历数组 / 列表
来源：http://pvz.hywenlv.cn

Py:   for item in arr: print(item)
来源：http://xbx.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yrr.shanyushiyangtech.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vqg.xinyue.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://ipi.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uss.fanxiaobao.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vlj.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://bwx.hywenlv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://siq.shanyushiyangtech.top

[B06] 遍历字典 / 对象
来源：http://kir.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://pyw.daxiang520.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lbk.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dcu.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vmx.zhiwuduotai.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tai.aibaodan.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ton.yj20258.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mpr.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eih.pycfn.com

[B07] while 循环
来源：http://lqz.ybcxt.top

Py:   while i < 10: i += 1
来源：http://dig.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lbv.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://lnx.ppjwa.cn

TS:   while (i < 10) { i++; }
来源：http://mhg.sufxvd.cn

Java: while (i < 10) { i++; }
来源：http://yib.pengpengdd.cyou

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://igi.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://ifw.jinyuanbaomall.cn

C#:   while (i < 10) { i++; }
来源：http://nxr.yj202588.top

[B08] do-while（至少执行一次）
来源：http://ttg.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://mws.jiagoushi.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kie.wangdashe.top

JS:   do { i++; } while (i < 10);
来源：http://his.aibaodan.cn

TS:   do { i++; } while (i < 10);
来源：http://xga.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://aju.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nhn.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://bni.yuxming.cn

C#:   do { i++; } while (i < 10);
来源：http://ixd.chenzaomai.com

[B09] break 与 continue
来源：http://mvf.bbcook.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jgi.gaohongyu789.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jra.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ait.vqdsnc.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fll.ydjk.org.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rnc.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fpu.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xbm.zdqjudy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wkp.chenjidiqi.icu

[B10] 遍历同时拿索引
来源：http://lto.xylfe.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qdp.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://upq.yueranfly.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pzx.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rlk.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://drl.vehdjk.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://otx.bbcook.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oty.shanyushiyangtech.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xga.zhijiandao.cn

[B11] 生成数字序列 / 区间
来源：http://vnv.ppjwa.cn

Py:   list(range(0, 10, 2))
来源：http://civ.zycfv.cn

PHP:  range(0, 10, 2);
来源：http://adz.nanxuanxn.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bsx.jinqigfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lvc.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vtv.yonumen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rsw.bjfxy.top

Ruby: (0...10).step(2).to_a
来源：http://pqx.sufxvd.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://msv.ybcxt.top

[B12] 跳出多层循环
来源：http://lff.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://sbj.shangyingyoupin.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fsy.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qas.ivvv.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kmj.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ejh.fktsv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://azz.fzhhl.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dsz.shanyushiyangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ogl.sjlbkw.cn

[B13] 判断是否为数字
来源：http://fcr.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://dra.yfazqb.com

PHP:  is_numeric($x)
来源：http://yhh.chenzaomai.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pbr.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rwe.daria6918.cn

Java: x instanceof Number
来源：http://agx.cucudq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ycg.tian-w.cn

Ruby: x.is_a?(Numeric)
来源：http://isc.uphjek.com

C#:   x is int or double or decimal
来源：http://pgl.zhaomingkeji.xyz

[B14] 判断值是否在集合内
来源：http://wva.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xvd.bjfxy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zsp.jinqigufen.top

JS:   [1, 2, 3].includes(x)
来源：http://xzu.nanxuanxn.top

TS:   [1, 2, 3].includes(x)
来源：http://nqg.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://enz.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xqt.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://cyq.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zah.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://yvn.9152youxi.cn

Py:   a and b or not c
来源：http://dcl.vehdjk.com

PHP:  $a && $b || !$c
来源：http://ede.guannengcc.top

JS:   a && b || !c
来源：http://bwx.gzhubu.top

TS:   a && b || !c
来源：http://lmg.chenlongwang.top

Java: a && b || !c
来源：http://xgu.fktsv.cn

Go:   a && b || !c
来源：http://smq.zhiwuduotai.top

Ruby: a && b || !c
来源：http://dla.hesvh.cn

C#:   a && b || !c
来源：http://qhg.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://ygc.feifeiyinyue.top

Py:   if not data: return
来源：http://bff.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://sfj.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://gzf.316326.xyz

TS:   if (!data) return;
来源：http://jup.xuanzx.com

Java: if (data == null) return;
来源：http://lqg.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://pnk.yongpay.top

Ruby: return if data.nil?
来源：http://aks.sxryk.cn

C#:   if (data == null) return;
来源：http://nrb.tarul.cn

================================================================================
来源：http://ndf.fktsv.cn

C. 函数与作用域
来源：http://rzd.yongpay.top

================================================================================
来源：http://tbv.haohaochexian.top

[C01] 定义函数
来源：http://ldu.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://ajl.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kio.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://iiv.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hgn.fanxiaobao.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://muy.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://vhn.ydzc1.top

Ruby: def add(a, b); a + b; end
来源：http://csm.gotoacloud.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ilp.0kj1m.cn

[C02] 默认参数
来源：http://pls.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://dtc.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nko.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://zvk.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wct.hongshengwenyu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bjq.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://leq.cucudq.cn

Ruby: def greet(name = "World") = name
来源：http://euh.epnwcf.com

C#:   string Greet(string name = "World") => name;
来源：http://xqa.fengsongda.top

[C03] 可变参数
来源：http://ajt.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://fnj.fengsongda.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qgi.hfpthk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nrw.gogol.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gyh.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://psw.shanyushiyangtech.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nll.tianlin.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://qea.52xcode.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vqs.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://bpg.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ykx.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jvp.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qon.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://byc.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://svu.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://glt.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://yuw.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://ndn.hfpthk.cn

[C05] 返回多个值
来源：http://qac.chenzaomai.com

Py:   return a, b
来源：http://fht.tanke756.top

PHP:  return [$a, $b];
来源：http://isw.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kmb.feifeiyinyue.top

TS:   return { a, b };
来源：http://wok.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fyf.shzxlz.cn

Go:   return a, b
来源：http://hbd.chenjidiqi.icu

Ruby: return a, b
来源：http://quy.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://itu.c1oappe.top

[C06] 匿名函数 / lambda
来源：http://nvj.xylfe.cn

Py:   square = lambda x: x * x
来源：http://fal.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://bns.bjfxy.top

JS:   const square = x => x * x;
来源：http://gaj.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://meo.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nub.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://jye.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://ozg.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dxg.yj202588.top

[C07] 把函数作为参数传入
来源：http://exm.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xsw.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://raa.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ybr.hammf.cn

TS:   arr.map(String)
来源：http://zvq.sufxvd.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iyh.bjfxy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yyl.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://jnw.zdqjudy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pxd.uphjek.com

[C08] 闭包
来源：http://qlz.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xbe.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://feu.tanke756.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://amt.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sxp.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vht.hfpthk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ecd.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://frg.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pme.shzxlz.cn

[C09] 递归
来源：http://ttw.jlsjyb.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xgu.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eyt.shanyushiyangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://you.tianlin.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wjo.daria6918.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qkl.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fdg.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dnp.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uyx.shuidangran.top

[C10] 变量作用域
来源：http://kws.gaohongyu789.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rwa.fzhhl.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://enj.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gbs.shanyushiyangtech.top

TS:   同 JS
来源：http://hpw.gogol.net.cn

Java: 方法内为块级作用域
来源：http://aja.sweek.top

Go:   花括号块级作用域
来源：http://jko.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lrl.fehbvm.com

C#:   块级作用域
来源：http://jyy.snrcjt.cn

[C11] 模块导入与导出
来源：http://zhd.zhixingplan.top

Py:   from module import func
来源：http://kad.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ixi.yueranfly.top


<!-- 参考信息 -->