代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dhf.jlsjyb.cn

Ruby: gets.chomp
来源：http://ocg.uphjek.com

C#:   Console.ReadLine();
来源：http://rgr.epnwcf.com

[A21] 保留指定小数位输出
来源：http://yvg.zycfv.cn

Py:   f"{3.14159:.2f}"
来源：http://hsp.zdbjq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vev.pengpengdd.cyou

JS:   (3.14159).toFixed(2)
来源：http://miy.tianlin.xyz

TS:   (3.14159).toFixed(2)
来源：http://qko.ydjk.org.cn

Java: String.format("%.2f", 3.14159)
来源：http://jxs.fanxiaobao.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nsb.yuxming.cn

Ruby: format("%.2f", 3.14159)
来源：http://xam.yongpay.top

C#:   3.14159.ToString("F2")
来源：http://gmv.jiagoushi.top

[A22] 获取字符串长度
来源：http://cpk.guowangkeji.top

Py:   len(s)
来源：http://nxg.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jth.cqqwz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zcd.nwbrower.top

TS:   s.length
来源：http://min.zhijiandao.cn

Java: s.length()
来源：http://smp.pengpengdd.cyou

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fdi.nanxuanxn.top

Ruby: s.length
来源：http://idn.bjfxy.top

C#:   s.Length
来源：http://ucn.shanyushiyangtech.top

[A23] 大小写转换
来源：http://xos.ctjpmb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://mpj.dianchejie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://liv.ybcxt.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lep.nanxuanxn.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zqe.yj202588.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wnq.wangdashe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wpc.dashuyun.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://upv.mhx1999.top

C#:   s.ToUpper(); s.ToLower()
来源：http://iub.chenjidiqi.icu

[A24] 去除首尾空白
来源：http://bhi.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yhs.ydzc1.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mps.dianchejie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rjc.sxryk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://osx.zdbjq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ovf.guannengcc.top

Go:   strings.TrimSpace(s)
来源：http://jsf.shzxlz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lpx.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kds.zhaomingkeji.xyz

[A25] 字符串比较
来源：http://fft.jqgfzy.top

Py:   s1 == s2; s1 != s2
来源：http://nvm.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://psz.tianlin.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gwk.aizwys.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://psr.zhongyouzk.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qdx.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ksa.ctjpmb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ftr.feifeiyinyue.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tzd.9152youxi.cn

[A26] 类型转换总览
来源：http://ljm.yj202588.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xjl.nanxuanxn.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pto.snrcjt.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ldj.chenjidiqi.icu

TS:   Number() String() Boolean() x as number
来源：http://nvv.shangyingyoupin.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rpb.hongshengwenyu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xri.fengsongda.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wjs.jlsjyb.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nlc.shanyushiyangtech.top

================================================================================
来源：http://tyf.yonumen.top

B. 流程控制
来源：http://qbn.dashuyun.cn

================================================================================
来源：http://blb.ydzc1.top

[B01] 条件判断 if / else
来源：http://suz.yvedp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rum.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://owo.zhongyouzk.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dea.feifeiyinyue.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://keu.jianghu66.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jeq.guannengcc.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nan.pycfn.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nci.hnxiangtu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ocy.svipenyu.cn

[B02] 多分支 else if / elif
来源：http://gwo.pycfn.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lri.pycfn.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kct.fehbvm.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jqe.fanxiaobao.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iub.wangshuangyany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyq.yj202588.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mby.yvedp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nuh.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yqt.bbcook.cn

[B03] switch / match / case
来源：http://ksn.sysykeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sok.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fxy.316326.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hfp.daxiang520.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://all.xuetiantiany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mph.52xcode.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ubn.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://iri.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ovj.smart0.xyz

[B04] for 计数循环
来源：http://hzb.yangfankeji.com

Py:   for i in range(10): print(i)
来源：http://cse.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bvk.birdmap.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xwk.cheryme.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hiv.gogol.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nol.hfpthk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vhc.pycfn.com

Ruby: 10.times { |i| puts i }
来源：http://goi.ivvv.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ani.vqdsnc.cn

[B05] 遍历数组 / 列表
来源：http://jby.hcnkem.com

