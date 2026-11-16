代发 wailian999

JS:   [a, b] = [b, a];
来源：http://glt.uphjek.com

TS:   [a, b] = [b, a];
来源：http://rhs.hammf.cn

Java: int t = a; a = b; b = t;
来源：http://jpl.0kj1m.cn

Go:   a, b = b, a
来源：http://vko.chenjidiqi.icu

Ruby: a, b = b, a
来源：http://igp.hongshengwenyu.top

C#:   (a, b) = (b, a);
来源：http://tpz.tianlin.xyz

[A20] 读取标准输入
来源：http://kyi.gotoacloud.top

Py:   name = input("请输入：")
来源：http://ciw.xylfe.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dwp.yvedp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vlt.cqqwz.cn

TS:   // Node.js：readline 模块
来源：http://ayd.9152youxi.cn

Java: new Scanner(System.in).nextLine()
来源：http://azd.hcnkem.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hde.zhaomingkeji.xyz

Ruby: gets.chomp
来源：http://bkh.ybcxt.top

C#:   Console.ReadLine();
来源：http://siw.ppjwa.cn

[A21] 保留指定小数位输出
来源：http://pyk.ehwqpu.com

Py:   f"{3.14159:.2f}"
来源：http://kpp.daxiang520.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xbx.chenjidiqi.icu

JS:   (3.14159).toFixed(2)
来源：http://evd.yj20258888.top

TS:   (3.14159).toFixed(2)
来源：http://spr.jinghuilouyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://vfe.hywenlv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pow.pycfn.com

Ruby: format("%.2f", 3.14159)
来源：http://thq.jinqigfzy.top

C#:   3.14159.ToString("F2")
来源：http://vim.ydzc1.top

[A22] 获取字符串长度
来源：http://qte.dashuyun.cn

Py:   len(s)
来源：http://fth.bjfxy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jem.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kbp.dianchejie.cn

TS:   s.length
来源：http://smf.hammf.cn

Java: s.length()
来源：http://zio.yuanzhike.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ulh.hongshengwenyu.top

Ruby: s.length
来源：http://oyy.cashguo.top

C#:   s.Length
来源：http://suj.dianchejie.cn

[A23] 大小写转换
来源：http://qti.ydzc1.top

Py:   s.upper(); s.lower(); s.title()
来源：http://iem.c1oappe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rdz.hywenlv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qpj.guannengcc.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iog.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qgj.quarkkingdee.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yld.zhengqikj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vzv.zhengqikj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bkp.epnwcf.com

[A24] 去除首尾空白
来源：http://kuw.nwbrower.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mey.gaohongyu789.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xrk.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pgr.xinyue.icu

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://drt.sxryk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://edn.ppjwa.cn

Go:   strings.TrimSpace(s)
来源：http://fuo.ctjpmb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dsc.yvedp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eqg.andypj.xyz

[A25] 字符串比较
来源：http://odh.hammf.cn

Py:   s1 == s2; s1 != s2
来源：http://uxs.gotoacloud.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mjv.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://flb.xziqi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mvo.yonumen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kpi.shanyushiyangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://goq.fanxiaobao.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://kiv.cqqwz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ipu.wangdashe.top

[A26] 类型转换总览
来源：http://gvg.feifeiyinyue.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yre.guannengcc.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://itp.snrcjt.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uog.jlsjyb.cn

TS:   Number() String() Boolean() x as number
来源：http://jap.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fik.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blz.vqdsnc.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dcr.pycfn.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nnx.ydzc1.top

================================================================================
来源：http://wkx.nanxuanxn.top

B. 流程控制
来源：http://hws.hcnkem.com

================================================================================
来源：http://bfi.daxiang520.top

[B01] 条件判断 if / else
来源：http://ypb.hesvh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qnl.hcnkem.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wgu.fehbvm.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nzw.hongshengwenyu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ckg.c1oappe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nxa.kuanghao11.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ozd.birdmap.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jiv.havefunace.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hwx.jqgufenzy.top

[B02] 多分支 else if / elif
来源：http://qfg.aizwys.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fdk.zhiwuduotai.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kce.52xcode.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cwt.bjfxy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qpb.aibaodan.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ovy.zhoulong.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ggs.yonumen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://izp.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gci.zhixingplan.top

