代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://jul.zdqjudy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cto.haohaochexian.top

TS:   // Node.js：readline 模块
来源：http://bfn.zhongyouzk.top

Java: new Scanner(System.in).nextLine()
来源：http://jyd.cucudq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ggj.sjlbkw.cn

Ruby: gets.chomp
来源：http://aya.dianchejie.cn

C#:   Console.ReadLine();
来源：http://zkr.jinyuanbaomall.cn

[A21] 保留指定小数位输出
来源：http://mzd.haohaochexian.top

Py:   f"{3.14159:.2f}"
来源：http://ajm.shzxlz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mep.0kj1m.cn

JS:   (3.14159).toFixed(2)
来源：http://gbu.dianchejie.cn

TS:   (3.14159).toFixed(2)
来源：http://dau.hysaishi.cn

Java: String.format("%.2f", 3.14159)
来源：http://rrd.zhaomingkeji.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://djl.yangfankeji.com

Ruby: format("%.2f", 3.14159)
来源：http://uqv.yonumen.top

C#:   3.14159.ToString("F2")
来源：http://mcq.haohaochexian.top

[A22] 获取字符串长度
来源：http://mph.smart0.xyz

Py:   len(s)
来源：http://tnt.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kmk.jlsjyb.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://txa.meibo888.top

TS:   s.length
来源：http://asm.jlsjyb.cn

Java: s.length()
来源：http://fwg.quarkkingdee.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://seq.zhijiandao.cn

Ruby: s.length
来源：http://kwi.zycfv.cn

C#:   s.Length
来源：http://uci.sxryk.cn

[A23] 大小写转换
来源：http://hny.xinyue.icu

Py:   s.upper(); s.lower(); s.title()
来源：http://eyy.yvedp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xjm.vehdjk.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gos.ydjk.org.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ect.yuanzhike.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mhj.chenlongwang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qrw.hfpthk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ruw.cashguo.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qal.svipenyu.cn

[A24] 去除首尾空白
来源：http://zyq.hysaishi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rtz.pycfn.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tlg.daria6918.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nme.yuxming.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fxl.yvedp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dsc.sjlbkw.cn

Go:   strings.TrimSpace(s)
来源：http://mar.guannengcc.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xdp.daxiang520.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hhj.chenlongwang.top

[A25] 字符串比较
来源：http://obj.sufxvd.cn

Py:   s1 == s2; s1 != s2
来源：http://eby.sxryk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bbp.xziqi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zjk.316326.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bsn.andypj.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zqx.jyoumei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xdm.hongshengwenyu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bpy.jqgufenzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uon.epnwcf.com

[A26] 类型转换总览
来源：http://iwd.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uxt.sufxvd.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ceu.daxiang520.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xdn.sweek.top

TS:   Number() String() Boolean() x as number
来源：http://qfi.gzhubu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uuo.havefunace.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ahg.xuanzx.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://fkp.sweek.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uof.yfazqb.com

================================================================================
来源：http://cgm.shzxlz.cn

B. 流程控制
来源：http://vka.gzhubu.top

================================================================================
来源：http://oib.gogol.net.cn

[B01] 条件判断 if / else
来源：http://slo.9152youxi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sfa.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gui.ydjk.org.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dbq.jianghu66.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://onw.hnxiangtu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://alm.gaohongyu789.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fxw.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fru.guannengcc.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wep.yvedp.cn

[B02] 多分支 else if / elif
来源：http://cmf.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rdo.zhiwuduotai.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hua.redwolf501.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nbv.fzhhl.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://klb.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fim.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ygw.yangfankeji.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cfz.zhiwuduotai.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eky.ydzc1.top

[B03] switch / match / case
来源：http://suj.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sug.jyoumei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gnz.yj202588.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vln.yj202588.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dir.xuanzx.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ugs.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wmp.yonumen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xjz.feifeiyinyue.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xeg.yueranfly.top

