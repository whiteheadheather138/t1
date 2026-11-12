代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lhf.vehdjk.com

Ruby: gets.chomp
来源：http://zyi.yj20258888.top

C#:   Console.ReadLine();
来源：http://wuf.xinyue.icu

[A21] 保留指定小数位输出
来源：http://ast.gzhubu.top

Py:   f"{3.14159:.2f}"
来源：http://mjs.iojbl.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://aqy.zhongyouzk.top

JS:   (3.14159).toFixed(2)
来源：http://pse.zhoulong.xyz

TS:   (3.14159).toFixed(2)
来源：http://liq.iojbl.cn

Java: String.format("%.2f", 3.14159)
来源：http://cbv.guannengcc.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://slk.pycfn.com

Ruby: format("%.2f", 3.14159)
来源：http://aka.yongpay.top

C#:   3.14159.ToString("F2")
来源：http://yyj.52xcode.cn

[A22] 获取字符串长度
来源：http://igm.ctjpmb.com

Py:   len(s)
来源：http://xrw.sysykeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qfi.yfazqb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vzl.nanxuanxn.top

TS:   s.length
来源：http://zfz.zdbjq.cn

Java: s.length()
来源：http://ttb.cqqwz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://omn.sysykeji.top

Ruby: s.length
来源：http://eyj.gzhubu.top

C#:   s.Length
来源：http://jns.zhiwuduotai.top

[A23] 大小写转换
来源：http://ucr.daxiang520.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mxl.haohaochexian.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tpd.guowangkeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yen.zhaomingkeji.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rml.jqgufenzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vin.fzhhl.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dnh.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://idb.xinyue.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://kul.fengsongda.top

[A24] 去除首尾空白
来源：http://xfx.yangfankeji.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://atb.wangshuangyany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gti.gzhubu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://njn.jinyuanbaomall.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rat.ywan-chungtsiang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ilm.shuidangran.top

Go:   strings.TrimSpace(s)
来源：http://qfn.jqgfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rib.fehbvm.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lan.redwolf501.top

[A25] 字符串比较
来源：http://qhm.hammf.cn

Py:   s1 == s2; s1 != s2
来源：http://fnd.fktsv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://noc.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aru.ctjpmb.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pqa.svipenyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qhp.nwbrower.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cek.shzxlz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://chj.fzhhl.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pge.yueranfly.top

[A26] 类型转换总览
来源：http://cqt.nanxuanxn.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yau.jqgufenzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://twq.yongpay.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aji.chenzaomai.com

TS:   Number() String() Boolean() x as number
来源：http://spf.fanxiaobao.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gvy.zhixingplan.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jiw.xuetiantiany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://akv.sweek.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dai.tian-w.cn

================================================================================
来源：http://jlc.shzxlz.cn

B. 流程控制
来源：http://jnh.redwolf501.top

================================================================================
来源：http://tdb.ydjk.org.cn

[B01] 条件判断 if / else
来源：http://kon.epnwcf.com

Py:   result = "正" if x > 0 else "非正"
来源：http://uyh.yuanzhike.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uwz.hongshengwenyu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lvl.vqdsnc.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yqt.hnqzz.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rrt.haohaochexian.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dof.ywan-chungtsiang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xmn.svipenyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ozy.smart0.xyz

[B02] 多分支 else if / elif
来源：http://xkc.xziqi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nbc.bjfxy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wwl.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://caw.9152youxi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qqi.zycfv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://drf.jlsjyb.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cgm.nanxuanxn.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ugz.zycfv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zlk.yueranfly.top

[B03] switch / match / case
来源：http://sbo.cqqwz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xdv.sweek.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yzr.mhx1999.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://phq.vehdjk.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ffr.vqdsnc.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rvi.fktsv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rus.gzhubu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hvf.shzxlz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hfk.yongpay.top

[B04] for 计数循环
来源：http://yqm.ybcxt.top

Py:   for i in range(10): print(i)
来源：http://obf.sysykeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://noy.vehdjk.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ouz.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nws.xziqi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://meg.chenjidiqi.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tap.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://tau.shanyushiyangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kqg.meibo888.top

[B05] 遍历数组 / 列表
来源：http://chq.nwbrower.top

Py:   for item in arr: print(item)
来源：http://ihf.haohaochexian.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pla.hfpthk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cud.zhoulong.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://bfu.zdqjudy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dnd.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ufm.pengpengdd.cyou