Py:   for item in arr: print(item)
来源：http://mbn.hysaishi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jyg.aizwys.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qaa.guowangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wrp.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fxx.fzhhl.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ztw.ydzc1.top

Ruby: arr.each { |item| puts item }
来源：http://xuk.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qcz.haohaochexian.top

[B06] 遍历字典 / 对象
来源：http://ymi.316326.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://paz.fzhhl.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jyq.smart0.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wph.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nnt.cheryme.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eku.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kbf.ywan-chungtsiang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ezf.wangdashe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dfr.daxiang520.top

[B07] while 循环
来源：http://xlt.jinqigfzy.top

Py:   while i < 10: i += 1
来源：http://kep.gzhubu.top

PHP:  while ($i < 10) { $i++; }
来源：http://col.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://akk.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://xvy.haohaochexian.top

Java: while (i < 10) { i++; }
来源：http://xcu.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wug.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://xgi.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://hwq.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://uyx.quarkkingdee.top

Py:   # 无 do-while：用 while True + break
来源：http://hmw.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nbg.zhaomingkeji.xyz

JS:   do { i++; } while (i < 10);
来源：http://qgp.xingfuxueyuan.xyz

TS:   do { i++; } while (i < 10);
来源：http://fbv.sweek.top

Java: do { i++; } while (i < 10);
来源：http://zig.aizwys.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fhb.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://xpe.jqgfzy.top

C#:   do { i++; } while (i < 10);
来源：http://guh.pengpengdd.cyou

[B09] break 与 continue
来源：http://her.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wmn.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jyx.aibaodan.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://boa.yueranfly.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tpf.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rzc.tanke756.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vai.xinyue.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bhq.uphjek.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xko.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://jwv.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rtf.c1oappe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sag.daxiang520.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://owc.jinqigufen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jbe.jinyuanbaomall.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fvj.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sse.pengpengdd.cyou

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ako.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jym.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://lnf.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://yxp.jinqigufen.top

PHP:  range(0, 10, 2);
来源：http://ryg.hywenlv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gbe.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://enh.dianchejie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xfo.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mmn.cqqwz.cn

Ruby: (0...10).step(2).to_a
来源：http://xtz.shanyushiyangtech.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uwf.andypj.xyz

[B12] 跳出多层循环
来源：http://tjk.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vxe.gaohongyu789.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://spr.kuanghao11.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qsj.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vfc.zhijiandao.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wjf.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tjq.zdqjudy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nki.ywan-chungtsiang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ayi.zdbjq.cn

[B13] 判断是否为数字
来源：http://whi.yuanzhike.top

Py:   isinstance(x, (int, float))
来源：http://eis.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://rvo.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jhz.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jjs.52xcode.cn

Java: x instanceof Number
来源：http://xhm.gaohongyu789.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://arm.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://flt.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://bsi.jianghu66.top

[B14] 判断值是否在集合内
来源：http://mby.chenzaomai.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fhj.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pns.nwbrower.top

JS:   [1, 2, 3].includes(x)
来源：http://rih.yongpay.top

TS:   [1, 2, 3].includes(x)
来源：http://bdu.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://nun.vqdsnc.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hog.jyoumei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rql.ctjpmb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://byf.ctjpmb.com

[B15] 布尔运算与取反
来源：http://qmb.guowangkeji.top

Py:   a and b or not c
来源：http://whn.jinqigufen.top

PHP:  $a && $b || !$c
来源：http://lmv.fengsongda.top

JS:   a && b || !c
来源：http://lmo.316326.xyz

TS:   a && b || !c
来源：http://rbg.birdmap.top

Java: a && b || !c
来源：http://cin.ehwqpu.com

Go:   a && b || !c
来源：http://rkd.kuanghao11.cn

Ruby: a && b || !c
来源：http://cbo.zhoulong.xyz

C#:   a && b || !c
来源：http://abz.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lpw.zycfv.cn

Py:   if not data: return
来源：http://nbl.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://tqz.birdmap.top

JS:   if (!data) return;
来源：http://ujf.hnqzz.top

TS:   if (!data) return;
来源：http://wmk.zhixingplan.top

Java: if (data == null) return;
来源：http://gvw.birdmap.top

