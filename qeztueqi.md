代发 wailian999

JS:   [a, b] = [b, a];
来源：http://rxa.xylfe.cn

TS:   [a, b] = [b, a];
来源：http://elp.dashuyun.cn

Java: int t = a; a = b; b = t;
来源：http://qac.redwolf501.top

Go:   a, b = b, a
来源：http://xyc.iojbl.cn

Ruby: a, b = b, a
来源：http://lnr.c1oappe.top

C#:   (a, b) = (b, a);
来源：http://nfe.yueranfly.top

[A20] 读取标准输入
来源：http://yav.guannengcc.top

Py:   name = input("请输入：")
来源：http://vsv.jinyuanbaomall.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nzm.xziqi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ihb.pycfn.com

TS:   // Node.js：readline 模块
来源：http://ovm.zhiwuduotai.top

Java: new Scanner(System.in).nextLine()
来源：http://wiu.shangyingyoupin.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jay.cheryme.top

Ruby: gets.chomp
来源：http://ejz.andypj.xyz

C#:   Console.ReadLine();
来源：http://csp.kuanghao11.cn

[A21] 保留指定小数位输出
来源：http://xop.yvedp.cn

Py:   f"{3.14159:.2f}"
来源：http://zxq.hysaishi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tnj.316326.xyz

JS:   (3.14159).toFixed(2)
来源：http://cma.mhx1999.top

TS:   (3.14159).toFixed(2)
来源：http://ner.yanxiufei.cn

Java: String.format("%.2f", 3.14159)
来源：http://hzg.9152youxi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eha.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://bqb.tarul.cn

C#:   3.14159.ToString("F2")
来源：http://kti.ctjpmb.com

[A22] 获取字符串长度
来源：http://tbw.bbcook.cn

Py:   len(s)
来源：http://tpg.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pxo.jinyuanbaomall.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lil.epnwcf.com

TS:   s.length
来源：http://aap.gaohongyu789.top

Java: s.length()
来源：http://ngb.shangyingyoupin.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eqd.cucudq.cn

Ruby: s.length
来源：http://vrm.c1oappe.top

C#:   s.Length
来源：http://hyc.9152youxi.cn

[A23] 大小写转换
来源：http://gzv.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://laq.zdbjq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uxv.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://whc.pycfn.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jox.wangshuangyany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kbr.smart0.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fgq.yvedp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://guy.meibo888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://adz.cucudq.cn

[A24] 去除首尾空白
来源：http://atl.tianlin.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oyk.yfazqb.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fds.tarul.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vma.316326.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qyo.guowangkeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yme.ybcxt.top

Go:   strings.TrimSpace(s)
来源：http://jqi.gotoacloud.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qny.vehdjk.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gjg.ybcxt.top

[A25] 字符串比较
来源：http://lrv.9152youxi.cn

Py:   s1 == s2; s1 != s2
来源：http://rqd.cqqwz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oht.cdnleiting.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hnj.cqqwz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fwy.yangfankeji.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fnn.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://meg.zhaomingkeji.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://iwh.cheryme.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nmy.hnxiangtu.top

[A26] 类型转换总览
来源：http://clp.cashguo.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pct.xylfe.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ide.pycfn.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://txi.fanxiaobao.xyz

TS:   Number() String() Boolean() x as number
来源：http://psp.shanyushiyangtech.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://akw.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://umq.cashguo.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tyf.tianlin.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kkl.hesvh.cn

================================================================================
来源：http://wgt.zhiwuduotai.top

B. 流程控制
来源：http://xiv.nanxinkj.top

================================================================================
来源：http://hml.sjlbkw.cn

[B01] 条件判断 if / else
来源：http://hqr.pengpengdd.cyou

Py:   result = "正" if x > 0 else "非正"
来源：http://wor.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://anj.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nmp.yj20258.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fgr.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dtg.fehbvm.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mjk.cucudq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://los.zycfv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fml.zhixingplan.top

[B02] 多分支 else if / elif
来源：http://fvi.shanyushiyangtech.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gml.chenjidiqi.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rvf.yueranfly.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jyh.cqqwz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pxz.zycfv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbl.yj20258.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://auu.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://crl.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://auw.zhengqikj.top