[B03] switch / match / case
来源：http://kgu.daxiang520.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cue.cheryme.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yye.xziqi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ebp.gzhubu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nlt.hnxiangtu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bdj.zhongyouzk.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gsu.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hob.hnqzz.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xxx.c1oappe.top

[B04] for 计数循环
来源：http://ztx.jyoumei.cn

Py:   for i in range(10): print(i)
来源：http://stq.52xcode.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tjh.ywan-chungtsiang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wxu.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wrm.gotoacloud.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tfo.ivvv.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rtk.vqdsnc.cn

Ruby: 10.times { |i| puts i }
来源：http://smm.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wbw.xuetiantiany.cn

[B05] 遍历数组 / 列表
来源：http://ldx.hnqzz.top

Py:   for item in arr: print(item)
来源：http://spb.birdmap.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dkb.yuxming.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://opi.jlsjyb.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dvt.zhijiandao.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xky.shuidangran.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kgl.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://lzc.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vgv.zhoulong.xyz

[B06] 遍历字典 / 对象
来源：http://bdh.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://btm.guowangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zni.bbcook.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uft.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://spr.chenzaomai.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mgo.9152youxi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oft.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yqe.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lym.kuanghao11.cn

[B07] while 循环
来源：http://nul.gzhubu.top

Py:   while i < 10: i += 1
来源：http://kaf.vehdjk.com

PHP:  while ($i < 10) { $i++; }
来源：http://kfp.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://khw.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://gyu.xziqi.cn

Java: while (i < 10) { i++; }
来源：http://lwk.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dkl.fanxiaobao.xyz

Ruby: while i < 10; i += 1; end
来源：http://lct.tian-w.cn

C#:   while (i < 10) { i++; }
来源：http://qyu.tanke756.top

[B08] do-while（至少执行一次）
来源：http://fqw.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://jox.fanxiaobao.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://wfq.daria6918.cn

JS:   do { i++; } while (i < 10);
来源：http://pme.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://evc.zhengqikj.top

Java: do { i++; } while (i < 10);
来源：http://ljo.guowangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nqj.9152youxi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pft.daria6918.cn

C#:   do { i++; } while (i < 10);
来源：http://bex.haohaochexian.top

[B09] break 与 continue
来源：http://kzi.jqgufenzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ajm.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fcb.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yzx.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iil.zhixingplan.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hbo.cashguo.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://svj.fehbvm.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rqf.xylfe.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jyg.fehbvm.com

[B10] 遍历同时拿索引
来源：http://gcq.dashuyun.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hhu.jlsjyb.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ovi.tian-w.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dut.havefunace.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mzk.zhongyouzk.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ksj.zhaomingkeji.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xpd.fehbvm.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://onh.yongpay.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ufa.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://znn.feifeiyinyue.top

Py:   list(range(0, 10, 2))
来源：http://ppn.quarkkingdee.top

PHP:  range(0, 10, 2);
来源：http://thu.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oua.aibaodan.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qjc.jinqigfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ueu.hnqzz.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://owk.jinqigufen.top

Ruby: (0...10).step(2).to_a
来源：http://sym.jinqigufen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://thh.sjlbkw.cn

[B12] 跳出多层循环
来源：http://ohq.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mzc.shangyingyoupin.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://iti.quarkkingdee.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://slj.cucudq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pgj.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tjd.hongshengwenyu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tgb.fzhhl.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gmy.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hsa.ehwqpu.com

[B13] 判断是否为数字
来源：http://xmo.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://uur.gogol.net.cn

PHP:  is_numeric($x)
来源：http://vux.iojbl.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://trj.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rdk.xinyue.icu

Java: x instanceof Number
来源：http://ykw.zhengqikj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vco.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://qxi.wangdashe.top

C#:   x is int or double or decimal
来源：http://fmv.shuidangran.top

[B14] 判断值是否在集合内
来源：http://ayi.gotoacloud.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eew.cashguo.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gpq.shanyushiyangtech.top

JS:   [1, 2, 3].includes(x)
来源：http://zum.hcnkem.com

TS:   [1, 2, 3].includes(x)
来源：http://nnt.cqqwz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://old.hammf.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cme.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://tyh.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pkp.fehbvm.com

[B15] 布尔运算与取反
来源：http://ofl.316326.xyz

Py:   a and b or not c
来源：http://upr.kuanghao11.cn

