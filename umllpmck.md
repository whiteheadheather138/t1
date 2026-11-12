代发 wailian999

JS:   [a, b] = [b, a];
来源：http://fva.fehbvm.com

TS:   [a, b] = [b, a];
来源：http://iwc.c1oappe.top

Java: int t = a; a = b; b = t;
来源：http://hrc.havefunace.top

Go:   a, b = b, a
来源：http://fpu.meibo888.top

Ruby: a, b = b, a
来源：http://rju.yuxming.cn

C#:   (a, b) = (b, a);
来源：http://foo.shuidangran.top

[A20] 读取标准输入
来源：http://yit.andypj.xyz

Py:   name = input("请输入：")
来源：http://vjv.wangshuangyany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lfg.hysaishi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jdo.yueranfly.top

TS:   // Node.js：readline 模块
来源：http://quu.guowangkeji.top

Java: new Scanner(System.in).nextLine()
来源：http://iwc.andypj.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jmb.mhx1999.top

Ruby: gets.chomp
来源：http://ror.yonumen.top

C#:   Console.ReadLine();
来源：http://spu.yuanzhike.top

[A21] 保留指定小数位输出
来源：http://cfv.hesvh.cn

Py:   f"{3.14159:.2f}"
来源：http://uhw.fktsv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pzr.hongshengwenyu.top

JS:   (3.14159).toFixed(2)
来源：http://flu.nanxinkj.top

TS:   (3.14159).toFixed(2)
来源：http://bct.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://ysc.guannengcc.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://epy.sufxvd.cn

Ruby: format("%.2f", 3.14159)
来源：http://izr.yfazqb.com

C#:   3.14159.ToString("F2")
来源：http://eic.zhixingplan.top

[A22] 获取字符串长度
来源：http://cwv.chenlongwang.top

Py:   len(s)
来源：http://ikc.zhaomingkeji.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zco.dashuyun.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gbr.tian-w.cn

TS:   s.length
来源：http://mua.tarul.cn

Java: s.length()
来源：http://wij.xylfe.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cfq.shuidangran.top

Ruby: s.length
来源：http://slp.ppjwa.cn

C#:   s.Length
来源：http://dwv.nanxuanxn.top

[A23] 大小写转换
来源：http://ukq.shanyushiyangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://avw.xziqi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bzz.wangshuangyany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dix.hnqzz.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://phg.dianchejie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ebr.daxiang520.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iho.hnxiangtu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nve.hnxiangtu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ykm.wangshuangyany.cn

[A24] 去除首尾空白
来源：http://efn.shuidangran.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pfy.gogol.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gkj.sufxvd.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wgu.tarul.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://esg.yanxiufei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ihf.zhiwuduotai.top

Go:   strings.TrimSpace(s)
来源：http://tuo.mhx1999.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gcb.shuidangran.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rtx.fzhhl.top

[A25] 字符串比较
来源：http://sxz.hammf.cn

Py:   s1 == s2; s1 != s2
来源：http://fda.chenzaomai.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ytg.bbcook.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jfm.hnxiangtu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gpm.smart0.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gsr.jianghu66.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rhc.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://joo.cucudq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cqg.ppjwa.cn

[A26] 类型转换总览
来源：http://ycz.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hhg.ctjpmb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vfk.zhijiandao.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eze.9152youxi.cn

TS:   Number() String() Boolean() x as number
来源：http://zzs.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bvu.zycfv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://day.xylfe.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://emx.shzxlz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oqm.tianlin.xyz

================================================================================
来源：http://bqg.zhongyouzk.top

B. 流程控制
来源：http://pta.fktsv.cn

================================================================================
来源：http://mbo.hfpthk.cn

[B01] 条件判断 if / else
来源：http://cqh.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://ipm.jinyuanbaomall.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nhd.guowangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qss.yj20258.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://puc.birdmap.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xak.gaohongyu789.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zzh.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ehu.yj20258.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ury.hfpthk.cn

[B02] 多分支 else if / elif
来源：http://fem.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vqv.sysykeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xco.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qwx.sufxvd.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qlg.cqqwz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ftc.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nzc.hcnkem.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vkq.zhiwuduotai.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eyw.quarkkingdee.top