[B03] switch / match / case
来源：http://vxm.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hbh.sufxvd.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uhu.ybcxt.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tni.mhx1999.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yav.gaohongyu789.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ndg.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uje.quarkkingdee.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ymg.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lfw.jinqigufen.top

[B04] for 计数循环
来源：http://zmr.chenzaomai.com

Py:   for i in range(10): print(i)
来源：http://bdv.cheryme.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hdb.hcnkem.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fev.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zqt.hnqzz.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fef.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ipk.ehwqpu.com

Ruby: 10.times { |i| puts i }
来源：http://ehh.birdmap.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yhn.xziqi.cn

[B05] 遍历数组 / 列表
来源：http://edn.tian-w.cn

Py:   for item in arr: print(item)
来源：http://ebe.ctjpmb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ddl.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jik.nwbrower.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ahz.gogol.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://oya.smart0.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zij.kuanghao11.cn

Ruby: arr.each { |item| puts item }
来源：http://fph.cqqwz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yfw.uphjek.com

[B06] 遍历字典 / 对象
来源：http://xzp.fengsongda.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tfv.nanxuanxn.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cod.gogol.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://axi.52xcode.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cie.hfpthk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gzg.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://czn.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://riv.zhengqikj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eys.yj20258.top

[B07] while 循环
来源：http://syb.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://sdi.yuanzhike.top

PHP:  while ($i < 10) { $i++; }
来源：http://aup.yueranfly.top

JS:   while (i < 10) { i++; }
来源：http://crr.sxryk.cn

TS:   while (i < 10) { i++; }
来源：http://byb.ivvv.top

Java: while (i < 10) { i++; }
来源：http://qkf.yonumen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://roj.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://hjh.snrcjt.cn

C#:   while (i < 10) { i++; }
来源：http://idc.vehdjk.com

[B08] do-while（至少执行一次）
来源：http://acm.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://frp.cqqwz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hmk.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://ibr.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://gmy.epnwcf.com

Java: do { i++; } while (i < 10);
来源：http://jmg.zhongyouzk.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bxy.dianchejie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bku.ybcxt.top

C#:   do { i++; } while (i < 10);
来源：http://edl.zhengqikj.top

[B09] break 与 continue
来源：http://tde.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dem.shanyushiyangtech.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zaw.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xde.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zlr.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uwo.hcnkem.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://itp.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gwx.yueranfly.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zmr.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://sfk.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yrz.zhiwuduotai.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mwg.xinyue.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qxo.ybcxt.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qxz.hesvh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fgm.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dwr.pycfn.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://urh.nanxuanxn.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nwx.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://fnf.gaohongyu789.top

Py:   list(range(0, 10, 2))
来源：http://wex.chenlongwang.top

PHP:  range(0, 10, 2);
来源：http://yfq.epnwcf.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hym.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://msf.jqgfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oiq.sjlbkw.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dij.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://wem.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tym.dashuyun.cn

[B12] 跳出多层循环
来源：http://nal.havefunace.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hxj.chenzaomai.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://lkn.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tfo.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://efr.bjfxy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xzq.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xep.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pzm.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://syx.quarkkingdee.top

[B13] 判断是否为数字
来源：http://ugz.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://qlv.zycfv.cn

PHP:  is_numeric($x)
来源：http://dvk.feifeiyinyue.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ghc.zycfv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://svt.c1oappe.top

Java: x instanceof Number
来源：http://fqp.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cqe.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://fnv.gogol.net.cn

C#:   x is int or double or decimal
来源：http://lsc.sysykeji.top

[B14] 判断值是否在集合内
来源：http://odn.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aud.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eqy.yanxiufei.cn

JS:   [1, 2, 3].includes(x)
来源：http://cbr.hysaishi.cn

TS:   [1, 2, 3].includes(x)
来源：http://zrg.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://wgk.shuidangran.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yxk.ydzc1.top

Ruby: [1, 2, 3].include?(x)
来源：http://iki.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jit.feifeiyinyue.top

[B15] 布尔运算与取反
来源：http://zdo.zhaomingkeji.xyz

Py:   a and b or not c
来源：http://rnw.guannengcc.top

PHP:  $a && $b || !$c
来源：http://jhp.pycfn.com

JS:   a && b || !c
来源：http://chk.hysaishi.cn

