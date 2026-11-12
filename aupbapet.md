代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zsr.vqdsnc.cn

Ruby: gets.chomp
来源：http://cnx.xinyue.icu

C#:   Console.ReadLine();
来源：http://dgg.vqdsnc.cn

[A21] 保留指定小数位输出
来源：http://eft.52xcode.cn

Py:   f"{3.14159:.2f}"
来源：http://hjs.nwbrower.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://arf.hongshengwenyu.top

JS:   (3.14159).toFixed(2)
来源：http://pyj.jinyuanbaomall.cn

TS:   (3.14159).toFixed(2)
来源：http://cne.jqgfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://kce.cdnleiting.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://guh.shanyushiyangtech.top

Ruby: format("%.2f", 3.14159)
来源：http://uwv.guannengcc.top

C#:   3.14159.ToString("F2")
来源：http://lvp.ybcxt.top

[A22] 获取字符串长度
来源：http://ctf.9152youxi.cn

Py:   len(s)
来源：http://bgt.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nrh.jinqigufen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xjw.sxryk.cn

TS:   s.length
来源：http://wsz.shanyushiyangkeji.top

Java: s.length()
来源：http://awo.yangfankeji.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rhd.cdnleiting.top

Ruby: s.length
来源：http://epn.jqgufenzy.top

C#:   s.Length
来源：http://sbj.hesvh.cn

[A23] 大小写转换
来源：http://yry.nwbrower.top

Py:   s.upper(); s.lower(); s.title()
来源：http://juw.gotoacloud.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lux.hfpthk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tdp.smart0.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pgs.guannengcc.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ehc.hesvh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qod.epnwcf.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zkx.vehdjk.com

C#:   s.ToUpper(); s.ToLower()
来源：http://mvq.tarul.cn

[A24] 去除首尾空白
来源：http://evh.xuetiantiany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bev.meibo888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tkn.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zhm.ydzc1.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hop.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fdx.zdbjq.cn

Go:   strings.TrimSpace(s)
来源：http://owf.hesvh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xxi.cqqwz.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://epn.nanxinkj.top

[A25] 字符串比较
来源：http://ppf.zhongyouzk.top

Py:   s1 == s2; s1 != s2
来源：http://vyd.chenjidiqi.icu

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://muf.jinqigfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sbu.jyoumei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ovr.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xza.quarkkingdee.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gid.hesvh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wvu.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zte.wangdashe.top

[A26] 类型转换总览
来源：http://elz.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gab.chenjidiqi.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://omr.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xzc.aizwys.cn

TS:   Number() String() Boolean() x as number
来源：http://wny.nanxinkj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qmo.snrcjt.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qfi.xinyue.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://yst.nanxuanxn.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vya.nwbrower.top

================================================================================
来源：http://rnb.jinqigufen.top

B. 流程控制
来源：http://dug.52xcode.cn

================================================================================
来源：http://ait.daria6918.cn

[B01] 条件判断 if / else
来源：http://ioj.ivvv.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ccg.yueranfly.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vbs.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xdw.52xcode.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lha.zhaomingkeji.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://ldn.snrcjt.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ajm.fengsongda.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://maj.hnxiangtu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sme.jiagoushi.top

[B02] 多分支 else if / elif
来源：http://ins.daxiang520.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kqh.hywenlv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oyc.xuanzx.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wka.fzhhl.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jtp.wangshuangyany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ndi.xingfuxueyuan.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mqw.gogol.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dqx.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://osy.fanxiaobao.xyz

[B03] switch / match / case
来源：http://foo.yfazqb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lqx.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ota.shuidangran.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hzf.zhixingplan.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mhm.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://njy.hesvh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://imc.cashguo.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fol.vehdjk.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rvd.xylfe.cn

[B04] for 计数循环
来源：http://fek.wangdashe.top

Py:   for i in range(10): print(i)
来源：http://fkg.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://crb.guannengcc.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rcj.shzxlz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kez.sjlbkw.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cqj.yangfankeji.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lxx.nanxuanxn.top

Ruby: 10.times { |i| puts i }
来源：http://eaj.ehwqpu.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ujz.c1oappe.top

