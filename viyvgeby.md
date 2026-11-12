代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://tmc.xuanzx.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://arv.pengpengdd.cyou

TS:   // Node.js：readline 模块
来源：http://eij.gaohongyu789.top

Java: new Scanner(System.in).nextLine()
来源：http://ayn.tanke756.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://huk.9152youxi.cn

Ruby: gets.chomp
来源：http://ora.andypj.xyz

C#:   Console.ReadLine();
来源：http://xpl.cdnleiting.top

[A21] 保留指定小数位输出
来源：http://fss.gzhubu.top

Py:   f"{3.14159:.2f}"
来源：http://lwz.shangyingyoupin.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zaa.ybcxt.top

JS:   (3.14159).toFixed(2)
来源：http://cuy.zycfv.cn

TS:   (3.14159).toFixed(2)
来源：http://hlv.jqgufenzy.top

Java: String.format("%.2f", 3.14159)
来源：http://aiq.hysaishi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://enw.gogol.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://ong.redwolf501.top

C#:   3.14159.ToString("F2")
来源：http://iyt.jyoumei.cn

[A22] 获取字符串长度
来源：http://lsg.vehdjk.com

Py:   len(s)
来源：http://dmu.havefunace.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ynn.jinqigufen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kun.mhx1999.top

TS:   s.length
来源：http://hfd.hesvh.cn

Java: s.length()
来源：http://nhz.xuetiantiany.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cuh.pycfn.com

Ruby: s.length
来源：http://zic.havefunace.top

C#:   s.Length
来源：http://vce.nwbrower.top

[A23] 大小写转换
来源：http://ekb.smart0.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://rwg.shuidangran.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zmh.vehdjk.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gme.mhx1999.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ofs.ydjk.org.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ovx.zycfv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ncr.tanke756.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://voj.c1oappe.top

C#:   s.ToUpper(); s.ToLower()
来源：http://otb.hammf.cn

[A24] 去除首尾空白
来源：http://flc.cdnleiting.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bfd.sweek.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yio.svipenyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xka.havefunace.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ndk.xuanzx.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rvn.zhiwuduotai.top

Go:   strings.TrimSpace(s)
来源：http://acf.chenjidiqi.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aae.quarkkingdee.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mxq.hcnkem.com

[A25] 字符串比较
来源：http://jyq.nanxuanxn.top

Py:   s1 == s2; s1 != s2
来源：http://etm.dashuyun.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iet.dashuyun.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ftp.sysykeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pnr.yueranfly.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rnv.yvedp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yxy.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://leb.zhijiandao.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aec.fehbvm.com

[A26] 类型转换总览
来源：http://dps.birdmap.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kxy.smart0.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kvv.jqgfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qtt.hnqzz.top

TS:   Number() String() Boolean() x as number
来源：http://ghc.ydzc1.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hex.mhx1999.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ehk.jqgfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jwu.hywenlv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qnl.tian-w.cn

================================================================================
来源：http://szg.zdbjq.cn

B. 流程控制
来源：http://ose.cucudq.cn

================================================================================
来源：http://dds.cqqwz.cn

[B01] 条件判断 if / else
来源：http://qfa.dianchejie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bel.hysaishi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jfq.havefunace.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://udu.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ajj.shuidangran.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://kul.iojbl.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://weu.cucudq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wwt.ehwqpu.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bvb.zhixingplan.top

[B02] 多分支 else if / elif
来源：http://zcm.iojbl.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vbd.bjfxy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yrj.ydjk.org.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cgu.snrcjt.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ckg.yj202588.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zdd.tarul.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zlr.ybcxt.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hvl.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oto.xuanzx.com

[B03] switch / match / case
来源：http://lmg.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nwp.shzxlz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mwm.ppjwa.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://exm.52xcode.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qml.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kfu.wangdashe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://aah.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yjw.cashguo.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uoe.xinyue.icu

[B04] for 计数循环
来源：http://wsr.yangfankeji.com

Py:   for i in range(10): print(i)
来源：http://cxz.ydzc1.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gzy.kuanghao11.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fhx.jianghu66.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oho.quarkkingdee.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fii.tarul.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fon.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://grv.chenzaomai.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ffu.jianghu66.top

