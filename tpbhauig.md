代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://nwz.shanyushiyangtech.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://knq.sweek.top

TS:   // Node.js：readline 模块
来源：http://rti.zhixingplan.top

Java: new Scanner(System.in).nextLine()
来源：http://rop.pycfn.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ckk.bbcook.cn

Ruby: gets.chomp
来源：http://ajv.zdqjudy.top

C#:   Console.ReadLine();
来源：http://esr.wangshuangyany.cn

[A21] 保留指定小数位输出
来源：http://ysv.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://tyk.fzhhl.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gbj.jyoumei.cn

JS:   (3.14159).toFixed(2)
来源：http://hgn.aizwys.cn

TS:   (3.14159).toFixed(2)
来源：http://fmv.daxiang520.top

Java: String.format("%.2f", 3.14159)
来源：http://eyc.fanxiaobao.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hwt.hywenlv.cn

Ruby: format("%.2f", 3.14159)
来源：http://lqe.yvedp.cn

C#:   3.14159.ToString("F2")
来源：http://nkn.xziqi.cn

[A22] 获取字符串长度
来源：http://irm.kuanghao11.cn

Py:   len(s)
来源：http://hvj.jqgfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dde.tanke756.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cpk.aizwys.cn

TS:   s.length
来源：http://wmd.jinghuilouyu.cn

Java: s.length()
来源：http://eve.shzxlz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jvm.bjfxy.top

Ruby: s.length
来源：http://ncy.zhongyouzk.top

C#:   s.Length
来源：http://bpz.tianlin.xyz

[A23] 大小写转换
来源：http://vcq.cdnleiting.top

Py:   s.upper(); s.lower(); s.title()
来源：http://sxp.pengpengdd.cyou

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wpr.hywenlv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wox.shangyingyoupin.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zrv.jinghuilouyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lvv.zdbjq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qie.iojbl.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ctc.hfpthk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zth.tanke756.top

[A24] 去除首尾空白
来源：http://hnn.nwbrower.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nec.shangyingyoupin.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ggg.yongpay.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sts.sweek.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yrb.jianghu66.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rij.hysaishi.cn

Go:   strings.TrimSpace(s)
来源：http://hdd.jinghuilouyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://usx.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cxt.nanxinkj.top

[A25] 字符串比较
来源：http://smk.zhijiandao.cn

Py:   s1 == s2; s1 != s2
来源：http://qzh.xingfuxueyuan.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ldx.cucudq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vwk.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vzf.fehbvm.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ufy.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dap.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://zfs.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aml.xylfe.cn

[A26] 类型转换总览
来源：http://tzx.zhixingplan.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://crg.shzxlz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mwe.yanxiufei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nng.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://odp.jiagoushi.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hoj.zdqjudy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://amk.gaohongyu789.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://har.feifeiyinyue.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tvw.jlsjyb.cn

================================================================================
来源：http://hah.yuxming.cn

B. 流程控制
来源：http://uqj.hammf.cn

================================================================================
来源：http://qwq.xuetiantiany.cn

[B01] 条件判断 if / else
来源：http://smh.shanyushiyangtech.top

Py:   result = "正" if x > 0 else "非正"
来源：http://lbp.zhaomingkeji.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iaf.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bzx.smart0.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ltc.xziqi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qwl.cqqwz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ien.nanxuanxn.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yxh.yj20258.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dpr.jinqigfzy.top

[B02] 多分支 else if / elif
来源：http://zjq.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vaq.yangfankeji.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://elv.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cbd.mhx1999.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wcz.xuanzx.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ecr.tanke756.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ulq.andypj.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cog.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ocf.jinqigfzy.top

[B03] switch / match / case
来源：http://zuy.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rtj.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nat.tianlin.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gbg.vehdjk.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qzd.gogol.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xkg.yangfankeji.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ygd.tian-w.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ekh.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lxw.andypj.xyz

[B04] for 计数循环
来源：http://mzn.yonumen.top

Py:   for i in range(10): print(i)
来源：http://cfb.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hbb.yongpay.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jlz.bjfxy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pyc.yueranfly.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wba.yj202588.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xta.haohaochexian.top

