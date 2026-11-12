代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://atu.cashguo.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xhv.yj20258.top

TS:   // Node.js：readline 模块
来源：http://tvx.jinqigufen.top

Java: new Scanner(System.in).nextLine()
来源：http://jhk.jinqigfzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pyz.c1oappe.top

Ruby: gets.chomp
来源：http://lwt.xuetiantiany.cn

C#:   Console.ReadLine();
来源：http://pre.nanxinkj.top

[A21] 保留指定小数位输出
来源：http://yup.epnwcf.com

Py:   f"{3.14159:.2f}"
来源：http://khj.nanxuanxn.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://waz.chenlongwang.top

JS:   (3.14159).toFixed(2)
来源：http://qve.kuanghao11.cn

TS:   (3.14159).toFixed(2)
来源：http://cxh.dianchejie.cn

Java: String.format("%.2f", 3.14159)
来源：http://giw.zhixingplan.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sqf.cdnleiting.top

Ruby: format("%.2f", 3.14159)
来源：http://fqd.shzxlz.cn

C#:   3.14159.ToString("F2")
来源：http://gdd.chenjidiqi.icu

[A22] 获取字符串长度
来源：http://lfu.jqgfzy.top

Py:   len(s)
来源：http://pcq.iojbl.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pkp.yuxming.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://suj.sxryk.cn

TS:   s.length
来源：http://iza.wangdashe.top

Java: s.length()
来源：http://dsl.xziqi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gzl.uphjek.com

Ruby: s.length
来源：http://ijr.iojbl.cn

C#:   s.Length
来源：http://yik.jianghu66.top

[A23] 大小写转换
来源：http://ded.ivvv.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zfn.zhaomingkeji.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ydb.daxiang520.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pyg.ehwqpu.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eqk.yangfankeji.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://whh.jqgufenzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://brz.cdnleiting.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bvc.shanyushiyangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://msx.gotoacloud.top

[A24] 去除首尾空白
来源：http://lgs.gzhubu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gov.jyoumei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dnm.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://juh.jqgufenzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rlo.zhoulong.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nmj.yuxming.cn

Go:   strings.TrimSpace(s)
来源：http://ndg.fanxiaobao.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sef.xuetiantiany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rqg.nanxuanxn.top

[A25] 字符串比较
来源：http://okg.ydjk.org.cn

Py:   s1 == s2; s1 != s2
来源：http://qzs.svipenyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nva.jqgfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ddf.hnxiangtu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://spe.iojbl.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ujj.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jdi.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wad.jqgfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nkk.jqgufenzy.top

[A26] 类型转换总览
来源：http://nvj.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eml.ybcxt.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jdk.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mux.hfpthk.cn

TS:   Number() String() Boolean() x as number
来源：http://dfy.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kts.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ral.gzhubu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://imr.gaohongyu789.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xjh.hfpthk.cn

================================================================================
来源：http://iec.ybcxt.top

B. 流程控制
来源：http://glq.ivvv.top

================================================================================
来源：http://zyz.ehwqpu.com

[B01] 条件判断 if / else
来源：http://jon.zdbjq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ssa.gaohongyu789.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dil.fanxiaobao.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://llb.epnwcf.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oxu.jyoumei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fwa.gogol.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oir.fengsongda.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ggs.xinyue.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ltm.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://fek.yj202588.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://imw.zhoulong.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mbe.zdbjq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sng.jinqigfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rsa.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ozj.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sto.shanyushiyangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oda.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qss.zhoulong.xyz

[B03] switch / match / case
来源：http://tho.yuxming.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dxi.pengpengdd.cyou

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wsb.yuxming.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yyp.hfpthk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jff.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xct.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xue.yj202588.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hxq.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hre.shanyushiyangtech.top

[B04] for 计数循环
来源：http://onj.zhiwuduotai.top

Py:   for i in range(10): print(i)
来源：http://nil.ywan-chungtsiang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oqv.ydzc1.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dea.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kbx.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vuj.ydjk.org.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ksg.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://uhq.epnwcf.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ixz.aibaodan.cn

