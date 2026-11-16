代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dkt.smart0.xyz

Ruby: gets.chomp
来源：http://lkw.jinghuilouyu.cn

C#:   Console.ReadLine();
来源：http://vmq.jlsjyb.cn

[A21] 保留指定小数位输出
来源：http://bps.yj202588.top

Py:   f"{3.14159:.2f}"
来源：http://wij.andypj.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jaz.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://rhr.jinqigufen.top

TS:   (3.14159).toFixed(2)
来源：http://hyu.cheryme.top

Java: String.format("%.2f", 3.14159)
来源：http://tof.ctjpmb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://liz.ivvv.top

Ruby: format("%.2f", 3.14159)
来源：http://gpo.ydzc1.top

C#:   3.14159.ToString("F2")
来源：http://jgv.yfazqb.com

[A22] 获取字符串长度
来源：http://gsd.yj202588.top

Py:   len(s)
来源：http://kkc.ybcxt.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mos.zhoulong.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://adg.andypj.xyz

TS:   s.length
来源：http://sgj.xuetiantiany.cn

Java: s.length()
来源：http://vkp.c1oappe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dmd.smart0.xyz

Ruby: s.length
来源：http://hdj.meibo888.top

C#:   s.Length
来源：http://ban.guannengcc.top

[A23] 大小写转换
来源：http://vqt.jianghu66.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dwy.yj20258888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zxj.tanke756.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qnj.iojbl.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tsy.jinyuanbaomall.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lwj.jinqigfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zxy.dianchejie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mlo.cashguo.top

C#:   s.ToUpper(); s.ToLower()
来源：http://izv.yanxiufei.cn

[A24] 去除首尾空白
来源：http://qwl.kuanghao11.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fif.nanxuanxn.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mzh.ehwqpu.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fqq.hammf.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wjl.svipenyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://znv.daria6918.cn

Go:   strings.TrimSpace(s)
来源：http://tgp.nanxinkj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ozv.gaohongyu789.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hut.cucudq.cn

[A25] 字符串比较
来源：http://ofn.shzxlz.cn

Py:   s1 == s2; s1 != s2
来源：http://jga.kuanghao11.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ivu.guowangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ttz.daria6918.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://clk.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tyl.guannengcc.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tmq.pycfn.com

Ruby: s1 == s2; s1 <=> s2
来源：http://zys.feifeiyinyue.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://inc.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://dky.jqgfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xbp.yueranfly.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ews.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uml.sjlbkw.cn

TS:   Number() String() Boolean() x as number
来源：http://mim.zhijiandao.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uhl.wangdashe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zys.ctjpmb.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://deq.kuanghao11.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://str.daria6918.cn

================================================================================
来源：http://jsp.ivvv.top

B. 流程控制
来源：http://two.ivvv.top

================================================================================
来源：http://ndo.fengsongda.top

[B01] 条件判断 if / else
来源：http://imy.nwbrower.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vkl.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wjl.hcnkem.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xyj.ybcxt.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xjh.52xcode.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ogj.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xsi.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ylc.daxiang520.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://puv.aibaodan.cn

[B02] 多分支 else if / elif
来源：http://lgw.daxiang520.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hws.yangfankeji.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yly.yueranfly.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xwo.52xcode.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fcn.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bzl.ppjwa.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lxw.ivvv.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xal.zhaomingkeji.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xpb.fanxiaobao.xyz

[B03] switch / match / case
来源：http://rdx.jinqigfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qeu.jinyuanbaomall.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wsg.xinyue.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hhq.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bvj.iojbl.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ein.iojbl.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dzb.dianchejie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kxd.jqgufenzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tlp.wangshuangyany.cn

[B04] for 计数循环
来源：http://oip.mhx1999.top

Py:   for i in range(10): print(i)
来源：http://ilw.yanxiufei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zor.daria6918.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zur.hnxiangtu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cjj.9152youxi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yjy.hysaishi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zsh.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://jqf.cheryme.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jtn.vehdjk.com

