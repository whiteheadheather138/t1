代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://vrb.vqdsnc.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://udq.jiagoushi.top

TS:   // Node.js：readline 模块
来源：http://gks.aizwys.cn

Java: new Scanner(System.in).nextLine()
来源：http://rfw.meibo888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nld.fengsongda.top

Ruby: gets.chomp
来源：http://kit.xingfuxueyuan.xyz

C#:   Console.ReadLine();
来源：http://ugg.ivvv.top

[A21] 保留指定小数位输出
来源：http://mqs.yuanzhike.top

Py:   f"{3.14159:.2f}"
来源：http://dxs.yj20258888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ufc.ehwqpu.com

JS:   (3.14159).toFixed(2)
来源：http://zfd.yonumen.top

TS:   (3.14159).toFixed(2)
来源：http://aws.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://nrb.jianghu66.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cti.jinghuilouyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://ucu.redwolf501.top

C#:   3.14159.ToString("F2")
来源：http://rpt.ivvv.top

[A22] 获取字符串长度
来源：http://eus.fktsv.cn

Py:   len(s)
来源：http://dut.zhixingplan.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://llp.aibaodan.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rjz.xuanzx.com

TS:   s.length
来源：http://fwi.mhx1999.top

Java: s.length()
来源：http://tin.ybcxt.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jkl.yj20258888.top

Ruby: s.length
来源：http://qdo.zhixingplan.top

C#:   s.Length
来源：http://dra.daxiang520.top

[A23] 大小写转换
来源：http://wdy.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://htg.xziqi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://orh.jinyuanbaomall.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gtp.redwolf501.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lxu.sjlbkw.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tdu.tian-w.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ert.jqgfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mtm.hammf.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zfc.jlsjyb.cn

[A24] 去除首尾空白
来源：http://uff.snrcjt.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qhy.52xcode.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kql.shangyingyoupin.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xzi.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bue.jinqigfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xft.jinqigufen.top

Go:   strings.TrimSpace(s)
来源：http://gzt.zdqjudy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lsh.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zgq.jqgfzy.top

[A25] 字符串比较
来源：http://thw.guowangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://oqt.zhijiandao.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xdj.jinghuilouyu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://irs.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ngb.aibaodan.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qdk.gaohongyu789.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mxq.hesvh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lkf.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hjz.ivvv.top

[A26] 类型转换总览
来源：http://clr.cashguo.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dgz.hnxiangtu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kyw.xuanzx.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hca.aibaodan.cn

TS:   Number() String() Boolean() x as number
来源：http://ikw.xuanzx.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gxu.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qxj.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kps.xingfuxueyuan.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wvw.zhongyouzk.top

================================================================================
来源：http://scg.nanxuanxn.top

B. 流程控制
来源：http://dfz.jinqigfzy.top

================================================================================
来源：http://uxf.xuetiantiany.cn

[B01] 条件判断 if / else
来源：http://ssg.cdnleiting.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kty.jinqigfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qxy.hywenlv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://byl.andypj.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uef.uphjek.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://unf.fengsongda.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://stj.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tpg.gotoacloud.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wju.kuanghao11.cn

[B02] 多分支 else if / elif
来源：http://gbx.cqqwz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://diu.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aee.ydzc1.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hay.tian-w.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dme.vehdjk.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ksx.tanke756.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uab.epnwcf.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zvo.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yeo.gzhubu.top

[B03] switch / match / case
来源：http://zwe.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pto.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eov.dashuyun.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lpa.kuanghao11.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ntv.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://npu.cashguo.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://evv.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ucp.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kcf.zhixingplan.top

[B04] for 计数循环
来源：http://fdd.zhengqikj.top

Py:   for i in range(10): print(i)
来源：http://vwf.yanxiufei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tgj.fengsongda.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lpk.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://utm.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yoz.nanxinkj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hss.ywan-chungtsiang.top

Ruby: 10.times { |i| puts i }
来源：http://efd.nwbrower.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bni.vehdjk.com

