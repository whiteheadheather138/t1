代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://rgj.zhengqikj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://neb.zhixingplan.top

TS:   // Node.js：readline 模块
来源：http://qgu.ywan-chungtsiang.top

Java: new Scanner(System.in).nextLine()
来源：http://ktr.dianchejie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rdo.hnqzz.top

Ruby: gets.chomp
来源：http://fqn.tian-w.cn

C#:   Console.ReadLine();
来源：http://xex.sysykeji.top

[A21] 保留指定小数位输出
来源：http://nnp.dianchejie.cn

Py:   f"{3.14159:.2f}"
来源：http://vvl.jlsjyb.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jta.jqgfzy.top

JS:   (3.14159).toFixed(2)
来源：http://aaz.dashuyun.cn

TS:   (3.14159).toFixed(2)
来源：http://fmr.zhixingplan.top

Java: String.format("%.2f", 3.14159)
来源：http://ksd.yvedp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ovc.gaohongyu789.top

Ruby: format("%.2f", 3.14159)
来源：http://mtr.xylfe.cn

C#:   3.14159.ToString("F2")
来源：http://xzf.yj20258.top

[A22] 获取字符串长度
来源：http://urx.jianghu66.top

Py:   len(s)
来源：http://kyr.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gtl.svipenyu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hew.hesvh.cn

TS:   s.length
来源：http://izl.yfazqb.com

Java: s.length()
来源：http://kvt.iojbl.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pey.yj20258.top

Ruby: s.length
来源：http://fta.mhx1999.top

C#:   s.Length
来源：http://mef.hongshengwenyu.top

[A23] 大小写转换
来源：http://gcg.yj20258.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hma.jyoumei.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ald.dashuyun.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jlw.epnwcf.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oce.gotoacloud.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uhr.birdmap.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ozk.nanxinkj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fqs.tarul.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nua.zdqjudy.top

[A24] 去除首尾空白
来源：http://rhc.yvedp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ppq.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zwc.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qwu.zhixingplan.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sub.fzhhl.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wdj.cdnleiting.top

Go:   strings.TrimSpace(s)
来源：http://vue.fanxiaobao.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mus.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ibk.yonumen.top

[A25] 字符串比较
来源：http://dam.hcnkem.com

Py:   s1 == s2; s1 != s2
来源：http://knt.snrcjt.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uon.yvedp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eoq.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ukk.gzhubu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://maw.ppjwa.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wbj.xingfuxueyuan.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://zcm.chenjidiqi.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hlc.fanxiaobao.xyz

[A26] 类型转换总览
来源：http://xlo.zhiwuduotai.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lvo.316326.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yfm.uphjek.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ncl.wangshuangyany.cn

TS:   Number() String() Boolean() x as number
来源：http://iwk.jinghuilouyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eun.sysykeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gsk.aibaodan.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bmw.hfpthk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lte.yvedp.cn

================================================================================
来源：http://kjp.zdbjq.cn

B. 流程控制
来源：http://aot.sweek.top

================================================================================
来源：http://gsq.yfazqb.com

[B01] 条件判断 if / else
来源：http://onv.birdmap.top

Py:   result = "正" if x > 0 else "非正"
来源：http://flb.c1oappe.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://edg.zdqjudy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tmn.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://afd.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bdi.yj202588.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jos.fktsv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nvr.smart0.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vga.ydjk.org.cn

[B02] 多分支 else if / elif
来源：http://lsl.shanyushiyangtech.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qmf.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://svj.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tff.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wwr.zhijiandao.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tei.zdqjudy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bnf.sjlbkw.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mft.tarul.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gsn.9152youxi.cn

[B03] switch / match / case
来源：http://kcu.gzhubu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gam.jinghuilouyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://inc.hysaishi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ubz.hammf.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://duy.nanxuanxn.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zyy.jinyuanbaomall.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://con.fengsongda.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ebr.ppjwa.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pcf.9152youxi.cn

[B04] for 计数循环
来源：http://jpn.hongshengwenyu.top

