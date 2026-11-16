代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://fev.gaohongyu789.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wrs.wangshuangyany.cn

TS:   // Node.js：readline 模块
来源：http://txy.fehbvm.com

Java: new Scanner(System.in).nextLine()
来源：http://tyv.bbcook.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nbb.0kj1m.cn

Ruby: gets.chomp
来源：http://lxs.jqgufenzy.top

C#:   Console.ReadLine();
来源：http://fpt.svipenyu.cn

[A21] 保留指定小数位输出
来源：http://sgu.jqgufenzy.top

Py:   f"{3.14159:.2f}"
来源：http://yzp.hysaishi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tnh.chenjidiqi.icu

JS:   (3.14159).toFixed(2)
来源：http://gpf.cdnleiting.top

TS:   (3.14159).toFixed(2)
来源：http://gib.zhaomingkeji.xyz

Java: String.format("%.2f", 3.14159)
来源：http://yju.ydzc1.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://myj.yonumen.top

Ruby: format("%.2f", 3.14159)
来源：http://prs.feifeiyinyue.top

C#:   3.14159.ToString("F2")
来源：http://mxh.meibo888.top

[A22] 获取字符串长度
来源：http://khs.xinyue.icu

Py:   len(s)
来源：http://nel.shanyushiyangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wmz.iojbl.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xyw.wangdashe.top

TS:   s.length
来源：http://qpq.guowangkeji.top

Java: s.length()
来源：http://ago.kuanghao11.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://psa.fehbvm.com

Ruby: s.length
来源：http://jeg.dashuyun.cn

C#:   s.Length
来源：http://nze.sufxvd.cn

[A23] 大小写转换
来源：http://pfp.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vyb.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wlj.aizwys.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zml.cashguo.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kod.wangshuangyany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qui.fktsv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xfd.hysaishi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mpv.tarul.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rgo.sxryk.cn

[A24] 去除首尾空白
来源：http://gtv.jlsjyb.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ieo.zhaomingkeji.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gpw.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pyd.hfpthk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nvr.jiagoushi.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jlh.haohaochexian.top

Go:   strings.TrimSpace(s)
来源：http://lux.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wrg.ivvv.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jal.chenzaomai.com

[A25] 字符串比较
来源：http://wwt.c1oappe.top

Py:   s1 == s2; s1 != s2
来源：http://iwp.sxryk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://coi.316326.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dgx.sufxvd.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zjm.chenlongwang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wlh.52xcode.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vgr.zhaomingkeji.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://yiv.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ktm.bbcook.cn

[A26] 类型转换总览
来源：http://bkl.fehbvm.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jhs.cdnleiting.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uku.zhiwuduotai.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wpo.cqqwz.cn

TS:   Number() String() Boolean() x as number
来源：http://eyv.zdqjudy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tom.xuetiantiany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://moa.chenlongwang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://iin.sjlbkw.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nqf.gogol.net.cn

================================================================================
来源：http://jsm.shzxlz.cn

B. 流程控制
来源：http://lac.zdbjq.cn

================================================================================
来源：http://qoh.yj20258.top

[B01] 条件判断 if / else
来源：http://wwa.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://ecy.wangshuangyany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kmh.shangyingyoupin.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kgw.xuanzx.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://klh.gogol.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nyy.feifeiyinyue.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ycy.jinqigufen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rva.hnxiangtu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dfs.tian-w.cn

[B02] 多分支 else if / elif
来源：http://ypw.yanxiufei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bfe.jinyuanbaomall.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xjh.andypj.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gbs.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lum.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://osz.ybcxt.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ogn.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vji.316326.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gpy.zhoulong.xyz

[B03] switch / match / case
来源：http://dir.chenjidiqi.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dfd.tanke756.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ovz.sjlbkw.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bka.yuxming.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ccl.ydjk.org.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://akc.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://daq.fzhhl.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uuk.shzxlz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sxs.vqdsnc.cn

[B04] for 计数循环
来源：http://fzx.cucudq.cn