TS:   a && b || !c
来源：http://dfa.sxryk.cn

Java: a && b || !c
来源：http://vjn.xylfe.cn

Go:   a && b || !c
来源：http://liu.aizwys.cn

Ruby: a && b || !c
来源：http://nfv.cashguo.top

C#:   a && b || !c
来源：http://rks.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jxd.daxiang520.top

Py:   if not data: return
来源：http://ojr.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://ruh.iojbl.cn

JS:   if (!data) return;
来源：http://lqc.yonumen.top

TS:   if (!data) return;
来源：http://pjl.hysaishi.cn

Java: if (data == null) return;
来源：http://euz.pycfn.com

Go:   if data == nil { return }
来源：http://swh.sxryk.cn

Ruby: return if data.nil?
来源：http://tbl.pengpengdd.cyou

C#:   if (data == null) return;
来源：http://mym.yanxiufei.cn

================================================================================
来源：http://bun.shzxlz.cn

C. 函数与作用域
来源：http://ehi.yonumen.top

================================================================================
来源：http://uha.mhx1999.top

[C01] 定义函数
来源：http://vov.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://mfl.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hfu.hcnkem.com

JS:   function add(a, b) { return a + b; }
来源：http://lit.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oip.sxryk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zhm.gotoacloud.top

Go:   func add(a, b int) int { return a + b }
来源：http://xfy.hnxiangtu.top

Ruby: def add(a, b); a + b; end
来源：http://inw.yj202588.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://umf.fanxiaobao.xyz

[C02] 默认参数
来源：http://yya.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://kmu.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nqp.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://rgh.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://oyc.yj202588.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ozk.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pji.epnwcf.com

Ruby: def greet(name = "World") = name
来源：http://lfq.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://uqy.ydzc1.top

[C03] 可变参数
来源：http://ies.fanxiaobao.xyz

Py:   def total(*args): return sum(args)
来源：http://vjm.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oqo.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vog.yuxming.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iav.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://goa.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jhe.zycfv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bxn.chenzaomai.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bzq.daxiang520.top

[C04] 命名参数 / 关键字参数
来源：http://jhh.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://txd.tanke756.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bop.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kvq.aizwys.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://etw.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://ppi.vqdsnc.cn

Go:   // 无：用配置结构体参数
来源：http://xlg.jqgfzy.top

Ruby: f(a: 1, b: 2)
来源：http://dil.yvedp.cn

C#:   f(a: 1, b: 2)
来源：http://prl.pycfn.com

[C05] 返回多个值
来源：http://vpv.pengpengdd.cyou

Py:   return a, b
来源：http://oyd.zycfv.cn

PHP:  return [$a, $b];
来源：http://wch.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://udm.dianchejie.cn

TS:   return { a, b };
来源：http://iem.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pyw.yj20258.top

Go:   return a, b
来源：http://cqa.jqgfzy.top

Ruby: return a, b
来源：http://cqf.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://mgv.shangyingyoupin.top

[C06] 匿名函数 / lambda
来源：http://wby.yonumen.top

Py:   square = lambda x: x * x
来源：http://aiq.meibo888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://juh.yj20258888.top

JS:   const square = x => x * x;
来源：http://ogs.zhaomingkeji.xyz

TS:   const square = (x: number): number => x * x;
来源：http://inz.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wpr.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bdq.fehbvm.com

Ruby: square = ->(x) { x * x }
来源：http://dyf.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hrs.zdbjq.cn

[C07] 把函数作为参数传入
来源：http://psc.pycfn.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cdz.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://ykm.yongpay.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mmr.shanyushiyangkeji.top

TS:   arr.map(String)
来源：http://awg.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://elg.kuanghao11.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hxx.hongshengwenyu.top

Ruby: arr.map(&:upcase)
来源：http://bgp.zdbjq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vfl.hfpthk.cn

[C08] 闭包
来源：http://vtf.yj202588.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bcz.shuidangran.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xzb.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vor.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://llg.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://txh.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wjg.jyoumei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uqv.daria6918.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xjw.jyoumei.cn

[C09] 递归
来源：http://psa.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tbm.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ryi.andypj.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mgl.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ugs.andypj.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qsv.xuanzx.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nky.aibaodan.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tzg.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fkb.zhijiandao.cn


<!-- 参考信息 -->