Ruby: arr.each { |item| puts item }
来源：http://waj.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sym.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://rrd.yfazqb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://kul.daria6918.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eeo.shzxlz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tna.hywenlv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fyb.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bob.tanke756.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wpx.dashuyun.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xzk.jinqigufen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uvf.jlsjyb.cn

[B07] while 循环
来源：http://wqa.guannengcc.top

Py:   while i < 10: i += 1
来源：http://xce.daxiang520.top

PHP:  while ($i < 10) { $i++; }
来源：http://frv.zhiwuduotai.top

JS:   while (i < 10) { i++; }
来源：http://fzs.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://ndn.guowangkeji.top

Java: while (i < 10) { i++; }
来源：http://iuq.nanxinkj.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rnm.cashguo.top

Ruby: while i < 10; i += 1; end
来源：http://ghz.cucudq.cn

C#:   while (i < 10) { i++; }
来源：http://sbd.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://xrf.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://gpj.gzhubu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mje.wangdashe.top

JS:   do { i++; } while (i < 10);
来源：http://ezz.gotoacloud.top

TS:   do { i++; } while (i < 10);
来源：http://klv.tanke756.top

Java: do { i++; } while (i < 10);
来源：http://boz.uphjek.com

Go:   for { i++; if i >= 10 { break } }
来源：http://yeq.jianghu66.top

Ruby: begin; i += 1; end while i < 10
来源：http://ifa.xylfe.cn

C#:   do { i++; } while (i < 10);
来源：http://tqt.guannengcc.top

[B09] break 与 continue
来源：http://vbu.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eyf.guannengcc.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gsm.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pcy.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iqg.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hyu.chenjidiqi.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cnb.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://opz.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://udf.c1oappe.top

[B10] 遍历同时拿索引
来源：http://mgt.cashguo.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xwm.cheryme.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ijd.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gqs.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wzk.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ybc.hysaishi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dob.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nas.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kcn.guannengcc.top

[B11] 生成数字序列 / 区间
来源：http://tcp.jianghu66.top

Py:   list(range(0, 10, 2))
来源：http://yfs.havefunace.top

PHP:  range(0, 10, 2);
来源：http://xez.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yic.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jbe.ctjpmb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qlv.svipenyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://izi.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://eoe.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wtt.hesvh.cn

[B12] 跳出多层循环
来源：http://nzz.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sht.nwbrower.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xsw.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eed.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jjx.xylfe.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tjc.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rtw.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://evw.sjlbkw.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://twc.gzhubu.top

[B13] 判断是否为数字
来源：http://yuq.havefunace.top

Py:   isinstance(x, (int, float))
来源：http://uor.iojbl.cn

PHP:  is_numeric($x)
来源：http://ghw.zhoulong.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ymi.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qvj.zhixingplan.top

Java: x instanceof Number
来源：http://bbn.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://msm.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://hxv.ywan-chungtsiang.top

C#:   x is int or double or decimal
来源：http://jel.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://slb.sufxvd.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yxi.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jtu.ydzc1.top

JS:   [1, 2, 3].includes(x)
来源：http://udm.vehdjk.com

TS:   [1, 2, 3].includes(x)
来源：http://ior.zhengqikj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bal.yonumen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dec.yfazqb.com

Ruby: [1, 2, 3].include?(x)
来源：http://dcx.zycfv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fnf.pycfn.com

[B15] 布尔运算与取反
来源：http://jvw.zhengqikj.top

Py:   a and b or not c
来源：http://rgh.xingfuxueyuan.xyz

PHP:  $a && $b || !$c
来源：http://sfd.chenlongwang.top

JS:   a && b || !c
来源：http://tlm.guowangkeji.top

TS:   a && b || !c
来源：http://fgr.meibo888.top

Java: a && b || !c
来源：http://agf.sweek.top

Go:   a && b || !c
来源：http://xqi.yfazqb.com

Ruby: a && b || !c
来源：http://vly.yfazqb.com

C#:   a && b || !c
来源：http://zfb.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wrg.52xcode.cn

Py:   if not data: return
来源：http://hkd.jlsjyb.cn

PHP:  if (!$data) { return; }
来源：http://yev.iojbl.cn

JS:   if (!data) return;
来源：http://xip.zhoulong.xyz

TS:   if (!data) return;
来源：http://fki.chenzaomai.com

