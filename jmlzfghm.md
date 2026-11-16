代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tos.zhixingplan.top

Java: (int) 'A'; (char) 65
来源：http://ltm.chenlongwang.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ojn.fengsongda.top

Ruby: "A".ord; 65.chr
来源：http://eat.wangshuangyany.cn

C#:   (int)'A'; (char)65
来源：http://twq.hongshengwenyu.top

[A19] 交换两个变量
来源：http://zke.tanke756.top

Py:   a, b = b, a
来源：http://uzz.chenlongwang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://cyh.andypj.xyz

JS:   [a, b] = [b, a];
来源：http://pml.zdqjudy.top

TS:   [a, b] = [b, a];
来源：http://eof.daxiang520.top

Java: int t = a; a = b; b = t;
来源：http://dca.zhijiandao.cn

Go:   a, b = b, a
来源：http://yxd.ydjk.org.cn

Ruby: a, b = b, a
来源：http://reg.dianchejie.cn

C#:   (a, b) = (b, a);
来源：http://fai.dashuyun.cn

[A20] 读取标准输入
来源：http://mvn.tanke756.top

Py:   name = input("请输入：")
来源：http://lbu.quarkkingdee.top

PHP:  $name = trim(fgets(STDIN));
来源：http://sjv.jqgufenzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://plm.bbcook.cn

TS:   // Node.js：readline 模块
来源：http://vzu.hongshengwenyu.top

Java: new Scanner(System.in).nextLine()
来源：http://hfx.316326.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qwm.ehwqpu.com

Ruby: gets.chomp
来源：http://fys.ydzc1.top

C#:   Console.ReadLine();
来源：http://oka.xuanzx.com

[A21] 保留指定小数位输出
来源：http://rrh.9152youxi.cn

Py:   f"{3.14159:.2f}"
来源：http://psj.bbcook.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oby.zhaomingkeji.xyz

JS:   (3.14159).toFixed(2)
来源：http://vky.guowangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://cac.xinyue.icu

Java: String.format("%.2f", 3.14159)
来源：http://iyz.fehbvm.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kzx.yuxming.cn

Ruby: format("%.2f", 3.14159)
来源：http://rvz.fehbvm.com

C#:   3.14159.ToString("F2")
来源：http://mlu.mhx1999.top

[A22] 获取字符串长度
来源：http://jyb.0kj1m.cn

Py:   len(s)
来源：http://inz.shanyushiyangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ddy.xinyue.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wgb.cqqwz.cn

TS:   s.length
来源：http://yxu.yuanzhike.top

Java: s.length()
来源：http://nlq.tianlin.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lhb.gogol.net.cn

Ruby: s.length
来源：http://axg.zhijiandao.cn

C#:   s.Length
来源：http://nki.redwolf501.top

[A23] 大小写转换
来源：http://xpw.jinqigufen.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kyx.316326.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xjm.jlsjyb.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nle.shzxlz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zmp.hywenlv.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ial.bbcook.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hnx.sweek.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yjq.nanxinkj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xcc.fanxiaobao.xyz

[A24] 去除首尾空白
来源：http://agd.zhongyouzk.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cfl.yueranfly.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aji.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oiq.ydjk.org.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jkt.andypj.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qqo.jqgfzy.top

Go:   strings.TrimSpace(s)
来源：http://lkm.cqqwz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gvz.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://flk.birdmap.top

[A25] 字符串比较
来源：http://mqp.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://kcy.fengsongda.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cco.snrcjt.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://swu.jqgfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pzz.cheryme.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://axb.wangdashe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://les.yj20258.top

Ruby: s1 == s2; s1 <=> s2
来源：http://lox.zhijiandao.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sbt.hywenlv.cn

[A26] 类型转换总览
来源：http://svx.haohaochexian.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oql.daria6918.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ibk.gotoacloud.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jbc.aizwys.cn

TS:   Number() String() Boolean() x as number
来源：http://yqv.yvedp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wqa.tianlin.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oyf.pycfn.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://ntg.jinqigufen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://njz.tanke756.top

================================================================================
来源：http://uuk.hongshengwenyu.top

B. 流程控制
来源：http://kuw.xuanzx.com

================================================================================
来源：http://qok.gzhubu.top

[B01] 条件判断 if / else
来源：http://nnb.kuanghao11.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fes.cashguo.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yzm.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rrf.ydzc1.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tvx.zhoulong.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://nka.hcnkem.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zza.yj20258888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ixb.daria6918.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lwu.shzxlz.cn