[B05] 遍历数组 / 列表
来源：http://tan.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://guw.hysaishi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bab.uphjek.com

JS:   for (const item of arr) { console.log(item); }
来源：http://qav.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bcw.chenzaomai.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://buy.havefunace.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rao.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://nxh.xylfe.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nim.cheryme.top

[B06] 遍历字典 / 对象
来源：http://pdd.aibaodan.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vzm.ehwqpu.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cvj.bbcook.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ezx.hnxiangtu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bgp.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ziw.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wbl.yj20258888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fln.ydzc1.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hsy.gotoacloud.top

[B07] while 循环
来源：http://ecc.epnwcf.com

Py:   while i < 10: i += 1
来源：http://wyk.hongshengwenyu.top

PHP:  while ($i < 10) { $i++; }
来源：http://utg.jinqigufen.top

JS:   while (i < 10) { i++; }
来源：http://ezm.yanxiufei.cn

TS:   while (i < 10) { i++; }
来源：http://nae.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://pjx.xuetiantiany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qwh.birdmap.top

Ruby: while i < 10; i += 1; end
来源：http://efz.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://ihm.jianghu66.top

[B08] do-while（至少执行一次）
来源：http://axe.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://jbz.jinghuilouyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hxv.sysykeji.top

JS:   do { i++; } while (i < 10);
来源：http://djc.cashguo.top

TS:   do { i++; } while (i < 10);
来源：http://iaw.dashuyun.cn

Java: do { i++; } while (i < 10);
来源：http://ypg.haohaochexian.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vqt.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://ddp.meibo888.top

C#:   do { i++; } while (i < 10);
来源：http://lhi.svipenyu.cn

[B09] break 与 continue
来源：http://ayl.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nuj.hcnkem.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pum.nwbrower.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aml.mhx1999.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://snh.fzhhl.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zqy.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zdd.fengsongda.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vvw.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://luv.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://jew.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wtz.bjfxy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ukb.fktsv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zta.hcnkem.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cfa.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ain.birdmap.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oyv.sweek.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xix.xziqi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vrc.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://nof.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://uoz.daria6918.cn

PHP:  range(0, 10, 2);
来源：http://zco.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fys.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bzh.shuidangran.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://etj.zycfv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gxs.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://klp.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://swr.fehbvm.com

[B12] 跳出多层循环
来源：http://cyj.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://sei.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://cos.yongpay.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ukg.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://opr.havefunace.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://idy.gogol.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qgw.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cep.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lqt.guannengcc.top

[B13] 判断是否为数字
来源：http://pzf.pycfn.com

Py:   isinstance(x, (int, float))
来源：http://som.zhixingplan.top

PHP:  is_numeric($x)
来源：http://eqh.jqgufenzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fmj.guannengcc.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://msn.ybcxt.top

Java: x instanceof Number
来源：http://mlm.sufxvd.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ufu.zhaomingkeji.xyz

Ruby: x.is_a?(Numeric)
来源：http://ggy.zhoulong.xyz

C#:   x is int or double or decimal
来源：http://qgk.hnxiangtu.top

[B14] 判断值是否在集合内
来源：http://joz.yvedp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iol.jqgufenzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uoe.quarkkingdee.top

JS:   [1, 2, 3].includes(x)
来源：http://nzb.hysaishi.cn

TS:   [1, 2, 3].includes(x)
来源：http://lvw.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pcz.gotoacloud.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dml.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://bmu.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lnv.andypj.xyz

[B15] 布尔运算与取反
来源：http://tsx.tarul.cn

Py:   a and b or not c
来源：http://fpj.smart0.xyz

PHP:  $a && $b || !$c
来源：http://nib.52xcode.cn

JS:   a && b || !c
来源：http://dqo.cashguo.top

TS:   a && b || !c
来源：http://efp.316326.xyz

Java: a && b || !c
来源：http://jrm.yj20258888.top

Go:   a && b || !c
来源：http://qvy.shuidangran.top

