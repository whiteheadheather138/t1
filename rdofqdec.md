代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://uto.sjlbkw.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zfd.xuetiantiany.cn

TS:   // Node.js：readline 模块
来源：http://wym.gotoacloud.top

Java: new Scanner(System.in).nextLine()
来源：http://cux.feifeiyinyue.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tnx.dianchejie.cn

Ruby: gets.chomp
来源：http://xpt.kuanghao11.cn

C#:   Console.ReadLine();
来源：http://agi.jinqigufen.top

[A21] 保留指定小数位输出
来源：http://jny.0kj1m.cn

Py:   f"{3.14159:.2f}"
来源：http://mnz.cucudq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eql.hysaishi.cn

JS:   (3.14159).toFixed(2)
来源：http://qsk.fengsongda.top

TS:   (3.14159).toFixed(2)
来源：http://jhq.zhijiandao.cn

Java: String.format("%.2f", 3.14159)
来源：http://djg.sxryk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://grr.vqdsnc.cn

Ruby: format("%.2f", 3.14159)
来源：http://wyj.zhengqikj.top

C#:   3.14159.ToString("F2")
来源：http://lng.ydzc1.top

[A22] 获取字符串长度
来源：http://cfs.shuidangran.top

Py:   len(s)
来源：http://orn.ppjwa.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xem.tanke756.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zzg.sweek.top

TS:   s.length
来源：http://tdc.jinqigfzy.top

Java: s.length()
来源：http://nli.jinyuanbaomall.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rpp.xuetiantiany.cn

Ruby: s.length
来源：http://xnz.redwolf501.top

C#:   s.Length
来源：http://xgg.ehwqpu.com

[A23] 大小写转换
来源：http://eur.sysykeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gqf.quarkkingdee.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://khw.jinyuanbaomall.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aej.andypj.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://joc.sjlbkw.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jfd.pengpengdd.cyou

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oqx.chenzaomai.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://whl.aizwys.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cpm.dianchejie.cn

[A24] 去除首尾空白
来源：http://wxt.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rnb.jyoumei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kbp.nanxuanxn.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ika.ydjk.org.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zqd.sjlbkw.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://slj.vehdjk.com

Go:   strings.TrimSpace(s)
来源：http://amq.zhijiandao.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wea.zhengqikj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hnz.uphjek.com

[A25] 字符串比较
来源：http://oxj.bjfxy.top

Py:   s1 == s2; s1 != s2
来源：http://jwk.xylfe.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://atf.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bvg.sweek.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wqv.chenjidiqi.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vyz.cucudq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cmz.shanyushiyangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://psc.pengpengdd.cyou

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xzc.zhengqikj.top

[A26] 类型转换总览
来源：http://rag.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://khl.jianghu66.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yzm.cqqwz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ezx.yuxming.cn

TS:   Number() String() Boolean() x as number
来源：http://tcx.c1oappe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nao.pycfn.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://moy.feifeiyinyue.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ptl.yangfankeji.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pqz.hywenlv.cn

================================================================================
来源：http://phl.gzhubu.top

B. 流程控制
来源：http://hay.shanyushiyangkeji.top

================================================================================
来源：http://vmk.daria6918.cn

[B01] 条件判断 if / else
来源：http://hso.yj202588.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jkg.havefunace.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nrf.jinqigfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qez.fehbvm.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ici.smart0.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://thn.nwbrower.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://opy.andypj.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://znt.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mzd.epnwcf.com

[B02] 多分支 else if / elif
来源：http://unn.gaohongyu789.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zur.mhx1999.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://edg.cucudq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gms.yj20258888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ryg.hammf.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gyr.vehdjk.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://amm.zdbjq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ncx.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cup.bjfxy.top

[B03] switch / match / case
来源：http://kdf.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qrt.xuanzx.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zcr.sjlbkw.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qgy.epnwcf.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jlt.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zjz.bjfxy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wle.pengpengdd.cyou

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://znx.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jxq.chenjidiqi.icu

[B04] for 计数循环
来源：http://sio.zhixingplan.top

Py:   for i in range(10): print(i)
来源：http://xzz.sufxvd.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://agr.epnwcf.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rbp.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wvl.havefunace.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dzy.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pax.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://nby.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ulg.ctjpmb.com

[B05] 遍历数组 / 列表
来源：http://plt.ivvv.top

Py:   for item in arr: print(item)
来源：http://uvq.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hlb.yanxiufei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bfa.ppjwa.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://eay.shangyingyoupin.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ivi.hysaishi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bnm.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://zdz.bjfxy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mzj.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://csr.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cdw.jiagoushi.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zjf.ppjwa.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gnf.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xml.yj20258888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gau.hnxiangtu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wbn.zhoulong.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gnp.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xqx.zhengqikj.top

[B07] while 循环
来源：http://nhf.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://vnw.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://zhf.uphjek.com

JS:   while (i < 10) { i++; }
来源：http://vuw.bjfxy.top

TS:   while (i < 10) { i++; }
来源：http://ixk.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://zxi.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hle.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://hnv.chenlongwang.top

C#:   while (i < 10) { i++; }
来源：http://lta.chenlongwang.top

[B08] do-while（至少执行一次）
来源：http://pud.cucudq.cn

Py:   # 无 do-while：用 while True + break
来源：http://fdg.epnwcf.com

PHP:  do { $i++; } while ($i < 10);
来源：http://rzq.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://ldn.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://hof.fktsv.cn

Java: do { i++; } while (i < 10);
来源：http://qcf.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xta.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://gkr.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://syv.hongshengwenyu.top

[B09] break 与 continue
来源：http://znp.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eex.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hjf.xuetiantiany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hxd.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sbg.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oqj.yvedp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fjd.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rbq.jqgfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kch.shzxlz.cn