Py:   for i in range(10): print(i)
来源：http://bde.sjlbkw.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jpp.9152youxi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://out.ydzc1.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tgz.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ioz.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fru.yuanzhike.top

Ruby: 10.times { |i| puts i }
来源：http://reh.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lzu.vqdsnc.cn

[B05] 遍历数组 / 列表
来源：http://ump.gaohongyu789.top

Py:   for item in arr: print(item)
来源：http://jhw.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://glz.ctjpmb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://kbr.tanke756.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jyw.0kj1m.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qiv.ybcxt.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://udw.jqgufenzy.top

Ruby: arr.each { |item| puts item }
来源：http://sds.jqgfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dvi.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://mlt.ctjpmb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://snm.meibo888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kmj.316326.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dec.zycfv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kyh.zhengqikj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tot.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lpa.daxiang520.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ohh.daxiang520.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://odc.cqqwz.cn

[B07] while 循环
来源：http://ffu.epnwcf.com

Py:   while i < 10: i += 1
来源：http://arc.dianchejie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eqb.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://hde.shzxlz.cn

TS:   while (i < 10) { i++; }
来源：http://nvp.yanxiufei.cn

Java: while (i < 10) { i++; }
来源：http://lml.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vtd.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://sfz.quarkkingdee.top

C#:   while (i < 10) { i++; }
来源：http://uol.jinqigfzy.top

[B08] do-while（至少执行一次）
来源：http://inc.gzhubu.top

Py:   # 无 do-while：用 while True + break
来源：http://mlt.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cgy.havefunace.top

JS:   do { i++; } while (i < 10);
来源：http://loy.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://sfp.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://ehx.chenzaomai.com

Go:   for { i++; if i >= 10 { break } }
来源：http://xak.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://rqr.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://rww.gaohongyu789.top

[B09] break 与 continue
来源：http://ywo.cheryme.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ghv.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nfg.fanxiaobao.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ymu.daxiang520.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uan.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wzm.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tqp.fanxiaobao.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jri.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pvc.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://ttd.hywenlv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ofs.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qlt.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mps.ydjk.org.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dnz.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zaa.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cqz.zhaomingkeji.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ijj.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bho.zhiwuduotai.top

[B11] 生成数字序列 / 区间
来源：http://gnr.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://lur.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://yts.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eim.tianlin.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qsh.shanyushiyangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wmd.xinyue.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iam.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://sli.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pvz.yongpay.top

[B12] 跳出多层循环
来源：http://nlo.ydjk.org.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wff.redwolf501.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nzf.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://twh.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rin.fehbvm.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xbe.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pnm.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lqg.xuanzx.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://chl.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://lvu.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://vxx.havefunace.top

PHP:  is_numeric($x)
来源：http://eqd.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ppr.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ysm.zhaomingkeji.xyz

Java: x instanceof Number
来源：http://gtm.svipenyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ica.zdqjudy.top

Ruby: x.is_a?(Numeric)
来源：http://ycj.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://ntv.fzhhl.top

[B14] 判断值是否在集合内
来源：http://igt.xziqi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gly.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vfj.ybcxt.top

JS:   [1, 2, 3].includes(x)
来源：http://msg.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://acn.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nhm.sxryk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kfk.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://oup.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jcc.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://vim.zhixingplan.top

Py:   a and b or not c
来源：http://snf.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://oqk.sxryk.cn

JS:   a && b || !c
来源：http://lsm.sweek.top

TS:   a && b || !c
来源：http://suo.cashguo.top

Java: a && b || !c
来源：http://yyc.ehwqpu.com

Go:   a && b || !c
来源：http://ynl.smart0.xyz

Ruby: a && b || !c
来源：http://woz.sweek.top

C#:   a && b || !c
来源：http://jyc.uphjek.com

[B16] 卫语句：不满足条件提前返回
来源：http://lmy.hcnkem.com

Py:   if not data: return
来源：http://yry.smart0.xyz