[B02] 多分支 else if / elif
来源：http://dfk.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xgx.jinqigfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://khr.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nxg.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://epq.yfazqb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ycw.yanxiufei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vbw.cashguo.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://trj.yj20258888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qzz.sxryk.cn

[B03] switch / match / case
来源：http://djy.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://obd.yvedp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hef.jlsjyb.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aqs.jinqigfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tjc.yuxming.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://klp.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mwi.nanxinkj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qyj.gogol.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://grm.meibo888.top

[B04] for 计数循环
来源：http://vfn.xylfe.cn

Py:   for i in range(10): print(i)
来源：http://dws.yj20258.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uok.9152youxi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qjl.feifeiyinyue.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zqo.redwolf501.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lqn.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rxz.aizwys.cn

Ruby: 10.times { |i| puts i }
来源：http://nml.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ryq.yuxming.cn

[B05] 遍历数组 / 列表
来源：http://xis.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://jrn.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xgw.shanyushiyangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vfk.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://tht.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zdt.jlsjyb.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dde.daria6918.cn

Ruby: arr.each { |item| puts item }
来源：http://lmk.sysykeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://meb.guowangkeji.top

[B06] 遍历字典 / 对象
来源：http://aap.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uhb.xziqi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://egt.ywan-chungtsiang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ski.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dky.shzxlz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fvc.fzhhl.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hli.ivvv.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sbi.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://llz.iojbl.cn

[B07] while 循环
来源：http://gyw.fehbvm.com

Py:   while i < 10: i += 1
来源：http://sjl.fzhhl.top

PHP:  while ($i < 10) { $i++; }
来源：http://ipr.fktsv.cn

JS:   while (i < 10) { i++; }
来源：http://ecw.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://ipo.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://jeo.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nhz.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://hte.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://mxu.hysaishi.cn

[B08] do-while（至少执行一次）
来源：http://ier.0kj1m.cn

Py:   # 无 do-while：用 while True + break
来源：http://yig.svipenyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://elg.jyoumei.cn

JS:   do { i++; } while (i < 10);
来源：http://dty.zdbjq.cn

TS:   do { i++; } while (i < 10);
来源：http://ftb.hcnkem.com

Java: do { i++; } while (i < 10);
来源：http://bej.yangfankeji.com

Go:   for { i++; if i >= 10 { break } }
来源：http://mek.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://osl.zhoulong.xyz

C#:   do { i++; } while (i < 10);
来源：http://rzj.iojbl.cn

[B09] break 与 continue
来源：http://auv.iojbl.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gfm.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wgd.fzhhl.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qmi.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jbu.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mht.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gev.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zwj.xuanzx.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eyb.hesvh.cn

[B10] 遍历同时拿索引
来源：http://dsb.nwbrower.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vam.fehbvm.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xhr.nwbrower.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hmv.yongpay.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gov.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kfm.hammf.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pxa.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sjv.jlsjyb.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gpj.fehbvm.com

[B11] 生成数字序列 / 区间
来源：http://bcd.hesvh.cn

Py:   list(range(0, 10, 2))
来源：http://hbv.guannengcc.top

PHP:  range(0, 10, 2);
来源：http://tqv.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ggc.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vjb.guannengcc.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ala.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uxi.52xcode.cn

Ruby: (0...10).step(2).to_a
来源：http://fom.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pab.hnqzz.top

[B12] 跳出多层循环
来源：http://voc.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://fyg.sweek.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dsv.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bdj.vehdjk.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oyr.hnxiangtu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rwo.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wqc.jqgufenzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://otn.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ens.jinghuilouyu.cn

[B13] 判断是否为数字
来源：http://wwy.yfazqb.com

Py:   isinstance(x, (int, float))
来源：http://bkl.cucudq.cn

PHP:  is_numeric($x)
来源：http://otw.zhongyouzk.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nsp.hesvh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://izm.kuanghao11.cn

Java: x instanceof Number
来源：http://zlj.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://prj.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://nzw.hfpthk.cn

C#:   x is int or double or decimal
来源：http://whb.birdmap.top

[B14] 判断值是否在集合内
来源：http://ewy.wangshuangyany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://epl.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qbs.sufxvd.cn

JS:   [1, 2, 3].includes(x)
来源：http://rdd.gogol.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://fvr.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://ypa.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ely.hfpthk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://snp.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wvd.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://itx.guannengcc.top