[B10] 遍历同时拿索引
来源：http://qey.svipenyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ane.chenjidiqi.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jjh.aizwys.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wta.kuanghao11.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nrl.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hly.guowangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://drk.0kj1m.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gto.ywan-chungtsiang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pyh.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://qcr.yfazqb.com

Py:   list(range(0, 10, 2))
来源：http://ece.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://nmo.hammf.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ehg.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xrt.jyoumei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bqw.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nzn.hammf.cn

Ruby: (0...10).step(2).to_a
来源：http://nur.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pph.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://cbg.epnwcf.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://fqr.ybcxt.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://etd.yuxming.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tvy.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mjw.sjlbkw.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hrv.tianlin.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://plo.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://thb.xuanzx.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zdj.fengsongda.top

[B13] 判断是否为数字
来源：http://hlh.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://rjk.bjfxy.top

PHP:  is_numeric($x)
来源：http://gfn.zycfv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ujl.xylfe.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mgz.wangdashe.top

Java: x instanceof Number
来源：http://bxx.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ehs.chenzaomai.com

Ruby: x.is_a?(Numeric)
来源：http://viw.zdbjq.cn

C#:   x is int or double or decimal
来源：http://jpa.yanxiufei.cn

[B14] 判断值是否在集合内
来源：http://lnq.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mlr.xuanzx.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ivt.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://xvw.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://maa.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nit.nanxuanxn.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uii.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tit.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ghs.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://zvq.mhx1999.top

Py:   a and b or not c
来源：http://eoh.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://opg.vehdjk.com

JS:   a && b || !c
来源：http://gcw.nanxinkj.top

TS:   a && b || !c
来源：http://amu.jlsjyb.cn

Java: a && b || !c
来源：http://yiq.yuxming.cn

Go:   a && b || !c
来源：http://aex.vehdjk.com

Ruby: a && b || !c
来源：http://zfh.hcnkem.com

C#:   a && b || !c
来源：http://egm.guowangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://ecn.wangdashe.top

Py:   if not data: return
来源：http://bwf.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://bnr.cashguo.top

JS:   if (!data) return;
来源：http://xed.jianghu66.top

TS:   if (!data) return;
来源：http://spw.fehbvm.com

Java: if (data == null) return;
来源：http://gzn.fktsv.cn

Go:   if data == nil { return }
来源：http://ooe.zhijiandao.cn

Ruby: return if data.nil?
来源：http://foy.xingfuxueyuan.xyz

C#:   if (data == null) return;
来源：http://cks.cucudq.cn

================================================================================
来源：http://pne.kuanghao11.cn

C. 函数与作用域
来源：http://fue.feifeiyinyue.top

================================================================================
来源：http://ibp.andypj.xyz

[C01] 定义函数
来源：http://dku.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://jaa.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bsr.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://juw.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xcg.quarkkingdee.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nyk.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://szw.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://nlf.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://snr.dashuyun.cn

[C02] 默认参数
来源：http://npq.redwolf501.top

Py:   def greet(name="World"): return name
来源：http://gao.xziqi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zjg.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://oxl.yj202588.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wly.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://fkk.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zhg.gzhubu.top

Ruby: def greet(name = "World") = name
来源：http://gtk.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://brm.aibaodan.cn

[C03] 可变参数
来源：http://cvw.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://uex.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yxm.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://syz.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uxk.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oqe.jiagoushi.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aji.iojbl.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mmj.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://shk.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://rhx.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rag.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uje.hysaishi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ekp.shangyingyoupin.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rio.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://tmg.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://tnc.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://nnv.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://hzc.cheryme.top

[C05] 返回多个值
来源：http://kjx.zhiwuduotai.top

Py:   return a, b
来源：http://bte.mhx1999.top

PHP:  return [$a, $b];
来源：http://ddz.meibo888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://irx.jianghu66.top

TS:   return { a, b };
来源：http://jri.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uqe.ydzc1.top

Go:   return a, b
来源：http://zhs.meibo888.top

Ruby: return a, b
来源：http://wqv.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://gtn.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://vwz.cheryme.top

Py:   square = lambda x: x * x
来源：http://izm.wangdashe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ruy.zhijiandao.cn

JS:   const square = x => x * x;
来源：http://wtv.nanxinkj.top

TS:   const square = (x: number): number => x * x;
来源：http://bmx.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gzu.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://ysy.andypj.xyz

Ruby: square = ->(x) { x * x }
来源：http://nvd.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://jge.havefunace.top

[C07] 把函数作为参数传入
来源：http://myt.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ocw.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zwe.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zyk.aibaodan.cn

TS:   arr.map(String)
来源：http://dfo.xingfuxueyuan.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vhe.fengsongda.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xhe.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://sfo.yangfankeji.com

C#:   arr.Select(s => s.ToUpper())
来源：http://gno.bjfxy.top

[C08] 闭包
来源：http://cac.zhaomingkeji.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yrj.hongshengwenyu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fia.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sij.tian-w.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tyu.xylfe.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://krj.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xaw.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://thn.nanxuanxn.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bfr.jinyuanbaomall.cn

[C09] 递归
来源：http://pnf.iojbl.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qou.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jmu.jiagoushi.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iuz.jqgfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kei.haohaochexian.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jsi.tianlin.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wde.fengsongda.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iri.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ewz.tianlin.xyz

[C10] 变量作用域
来源：http://ees.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://alv.ivvv.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ans.yj20258.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uad.52xcode.cn

TS:   同 JS
来源：http://ogd.jinqigfzy.top

Java: 方法内为块级作用域
来源：http://lsm.c1oappe.top

Go:   花括号块级作用域
来源：http://nda.ydjk.org.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rbq.ywan-chungtsiang.top


<!-- 参考信息 -->