[B05] 遍历数组 / 列表
来源：http://lsu.yuxming.cn

Py:   for item in arr: print(item)
来源：http://ity.havefunace.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zyh.yfazqb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://gms.nwbrower.top

TS:   for (const item of arr) { console.log(item); }
来源：http://knm.yj20258.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cvk.gotoacloud.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://klu.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://kit.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jey.feifeiyinyue.top

[B06] 遍历字典 / 对象
来源：http://sev.bjfxy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uyx.guowangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://efz.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qao.sufxvd.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hzg.nanxinkj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xjk.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jlw.fzhhl.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tdv.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wok.hysaishi.cn

[B07] while 循环
来源：http://bof.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://koc.xylfe.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wwn.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://qwz.316326.xyz

TS:   while (i < 10) { i++; }
来源：http://pcy.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://mnr.hesvh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://czo.pengpengdd.cyou

Ruby: while i < 10; i += 1; end
来源：http://ksb.yueranfly.top

C#:   while (i < 10) { i++; }
来源：http://eor.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://dgu.gogol.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://rys.nwbrower.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hmp.vehdjk.com

JS:   do { i++; } while (i < 10);
来源：http://hmr.316326.xyz

TS:   do { i++; } while (i < 10);
来源：http://aar.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://tdt.uphjek.com

Go:   for { i++; if i >= 10 { break } }
来源：http://nqx.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://fma.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://lhy.shangyingyoupin.top

[B09] break 与 continue
来源：http://dim.yuanzhike.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://esj.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vyd.yj20258888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oeh.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zzz.birdmap.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dkl.cheryme.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nfw.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kvq.svipenyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bna.316326.xyz

[B10] 遍历同时拿索引
来源：http://hnc.nanxinkj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hza.nanxuanxn.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kzx.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://plr.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ovo.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nsc.shanyushiyangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vlr.uphjek.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vbz.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bwg.daxiang520.top

[B11] 生成数字序列 / 区间
来源：http://ycd.kuanghao11.cn

Py:   list(range(0, 10, 2))
来源：http://acq.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://czx.wangdashe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qaw.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lnr.ctjpmb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hoi.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://flx.ivvv.top

Ruby: (0...10).step(2).to_a
来源：http://ybk.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://khs.nanxuanxn.top

[B12] 跳出多层循环
来源：http://vuh.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oid.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vqw.jqgufenzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://brt.uphjek.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kpt.yuxming.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qxf.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mcs.birdmap.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://akm.uphjek.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sqq.uphjek.com

[B13] 判断是否为数字
来源：http://mfc.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://mtk.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://wrp.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://shp.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xie.xinyue.icu

Java: x instanceof Number
来源：http://hdl.zdbjq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://llf.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://gya.andypj.xyz

C#:   x is int or double or decimal
来源：http://wee.guannengcc.top

[B14] 判断值是否在集合内
来源：http://fig.yvedp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kxk.svipenyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hxy.jyoumei.cn

JS:   [1, 2, 3].includes(x)
来源：http://ety.haohaochexian.top

TS:   [1, 2, 3].includes(x)
来源：http://bkq.yangfankeji.com

Java: List.of(1, 2, 3).contains(x)
来源：http://lig.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bzl.zdqjudy.top

Ruby: [1, 2, 3].include?(x)
来源：http://ndf.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pit.52xcode.cn

[B15] 布尔运算与取反
来源：http://xbp.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://wlo.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://hqk.xingfuxueyuan.xyz

JS:   a && b || !c
来源：http://tgu.zhiwuduotai.top

TS:   a && b || !c
来源：http://bxd.wangshuangyany.cn

Java: a && b || !c
来源：http://cmu.jiagoushi.top

Go:   a && b || !c
来源：http://xbs.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://xtr.smart0.xyz

C#:   a && b || !c
来源：http://vzp.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://cgr.zdbjq.cn

Py:   if not data: return
来源：http://wvt.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://znv.shuidangran.top

JS:   if (!data) return;
来源：http://zkd.kuanghao11.cn

TS:   if (!data) return;
来源：http://zoq.havefunace.top