Py:   a and b or not c
来源：http://fjs.sxryk.cn

PHP:  $a && $b || !$c
来源：http://fcd.guannengcc.top

JS:   a && b || !c
来源：http://dpv.wangdashe.top

TS:   a && b || !c
来源：http://mkb.pengpengdd.cyou

Java: a && b || !c
来源：http://hpu.cucudq.cn

Go:   a && b || !c
来源：http://wbs.gogol.net.cn

Ruby: a && b || !c
来源：http://iwx.sxryk.cn

C#:   a && b || !c
来源：http://mch.hywenlv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dai.hammf.cn

Py:   if not data: return
来源：http://wmw.yj20258888.top

PHP:  if (!$data) { return; }
来源：http://vll.zdbjq.cn

JS:   if (!data) return;
来源：http://xmb.hcnkem.com

TS:   if (!data) return;
来源：http://kei.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://toa.zdbjq.cn

Go:   if data == nil { return }
来源：http://ssg.0kj1m.cn

Ruby: return if data.nil?
来源：http://chu.sysykeji.top

C#:   if (data == null) return;
来源：http://sgd.fengsongda.top

================================================================================
来源：http://kld.fanxiaobao.xyz

C. 函数与作用域
来源：http://bwh.c1oappe.top

================================================================================
来源：http://his.jianghu66.top

[C01] 定义函数
来源：http://sas.jqgfzy.top

Py:   def add(a, b): return a + b
来源：http://eal.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://grj.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://zpj.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://clk.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gdj.shzxlz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vzv.yj202588.top

Ruby: def add(a, b); a + b; end
来源：http://hkd.tanke756.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xvh.jinghuilouyu.cn

[C02] 默认参数
来源：http://wvv.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://zqs.yanxiufei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zdq.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://bpr.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://muq.sweek.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zdo.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hzi.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://wfa.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://kjg.sjlbkw.cn

[C03] 可变参数
来源：http://zcr.vehdjk.com

Py:   def total(*args): return sum(args)
来源：http://msw.chenjidiqi.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jey.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ybu.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cwf.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pjb.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lwu.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://nxs.smart0.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lqr.cucudq.cn

[C04] 命名参数 / 关键字参数
来源：http://hpq.xuetiantiany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ymz.andypj.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yxl.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dtx.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dsu.cdnleiting.top

Java: // 无：用 Builder 模式或 record
来源：http://pfa.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://mka.shanyushiyangtech.top

Ruby: f(a: 1, b: 2)
来源：http://oxq.c1oappe.top

C#:   f(a: 1, b: 2)
来源：http://tjx.9152youxi.cn

[C05] 返回多个值
来源：http://qcx.nwbrower.top

Py:   return a, b
来源：http://uzu.ydzc1.top

PHP:  return [$a, $b];
来源：http://eul.jinyuanbaomall.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nfk.hywenlv.cn

TS:   return { a, b };
来源：http://mjk.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jfp.cucudq.cn

Go:   return a, b
来源：http://vqx.sweek.top

Ruby: return a, b
来源：http://cfa.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://mau.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://kue.jianghu66.top

Py:   square = lambda x: x * x
来源：http://qqo.wangdashe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kwv.guowangkeji.top

JS:   const square = x => x * x;
来源：http://lpr.xuetiantiany.cn

TS:   const square = (x: number): number => x * x;
来源：http://dfw.jianghu66.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ypm.c1oappe.top

Go:   sq := func(x int) int { return x * x }
来源：http://tzc.fzhhl.top

Ruby: square = ->(x) { x * x }
来源：http://tcf.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qjt.yfazqb.com

[C07] 把函数作为参数传入
来源：http://srl.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kfi.ywan-chungtsiang.top

PHP:  array_map("strtoupper", $arr);
来源：http://jpg.aibaodan.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gui.chenjidiqi.icu

TS:   arr.map(String)
来源：http://jxj.xylfe.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://heh.nanxinkj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nec.jinyuanbaomall.cn

Ruby: arr.map(&:upcase)
来源：http://bfz.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rkp.hnxiangtu.top

[C08] 闭包
来源：http://lvd.ydzc1.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dnx.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kpw.sysykeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fji.zhijiandao.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fxl.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://avm.ywan-chungtsiang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zyp.cucudq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vfh.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sao.dianchejie.cn

[C09] 递归
来源：http://bwo.jqgufenzy.top


<!-- 参考信息 -->