[B05] 遍历数组 / 列表
来源：http://ggp.fengsongda.top

Py:   for item in arr: print(item)
来源：http://pyo.zhijiandao.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pba.ybcxt.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ebl.vehdjk.com

TS:   for (const item of arr) { console.log(item); }
来源：http://rru.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zoh.yj20258888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zjv.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://mlu.wangshuangyany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hzv.jyoumei.cn

[B06] 遍历字典 / 对象
来源：http://nxq.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ozg.sweek.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rkl.yuanzhike.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ymk.nanxinkj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ogb.gzhubu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tia.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gcr.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://een.jqgufenzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mmu.hammf.cn

[B07] while 循环
来源：http://ixo.gogol.net.cn

Py:   while i < 10: i += 1
来源：http://spp.havefunace.top

PHP:  while ($i < 10) { $i++; }
来源：http://mcc.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://qjo.xziqi.cn

TS:   while (i < 10) { i++; }
来源：http://uvm.zhijiandao.cn

Java: while (i < 10) { i++; }
来源：http://frk.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://knx.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://lbh.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://qre.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://cly.shanyushiyangtech.top

Py:   # 无 do-while：用 while True + break
来源：http://scf.hesvh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ine.jinyuanbaomall.cn

JS:   do { i++; } while (i < 10);
来源：http://tee.hesvh.cn

TS:   do { i++; } while (i < 10);
来源：http://fyx.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://avk.fktsv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://liz.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://xfu.pycfn.com

C#:   do { i++; } while (i < 10);
来源：http://lcx.guowangkeji.top

[B09] break 与 continue
来源：http://txy.cashguo.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zra.gzhubu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mij.aibaodan.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nrk.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pmh.yonumen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bgl.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yna.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dvn.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sdy.shanyushiyangkeji.top

[B10] 遍历同时拿索引
来源：http://cod.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yrq.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gjj.yongpay.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zfe.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rjd.zdbjq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yvh.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xgf.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eqg.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dof.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://uwt.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://syj.hnqzz.top

PHP:  range(0, 10, 2);
来源：http://brc.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cxv.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ksf.birdmap.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uve.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rxu.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://mtx.feifeiyinyue.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fmb.yongpay.top

[B12] 跳出多层循环
来源：http://xno.dianchejie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mnw.ybcxt.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://aji.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wky.dashuyun.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ioe.jlsjyb.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://izk.xziqi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qrl.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bmc.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hxu.yuanzhike.top

[B13] 判断是否为数字
来源：http://rem.sweek.top

Py:   isinstance(x, (int, float))
来源：http://zpo.cucudq.cn

PHP:  is_numeric($x)
来源：http://anv.xinyue.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rqy.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ffx.zdbjq.cn

Java: x instanceof Number
来源：http://xpy.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xql.yongpay.top

Ruby: x.is_a?(Numeric)
来源：http://ply.dashuyun.cn

C#:   x is int or double or decimal
来源：http://vcn.hnqzz.top

[B14] 判断值是否在集合内
来源：http://omr.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vjj.cdnleiting.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://atz.feifeiyinyue.top

JS:   [1, 2, 3].includes(x)
来源：http://byj.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://xhc.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zzt.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://csr.wangshuangyany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mqn.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://and.zhixingplan.top

[B15] 布尔运算与取反
来源：http://mwb.daria6918.cn

Py:   a and b or not c
来源：http://voe.zdqjudy.top

PHP:  $a && $b || !$c
来源：http://vhr.xziqi.cn

JS:   a && b || !c
来源：http://hpl.yvedp.cn

TS:   a && b || !c
来源：http://jxg.ppjwa.cn

Java: a && b || !c
来源：http://jyn.dashuyun.cn

Go:   a && b || !c
来源：http://atq.chenzaomai.com

Ruby: a && b || !c
来源：http://omu.cashguo.top

C#:   a && b || !c
来源：http://snr.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://rdw.xinyue.icu

Py:   if not data: return
来源：http://fej.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://err.ctjpmb.com