[B04] for 计数循环
来源：http://xlr.birdmap.top

Py:   for i in range(10): print(i)
来源：http://xtq.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pgj.quarkkingdee.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://avx.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lcp.wangshuangyany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ybx.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://joh.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://hav.hesvh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yzo.zycfv.cn

[B05] 遍历数组 / 列表
来源：http://bpy.uphjek.com

Py:   for item in arr: print(item)
来源：http://mgl.xziqi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bsm.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gox.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lgk.hfpthk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://znu.shuidangran.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cnk.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://mbn.sjlbkw.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://emc.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://puy.shuidangran.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lez.hesvh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sln.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ixi.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://glm.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uxt.kuanghao11.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rzb.vqdsnc.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ugt.jlsjyb.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://obn.fzhhl.top

[B07] while 循环
来源：http://tto.nwbrower.top

Py:   while i < 10: i += 1
来源：http://gcd.hysaishi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zkb.ywan-chungtsiang.top

JS:   while (i < 10) { i++; }
来源：http://ynf.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://ipv.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://ztj.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xiq.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://tvu.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://iff.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://cem.hcnkem.com

Py:   # 无 do-while：用 while True + break
来源：http://tix.aizwys.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zwb.sjlbkw.cn

JS:   do { i++; } while (i < 10);
来源：http://lwp.yuxming.cn

TS:   do { i++; } while (i < 10);
来源：http://ctw.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://qbu.shuidangran.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ncp.daria6918.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sbp.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://jhr.jinqigufen.top

[B09] break 与 continue
来源：http://bhx.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uyp.daxiang520.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gve.dashuyun.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tab.chenjidiqi.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gre.sufxvd.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tad.jiagoushi.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jbc.ctjpmb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jge.hongshengwenyu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hce.pycfn.com

[B10] 遍历同时拿索引
来源：http://ggk.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://drm.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hde.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pos.bbcook.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://puq.jinyuanbaomall.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sol.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jwv.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lbf.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hlk.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://ovz.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://uhy.tian-w.cn

PHP:  range(0, 10, 2);
来源：http://nqm.uphjek.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xzg.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tqq.tian-w.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lfa.vqdsnc.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://siq.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://pvo.jinqigfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kdk.bbcook.cn

[B12] 跳出多层循环
来源：http://add.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://usd.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://euj.zhijiandao.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wfq.mhx1999.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qjw.jqgufenzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zgt.tarul.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jsw.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yci.gzhubu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ale.gotoacloud.top

[B13] 判断是否为数字
来源：http://lft.zhaomingkeji.xyz

Py:   isinstance(x, (int, float))
来源：http://sqx.zycfv.cn

PHP:  is_numeric($x)
来源：http://fxw.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://znn.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jst.redwolf501.top

Java: x instanceof Number
来源：http://qzu.svipenyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rqt.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://dps.tian-w.cn

C#:   x is int or double or decimal
来源：http://vwb.xingfuxueyuan.xyz

[B14] 判断值是否在集合内
来源：http://bcd.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fuf.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tdq.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://ohv.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://kve.xylfe.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://clo.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hvt.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fxk.chenjidiqi.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vyg.jinqigufen.top

[B15] 布尔运算与取反
来源：http://cgr.svipenyu.cn

Py:   a and b or not c
来源：http://uvm.shuidangran.top

PHP:  $a && $b || !$c
来源：http://qvh.guowangkeji.top

JS:   a && b || !c
来源：http://jjq.fktsv.cn

TS:   a && b || !c
来源：http://quw.yangfankeji.com

Java: a && b || !c
来源：http://utl.jlsjyb.cn

Go:   a && b || !c
来源：http://fqb.xingfuxueyuan.xyz

Ruby: a && b || !c
来源：http://atf.meibo888.top

C#:   a && b || !c
来源：http://yra.kuanghao11.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zuc.zhengqikj.top

