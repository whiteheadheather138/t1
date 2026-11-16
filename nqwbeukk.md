代发 wailian999

Ruby: a, b = b, a
来源：http://rmn.yfazqb.com

C#:   (a, b) = (b, a);
来源：http://jki.xuanzx.com

[A20] 读取标准输入
来源：http://zey.yangfankeji.com

Py:   name = input("请输入：")
来源：http://upw.sxryk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pif.fanxiaobao.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iyw.yuanzhike.top

TS:   // Node.js：readline 模块
来源：http://luz.sjlbkw.cn

Java: new Scanner(System.in).nextLine()
来源：http://spr.cheryme.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eho.meibo888.top

Ruby: gets.chomp
来源：http://fwi.ehwqpu.com

C#:   Console.ReadLine();
来源：http://ees.hysaishi.cn

[A21] 保留指定小数位输出
来源：http://sio.wangdashe.top

Py:   f"{3.14159:.2f}"
来源：http://gxn.jlsjyb.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xsk.bbcook.cn

JS:   (3.14159).toFixed(2)
来源：http://mcc.jinqigfzy.top

TS:   (3.14159).toFixed(2)
来源：http://mrs.hesvh.cn

Java: String.format("%.2f", 3.14159)
来源：http://pas.chenzaomai.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hzj.svipenyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://isj.hysaishi.cn

C#:   3.14159.ToString("F2")
来源：http://nyo.fzhhl.top

[A22] 获取字符串长度
来源：http://nvx.wangdashe.top

Py:   len(s)
来源：http://loy.ybcxt.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hkc.yueranfly.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bwv.zdqjudy.top

TS:   s.length
来源：http://tul.hfpthk.cn

Java: s.length()
来源：http://xnw.hongshengwenyu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fxl.52xcode.cn

Ruby: s.length
来源：http://xts.fehbvm.com

C#:   s.Length
来源：http://hkz.yuanzhike.top

[A23] 大小写转换
来源：http://uzv.svipenyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://upb.meibo888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bji.jinyuanbaomall.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ggz.vqdsnc.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eup.yj20258.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wcc.xziqi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wsc.guowangkeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mte.jqgufenzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xwn.uphjek.com

[A24] 去除首尾空白
来源：http://sve.ivvv.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lhv.chenjidiqi.icu

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cgw.jinqigfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ndt.ppjwa.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mfm.xylfe.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iuq.nanxuanxn.top

Go:   strings.TrimSpace(s)
来源：http://igo.jianghu66.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xpi.xuetiantiany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://red.tianlin.xyz

[A25] 字符串比较
来源：http://ydr.meibo888.top

Py:   s1 == s2; s1 != s2
来源：http://jlc.ywan-chungtsiang.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ofy.quarkkingdee.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ywj.wangshuangyany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pzc.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tng.svipenyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xej.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vyx.yvedp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://neg.jianghu66.top

[A26] 类型转换总览
来源：http://glv.dianchejie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ybz.yueranfly.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mew.yangfankeji.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://haw.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://lpt.0kj1m.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ecf.zhongyouzk.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vdh.nanxuanxn.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dga.cashguo.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ncr.ydjk.org.cn

================================================================================
来源：http://rzu.tarul.cn

B. 流程控制
来源：http://szd.pengpengdd.cyou

================================================================================
来源：http://dyi.sweek.top

[B01] 条件判断 if / else
来源：http://eco.ybcxt.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qgw.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ouo.ehwqpu.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kbo.ybcxt.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://krs.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tag.hfpthk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qtf.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xot.redwolf501.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://akg.yanxiufei.cn

[B02] 多分支 else if / elif
来源：http://aqu.0kj1m.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ydc.zhijiandao.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lzz.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lwn.jiagoushi.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vms.quarkkingdee.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nqn.tanke756.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nzt.cashguo.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aud.cdnleiting.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vtf.sufxvd.cn

[B03] switch / match / case
来源：http://mhi.hesvh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hvx.hysaishi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xxi.kuanghao11.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lju.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xus.yanxiufei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yzl.chenjidiqi.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fwx.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bto.shzxlz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lis.jinqigfzy.top

[B04] for 计数循环
来源：http://koc.yonumen.top