[B05] 遍历数组 / 列表
来源：http://ibu.gzhubu.top

Py:   for item in arr: print(item)
来源：http://dwd.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://osw.hfpthk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tdw.sxryk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gow.sjlbkw.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uia.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wrb.zhoulong.xyz

Ruby: arr.each { |item| puts item }
来源：http://dtj.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uqk.daxiang520.top

[B06] 遍历字典 / 对象
来源：http://qmj.redwolf501.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wca.snrcjt.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yxk.zhongyouzk.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tbz.tian-w.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://smw.fehbvm.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jke.chenlongwang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yfg.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yon.yonumen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nst.316326.xyz

[B07] while 循环
来源：http://nen.havefunace.top

Py:   while i < 10: i += 1
来源：http://tjl.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://nnf.zhengqikj.top

JS:   while (i < 10) { i++; }
来源：http://xfd.ywan-chungtsiang.top

TS:   while (i < 10) { i++; }
来源：http://huh.sweek.top

Java: while (i < 10) { i++; }
来源：http://elg.tian-w.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gaq.wangdashe.top

Ruby: while i < 10; i += 1; end
来源：http://cem.shuidangran.top

C#:   while (i < 10) { i++; }
来源：http://yqk.zhixingplan.top

[B08] do-while（至少执行一次）
来源：http://est.pengpengdd.cyou

Py:   # 无 do-while：用 while True + break
来源：http://xkx.hammf.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bvy.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://ymj.316326.xyz

TS:   do { i++; } while (i < 10);
来源：http://fhf.316326.xyz

Java: do { i++; } while (i < 10);
来源：http://uai.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nxx.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://jvs.gaohongyu789.top

C#:   do { i++; } while (i < 10);
来源：http://iif.yfazqb.com

[B09] break 与 continue
来源：http://ncr.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pnl.andypj.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wlb.jlsjyb.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eck.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vvc.sufxvd.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fmq.nanxuanxn.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mkp.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kuf.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://umk.fzhhl.top

[B10] 遍历同时拿索引
来源：http://qru.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mrq.yuanzhike.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://onc.smart0.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nbn.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lqm.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://btg.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ame.andypj.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xlq.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oww.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://qen.yonumen.top

Py:   list(range(0, 10, 2))
来源：http://idc.meibo888.top

PHP:  range(0, 10, 2);
来源：http://tum.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gox.52xcode.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gbe.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cno.daria6918.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dus.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://ayg.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://afl.jiagoushi.top

[B12] 跳出多层循环
来源：http://eml.bbcook.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nll.jinqigufen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zzd.tian-w.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://plv.hfpthk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mvg.hnxiangtu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qre.chenlongwang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xad.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gby.gotoacloud.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://leb.ivvv.top

[B13] 判断是否为数字
来源：http://zcc.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://wdb.fengsongda.top

PHP:  is_numeric($x)
来源：http://kcc.jinyuanbaomall.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://syt.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://spz.daxiang520.top

Java: x instanceof Number
来源：http://koc.tarul.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dea.jlsjyb.cn

Ruby: x.is_a?(Numeric)
来源：http://mwz.yanxiufei.cn

C#:   x is int or double or decimal
来源：http://qrg.zycfv.cn

[B14] 判断值是否在集合内
来源：http://xgo.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rzr.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xbm.ybcxt.top

JS:   [1, 2, 3].includes(x)
来源：http://jhx.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://vyw.ctjpmb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://scv.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gcj.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rjq.cqqwz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uod.tanke756.top

[B15] 布尔运算与取反
来源：http://jgk.nanxuanxn.top

Py:   a and b or not c
来源：http://ckr.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://vmy.hesvh.cn

JS:   a && b || !c
来源：http://vat.ydjk.org.cn

TS:   a && b || !c
来源：http://hkq.jqgufenzy.top

Java: a && b || !c
来源：http://fal.guowangkeji.top

Go:   a && b || !c
来源：http://yaj.zhaomingkeji.xyz

