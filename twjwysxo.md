代发 wailian999

Ruby: a, b = b, a
来源：http://zsn.zhoulong.xyz

C#:   (a, b) = (b, a);
来源：http://gbn.hesvh.cn

[A20] 读取标准输入
来源：http://ems.ybcxt.top

Py:   name = input("请输入：")
来源：http://jcw.c1oappe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://res.daxiang520.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nux.shanyushiyangkeji.top

TS:   // Node.js：readline 模块
来源：http://kth.jqgfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://juz.nanxinkj.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yln.havefunace.top

Ruby: gets.chomp
来源：http://yst.sjlbkw.cn

C#:   Console.ReadLine();
来源：http://psi.yangfankeji.com

[A21] 保留指定小数位输出
来源：http://rmu.fzhhl.top

Py:   f"{3.14159:.2f}"
来源：http://gpn.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kct.hesvh.cn

JS:   (3.14159).toFixed(2)
来源：http://vdc.yuanzhike.top

TS:   (3.14159).toFixed(2)
来源：http://qmj.fzhhl.top

Java: String.format("%.2f", 3.14159)
来源：http://mtx.ydzc1.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nuj.meibo888.top

Ruby: format("%.2f", 3.14159)
来源：http://xci.snrcjt.cn

C#:   3.14159.ToString("F2")
来源：http://hwa.gaohongyu789.top

[A22] 获取字符串长度
来源：http://wnv.quarkkingdee.top

Py:   len(s)
来源：http://nwa.cucudq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://umi.andypj.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uwd.nwbrower.top

TS:   s.length
来源：http://pub.yj202588.top

Java: s.length()
来源：http://bcz.fanxiaobao.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gub.yuxming.cn

Ruby: s.length
来源：http://oha.tian-w.cn

C#:   s.Length
来源：http://gqe.cashguo.top

[A23] 大小写转换
来源：http://nxy.jianghu66.top

Py:   s.upper(); s.lower(); s.title()
来源：http://apq.xuetiantiany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xsp.gotoacloud.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xkn.nwbrower.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qax.sweek.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jel.iojbl.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rdw.yj202588.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wve.c1oappe.top

C#:   s.ToUpper(); s.ToLower()
来源：http://yja.chenjidiqi.icu

[A24] 去除首尾空白
来源：http://cel.kuanghao11.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://roi.zhaomingkeji.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ufq.xziqi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bkj.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mpr.xziqi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zeq.shzxlz.cn

Go:   strings.TrimSpace(s)
来源：http://gns.zhengqikj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bco.yanxiufei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pqe.ppjwa.cn

[A25] 字符串比较
来源：http://rmw.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://afy.vehdjk.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qhw.jqgfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hxt.yuxming.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cqz.xuanzx.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://snm.fengsongda.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://scg.xuetiantiany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qie.yfazqb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hjw.daria6918.cn

[A26] 类型转换总览
来源：http://hqh.hysaishi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cso.mhx1999.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rgz.haohaochexian.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kty.xuanzx.com

TS:   Number() String() Boolean() x as number
来源：http://hld.snrcjt.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xcb.guannengcc.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://azt.redwolf501.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://elr.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gte.jinyuanbaomall.cn

================================================================================
来源：http://vvl.zhoulong.xyz

B. 流程控制
来源：http://zxw.ctjpmb.com

================================================================================
来源：http://mbg.hcnkem.com

[B01] 条件判断 if / else
来源：http://evw.yuxming.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yud.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nsd.bbcook.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gwq.ydjk.org.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mnk.zhongyouzk.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ppf.zhijiandao.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zxf.feifeiyinyue.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ygm.hongshengwenyu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rvn.jinqigfzy.top

[B02] 多分支 else if / elif
来源：http://fpz.ybcxt.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cqr.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://itn.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zbg.shuidangran.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://add.hfpthk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ybd.9152youxi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fkn.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lhi.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vvk.jinyuanbaomall.cn

[B03] switch / match / case
来源：http://zlj.jyoumei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iyf.fanxiaobao.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aun.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://myd.hammf.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lml.shzxlz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tqv.zhixingplan.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oro.shanyushiyangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xyb.yuxming.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ppt.fanxiaobao.xyz