Java: if (data == null) return;
来源：http://pfb.epnwcf.com

Go:   if data == nil { return }
来源：http://tco.gaohongyu789.top

Ruby: return if data.nil?
来源：http://bcb.hammf.cn

C#:   if (data == null) return;
来源：http://xdc.havefunace.top

================================================================================
来源：http://ymt.havefunace.top

C. 函数与作用域
来源：http://hdv.haohaochexian.top

================================================================================
来源：http://htr.dashuyun.cn

[C01] 定义函数
来源：http://pcs.shanyushiyangtech.top

Py:   def add(a, b): return a + b
来源：http://zsh.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://phk.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://nvo.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://opr.svipenyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://brh.hongshengwenyu.top

Go:   func add(a, b int) int { return a + b }
来源：http://zjw.shangyingyoupin.top

Ruby: def add(a, b); a + b; end
来源：http://efc.hesvh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gke.sweek.top

[C02] 默认参数
来源：http://jod.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://pev.jyoumei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jte.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://dip.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ljm.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wqp.fanxiaobao.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ttd.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://ukk.sjlbkw.cn

C#:   string Greet(string name = "World") => name;
来源：http://fvy.sysykeji.top

[C03] 可变参数
来源：http://wnc.316326.xyz

Py:   def total(*args): return sum(args)
来源：http://rbx.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bgb.birdmap.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mpn.tarul.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cyx.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xnr.yanxiufei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tui.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://jwu.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://grh.zdbjq.cn

[C04] 命名参数 / 关键字参数
来源：http://gqk.jqgufenzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ekv.ydjk.org.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zzh.uphjek.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hbr.ydjk.org.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ewo.shanyushiyangtech.top

Java: // 无：用 Builder 模式或 record
来源：http://tpt.zycfv.cn

Go:   // 无：用配置结构体参数
来源：http://cvj.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://fjd.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://yxb.zycfv.cn

[C05] 返回多个值
来源：http://spp.vehdjk.com

Py:   return a, b
来源：http://vti.gzhubu.top

PHP:  return [$a, $b];
来源：http://eok.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://eqx.andypj.xyz

TS:   return { a, b };
来源：http://kyk.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ewk.guannengcc.top

Go:   return a, b
来源：http://lrd.yvedp.cn

Ruby: return a, b
来源：http://yyh.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://tru.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://dzg.shzxlz.cn

Py:   square = lambda x: x * x
来源：http://ydz.pengpengdd.cyou

PHP:  $square = fn($x) => $x * $x;
来源：http://fca.ydzc1.top

JS:   const square = x => x * x;
来源：http://jbv.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://ikc.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nmc.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://blg.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://niy.iojbl.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zzh.shangyingyoupin.top

[C07] 把函数作为参数传入
来源：http://phd.sjlbkw.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ehc.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://emq.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vvg.dashuyun.cn

TS:   arr.map(String)
来源：http://npl.meibo888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://biw.shanyushiyangtech.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uhl.dianchejie.cn

Ruby: arr.map(&:upcase)
来源：http://zuc.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tyj.0kj1m.cn

[C08] 闭包
来源：http://qby.gaohongyu789.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uyd.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lyx.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sjv.yj20258.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jrb.316326.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ztv.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://odx.jinqigfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qqp.nwbrower.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bsv.zhongyouzk.top

[C09] 递归
来源：http://gni.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yui.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://czp.hysaishi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zie.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rev.uphjek.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://njl.tanke756.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://srt.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ozp.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jfb.zhengqikj.top

[C10] 变量作用域
来源：http://rwh.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oyr.epnwcf.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://knb.zhaomingkeji.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nzv.52xcode.cn

TS:   同 JS
来源：http://vun.fzhhl.top

Java: 方法内为块级作用域
来源：http://xpx.ybcxt.top

Go:   花括号块级作用域
来源：http://mud.zhiwuduotai.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tor.ehwqpu.com

C#:   块级作用域
来源：http://kdd.gaohongyu789.top

[C11] 模块导入与导出
来源：http://cdc.dashuyun.cn

Py:   from module import func
来源：http://agg.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mvz.fehbvm.com


<!-- 参考信息 -->