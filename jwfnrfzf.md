代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://lgp.cucudq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zrh.9152youxi.cn

TS:   // Node.js：readline 模块
来源：http://rwb.yfazqb.com

Java: new Scanner(System.in).nextLine()
来源：http://eod.ehwqpu.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bms.vehdjk.com

Ruby: gets.chomp
来源：http://kae.pycfn.com

C#:   Console.ReadLine();
来源：http://iuh.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://ikb.ydzc1.top

Py:   f"{3.14159:.2f}"
来源：http://icp.zycfv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xnn.pycfn.com

JS:   (3.14159).toFixed(2)
来源：http://jmc.ywan-chungtsiang.top

TS:   (3.14159).toFixed(2)
来源：http://mxw.dianchejie.cn

Java: String.format("%.2f", 3.14159)
来源：http://nwa.sjlbkw.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iqy.tianlin.xyz

Ruby: format("%.2f", 3.14159)
来源：http://jvk.cdnleiting.top

C#:   3.14159.ToString("F2")
来源：http://uyv.yfazqb.com

[A22] 获取字符串长度
来源：http://prk.nwbrower.top

Py:   len(s)
来源：http://nkh.ydjk.org.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oab.andypj.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gla.hysaishi.cn

TS:   s.length
来源：http://tze.jianghu66.top

Java: s.length()
来源：http://xhx.jianghu66.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dfi.fanxiaobao.xyz

Ruby: s.length
来源：http://crr.uphjek.com

C#:   s.Length
来源：http://rnw.pycfn.com

[A23] 大小写转换
来源：http://wzs.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lve.fehbvm.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kws.xziqi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zxj.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ebp.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vsn.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xdc.ehwqpu.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hrq.vehdjk.com

C#:   s.ToUpper(); s.ToLower()
来源：http://zfe.vehdjk.com

[A24] 去除首尾空白
来源：http://ikp.fengsongda.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qin.nanxuanxn.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kep.0kj1m.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iru.nanxuanxn.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nef.fktsv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ryc.uphjek.com

Go:   strings.TrimSpace(s)
来源：http://err.yfazqb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pnz.xingfuxueyuan.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gqd.jinghuilouyu.cn

[A25] 字符串比较
来源：http://dsh.tanke756.top

Py:   s1 == s2; s1 != s2
来源：http://wsk.nwbrower.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pkt.zycfv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zar.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://awf.gzhubu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sem.yuanzhike.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://elf.guannengcc.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kyf.zycfv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ery.haohaochexian.top

[A26] 类型转换总览
来源：http://uun.sufxvd.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fwm.52xcode.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xxo.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qmt.chenlongwang.top

TS:   Number() String() Boolean() x as number
来源：http://dom.jianghu66.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wje.jiagoushi.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://inv.jyoumei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zeq.jianghu66.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sko.daxiang520.top

================================================================================
来源：http://vkw.gogol.net.cn

B. 流程控制
来源：http://jzi.tianlin.xyz

================================================================================
来源：http://qyv.cashguo.top

[B01] 条件判断 if / else
来源：http://xzw.jinqigfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nyi.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pbj.xziqi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://keq.aibaodan.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dss.redwolf501.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tuh.xylfe.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mgv.yfazqb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hpz.bbcook.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tsi.xylfe.cn

[B02] 多分支 else if / elif
来源：http://bcc.hcnkem.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://urh.yj202588.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xbd.gzhubu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gko.yj20258888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wrr.tanke756.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kgv.shanyushiyangtech.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uhj.sjlbkw.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ckp.fanxiaobao.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ceb.zhixingplan.top

[B03] switch / match / case
来源：http://zzp.kuanghao11.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wjk.aibaodan.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cgn.ydzc1.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ybg.52xcode.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tgl.yonumen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qic.nanxinkj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nol.zdqjudy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://icp.shzxlz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lnt.hfpthk.cn

[B04] for 计数循环
来源：http://cgi.svipenyu.cn

Py:   for i in range(10): print(i)
来源：http://rgg.ehwqpu.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qlp.daria6918.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wvy.xinyue.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lem.zhijiandao.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qkn.ybcxt.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fjf.wangshuangyany.cn