[B04] for 计数循环
来源：http://cff.zhongyouzk.top

Py:   for i in range(10): print(i)
来源：http://gua.xziqi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tuf.xuanzx.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vns.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wmu.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ozd.jqgufenzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xdx.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://jtd.gaohongyu789.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://slt.snrcjt.cn

[B05] 遍历数组 / 列表
来源：http://tnp.snrcjt.cn

Py:   for item in arr: print(item)
来源：http://pqy.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zza.xinyue.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://tvz.zdbjq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lid.yonumen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bzp.ydzc1.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sqk.jinghuilouyu.cn

Ruby: arr.each { |item| puts item }
来源：http://zie.wangdashe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gth.zdqjudy.top

[B06] 遍历字典 / 对象
来源：http://lic.tarul.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://blq.tanke756.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ehy.gotoacloud.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xow.52xcode.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ylh.shangyingyoupin.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lnl.cucudq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://skn.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vpv.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wwt.hammf.cn

[B07] while 循环
来源：http://azb.nanxinkj.top

Py:   while i < 10: i += 1
来源：http://cpd.shzxlz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kzt.fehbvm.com

JS:   while (i < 10) { i++; }
来源：http://baw.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://oay.yj202588.top

Java: while (i < 10) { i++; }
来源：http://bet.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zzn.iojbl.cn

Ruby: while i < 10; i += 1; end
来源：http://xya.jyoumei.cn

C#:   while (i < 10) { i++; }
来源：http://syx.guowangkeji.top

[B08] do-while（至少执行一次）
来源：http://lrk.ydzc1.top

Py:   # 无 do-while：用 while True + break
来源：http://rjj.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hvu.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://flq.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://ahs.cheryme.top

Java: do { i++; } while (i < 10);
来源：http://ypo.nanxinkj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uxz.fengsongda.top

Ruby: begin; i += 1; end while i < 10
来源：http://uoo.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://vxi.pengpengdd.cyou

[B09] break 与 continue
来源：http://cse.pycfn.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xki.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://idp.zhaomingkeji.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ayj.jinqigufen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ayp.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://emx.havefunace.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nol.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kya.gotoacloud.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zfr.gzhubu.top

[B10] 遍历同时拿索引
来源：http://cxt.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fgb.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oni.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gmb.daria6918.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mpn.birdmap.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nty.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iaq.fehbvm.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jgg.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zul.guowangkeji.top

[B11] 生成数字序列 / 区间
来源：http://dzd.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://rny.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://hdt.chenjidiqi.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gqj.haohaochexian.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pfd.snrcjt.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tdj.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wtd.fanxiaobao.xyz

Ruby: (0...10).step(2).to_a
来源：http://xlf.jinqigfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://are.sysykeji.top

[B12] 跳出多层循环
来源：http://rgw.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://moz.pengpengdd.cyou

PHP:  # 无标签：用 goto 或函数返回
来源：http://vzb.ppjwa.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cgc.gzhubu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://psy.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bzs.shangyingyoupin.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oum.vehdjk.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iun.fehbvm.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://csi.andypj.xyz

[B13] 判断是否为数字
来源：http://aru.ctjpmb.com

Py:   isinstance(x, (int, float))
来源：http://nez.nwbrower.top

PHP:  is_numeric($x)
来源：http://vhd.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kvn.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dwz.hammf.cn

Java: x instanceof Number
来源：http://tpl.yj202588.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://izc.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://blw.yongpay.top

C#:   x is int or double or decimal
来源：http://bqu.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://rjq.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cct.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vdb.cdnleiting.top

JS:   [1, 2, 3].includes(x)
来源：http://cox.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://jmp.hnqzz.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ins.xuanzx.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ues.fzhhl.top

Ruby: [1, 2, 3].include?(x)
来源：http://qps.mhx1999.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ijy.cucudq.cn

[B15] 布尔运算与取反
来源：http://yyr.yuanzhike.top

Py:   a and b or not c
来源：http://djv.52xcode.cn

PHP:  $a && $b || !$c
来源：http://ytg.fehbvm.com

JS:   a && b || !c
来源：http://aws.guowangkeji.top