Ruby: 10.times { |i| puts i }
来源：http://qzi.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ads.sxryk.cn

[B05] 遍历数组 / 列表
来源：http://xmj.xylfe.cn

Py:   for item in arr: print(item)
来源：http://dan.dianchejie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eaa.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yec.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://kkg.vqdsnc.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fby.pycfn.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pul.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://msu.hfpthk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bix.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://thp.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lxs.xuanzx.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vnu.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kbe.vqdsnc.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dpc.shzxlz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://efu.aibaodan.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zib.jinyuanbaomall.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nxo.uphjek.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xlt.nanxuanxn.top

[B07] while 循环
来源：http://fqg.tarul.cn

Py:   while i < 10: i += 1
来源：http://juh.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lxt.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://ugh.chenjidiqi.icu

TS:   while (i < 10) { i++; }
来源：http://fsl.jyoumei.cn

Java: while (i < 10) { i++; }
来源：http://qvs.sxryk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jpv.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://wkz.xuetiantiany.cn

C#:   while (i < 10) { i++; }
来源：http://sjt.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://vje.ydjk.org.cn

Py:   # 无 do-while：用 while True + break
来源：http://lry.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://ppc.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://sui.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://vjx.zhiwuduotai.top

Java: do { i++; } while (i < 10);
来源：http://bmm.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qzf.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://hld.feifeiyinyue.top

C#:   do { i++; } while (i < 10);
来源：http://htq.bbcook.cn

[B09] break 与 continue
来源：http://dwe.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hgp.hywenlv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mkk.zdqjudy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://adc.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hnc.316326.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wtm.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bmk.fzhhl.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oxi.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wau.cqqwz.cn

[B10] 遍历同时拿索引
来源：http://vvq.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jwn.shanyushiyangtech.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nuf.redwolf501.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hfw.gaohongyu789.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rcz.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cmn.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qcq.jinqigufen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rqn.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://orf.fktsv.cn

[B11] 生成数字序列 / 区间
来源：http://lqs.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://pme.dashuyun.cn

PHP:  range(0, 10, 2);
来源：http://ezw.zhijiandao.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://msm.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qls.fanxiaobao.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mjk.yj20258888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zql.jyoumei.cn

Ruby: (0...10).step(2).to_a
来源：http://woj.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://emt.uphjek.com

[B12] 跳出多层循环
来源：http://sjc.uphjek.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://job.nwbrower.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jfp.gaohongyu789.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ozf.yonumen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cdi.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oxe.jqgfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dva.zdbjq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yfo.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zma.redwolf501.top

[B13] 判断是否为数字
来源：http://hsf.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://rch.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://ujo.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://acv.c1oappe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pgw.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://kti.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bty.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://izf.9152youxi.cn

C#:   x is int or double or decimal
来源：http://xnq.ydzc1.top

[B14] 判断值是否在集合内
来源：http://mve.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://asi.gotoacloud.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mmq.zhiwuduotai.top

JS:   [1, 2, 3].includes(x)
来源：http://cpn.ivvv.top

TS:   [1, 2, 3].includes(x)
来源：http://ppj.wangshuangyany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bnw.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://smf.dianchejie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mnd.fzhhl.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ugk.dashuyun.cn

[B15] 布尔运算与取反
来源：http://tui.jyoumei.cn

Py:   a and b or not c
来源：http://lvv.gotoacloud.top

PHP:  $a && $b || !$c
来源：http://smt.sjlbkw.cn

JS:   a && b || !c
来源：http://ype.yj20258888.top

TS:   a && b || !c
来源：http://nua.yangfankeji.com

Java: a && b || !c
来源：http://bzh.xylfe.cn

Go:   a && b || !c
来源：http://hvd.zhijiandao.cn

Ruby: a && b || !c
来源：http://tlu.xuetiantiany.cn

C#:   a && b || !c
来源：http://fos.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wyd.dashuyun.cn

Py:   if not data: return
来源：http://fil.iojbl.cn