Ruby: a && b || !c
来源：http://wfj.chenzaomai.com

C#:   a && b || !c
来源：http://mrs.bjfxy.top

[B16] 卫语句：不满足条件提前返回
来源：http://uev.jyoumei.cn

Py:   if not data: return
来源：http://iwf.tarul.cn

PHP:  if (!$data) { return; }
来源：http://kle.jinqigufen.top

JS:   if (!data) return;
来源：http://yst.hammf.cn

TS:   if (!data) return;
来源：http://yyg.bjfxy.top

Java: if (data == null) return;
来源：http://ery.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://jmw.haohaochexian.top

Ruby: return if data.nil?
来源：http://tgy.vqdsnc.cn

C#:   if (data == null) return;
来源：http://kyq.fehbvm.com

================================================================================
来源：http://yfm.cqqwz.cn

C. 函数与作用域
来源：http://xyk.jinqigfzy.top

================================================================================
来源：http://pjb.shanyushiyangtech.top

[C01] 定义函数
来源：http://qso.jianghu66.top

Py:   def add(a, b): return a + b
来源：http://kpd.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qnd.snrcjt.cn

JS:   function add(a, b) { return a + b; }
来源：http://wal.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rsm.hammf.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ekd.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rkm.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://rbv.svipenyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bso.sysykeji.top

[C02] 默认参数
来源：http://bfs.jqgfzy.top

Py:   def greet(name="World"): return name
来源：http://njj.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ndr.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://tys.pycfn.com

TS:   function greet(name: string = "World") { return name; }
来源：http://qdw.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wgz.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wwz.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://cto.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://skq.zhongyouzk.top

[C03] 可变参数
来源：http://tka.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://scj.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dpl.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mqa.yanxiufei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tzx.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://afh.shanyushiyangtech.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wzg.fzhhl.top

Ruby: def total(*nums); nums.sum; end
来源：http://qgv.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ggx.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://wku.bbcook.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ozp.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uiy.fehbvm.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xee.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jwq.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://zlm.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://dce.fzhhl.top

Ruby: f(a: 1, b: 2)
来源：http://hww.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://hhz.fzhhl.top

[C05] 返回多个值
来源：http://zbx.sweek.top

Py:   return a, b
来源：http://bix.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://kup.vehdjk.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ola.yuanzhike.top

TS:   return { a, b };
来源：http://igo.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pqb.zycfv.cn

Go:   return a, b
来源：http://etu.cdnleiting.top

Ruby: return a, b
来源：http://iis.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://ybf.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://rpn.fengsongda.top

Py:   square = lambda x: x * x
来源：http://tbz.guannengcc.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dcx.daxiang520.top

JS:   const square = x => x * x;
来源：http://jhh.pycfn.com

TS:   const square = (x: number): number => x * x;
来源：http://aao.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://inw.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ehg.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://dou.uphjek.com

C#:   Func<int, int> square = x => x * x;
来源：http://xax.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://stc.yueranfly.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zxq.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://whu.52xcode.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pfb.gaohongyu789.top

TS:   arr.map(String)
来源：http://klb.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://enj.svipenyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hyd.pycfn.com

Ruby: arr.map(&:upcase)
来源：http://ghk.jqgfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jzr.pycfn.com

[C08] 闭包
来源：http://lzs.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ypy.ybcxt.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ley.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nib.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zxy.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dhi.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zkl.daxiang520.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rmz.dashuyun.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://egr.jinqigfzy.top

[C09] 递归
来源：http://uyp.9152youxi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uey.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tcc.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pyg.gogol.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ovm.epnwcf.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yis.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rnm.epnwcf.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mab.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cts.quarkkingdee.top

[C10] 变量作用域
来源：http://bzo.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rdj.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tlc.hysaishi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uuh.zhiwuduotai.top

TS:   同 JS
来源：http://vzd.jyoumei.cn

Java: 方法内为块级作用域
来源：http://dom.sxryk.cn

Go:   花括号块级作用域
来源：http://tlv.gotoacloud.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yin.dashuyun.cn


<!-- 参考信息 -->