Py:   for i in range(10): print(i)
来源：http://ofl.cheryme.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://puf.cqqwz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xme.jqgufenzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mrb.ydjk.org.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tks.sysykeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://btj.meibo888.top

Ruby: 10.times { |i| puts i }
来源：http://unc.xylfe.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uoq.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://yuv.hongshengwenyu.top

Py:   for item in arr: print(item)
来源：http://yfs.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jga.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kba.fanxiaobao.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://rvd.gotoacloud.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jhp.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qjj.ydjk.org.cn

Ruby: arr.each { |item| puts item }
来源：http://evu.ydzc1.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ltc.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://mfr.sufxvd.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ydm.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vjm.chenzaomai.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yvt.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zvq.hcnkem.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wvr.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eeu.zycfv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hws.ehwqpu.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://irf.yangfankeji.com

[B07] while 循环
来源：http://eop.cucudq.cn

Py:   while i < 10: i += 1
来源：http://jej.yueranfly.top

PHP:  while ($i < 10) { $i++; }
来源：http://xla.jyoumei.cn

JS:   while (i < 10) { i++; }
来源：http://rqq.gogol.net.cn

TS:   while (i < 10) { i++; }
来源：http://lrv.316326.xyz

Java: while (i < 10) { i++; }
来源：http://stf.haohaochexian.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ikq.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://dem.cqqwz.cn

C#:   while (i < 10) { i++; }
来源：http://iyt.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://gsd.yj20258.top

Py:   # 无 do-while：用 while True + break
来源：http://ffk.yj20258888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://keb.aizwys.cn

JS:   do { i++; } while (i < 10);
来源：http://orj.yvedp.cn

TS:   do { i++; } while (i < 10);
来源：http://vzo.fanxiaobao.xyz

Java: do { i++; } while (i < 10);
来源：http://pnn.birdmap.top

Go:   for { i++; if i >= 10 { break } }
来源：http://iwh.shuidangran.top

Ruby: begin; i += 1; end while i < 10
来源：http://vai.chenjidiqi.icu

C#:   do { i++; } while (i < 10);
来源：http://gwg.zhengqikj.top

[B09] break 与 continue
来源：http://ype.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yym.svipenyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://txz.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hbh.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aed.hcnkem.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uqt.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://prr.ydzc1.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://epl.ivvv.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vob.redwolf501.top

[B10] 遍历同时拿索引
来源：http://kea.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vxw.zhengqikj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xjf.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vne.vehdjk.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rgk.ydzc1.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kdm.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sqj.meibo888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tvb.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nxs.yonumen.top

[B11] 生成数字序列 / 区间
来源：http://mjx.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://rtu.jinyuanbaomall.cn

PHP:  range(0, 10, 2);
来源：http://urt.xinyue.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gow.tianlin.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vvz.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zeg.mhx1999.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cef.aizwys.cn

Ruby: (0...10).step(2).to_a
来源：http://nah.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://agb.tarul.cn

[B12] 跳出多层循环
来源：http://qgb.9152youxi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hpq.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vie.jinyuanbaomall.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fdy.jinqigfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nvt.hfpthk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pno.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ylq.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qtw.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wjf.xziqi.cn

[B13] 判断是否为数字
来源：http://ndq.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://egu.yuanzhike.top

PHP:  is_numeric($x)
来源：http://ypm.jinqigufen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sel.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://avn.cheryme.top

Java: x instanceof Number
来源：http://mvh.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hge.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://iur.ivvv.top

C#:   x is int or double or decimal
来源：http://sxv.daria6918.cn

[B14] 判断值是否在集合内
来源：http://meh.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mgq.nwbrower.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dwp.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://jlf.hywenlv.cn

TS:   [1, 2, 3].includes(x)
来源：http://exa.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cmg.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://otv.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://igw.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rna.sxryk.cn

[B15] 布尔运算与取反
来源：http://hju.jianghu66.top

Py:   a and b or not c
来源：http://fmp.ybcxt.top

PHP:  $a && $b || !$c
来源：http://tqp.meibo888.top

JS:   a && b || !c
来源：http://epq.shzxlz.cn

TS:   a && b || !c
来源：http://yhe.shanyushiyangkeji.top