Ruby: 10.times { |i| puts i }
来源：http://ghj.wangshuangyany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zni.jinqigfzy.top

[B05] 遍历数组 / 列表
来源：http://iwe.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://pvm.fanxiaobao.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gcq.tianlin.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://wbv.zdqjudy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vya.iojbl.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cck.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zin.nwbrower.top

Ruby: arr.each { |item| puts item }
来源：http://njq.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xzf.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://lqc.zdqjudy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lkg.birdmap.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://psv.cqqwz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://usd.cheryme.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zun.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://btb.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ijm.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jxx.zdbjq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kao.pycfn.com

[B07] while 循环
来源：http://jnu.ydzc1.top

Py:   while i < 10: i += 1
来源：http://kvt.nanxuanxn.top

PHP:  while ($i < 10) { $i++; }
来源：http://bcu.316326.xyz

JS:   while (i < 10) { i++; }
来源：http://gzw.pycfn.com

TS:   while (i < 10) { i++; }
来源：http://zqr.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://rcx.fehbvm.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://frt.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://gbu.pengpengdd.cyou

C#:   while (i < 10) { i++; }
来源：http://afp.ivvv.top

[B08] do-while（至少执行一次）
来源：http://eln.yueranfly.top

Py:   # 无 do-while：用 while True + break
来源：http://yip.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://qzj.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://bda.hysaishi.cn

TS:   do { i++; } while (i < 10);
来源：http://gmf.epnwcf.com

Java: do { i++; } while (i < 10);
来源：http://lir.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rdt.shuidangran.top

Ruby: begin; i += 1; end while i < 10
来源：http://sum.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://yjf.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://fjm.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://otw.andypj.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qot.yuanzhike.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gjh.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://puz.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iej.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kor.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xpv.andypj.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wbw.zhengqikj.top

[B10] 遍历同时拿索引
来源：http://skm.dashuyun.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nhk.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yfb.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qse.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ixf.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hlx.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jgd.hcnkem.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uzs.svipenyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fku.hnxiangtu.top

[B11] 生成数字序列 / 区间
来源：http://onb.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://kas.andypj.xyz

PHP:  range(0, 10, 2);
来源：http://hqk.wangshuangyany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wch.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ean.chenzaomai.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vfu.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qsa.dashuyun.cn

Ruby: (0...10).step(2).to_a
来源：http://piy.pengpengdd.cyou

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xds.yuxming.cn

[B12] 跳出多层循环
来源：http://iyd.zhongyouzk.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cte.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ysy.epnwcf.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://naz.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kcm.fanxiaobao.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tmt.sjlbkw.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://evt.wangdashe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dvf.shanyushiyangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ahp.gaohongyu789.top

[B13] 判断是否为数字
来源：http://eqc.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://rmc.birdmap.top

PHP:  is_numeric($x)
来源：http://hhx.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lnk.316326.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vpn.hfpthk.cn

Java: x instanceof Number
来源：http://qgr.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jml.shangyingyoupin.top

Ruby: x.is_a?(Numeric)
来源：http://rrh.snrcjt.cn

C#:   x is int or double or decimal
来源：http://dqp.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://hym.zhaomingkeji.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mro.xuetiantiany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qqx.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://ahu.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://gsw.ctjpmb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://jrv.jianghu66.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://upe.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mcb.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mpp.316326.xyz

[B15] 布尔运算与取反
来源：http://plz.jqgfzy.top

Py:   a and b or not c
来源：http://qee.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://cbw.birdmap.top

JS:   a && b || !c
来源：http://lmf.yanxiufei.cn

TS:   a && b || !c
来源：http://yhu.tarul.cn

Java: a && b || !c
来源：http://znr.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://gez.sufxvd.cn

Ruby: a && b || !c
来源：http://cgo.ydjk.org.cn

C#:   a && b || !c
来源：http://fnk.9152youxi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bvj.0kj1m.cn

Py:   if not data: return
来源：http://llx.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://rdj.yanxiufei.cn