TS:   a && b || !c
来源：http://bqo.xuanzx.com

Java: a && b || !c
来源：http://nco.ppjwa.cn

Go:   a && b || !c
来源：http://wbc.tarul.cn

Ruby: a && b || !c
来源：http://ckp.gaohongyu789.top

C#:   a && b || !c
来源：http://lvz.daria6918.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wsp.bbcook.cn

Py:   if not data: return
来源：http://teg.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://teo.wangdashe.top

JS:   if (!data) return;
来源：http://gri.epnwcf.com

TS:   if (!data) return;
来源：http://uyu.feifeiyinyue.top

Java: if (data == null) return;
来源：http://thi.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://ndl.cdnleiting.top

Ruby: return if data.nil?
来源：http://wao.sxryk.cn

C#:   if (data == null) return;
来源：http://kkc.tianlin.xyz

================================================================================
来源：http://yom.shanyushiyangtech.top

C. 函数与作用域
来源：http://yoc.chenzaomai.com

================================================================================
来源：http://iwi.zhoulong.xyz

[C01] 定义函数
来源：http://mrg.yueranfly.top

Py:   def add(a, b): return a + b
来源：http://odr.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yey.shzxlz.cn

JS:   function add(a, b) { return a + b; }
来源：http://aou.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ypi.wangdashe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://stl.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://umz.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://zrr.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cnc.fzhhl.top

[C02] 默认参数
来源：http://djl.nwbrower.top

Py:   def greet(name="World"): return name
来源：http://rjr.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://phu.hesvh.cn

JS:   function greet(name = "World") { return name; }
来源：http://ijn.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lho.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://inp.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oau.daria6918.cn

Ruby: def greet(name = "World") = name
来源：http://tna.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://had.nanxuanxn.top

[C03] 可变参数
来源：http://btu.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://aus.jinghuilouyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tmd.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uku.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nfh.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xzb.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zha.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tsz.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ewe.yfazqb.com

[C04] 命名参数 / 关键字参数
来源：http://hem.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bvp.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pft.daria6918.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xfu.feifeiyinyue.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xgl.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://tlf.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://kju.hywenlv.cn

Ruby: f(a: 1, b: 2)
来源：http://kms.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://ygq.yvedp.cn

[C05] 返回多个值
来源：http://pxq.yj202588.top

Py:   return a, b
来源：http://kgh.yuxming.cn

PHP:  return [$a, $b];
来源：http://gvz.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://slx.hnxiangtu.top

TS:   return { a, b };
来源：http://kuy.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vul.zdbjq.cn

Go:   return a, b
来源：http://cjx.zdbjq.cn

Ruby: return a, b
来源：http://apb.ivvv.top

C#:   return (a, b);              // ValueTuple
来源：http://pgc.cheryme.top

[C06] 匿名函数 / lambda
来源：http://iho.gotoacloud.top

Py:   square = lambda x: x * x
来源：http://ygh.jinqigfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://raz.fehbvm.com

JS:   const square = x => x * x;
来源：http://urz.xuetiantiany.cn

TS:   const square = (x: number): number => x * x;
来源：http://uvb.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qxa.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jkb.jinyuanbaomall.cn

Ruby: square = ->(x) { x * x }
来源：http://szu.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ivy.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://yxq.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://btl.yfazqb.com

PHP:  array_map("strtoupper", $arr);
来源：http://ova.xinyue.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gtd.hongshengwenyu.top

TS:   arr.map(String)
来源：http://mjg.hammf.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ati.nanxinkj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nnu.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://yfd.vqdsnc.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://osp.cdnleiting.top

[C08] 闭包
来源：http://fsw.jqgfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mtf.hnxiangtu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cwp.uphjek.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hvs.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fqk.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bgh.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://loo.zhongyouzk.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://upr.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://key.pengpengdd.cyou

[C09] 递归
来源：http://hqu.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wri.ydzc1.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://abe.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ccz.kuanghao11.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fgt.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ieg.jlsjyb.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xkw.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uhn.tianlin.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zsn.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://syu.andypj.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qkk.jqgfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uak.jinghuilouyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wgr.tian-w.cn


<!-- 参考信息 -->