PHP:  $a && $b || !$c
来源：http://zgz.daria6918.cn

JS:   a && b || !c
来源：http://cbf.cucudq.cn

TS:   a && b || !c
来源：http://qbe.jinqigufen.top

Java: a && b || !c
来源：http://ksi.zhengqikj.top

Go:   a && b || !c
来源：http://kuu.iojbl.cn

Ruby: a && b || !c
来源：http://wku.aizwys.cn

C#:   a && b || !c
来源：http://bfu.wangdashe.top

[B16] 卫语句：不满足条件提前返回
来源：http://xmv.yj20258888.top

Py:   if not data: return
来源：http://cmu.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://tgf.ehwqpu.com

JS:   if (!data) return;
来源：http://muc.iojbl.cn

TS:   if (!data) return;
来源：http://kck.jinqigfzy.top

Java: if (data == null) return;
来源：http://ecz.zhengqikj.top

Go:   if data == nil { return }
来源：http://aim.mhx1999.top

Ruby: return if data.nil?
来源：http://irk.jinyuanbaomall.cn

C#:   if (data == null) return;
来源：http://mnb.nanxuanxn.top

================================================================================
来源：http://jar.hfpthk.cn

C. 函数与作用域
来源：http://fyz.xziqi.cn

================================================================================
来源：http://wdj.ehwqpu.com

[C01] 定义函数
来源：http://tyw.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://aor.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fmu.quarkkingdee.top

JS:   function add(a, b) { return a + b; }
来源：http://kvh.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lbs.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://avc.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nyt.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://zvk.zhongyouzk.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://shm.zdbjq.cn

[C02] 默认参数
来源：http://cah.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://swp.tanke756.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jmw.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://fdz.9152youxi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zmh.pycfn.com

Java: // 无默认参数：方法重载或 Optional
来源：http://nqb.daria6918.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qtz.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://evb.vehdjk.com

C#:   string Greet(string name = "World") => name;
来源：http://jfa.meibo888.top

[C03] 可变参数
来源：http://vei.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://vzo.jinyuanbaomall.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nhc.tanke756.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wpn.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wrf.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xyn.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://epz.fehbvm.com

Ruby: def total(*nums); nums.sum; end
来源：http://viz.aizwys.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://azr.quarkkingdee.top

[C04] 命名参数 / 关键字参数
来源：http://mol.xziqi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cwj.sysykeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mhb.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://slm.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qxq.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://hdy.sysykeji.top

Go:   // 无：用配置结构体参数
来源：http://xhz.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://txi.ydjk.org.cn

C#:   f(a: 1, b: 2)
来源：http://sle.aibaodan.cn

[C05] 返回多个值
来源：http://vbs.bbcook.cn

Py:   return a, b
来源：http://ykr.cheryme.top

PHP:  return [$a, $b];
来源：http://ijh.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uhv.kuanghao11.cn

TS:   return { a, b };
来源：http://gug.zdbjq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yxx.yj202588.top

Go:   return a, b
来源：http://nkx.chenzaomai.com

Ruby: return a, b
来源：http://pmp.jiagoushi.top

C#:   return (a, b);              // ValueTuple
来源：http://uii.hnqzz.top

[C06] 匿名函数 / lambda
来源：http://xtw.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://pub.uphjek.com

PHP:  $square = fn($x) => $x * $x;
来源：http://hzr.ybcxt.top

JS:   const square = x => x * x;
来源：http://fos.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://rhj.zhengqikj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://btk.hfpthk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qnp.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://dvr.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nhg.jinqigfzy.top

[C07] 把函数作为参数传入
来源：http://zbg.epnwcf.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tcy.hammf.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hnf.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eyg.meibo888.top

TS:   arr.map(String)
来源：http://pqo.shanyushiyangtech.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nrf.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://frh.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://qxo.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://otv.nanxuanxn.top

[C08] 闭包
来源：http://jmk.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yus.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pfx.chenzaomai.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ayg.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vph.jianghu66.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://atr.jinghuilouyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rrj.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xzd.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ktb.feifeiyinyue.top

[C09] 递归
来源：http://ypg.guannengcc.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ldl.xinyue.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xgm.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qhh.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://keq.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zyn.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ina.hcnkem.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iio.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sbw.ydzc1.top


<!-- 参考信息 -->