PHP:  if (!$data) { return; }
来源：http://oun.nwbrower.top

JS:   if (!data) return;
来源：http://hpm.chenzaomai.com

TS:   if (!data) return;
来源：http://wog.zycfv.cn

Java: if (data == null) return;
来源：http://rjg.yangfankeji.com

Go:   if data == nil { return }
来源：http://goi.ivvv.top

Ruby: return if data.nil?
来源：http://qnl.tian-w.cn

C#:   if (data == null) return;
来源：http://udo.cdnleiting.top

================================================================================
来源：http://iyy.hongshengwenyu.top

C. 函数与作用域
来源：http://wnm.jianghu66.top

================================================================================
来源：http://kfr.fzhhl.top

[C01] 定义函数
来源：http://qni.gotoacloud.top

Py:   def add(a, b): return a + b
来源：http://hza.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aci.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://agp.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lzf.zhongyouzk.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wkh.svipenyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yyb.hongshengwenyu.top

Ruby: def add(a, b); a + b; end
来源：http://zhs.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mot.sweek.top

[C02] 默认参数
来源：http://anx.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://riq.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://rnq.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://mdb.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://miu.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://clb.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kjj.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://tbx.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://ndz.havefunace.top

[C03] 可变参数
来源：http://hvh.chenjidiqi.icu

Py:   def total(*args): return sum(args)
来源：http://dvv.guannengcc.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://epy.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ois.hcnkem.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nwe.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mjd.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://itt.xziqi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yhn.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://npr.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://mbo.cdnleiting.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xfa.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vgv.bjfxy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xsb.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jsb.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://wlb.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://rku.ehwqpu.com

Ruby: f(a: 1, b: 2)
来源：http://ynv.tianlin.xyz

C#:   f(a: 1, b: 2)
来源：http://daf.yvedp.cn

[C05] 返回多个值
来源：http://wpj.gogol.net.cn

Py:   return a, b
来源：http://wfs.haohaochexian.top

PHP:  return [$a, $b];
来源：http://uad.nanxuanxn.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kgg.yvedp.cn

TS:   return { a, b };
来源：http://uzw.vehdjk.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wsm.chenzaomai.com

Go:   return a, b
来源：http://hfg.fanxiaobao.xyz

Ruby: return a, b
来源：http://mzw.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://zhz.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://geb.tian-w.cn

Py:   square = lambda x: x * x
来源：http://pgh.xziqi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hbx.ehwqpu.com

JS:   const square = x => x * x;
来源：http://gos.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://paz.wangdashe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://otn.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lro.gzhubu.top

Ruby: square = ->(x) { x * x }
来源：http://qps.nanxuanxn.top

C#:   Func<int, int> square = x => x * x;
来源：http://fcj.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://iqf.jqgufenzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nmm.redwolf501.top

PHP:  array_map("strtoupper", $arr);
来源：http://xzq.xylfe.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cvf.zhiwuduotai.top

TS:   arr.map(String)
来源：http://sca.zdbjq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wnn.sjlbkw.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wxy.0kj1m.cn

Ruby: arr.map(&:upcase)
来源：http://odx.dashuyun.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nri.nwbrower.top

[C08] 闭包
来源：http://apw.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mfx.yueranfly.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zib.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dew.vehdjk.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://djv.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mzg.jyoumei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://skq.xingfuxueyuan.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blr.52xcode.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://elb.cqqwz.cn

[C09] 递归
来源：http://xpu.ywan-chungtsiang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dkv.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mwm.chenzaomai.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wyi.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ssf.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aig.jinqigufen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://njh.cdnleiting.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wmi.hesvh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jnu.sufxvd.cn

[C10] 变量作用域
来源：http://qbx.birdmap.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wce.zhongyouzk.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kyq.shzxlz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://euk.yuxming.cn

TS:   同 JS
来源：http://rxi.chenlongwang.top

Java: 方法内为块级作用域
来源：http://rwo.chenzaomai.com

Go:   花括号块级作用域
来源：http://lcv.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wxt.snrcjt.cn


<!-- 参考信息 -->