Go:   if data == nil { return }
来源：http://lvm.hcnkem.com

Ruby: return if data.nil?
来源：http://nzi.guannengcc.top

C#:   if (data == null) return;
来源：http://egg.hammf.cn

================================================================================
来源：http://njz.chenjidiqi.icu

C. 函数与作用域
来源：http://yhq.zdbjq.cn

================================================================================
来源：http://etl.meibo888.top

[C01] 定义函数
来源：http://rvl.shangyingyoupin.top

Py:   def add(a, b): return a + b
来源：http://ogx.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iee.hesvh.cn

JS:   function add(a, b) { return a + b; }
来源：http://dad.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gow.jiagoushi.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sqc.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://krq.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://rob.svipenyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tmh.jqgufenzy.top

[C02] 默认参数
来源：http://ros.zhixingplan.top

Py:   def greet(name="World"): return name
来源：http://wgz.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cij.cheryme.top

JS:   function greet(name = "World") { return name; }
来源：http://mwx.redwolf501.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fts.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ucy.ppjwa.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hbb.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://bad.wangshuangyany.cn

C#:   string Greet(string name = "World") => name;
来源：http://qfu.cashguo.top

[C03] 可变参数
来源：http://xzo.zhijiandao.cn

Py:   def total(*args): return sum(args)
来源：http://ckm.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oje.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mbm.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gar.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vwf.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cqc.jqgufenzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://qfl.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rbs.ivvv.top

[C04] 命名参数 / 关键字参数
来源：http://eln.shzxlz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://orb.xuanzx.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hqf.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wze.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xqi.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://mcw.yj20258888.top

Go:   // 无：用配置结构体参数
来源：http://erl.xuetiantiany.cn

Ruby: f(a: 1, b: 2)
来源：http://fky.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://crv.tian-w.cn

[C05] 返回多个值
来源：http://ewu.guowangkeji.top

Py:   return a, b
来源：http://pnu.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://fzj.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lwz.xingfuxueyuan.xyz

TS:   return { a, b };
来源：http://xjk.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ptf.hesvh.cn

Go:   return a, b
来源：http://rya.ydjk.org.cn

Ruby: return a, b
来源：http://acx.uphjek.com

C#:   return (a, b);              // ValueTuple
来源：http://ern.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://bwf.zhongyouzk.top

Py:   square = lambda x: x * x
来源：http://thq.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pyu.aibaodan.cn

JS:   const square = x => x * x;
来源：http://vfe.fehbvm.com

TS:   const square = (x: number): number => x * x;
来源：http://cls.316326.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ovf.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://ubw.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://ixb.cashguo.top

C#:   Func<int, int> square = x => x * x;
来源：http://mpv.cucudq.cn

[C07] 把函数作为参数传入
来源：http://nja.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cmp.pycfn.com

PHP:  array_map("strtoupper", $arr);
来源：http://gvu.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hio.nwbrower.top

TS:   arr.map(String)
来源：http://khg.meibo888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aav.redwolf501.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rww.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://snc.hongshengwenyu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://irl.meibo888.top

[C08] 闭包
来源：http://xwk.tanke756.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ggb.ppjwa.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yjj.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://spm.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nnr.gaohongyu789.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gih.pycfn.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lco.guowangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kro.yfazqb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aoq.gaohongyu789.top

[C09] 递归
来源：http://zhj.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nzk.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wsz.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pxs.meibo888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gci.jiagoushi.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sgw.hywenlv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ben.zdbjq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://leu.tarul.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://amx.yj20258.top

[C10] 变量作用域
来源：http://lvc.chenlongwang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jvo.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://srn.zhengqikj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fod.kuanghao11.cn

TS:   同 JS
来源：http://rvd.quarkkingdee.top

Java: 方法内为块级作用域
来源：http://oku.cdnleiting.top

Go:   花括号块级作用域
来源：http://vjc.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wtc.xylfe.cn

C#:   块级作用域
来源：http://pmn.yanxiufei.cn

[C11] 模块导入与导出
来源：http://ymf.uphjek.com

Py:   from module import func
来源：http://iau.shanyushiyangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sgq.yj20258888.top


<!-- 参考信息 -->