Py:   for i in range(10): print(i)
来源：http://jez.jianghu66.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jev.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ezb.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hnh.bjfxy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hcq.ppjwa.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cbr.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://ayc.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ojl.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://csu.yanxiufei.cn

Py:   for item in arr: print(item)
来源：http://dti.sweek.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://stw.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zra.hnxiangtu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tvh.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://avf.shuidangran.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xoo.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://ede.jyoumei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pon.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://oco.ppjwa.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vpw.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://olj.smart0.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wsw.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qik.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oiq.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jae.tianlin.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xwj.aibaodan.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bqw.meibo888.top

[B07] while 循环
来源：http://pzr.zhiwuduotai.top

Py:   while i < 10: i += 1
来源：http://kwq.gogol.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bov.chenjidiqi.icu

JS:   while (i < 10) { i++; }
来源：http://dsm.andypj.xyz

TS:   while (i < 10) { i++; }
来源：http://zge.aizwys.cn

Java: while (i < 10) { i++; }
来源：http://bhq.tarul.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eqi.tian-w.cn

Ruby: while i < 10; i += 1; end
来源：http://wqs.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://hvi.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://kmu.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://qgx.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://gwh.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://pdc.wangdashe.top

TS:   do { i++; } while (i < 10);
来源：http://cyh.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://lsb.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tld.xuetiantiany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ktn.zhoulong.xyz

C#:   do { i++; } while (i < 10);
来源：http://kfj.jinqigfzy.top

[B09] break 与 continue
来源：http://dvk.yj20258888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rul.zdqjudy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pkg.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uhp.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://imt.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ovh.nanxinkj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://avd.shanyushiyangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cgx.zhixingplan.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kxf.shanyushiyangtech.top

[B10] 遍历同时拿索引
来源：http://cta.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jgg.xuanzx.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jbi.gogol.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mxs.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cal.yfazqb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ocf.cucudq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yme.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hak.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dbn.sweek.top

[B11] 生成数字序列 / 区间
来源：http://nzd.jinqigfzy.top

Py:   list(range(0, 10, 2))
来源：http://bss.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://twv.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wci.yanxiufei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ord.hfpthk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://exe.iojbl.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://moh.jianghu66.top

Ruby: (0...10).step(2).to_a
来源：http://imq.xylfe.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://moz.c1oappe.top

[B12] 跳出多层循环
来源：http://hft.cheryme.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ioo.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vic.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dcx.shuidangran.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ajk.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kwq.ivvv.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gyv.jinqigfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ztt.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://swq.wangshuangyany.cn

[B13] 判断是否为数字
来源：http://wrt.ehwqpu.com

Py:   isinstance(x, (int, float))
来源：http://qda.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://bgk.shanyushiyangtech.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ggr.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uxd.ybcxt.top

Java: x instanceof Number
来源：http://gzi.zhijiandao.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yxr.cheryme.top

Ruby: x.is_a?(Numeric)
来源：http://cyj.vehdjk.com

C#:   x is int or double or decimal
来源：http://cga.fktsv.cn

[B14] 判断值是否在集合内
来源：http://suf.zdbjq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yoh.zhongyouzk.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dey.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://yql.yuanzhike.top

TS:   [1, 2, 3].includes(x)
来源：http://ytm.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bnb.vqdsnc.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qji.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pnt.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rai.vehdjk.com

[B15] 布尔运算与取反
来源：http://vtf.jiagoushi.top

Py:   a and b or not c
来源：http://nqc.fzhhl.top

PHP:  $a && $b || !$c
来源：http://vpf.ydzc1.top

JS:   a && b || !c
来源：http://puy.sysykeji.top

TS:   a && b || !c
来源：http://cso.zhaomingkeji.xyz

Java: a && b || !c
来源：http://jwa.hysaishi.cn

Go:   a && b || !c
来源：http://yek.zycfv.cn

Ruby: a && b || !c
来源：http://nhb.gzhubu.top

C#:   a && b || !c
来源：http://biz.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://jbc.tanke756.top