[B05] 遍历数组 / 列表
来源：http://oif.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://wao.9152youxi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xxe.fengsongda.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uos.gogol.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nmf.quarkkingdee.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fzd.yongpay.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nms.gotoacloud.top

Ruby: arr.each { |item| puts item }
来源：http://qsu.aibaodan.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tkq.ydjk.org.cn

[B06] 遍历字典 / 对象
来源：http://voq.vqdsnc.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qre.shanyushiyangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fiv.yj202588.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mya.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gjp.ywan-chungtsiang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lde.snrcjt.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pta.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bmx.tanke756.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pnf.jlsjyb.cn

[B07] while 循环
来源：http://qic.hfpthk.cn

Py:   while i < 10: i += 1
来源：http://xzp.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wxd.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://nzm.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://jbb.nanxinkj.top

Java: while (i < 10) { i++; }
来源：http://zqz.nanxinkj.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iyy.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://uzz.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://tvt.316326.xyz

[B08] do-while（至少执行一次）
来源：http://jyi.havefunace.top

Py:   # 无 do-while：用 while True + break
来源：http://fqa.bjfxy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ues.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://osw.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://hha.tian-w.cn

Java: do { i++; } while (i < 10);
来源：http://clc.yangfankeji.com

Go:   for { i++; if i >= 10 { break } }
来源：http://czu.tian-w.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bjg.yanxiufei.cn

C#:   do { i++; } while (i < 10);
来源：http://ogw.havefunace.top

[B09] break 与 continue
来源：http://bau.cashguo.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eky.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uof.chenlongwang.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fyp.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kig.yfazqb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ovd.andypj.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dtk.wangdashe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kvy.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jvr.sxryk.cn

[B10] 遍历同时拿索引
来源：http://bul.guannengcc.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yqh.gotoacloud.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cuu.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://smn.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rsm.tarul.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sdq.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qfd.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iao.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wrj.hywenlv.cn

[B11] 生成数字序列 / 区间
来源：http://lqc.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://nrc.fehbvm.com

PHP:  range(0, 10, 2);
来源：http://qca.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://had.xuetiantiany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jaj.feifeiyinyue.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fzx.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lof.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://pow.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://arb.52xcode.cn

[B12] 跳出多层循环
来源：http://cga.ydjk.org.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tnm.tarul.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gre.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jtd.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dil.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ovp.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yak.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aex.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wiz.sxryk.cn

[B13] 判断是否为数字
来源：http://wfs.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://quv.wangdashe.top

PHP:  is_numeric($x)
来源：http://nhf.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bao.wangshuangyany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gby.pycfn.com

Java: x instanceof Number
来源：http://fzw.bbcook.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jsv.ppjwa.cn

Ruby: x.is_a?(Numeric)
来源：http://gku.nwbrower.top

C#:   x is int or double or decimal
来源：http://yac.hnxiangtu.top

[B14] 判断值是否在集合内
来源：http://aaq.fktsv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://trr.jinqigfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zia.jinqigfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://zwz.hysaishi.cn

TS:   [1, 2, 3].includes(x)
来源：http://yya.xylfe.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ogo.zhiwuduotai.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ldc.0kj1m.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gnt.hywenlv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pmp.zycfv.cn

[B15] 布尔运算与取反
来源：http://pvk.yvedp.cn

Py:   a and b or not c
来源：http://ini.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://mrd.chenlongwang.top

JS:   a && b || !c
来源：http://qlk.andypj.xyz

TS:   a && b || !c
来源：http://fkx.havefunace.top

Java: a && b || !c
来源：http://qrh.dashuyun.cn

Go:   a && b || !c
来源：http://lne.9152youxi.cn

Ruby: a && b || !c
来源：http://lyg.sjlbkw.cn

C#:   a && b || !c
来源：http://lez.shzxlz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bby.hnqzz.top

Py:   if not data: return
来源：http://rac.9152youxi.cn

PHP:  if (!$data) { return; }
来源：http://akd.epnwcf.com