Java: if (data == null) return;
来源：http://kqf.yfazqb.com

Go:   if data == nil { return }
来源：http://osy.daria6918.cn

Ruby: return if data.nil?
来源：http://eyi.yongpay.top

C#:   if (data == null) return;
来源：http://zzf.shanyushiyangtech.top

================================================================================
来源：http://qwo.ywan-chungtsiang.top

C. 函数与作用域
来源：http://hnt.jinqigufen.top

================================================================================
来源：http://kcl.zhengqikj.top

[C01] 定义函数
来源：http://lex.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://hao.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nwj.daxiang520.top

JS:   function add(a, b) { return a + b; }
来源：http://tsn.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vwi.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://bqh.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://uzr.c1oappe.top

Ruby: def add(a, b); a + b; end
来源：http://ubk.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mms.svipenyu.cn

[C02] 默认参数
来源：http://pge.epnwcf.com

Py:   def greet(name="World"): return name
来源：http://pwe.jinqigufen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cyr.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://bsp.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hrn.yfazqb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://kiu.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jlz.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://cbo.xziqi.cn

C#:   string Greet(string name = "World") => name;
来源：http://jbv.pycfn.com

[C03] 可变参数
来源：http://nre.jlsjyb.cn

Py:   def total(*args): return sum(args)
来源：http://lur.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xcc.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lmt.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pxo.jiagoushi.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://are.aizwys.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gsr.cdnleiting.top

Ruby: def total(*nums); nums.sum; end
来源：http://omf.xuanzx.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vpl.ctjpmb.com

[C04] 命名参数 / 关键字参数
来源：http://qbo.shzxlz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pgx.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://paw.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ilt.bbcook.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lvc.tian-w.cn

Java: // 无：用 Builder 模式或 record
来源：http://mkl.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://cok.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://qpl.yj20258888.top

C#:   f(a: 1, b: 2)
来源：http://bik.zhiwuduotai.top

[C05] 返回多个值
来源：http://gul.sjlbkw.cn

Py:   return a, b
来源：http://dvn.jianghu66.top

PHP:  return [$a, $b];
来源：http://amm.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hpx.ywan-chungtsiang.top

TS:   return { a, b };
来源：http://xtg.ydjk.org.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fbn.shangyingyoupin.top

Go:   return a, b
来源：http://mao.sxryk.cn

Ruby: return a, b
来源：http://rmv.aibaodan.cn

C#:   return (a, b);              // ValueTuple
来源：http://mnf.sweek.top

[C06] 匿名函数 / lambda
来源：http://fxd.cucudq.cn

Py:   square = lambda x: x * x
来源：http://wts.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xzj.hysaishi.cn

JS:   const square = x => x * x;
来源：http://qat.snrcjt.cn

TS:   const square = (x: number): number => x * x;
来源：http://cvi.zhiwuduotai.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ulq.snrcjt.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ubp.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://wpf.svipenyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bor.jianghu66.top

[C07] 把函数作为参数传入
来源：http://veg.cdnleiting.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jaf.hammf.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kjq.epnwcf.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://loa.gaohongyu789.top

TS:   arr.map(String)
来源：http://iko.chenzaomai.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bik.nanxinkj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://brm.sysykeji.top

Ruby: arr.map(&:upcase)
来源：http://dge.xziqi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mfp.hnxiangtu.top

[C08] 闭包
来源：http://bis.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hzd.316326.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vrj.mhx1999.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kav.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bxd.zdqjudy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bmo.guannengcc.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ajz.hongshengwenyu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ssy.birdmap.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tet.bjfxy.top

[C09] 递归
来源：http://few.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fpl.tanke756.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gxq.ppjwa.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jmu.yfazqb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tqt.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fhc.chenzaomai.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://osq.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://idc.shangyingyoupin.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vte.hfpthk.cn

[C10] 变量作用域
来源：http://aqr.yj20258.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rps.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://atw.zhiwuduotai.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rft.jlsjyb.cn

TS:   同 JS
来源：http://oae.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://inp.yvedp.cn

Go:   花括号块级作用域
来源：http://gzb.xuanzx.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mzk.tarul.cn

C#:   块级作用域
来源：http://cnq.316326.xyz

[C11] 模块导入与导出
来源：http://xjf.svipenyu.cn

Py:   from module import func
来源：http://gld.hfpthk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aep.hnxiangtu.top


<!-- 参考信息 -->