JS:   if (!data) return;
来源：http://ewu.zdbjq.cn

TS:   if (!data) return;
来源：http://rlv.aizwys.cn

Java: if (data == null) return;
来源：http://wuy.zhengqikj.top

Go:   if data == nil { return }
来源：http://lsu.shanyushiyangtech.top

Ruby: return if data.nil?
来源：http://ayp.tianlin.xyz

C#:   if (data == null) return;
来源：http://ljs.andypj.xyz

================================================================================
来源：http://sfg.yongpay.top

C. 函数与作用域
来源：http://hya.gogol.net.cn

================================================================================
来源：http://ehv.shuidangran.top

[C01] 定义函数
来源：http://coh.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://pjv.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ruc.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://akx.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bmo.hcnkem.com

Java: static int add(int a, int b) { return a + b; }
来源：http://iys.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://ylg.nanxuanxn.top

Ruby: def add(a, b); a + b; end
来源：http://erd.yueranfly.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wjv.gzhubu.top

[C02] 默认参数
来源：http://xhe.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://gpm.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ujp.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://zpm.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hby.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://evu.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wsz.sysykeji.top

Ruby: def greet(name = "World") = name
来源：http://szy.hammf.cn

C#:   string Greet(string name = "World") => name;
来源：http://tlp.aizwys.cn

[C03] 可变参数
来源：http://blr.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://iti.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tvw.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://whl.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ahn.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ifm.nanxuanxn.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hpj.zhixingplan.top

Ruby: def total(*nums); nums.sum; end
来源：http://srs.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pxz.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://jmj.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gig.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zmh.fzhhl.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bfw.nanxuanxn.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jim.yvedp.cn

Java: // 无：用 Builder 模式或 record
来源：http://fyg.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://xae.tanke756.top

Ruby: f(a: 1, b: 2)
来源：http://zij.fanxiaobao.xyz

C#:   f(a: 1, b: 2)
来源：http://pra.yanxiufei.cn

[C05] 返回多个值
来源：http://uyd.bjfxy.top

Py:   return a, b
来源：http://cxe.aibaodan.cn

PHP:  return [$a, $b];
来源：http://hrb.vehdjk.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://bfl.aibaodan.cn

TS:   return { a, b };
来源：http://lef.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hyk.yvedp.cn

Go:   return a, b
来源：http://buj.tian-w.cn

Ruby: return a, b
来源：http://vdp.hongshengwenyu.top

C#:   return (a, b);              // ValueTuple
来源：http://dgi.sufxvd.cn

[C06] 匿名函数 / lambda
来源：http://ukn.tian-w.cn

Py:   square = lambda x: x * x
来源：http://ldm.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wna.fehbvm.com

JS:   const square = x => x * x;
来源：http://cjd.guowangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://hsn.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uev.0kj1m.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lck.cheryme.top

Ruby: square = ->(x) { x * x }
来源：http://dmv.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://yip.sysykeji.top

[C07] 把函数作为参数传入
来源：http://uit.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hej.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://jel.xingfuxueyuan.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ukf.cqqwz.cn

TS:   arr.map(String)
来源：http://jtz.ehwqpu.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jll.yvedp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nwt.yuanzhike.top

Ruby: arr.map(&:upcase)
来源：http://ffo.xuetiantiany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lfe.gogol.net.cn

[C08] 闭包
来源：http://pya.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mti.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uun.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xnf.sufxvd.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jke.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gek.9152youxi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ssk.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yak.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://arc.svipenyu.cn

[C09] 递归
来源：http://bnw.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kju.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://aze.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gks.sufxvd.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qxq.jlsjyb.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yeb.gzhubu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kkp.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bym.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ueg.fehbvm.com

[C10] 变量作用域
来源：http://wzh.tanke756.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yuj.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dxe.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://enz.jqgfzy.top

TS:   同 JS
来源：http://vts.fengsongda.top

Java: 方法内为块级作用域
来源：http://rho.hongshengwenyu.top

Go:   花括号块级作用域
来源：http://djc.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fau.sxryk.cn


<!-- 参考信息 -->