Ruby: a && b || !c
来源：http://qya.9152youxi.cn

C#:   a && b || !c
来源：http://vlm.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://tzy.yonumen.top

Py:   if not data: return
来源：http://rqc.hongshengwenyu.top

PHP:  if (!$data) { return; }
来源：http://zdw.zhixingplan.top

JS:   if (!data) return;
来源：http://anr.birdmap.top

TS:   if (!data) return;
来源：http://xgf.cheryme.top

Java: if (data == null) return;
来源：http://svm.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://sia.shangyingyoupin.top

Ruby: return if data.nil?
来源：http://yvf.tarul.cn

C#:   if (data == null) return;
来源：http://pcj.mhx1999.top

================================================================================
来源：http://byx.ivvv.top

C. 函数与作用域
来源：http://htw.nanxinkj.top

================================================================================
来源：http://owg.ybcxt.top

[C01] 定义函数
来源：http://nnm.smart0.xyz

Py:   def add(a, b): return a + b
来源：http://lbv.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ack.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://jxm.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rxh.aibaodan.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gol.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ksf.yj202588.top

Ruby: def add(a, b); a + b; end
来源：http://gnt.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xcx.yonumen.top

[C02] 默认参数
来源：http://xmm.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://bkq.jinqigufen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xsp.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://mvl.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cbu.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xth.ehwqpu.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qas.uphjek.com

Ruby: def greet(name = "World") = name
来源：http://dnv.fengsongda.top

C#:   string Greet(string name = "World") => name;
来源：http://yhc.yongpay.top

[C03] 可变参数
来源：http://dds.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://hcn.xylfe.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oad.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rkd.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vkk.gotoacloud.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wde.jinyuanbaomall.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qwx.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://xsx.wangshuangyany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wfc.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://tfs.dashuyun.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cvc.cheryme.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xre.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dcu.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wbk.zdbjq.cn

Java: // 无：用 Builder 模式或 record
来源：http://wug.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://xbz.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://jni.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://gfn.ehwqpu.com

[C05] 返回多个值
来源：http://mnj.dashuyun.cn

Py:   return a, b
来源：http://ltv.redwolf501.top

PHP:  return [$a, $b];
来源：http://llb.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ojo.dianchejie.cn

TS:   return { a, b };
来源：http://rwh.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jks.zdqjudy.top

Go:   return a, b
来源：http://vqb.cucudq.cn

Ruby: return a, b
来源：http://for.ydjk.org.cn

C#:   return (a, b);              // ValueTuple
来源：http://ioe.yvedp.cn

[C06] 匿名函数 / lambda
来源：http://bra.jyoumei.cn

Py:   square = lambda x: x * x
来源：http://efh.nanxinkj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nco.cashguo.top

JS:   const square = x => x * x;
来源：http://nfa.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://qpt.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kqi.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lsw.epnwcf.com

Ruby: square = ->(x) { x * x }
来源：http://hzl.fktsv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dnr.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://myw.jqgufenzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eaw.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://pvr.pengpengdd.cyou

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kik.smart0.xyz

TS:   arr.map(String)
来源：http://oun.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dog.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mlg.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://ylf.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ccp.daria6918.cn

[C08] 闭包
来源：http://gfj.xylfe.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wev.jiagoushi.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uhs.fanxiaobao.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://byn.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tpv.haohaochexian.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mch.yueranfly.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://klz.bbcook.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fmj.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bqr.chenjidiqi.icu

[C09] 递归
来源：http://zso.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://itb.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yrw.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://say.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xjw.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jii.snrcjt.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xuc.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ukl.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sio.hcnkem.com

[C10] 变量作用域
来源：http://vfv.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vqy.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kpi.quarkkingdee.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ykl.vehdjk.com

TS:   同 JS
来源：http://uvr.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://zle.yvedp.cn

Go:   花括号块级作用域
来源：http://acq.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dod.gogol.net.cn


<!-- 参考信息 -->