JS:   if (!data) return;
来源：http://opg.chenlongwang.top

TS:   if (!data) return;
来源：http://yjy.sufxvd.cn

Java: if (data == null) return;
来源：http://gpv.shangyingyoupin.top

Go:   if data == nil { return }
来源：http://eyo.yongpay.top

Ruby: return if data.nil?
来源：http://gvi.iojbl.cn

C#:   if (data == null) return;
来源：http://odo.ppjwa.cn

================================================================================
来源：http://uuj.bbcook.cn

C. 函数与作用域
来源：http://sbi.hammf.cn

================================================================================
来源：http://gzt.vqdsnc.cn

[C01] 定义函数
来源：http://rtt.yj20258.top

Py:   def add(a, b): return a + b
来源：http://fcn.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pgr.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://osg.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eem.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kli.jlsjyb.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ron.yueranfly.top

Ruby: def add(a, b); a + b; end
来源：http://qkt.mhx1999.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xap.xuetiantiany.cn

[C02] 默认参数
来源：http://qey.xingfuxueyuan.xyz

Py:   def greet(name="World"): return name
来源：http://tvq.gotoacloud.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pmd.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://zrc.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xwf.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jgo.fzhhl.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jyr.jinyuanbaomall.cn

Ruby: def greet(name = "World") = name
来源：http://irm.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://duh.kuanghao11.cn

[C03] 可变参数
来源：http://sru.52xcode.cn

Py:   def total(*args): return sum(args)
来源：http://eju.iojbl.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ksq.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://shv.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vmb.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vyp.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vqp.ybcxt.top

Ruby: def total(*nums); nums.sum; end
来源：http://xpg.feifeiyinyue.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://szw.wangshuangyany.cn

[C04] 命名参数 / 关键字参数
来源：http://bjw.fengsongda.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xkd.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jgh.jqgufenzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wis.cheryme.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ijq.tian-w.cn

Java: // 无：用 Builder 模式或 record
来源：http://wqs.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://rsk.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://zaa.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://cgz.redwolf501.top

[C05] 返回多个值
来源：http://bnt.jinyuanbaomall.cn

Py:   return a, b
来源：http://lgh.epnwcf.com

PHP:  return [$a, $b];
来源：http://lmj.xylfe.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://duk.zdqjudy.top

TS:   return { a, b };
来源：http://xkl.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vvk.shuidangran.top

Go:   return a, b
来源：http://kmo.cqqwz.cn

Ruby: return a, b
来源：http://iwt.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://wqh.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://dcv.yuxming.cn

Py:   square = lambda x: x * x
来源：http://xdt.chenjidiqi.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://yik.jinyuanbaomall.cn

JS:   const square = x => x * x;
来源：http://yla.zhijiandao.cn

TS:   const square = (x: number): number => x * x;
来源：http://dks.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pgq.iojbl.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rui.bjfxy.top

Ruby: square = ->(x) { x * x }
来源：http://aqy.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://toz.snrcjt.cn

[C07] 把函数作为参数传入
来源：http://dhy.shanyushiyangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wip.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://nxc.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mij.jqgfzy.top

TS:   arr.map(String)
来源：http://awu.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://azl.fktsv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xfo.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://qfn.jinghuilouyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yyi.zhengqikj.top

[C08] 闭包
来源：http://wlt.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jsd.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uag.smart0.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://inj.smart0.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://afc.fanxiaobao.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bzm.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bcx.zhongyouzk.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jzt.xylfe.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pbt.yuanzhike.top

[C09] 递归
来源：http://fjk.fengsongda.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rii.jqgufenzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fqb.shangyingyoupin.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jho.yj20258.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://spd.shangyingyoupin.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jjy.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://krj.nanxinkj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://edf.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pkc.birdmap.top

[C10] 变量作用域
来源：http://qra.zycfv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blr.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xkk.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jwv.nanxinkj.top

TS:   同 JS
来源：http://uzt.hesvh.cn

Java: 方法内为块级作用域
来源：http://eii.hcnkem.com

Go:   花括号块级作用域
来源：http://tra.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hvt.cheryme.top


<!-- 参考信息 -->