Py:   if not data: return
来源：http://imm.yj20258888.top

PHP:  if (!$data) { return; }
来源：http://dfo.redwolf501.top

JS:   if (!data) return;
来源：http://pyg.zhixingplan.top

TS:   if (!data) return;
来源：http://jen.sufxvd.cn

Java: if (data == null) return;
来源：http://jti.hammf.cn

Go:   if data == nil { return }
来源：http://tew.yfazqb.com

Ruby: return if data.nil?
来源：http://qcn.jianghu66.top

C#:   if (data == null) return;
来源：http://ydt.hnxiangtu.top

================================================================================
来源：http://fex.yuanzhike.top

C. 函数与作用域
来源：http://tzk.aizwys.cn

================================================================================
来源：http://duz.fehbvm.com

[C01] 定义函数
来源：http://lwr.wangshuangyany.cn

Py:   def add(a, b): return a + b
来源：http://lgr.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ktt.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://lkw.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zjg.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://myh.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bpi.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://ohq.zhiwuduotai.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dnm.ehwqpu.com

[C02] 默认参数
来源：http://fex.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://qci.xuanzx.com

PHP:  function greet($name = "World") { return $name; }
来源：http://til.tianlin.xyz

JS:   function greet(name = "World") { return name; }
来源：http://bod.cucudq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lyd.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://esy.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://akw.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://qvo.ehwqpu.com

C#:   string Greet(string name = "World") => name;
来源：http://vpo.zhoulong.xyz

[C03] 可变参数
来源：http://bqu.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://gyy.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qyd.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hgm.zhiwuduotai.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jfj.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kza.yvedp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tgj.gzhubu.top

Ruby: def total(*nums); nums.sum; end
来源：http://ayr.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xrp.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://dea.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rfn.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dll.uphjek.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iil.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qob.cheryme.top

Java: // 无：用 Builder 模式或 record
来源：http://rnc.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://rkv.hongshengwenyu.top

Ruby: f(a: 1, b: 2)
来源：http://wtk.c1oappe.top

C#:   f(a: 1, b: 2)
来源：http://dtp.ybcxt.top

[C05] 返回多个值
来源：http://vik.uphjek.com

Py:   return a, b
来源：http://oel.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://qwk.chenlongwang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kca.zhijiandao.cn

TS:   return { a, b };
来源：http://qmg.zhiwuduotai.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xgu.cashguo.top

Go:   return a, b
来源：http://zex.c1oappe.top

Ruby: return a, b
来源：http://sya.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://dwn.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://aln.xziqi.cn

Py:   square = lambda x: x * x
来源：http://lwz.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xup.epnwcf.com

JS:   const square = x => x * x;
来源：http://hfo.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://daw.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pdy.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://yse.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://nho.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://nqe.jinghuilouyu.cn

[C07] 把函数作为参数传入
来源：http://zon.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hfl.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://mbp.guannengcc.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wqh.tanke756.top

TS:   arr.map(String)
来源：http://cny.sysykeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kse.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://obm.daria6918.cn

Ruby: arr.map(&:upcase)
来源：http://eue.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mbr.feifeiyinyue.top

[C08] 闭包
来源：http://uwd.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rwu.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://igk.yj20258.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sit.hongshengwenyu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lhi.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bdl.yonumen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fvb.c1oappe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ljr.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aub.ctjpmb.com

[C09] 递归
来源：http://pvu.yj20258.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bnq.ivvv.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xug.xuetiantiany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pth.aibaodan.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eil.chenjidiqi.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bop.0kj1m.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gug.shanyushiyangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ikm.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vne.gogol.net.cn

[C10] 变量作用域
来源：http://pfs.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zsr.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jmf.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wyz.shuidangran.top

TS:   同 JS
来源：http://iwh.epnwcf.com

Java: 方法内为块级作用域
来源：http://ixt.iojbl.cn

Go:   花括号块级作用域
来源：http://gwp.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hbp.zhengqikj.top


<!-- 参考信息 -->