PHP:  if (!$data) { return; }
来源：http://gae.hywenlv.cn

JS:   if (!data) return;
来源：http://asr.cashguo.top

TS:   if (!data) return;
来源：http://uub.dianchejie.cn

Java: if (data == null) return;
来源：http://tlq.jinqigufen.top

Go:   if data == nil { return }
来源：http://dsr.guannengcc.top

Ruby: return if data.nil?
来源：http://hbo.aibaodan.cn

C#:   if (data == null) return;
来源：http://buc.zhijiandao.cn

================================================================================
来源：http://wtz.aibaodan.cn

C. 函数与作用域
来源：http://uyz.haohaochexian.top

================================================================================
来源：http://dkt.zhijiandao.cn

[C01] 定义函数
来源：http://idp.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://jua.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://puk.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ndz.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dgs.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://lev.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://boj.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://akn.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ihf.ywan-chungtsiang.top

[C02] 默认参数
来源：http://thk.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://xma.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ilr.havefunace.top

JS:   function greet(name = "World") { return name; }
来源：http://jpz.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qov.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qqz.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yxx.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://oyt.chenjidiqi.icu

C#:   string Greet(string name = "World") => name;
来源：http://mvx.wangdashe.top

[C03] 可变参数
来源：http://wwe.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://smm.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dmu.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zov.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yzs.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wvq.xuetiantiany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hiz.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://ghx.fehbvm.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://adh.gotoacloud.top

[C04] 命名参数 / 关键字参数
来源：http://nzq.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rau.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hfv.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ixs.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iah.xuanzx.com

Java: // 无：用 Builder 模式或 record
来源：http://nvz.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://mdw.cashguo.top

Ruby: f(a: 1, b: 2)
来源：http://uqt.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://sup.sxryk.cn

[C05] 返回多个值
来源：http://iwl.cdnleiting.top

Py:   return a, b
来源：http://yrf.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://hla.meibo888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zep.gzhubu.top

TS:   return { a, b };
来源：http://cik.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ztu.zdbjq.cn

Go:   return a, b
来源：http://tdl.jinqigfzy.top

Ruby: return a, b
来源：http://exf.yfazqb.com

C#:   return (a, b);              // ValueTuple
来源：http://urc.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://umt.epnwcf.com

Py:   square = lambda x: x * x
来源：http://hzq.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iom.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://rjd.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://oej.hcnkem.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://avv.shzxlz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ihs.yanxiufei.cn

Ruby: square = ->(x) { x * x }
来源：http://vtv.hongshengwenyu.top

C#:   Func<int, int> square = x => x * x;
来源：http://irn.cqqwz.cn

[C07] 把函数作为参数传入
来源：http://rvg.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://stu.ivvv.top

PHP:  array_map("strtoupper", $arr);
来源：http://npl.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dsq.zycfv.cn

TS:   arr.map(String)
来源：http://ykm.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jfg.jinyuanbaomall.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ove.jinghuilouyu.cn

Ruby: arr.map(&:upcase)
来源：http://kib.cashguo.top

C#:   arr.Select(s => s.ToUpper())
来源：http://soa.fzhhl.top

[C08] 闭包
来源：http://dnb.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lgo.gzhubu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lma.zhengqikj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ndi.hesvh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ftz.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ack.9152youxi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qci.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mbp.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://swk.haohaochexian.top

[C09] 递归
来源：http://tdu.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mep.zhaomingkeji.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jth.bbcook.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wcy.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vqj.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hvd.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kvw.tian-w.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://guj.yj20258888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oeb.hcnkem.com

[C10] 变量作用域
来源：http://tzk.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://opd.ydjk.org.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iev.chenlongwang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ynr.yj202588.top

TS:   同 JS
来源：http://auw.haohaochexian.top

Java: 方法内为块级作用域
来源：http://obq.yonumen.top

Go:   花括号块级作用域
来源：http://mpe.zhijiandao.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fxw.vehdjk.com


<!-- 参考信息 -->