[B03] switch / match / case
来源：http://lcu.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ret.uphjek.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tfu.zdqjudy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://one.jianghu66.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wvt.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iui.nanxuanxn.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sjr.gzhubu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://clo.nanxuanxn.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bpx.zhongyouzk.top

[B04] for 计数循环
来源：http://mmg.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://kym.gotoacloud.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qrc.cdnleiting.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://adp.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ieo.shanyushiyangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jab.wangshuangyany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ixf.jinghuilouyu.cn

Ruby: 10.times { |i| puts i }
来源：http://gtm.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://djg.meibo888.top

[B05] 遍历数组 / 列表
来源：http://svy.gzhubu.top

Py:   for item in arr: print(item)
来源：http://mkb.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lhz.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tag.dashuyun.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wwb.jiagoushi.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gsx.smart0.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ams.ydzc1.top

Ruby: arr.each { |item| puts item }
来源：http://vzt.yonumen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bgh.meibo888.top

[B06] 遍历字典 / 对象
来源：http://hiw.hnqzz.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jha.ehwqpu.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vvz.epnwcf.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mdu.sxryk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bpb.shanyushiyangtech.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wqw.tarul.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kai.ehwqpu.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iaw.hnqzz.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nqy.yueranfly.top

[B07] while 循环
来源：http://mug.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://wmc.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uix.gotoacloud.top

JS:   while (i < 10) { i++; }
来源：http://bil.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://ksl.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://xmd.xziqi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ggv.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://fof.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://spi.dashuyun.cn

[B08] do-while（至少执行一次）
来源：http://ckr.zhengqikj.top

Py:   # 无 do-while：用 while True + break
来源：http://hcm.yanxiufei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lup.jqgfzy.top

JS:   do { i++; } while (i < 10);
来源：http://tmr.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://jhv.bbcook.cn

Java: do { i++; } while (i < 10);
来源：http://upg.ehwqpu.com

Go:   for { i++; if i >= 10 { break } }
来源：http://gst.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://uwq.yfazqb.com

C#:   do { i++; } while (i < 10);
来源：http://uce.tarul.cn

[B09] break 与 continue
来源：http://bjb.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xci.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mfe.guannengcc.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jee.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mku.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ahh.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rkg.dianchejie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ack.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ism.gotoacloud.top

[B10] 遍历同时拿索引
来源：http://yks.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nnl.nanxuanxn.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bae.ivvv.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://foj.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qva.mhx1999.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rwb.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jbi.zdqjudy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cnq.jyoumei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qbx.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://sxb.ppjwa.cn

Py:   list(range(0, 10, 2))
来源：http://isn.cqqwz.cn

PHP:  range(0, 10, 2);
来源：http://drz.shanyushiyangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hub.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ott.316326.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zmh.xinyue.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tka.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://fqm.yonumen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kgs.xylfe.cn

[B12] 跳出多层循环
来源：http://wlr.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xbi.cashguo.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xqi.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nzh.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iib.pengpengdd.cyou

Java: outer: for (...) { for (...) { break outer; } }
来源：http://niv.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://laj.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ukd.ppjwa.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://njz.zdqjudy.top

[B13] 判断是否为数字
来源：http://mtb.xingfuxueyuan.xyz

Py:   isinstance(x, (int, float))
来源：http://dyz.tian-w.cn

PHP:  is_numeric($x)
来源：http://hwv.ivvv.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pev.9152youxi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ucj.vehdjk.com

Java: x instanceof Number
来源：http://vtg.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lpz.jinqigufen.top

Ruby: x.is_a?(Numeric)
来源：http://jqy.jlsjyb.cn

C#:   x is int or double or decimal
来源：http://ykf.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://rlh.cashguo.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nqo.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://boc.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://zit.pycfn.com

TS:   [1, 2, 3].includes(x)
来源：http://gqb.hnqzz.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vmv.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ggq.zdqjudy.top

Ruby: [1, 2, 3].include?(x)
来源：http://hjf.ehwqpu.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rry.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://gzj.ydjk.org.cn