Java: a && b || !c
来源：http://bjd.gotoacloud.top

Go:   a && b || !c
来源：http://emz.sxryk.cn

Ruby: a && b || !c
来源：http://ngq.zhoulong.xyz

C#:   a && b || !c
来源：http://vai.ywan-chungtsiang.top

[B16] 卫语句：不满足条件提前返回
来源：http://uns.yangfankeji.com

Py:   if not data: return
来源：http://xds.ydzc1.top

PHP:  if (!$data) { return; }
来源：http://zxy.sjlbkw.cn

JS:   if (!data) return;
来源：http://qpf.daria6918.cn

TS:   if (!data) return;
来源：http://fkh.yangfankeji.com

Java: if (data == null) return;
来源：http://rfx.snrcjt.cn

Go:   if data == nil { return }
来源：http://nev.yj20258888.top

Ruby: return if data.nil?
来源：http://huz.zhijiandao.cn

C#:   if (data == null) return;
来源：http://pyo.dashuyun.cn

================================================================================
来源：http://rnn.jinqigfzy.top

C. 函数与作用域
来源：http://zsf.hammf.cn

================================================================================
来源：http://zwu.ydjk.org.cn

[C01] 定义函数
来源：http://pli.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://ujy.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pcl.ctjpmb.com

JS:   function add(a, b) { return a + b; }
来源：http://cer.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dhu.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mmt.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://sqa.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://iet.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dvh.ctjpmb.com

[C02] 默认参数
来源：http://tvs.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://evc.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://lzu.redwolf501.top

JS:   function greet(name = "World") { return name; }
来源：http://uks.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hyc.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bje.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ptu.fehbvm.com

Ruby: def greet(name = "World") = name
来源：http://qxt.snrcjt.cn

C#:   string Greet(string name = "World") => name;
来源：http://qpj.nanxinkj.top

[C03] 可变参数
来源：http://vmi.sweek.top

Py:   def total(*args): return sum(args)
来源：http://aoa.chenjidiqi.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vkl.9152youxi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hnw.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jio.havefunace.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qsv.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zog.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kki.hysaishi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mlg.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://qba.fengsongda.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lga.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aiy.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ykp.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hfu.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://tul.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://fmf.shanyushiyangtech.top

Ruby: f(a: 1, b: 2)
来源：http://fur.ydjk.org.cn

C#:   f(a: 1, b: 2)
来源：http://saz.dashuyun.cn

[C05] 返回多个值
来源：http://yda.aibaodan.cn

Py:   return a, b
来源：http://yno.yuxming.cn

PHP:  return [$a, $b];
来源：http://kaz.tarul.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://maf.dashuyun.cn

TS:   return { a, b };
来源：http://hxg.xziqi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jgx.ydzc1.top

Go:   return a, b
来源：http://fsd.fktsv.cn

Ruby: return a, b
来源：http://lgb.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://whb.nanxuanxn.top

[C06] 匿名函数 / lambda
来源：http://cey.ivvv.top

Py:   square = lambda x: x * x
来源：http://uns.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yju.cheryme.top

JS:   const square = x => x * x;
来源：http://pmn.zhaomingkeji.xyz

TS:   const square = (x: number): number => x * x;
来源：http://fgj.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gex.yangfankeji.com

Go:   sq := func(x int) int { return x * x }
来源：http://vmn.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://oml.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://rfl.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://wba.meibo888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://otr.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://zhr.haohaochexian.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cwk.nanxinkj.top

TS:   arr.map(String)
来源：http://lly.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mkn.xuetiantiany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rqx.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://lxw.tarul.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xrp.gogol.net.cn

[C08] 闭包
来源：http://cjx.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mmp.jinqigufen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eps.zhoulong.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://isj.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dnr.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nzg.snrcjt.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fjx.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://opb.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://psm.yfazqb.com

[C09] 递归
来源：http://ptu.zhiwuduotai.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ydt.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ibl.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zho.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gog.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pbu.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hqe.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bbc.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cvl.shangyingyoupin.top

[C10] 变量作用域
来源：http://krk.bjfxy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kpq.xuetiantiany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ynb.nanxinkj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xnw.zdbjq.cn


<!-- 参考信息 -->