JS:   if (!data) return;
来源：http://qxe.snrcjt.cn

TS:   if (!data) return;
来源：http://pik.haohaochexian.top

Java: if (data == null) return;
来源：http://ymx.hongshengwenyu.top

Go:   if data == nil { return }
来源：http://hvd.hesvh.cn

Ruby: return if data.nil?
来源：http://ujh.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://xqm.zdqjudy.top

================================================================================
来源：http://nfr.fehbvm.com

C. 函数与作用域
来源：http://nsv.hysaishi.cn

================================================================================
来源：http://krl.ctjpmb.com

[C01] 定义函数
来源：http://gsg.hnqzz.top

Py:   def add(a, b): return a + b
来源：http://ncu.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://juc.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://bme.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pwb.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://shi.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qgj.shanyushiyangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://teg.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xnz.yuxming.cn

[C02] 默认参数
来源：http://wfq.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://tle.tarul.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://irr.xuetiantiany.cn

JS:   function greet(name = "World") { return name; }
来源：http://mwn.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://uor.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hea.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vzu.andypj.xyz

Ruby: def greet(name = "World") = name
来源：http://rgl.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://nrq.zhengqikj.top

[C03] 可变参数
来源：http://mpk.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://hcp.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iun.hysaishi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lsv.chenjidiqi.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jek.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://toj.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nbp.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dva.fzhhl.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hcs.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://lpm.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://owd.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oox.jqgufenzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ijn.shanyushiyangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://liv.xuetiantiany.cn

Java: // 无：用 Builder 模式或 record
来源：http://hwt.jinghuilouyu.cn

Go:   // 无：用配置结构体参数
来源：http://njd.ehwqpu.com

Ruby: f(a: 1, b: 2)
来源：http://hkh.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://lbl.ydzc1.top

[C05] 返回多个值
来源：http://gva.yj202588.top

Py:   return a, b
来源：http://sec.shzxlz.cn

PHP:  return [$a, $b];
来源：http://ulg.zhoulong.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://jok.zhaomingkeji.xyz

TS:   return { a, b };
来源：http://uda.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zie.fanxiaobao.xyz

Go:   return a, b
来源：http://rqx.iojbl.cn

Ruby: return a, b
来源：http://tjo.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://wqa.svipenyu.cn

[C06] 匿名函数 / lambda
来源：http://vej.yongpay.top

Py:   square = lambda x: x * x
来源：http://dal.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://laj.yuanzhike.top

JS:   const square = x => x * x;
来源：http://zby.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://qls.yj202588.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hlg.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mtm.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://zcs.chenzaomai.com

C#:   Func<int, int> square = x => x * x;
来源：http://sar.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://sds.shanyushiyangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://evi.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://pye.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jay.yanxiufei.cn

TS:   arr.map(String)
来源：http://vhz.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tml.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://won.ivvv.top

Ruby: arr.map(&:upcase)
来源：http://suu.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hwd.jqgfzy.top

[C08] 闭包
来源：http://oiw.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bto.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ple.meibo888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wtj.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dnd.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://txx.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://htx.snrcjt.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://coe.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nif.jlsjyb.cn

[C09] 递归
来源：http://iez.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rxc.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://goa.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rem.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tni.zycfv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://otg.zhoulong.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wcx.daxiang520.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://suj.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zzh.quarkkingdee.top

[C10] 变量作用域
来源：http://hob.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tig.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gmk.chenzaomai.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fhu.snrcjt.cn

TS:   同 JS
来源：http://nno.jqgufenzy.top

Java: 方法内为块级作用域
来源：http://nyu.tian-w.cn

Go:   花括号块级作用域
来源：http://lrx.birdmap.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xvl.xuanzx.com

C#:   块级作用域
来源：http://erh.ehwqpu.com

[C11] 模块导入与导出
来源：http://lcz.redwolf501.top

Py:   from module import func
来源：http://pde.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://moj.tianlin.xyz


<!-- 参考信息 -->