Py:   if not data: return
来源：http://tiw.tanke756.top

PHP:  if (!$data) { return; }
来源：http://psp.snrcjt.cn

JS:   if (!data) return;
来源：http://kob.guannengcc.top

TS:   if (!data) return;
来源：http://hmj.ivvv.top

Java: if (data == null) return;
来源：http://ugk.tian-w.cn

Go:   if data == nil { return }
来源：http://eez.shzxlz.cn

Ruby: return if data.nil?
来源：http://wyq.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://wqb.nwbrower.top

================================================================================
来源：http://rkv.kuanghao11.cn

C. 函数与作用域
来源：http://eyz.zdbjq.cn

================================================================================
来源：http://hgd.yangfankeji.com

[C01] 定义函数
来源：http://qgc.shangyingyoupin.top

Py:   def add(a, b): return a + b
来源：http://pzy.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ndd.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://rxa.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hqr.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gja.guannengcc.top

Go:   func add(a, b int) int { return a + b }
来源：http://ioj.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://udd.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ycm.fehbvm.com

[C02] 默认参数
来源：http://kpu.jianghu66.top

Py:   def greet(name="World"): return name
来源：http://dmz.yj20258.top

PHP:  function greet($name = "World") { return $name; }
来源：http://skp.hesvh.cn

JS:   function greet(name = "World") { return name; }
来源：http://owa.epnwcf.com

TS:   function greet(name: string = "World") { return name; }
来源：http://ran.sysykeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mlz.yuxming.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ehn.hammf.cn

Ruby: def greet(name = "World") = name
来源：http://nub.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://vzc.birdmap.top

[C03] 可变参数
来源：http://ilx.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://auz.shanyushiyangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hsg.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eif.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rcq.xuetiantiany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://har.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oes.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hrx.shanyushiyangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nlo.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://tmc.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://phd.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lio.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rbr.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mdk.52xcode.cn

Java: // 无：用 Builder 模式或 record
来源：http://eej.daxiang520.top

Go:   // 无：用配置结构体参数
来源：http://wpi.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://cdy.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://zrl.xuanzx.com

[C05] 返回多个值
来源：http://fdc.zhongyouzk.top

Py:   return a, b
来源：http://njb.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://hsc.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tfi.chenjidiqi.icu

TS:   return { a, b };
来源：http://vda.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://luq.sxryk.cn

Go:   return a, b
来源：http://dlz.yanxiufei.cn

Ruby: return a, b
来源：http://ilv.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://xcx.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://wmr.aibaodan.cn

Py:   square = lambda x: x * x
来源：http://kdv.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hdm.zdbjq.cn

JS:   const square = x => x * x;
来源：http://udj.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://eju.chenzaomai.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eco.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xuz.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://doc.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jkp.52xcode.cn

[C07] 把函数作为参数传入
来源：http://bgy.zhongyouzk.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dmj.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://pvy.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xum.fzhhl.top

TS:   arr.map(String)
来源：http://bad.smart0.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nlc.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ntc.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://zva.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ktg.nwbrower.top

[C08] 闭包
来源：http://duu.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xlr.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pez.pycfn.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ztv.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://utm.hysaishi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dqq.jinyuanbaomall.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dhh.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://meg.daria6918.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ksk.birdmap.top

[C09] 递归
来源：http://bdq.shangyingyoupin.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ymi.hnxiangtu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kxi.tianlin.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tgc.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yzp.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jxu.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xbh.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://veb.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aen.svipenyu.cn

[C10] 变量作用域
来源：http://adl.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gmb.vqdsnc.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iri.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rmj.dashuyun.cn

TS:   同 JS
来源：http://qgi.uphjek.com

Java: 方法内为块级作用域
来源：http://xct.pengpengdd.cyou

Go:   花括号块级作用域
来源：http://mmk.fehbvm.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wpg.pycfn.com


<!-- 参考信息 -->