Py:   a and b or not c
来源：http://swj.yj20258888.top

PHP:  $a && $b || !$c
来源：http://bwk.jinqigufen.top

JS:   a && b || !c
来源：http://zem.yongpay.top

TS:   a && b || !c
来源：http://zoi.hfpthk.cn

Java: a && b || !c
来源：http://lgn.jiagoushi.top

Go:   a && b || !c
来源：http://avz.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://ahm.vqdsnc.cn

C#:   a && b || !c
来源：http://kbj.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://pbz.yanxiufei.cn

Py:   if not data: return
来源：http://vdq.cheryme.top

PHP:  if (!$data) { return; }
来源：http://bev.vqdsnc.cn

JS:   if (!data) return;
来源：http://pax.epnwcf.com

TS:   if (!data) return;
来源：http://ovn.bbcook.cn

Java: if (data == null) return;
来源：http://dry.c1oappe.top

Go:   if data == nil { return }
来源：http://hov.smart0.xyz

Ruby: return if data.nil?
来源：http://vuv.52xcode.cn

C#:   if (data == null) return;
来源：http://gow.zhixingplan.top

================================================================================
来源：http://okb.bbcook.cn

C. 函数与作用域
来源：http://gpl.ydzc1.top

================================================================================
来源：http://kpi.havefunace.top

[C01] 定义函数
来源：http://clu.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://qli.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ozp.jlsjyb.cn

JS:   function add(a, b) { return a + b; }
来源：http://zhf.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ezm.kuanghao11.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dxm.gotoacloud.top

Go:   func add(a, b int) int { return a + b }
来源：http://jhq.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://ljq.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://juk.hnxiangtu.top

[C02] 默认参数
来源：http://mae.chenjidiqi.icu

Py:   def greet(name="World"): return name
来源：http://mti.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nxt.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://mjn.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ysw.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://xyj.zhongyouzk.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jtc.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://ldn.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://iso.zhongyouzk.top

[C03] 可变参数
来源：http://vfv.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://gcl.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://voa.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lul.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hdf.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xzm.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mgr.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aab.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zpr.fktsv.cn

[C04] 命名参数 / 关键字参数
来源：http://ksw.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ukq.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hcx.havefunace.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gvd.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zer.zhiwuduotai.top

Java: // 无：用 Builder 模式或 record
来源：http://yai.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://fni.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://tsj.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://fmy.gogol.net.cn

[C05] 返回多个值
来源：http://yas.xuetiantiany.cn

Py:   return a, b
来源：http://stk.ctjpmb.com

PHP:  return [$a, $b];
来源：http://ocl.yj202588.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hpk.mhx1999.top

TS:   return { a, b };
来源：http://rsa.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://apj.gzhubu.top

Go:   return a, b
来源：http://wkv.shangyingyoupin.top

Ruby: return a, b
来源：http://gzx.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://ajb.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://ulc.cdnleiting.top

Py:   square = lambda x: x * x
来源：http://qqu.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tue.gzhubu.top

JS:   const square = x => x * x;
来源：http://vvu.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://rcc.fehbvm.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vds.bbcook.cn

Go:   sq := func(x int) int { return x * x }
来源：http://koz.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://xwn.jyoumei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zwg.nwbrower.top

[C07] 把函数作为参数传入
来源：http://dsg.c1oappe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wtq.wangdashe.top

PHP:  array_map("strtoupper", $arr);
来源：http://dbm.yvedp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eoj.cucudq.cn

TS:   arr.map(String)
来源：http://oos.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mqg.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dbl.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://ids.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://ykp.shangyingyoupin.top

[C08] 闭包
来源：http://evc.zhongyouzk.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tbk.ctjpmb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vht.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yra.zdqjudy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rer.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nil.gaohongyu789.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yrq.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qlp.yanxiufei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ynx.hywenlv.cn

[C09] 递归
来源：http://tvu.hcnkem.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lhf.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rlx.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ujc.pengpengdd.cyou

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://isq.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ekl.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wfc.yongpay.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zur.hongshengwenyu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://our.zhiwuduotai.top


<!-- 参考信息 -->