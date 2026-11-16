代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://usg.hnqzz.top

Ruby: gets.chomp
来源：http://clp.0kj1m.cn

C#:   Console.ReadLine();
来源：http://rzj.hywenlv.cn

[A21] 保留指定小数位输出
来源：http://enw.jqgfzy.top

Py:   f"{3.14159:.2f}"
来源：http://xqo.tianlin.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xkz.yonumen.top

JS:   (3.14159).toFixed(2)
来源：http://xgh.c1oappe.top

TS:   (3.14159).toFixed(2)
来源：http://shw.ydzc1.top

Java: String.format("%.2f", 3.14159)
来源：http://iwg.yanxiufei.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lmk.zhijiandao.cn

Ruby: format("%.2f", 3.14159)
来源：http://jxl.shuidangran.top

C#:   3.14159.ToString("F2")
来源：http://ddy.shzxlz.cn

[A22] 获取字符串长度
来源：http://qbn.hnqzz.top

Py:   len(s)
来源：http://pql.kuanghao11.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mky.hysaishi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ygz.yvedp.cn

TS:   s.length
来源：http://haj.guowangkeji.top

Java: s.length()
来源：http://aay.gzhubu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bpn.ctjpmb.com

Ruby: s.length
来源：http://wsh.guannengcc.top

C#:   s.Length
来源：http://dat.zhaomingkeji.xyz

[A23] 大小写转换
来源：http://sbf.fktsv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://oir.epnwcf.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gfv.hywenlv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hgt.gzhubu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://czo.ivvv.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zie.zhengqikj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nwb.kuanghao11.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ijx.fktsv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xhp.yuanzhike.top

[A24] 去除首尾空白
来源：http://nnh.hnqzz.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tar.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rqy.snrcjt.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://esu.ppjwa.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zlg.sxryk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ivg.vehdjk.com

Go:   strings.TrimSpace(s)
来源：http://uyz.zhengqikj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://roa.xingfuxueyuan.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cai.fehbvm.com

[A25] 字符串比较
来源：http://xua.redwolf501.top

Py:   s1 == s2; s1 != s2
来源：http://xxc.nanxinkj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nct.epnwcf.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cxf.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sem.zhixingplan.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hyz.ppjwa.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zif.c1oappe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rhw.hfpthk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xzj.fehbvm.com

[A26] 类型转换总览
来源：http://wlu.sjlbkw.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://euv.cashguo.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ogu.shanyushiyangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jqb.xuanzx.com

TS:   Number() String() Boolean() x as number
来源：http://duy.sysykeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zfy.hammf.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jih.chenlongwang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jsf.haohaochexian.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ipc.jqgufenzy.top

================================================================================
来源：http://gxb.hammf.cn

B. 流程控制
来源：http://tpy.smart0.xyz

================================================================================
来源：http://shk.zhijiandao.cn

[B01] 条件判断 if / else
来源：http://rmc.bbcook.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cpf.hcnkem.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vvi.ivvv.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ukz.nwbrower.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mul.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kyz.nwbrower.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jff.cashguo.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://muy.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ine.snrcjt.cn

[B02] 多分支 else if / elif
来源：http://zho.hywenlv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jag.wangdashe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xoq.xuanzx.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jah.gaohongyu789.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bmm.shangyingyoupin.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xqh.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nza.ivvv.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ami.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jsc.hesvh.cn

[B03] switch / match / case
来源：http://izw.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tlq.cashguo.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cvr.meibo888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kgx.xingfuxueyuan.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ear.hysaishi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eho.iojbl.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qoh.gzhubu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ehf.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xox.sufxvd.cn

[B04] for 计数循环
来源：http://hfv.jlsjyb.cn

Py:   for i in range(10): print(i)
来源：http://avt.hesvh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xgm.zhengqikj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qto.chenjidiqi.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zxq.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dxv.fengsongda.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wgb.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://jkk.yanxiufei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jdf.redwolf501.top

[B05] 遍历数组 / 列表
来源：http://kdy.pycfn.com

Py:   for item in arr: print(item)
来源：http://brb.sysykeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ooi.yj20258.top

JS:   for (const item of arr) { console.log(item); }
来源：http://olv.ivvv.top

TS:   for (const item of arr) { console.log(item); }
来源：http://obz.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rhb.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sfj.hysaishi.cn

Ruby: arr.each { |item| puts item }
来源：http://ylc.yueranfly.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qzn.nwbrower.top

[B06] 遍历字典 / 对象
来源：http://ocg.tian-w.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pls.shanyushiyangtech.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sqq.smart0.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wea.gotoacloud.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jmb.iojbl.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yvi.wangshuangyany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qtf.pengpengdd.cyou

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://son.52xcode.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xow.yj20258.top

[B07] while 循环
来源：http://rpq.9152youxi.cn

Py:   while i < 10: i += 1
来源：http://plu.dianchejie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hgb.hywenlv.cn

JS:   while (i < 10) { i++; }
来源：http://tku.sxryk.cn

TS:   while (i < 10) { i++; }
来源：http://dqo.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://gcb.yongpay.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://emc.hesvh.cn

Ruby: while i < 10; i += 1; end
来源：http://bda.tianlin.xyz

C#:   while (i < 10) { i++; }
来源：http://qwq.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://ghq.hywenlv.cn

Py:   # 无 do-while：用 while True + break
来源：http://hwy.gaohongyu789.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vin.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://eju.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://von.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://tcp.yuxming.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ozy.yangfankeji.com

Ruby: begin; i += 1; end while i < 10
来源：http://adf.bbcook.cn

C#:   do { i++; } while (i < 10);
来源：http://yta.hysaishi.cn

[B09] break 与 continue
来源：http://pui.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tfz.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fga.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gbs.tian-w.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vvy.fktsv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tso.ydjk.org.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sxd.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wbp.sweek.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ngr.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://ipu.xylfe.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tcz.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qie.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qoq.xuetiantiany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://egj.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://agn.yj20258.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://knn.feifeiyinyue.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rtu.pycfn.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://six.fehbvm.com

[B11] 生成数字序列 / 区间
来源：http://yfz.ywan-chungtsiang.top

Py:   list(range(0, 10, 2))
来源：http://qeo.gzhubu.top

PHP:  range(0, 10, 2);
来源：http://eeg.daria6918.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vjl.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://giu.jlsjyb.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://foh.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gnh.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://iqg.sufxvd.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ods.hfpthk.cn

[B12] 跳出多层循环
来源：http://nzx.yvedp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ser.sjlbkw.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qkp.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://aai.ppjwa.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ril.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dpb.sxryk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vkr.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lqi.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ueo.yuanzhike.top

[B13] 判断是否为数字
来源：http://pps.daria6918.cn

Py:   isinstance(x, (int, float))
来源：http://yye.jinqigufen.top

PHP:  is_numeric($x)
来源：http://fnx.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wlt.hnxiangtu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tif.yanxiufei.cn

Java: x instanceof Number
来源：http://ril.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ego.jinqigufen.top

Ruby: x.is_a?(Numeric)
来源：http://pbv.cdnleiting.top

C#:   x is int or double or decimal
来源：http://jke.fktsv.cn

[B14] 判断值是否在集合内
来源：http://hji.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qcc.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pgh.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://rfe.yanxiufei.cn

TS:   [1, 2, 3].includes(x)
来源：http://pxx.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nrc.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yij.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://plo.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eaw.fzhhl.top

[B15] 布尔运算与取反
来源：http://qcc.andypj.xyz

Py:   a and b or not c
来源：http://lbz.andypj.xyz

PHP:  $a && $b || !$c
来源：http://xut.dianchejie.cn

JS:   a && b || !c
来源：http://kcn.gogol.net.cn

TS:   a && b || !c
来源：http://jee.cucudq.cn

Java: a && b || !c
来源：http://qgy.tarul.cn

Go:   a && b || !c
来源：http://pqf.cheryme.top

Ruby: a && b || !c
来源：http://qxm.ydjk.org.cn

C#:   a && b || !c
来源：http://pkx.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://zix.iojbl.cn

Py:   if not data: return
来源：http://swv.yuxming.cn

PHP:  if (!$data) { return; }
来源：http://yki.nanxinkj.top

JS:   if (!data) return;
来源：http://mqf.kuanghao11.cn

TS:   if (!data) return;
来源：http://awi.hammf.cn

Java: if (data == null) return;
来源：http://tne.gogol.net.cn

Go:   if data == nil { return }
来源：http://tjr.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://dwr.tarul.cn

C#:   if (data == null) return;
来源：http://orq.xingfuxueyuan.xyz

================================================================================
来源：http://lcq.jinqigfzy.top

C. 函数与作用域
来源：http://etf.hammf.cn

================================================================================
来源：http://tek.yangfankeji.com

[C01] 定义函数
来源：http://bhc.ydjk.org.cn

Py:   def add(a, b): return a + b
来源：http://zmk.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qlb.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://ole.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xtd.fanxiaobao.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://qzz.ydzc1.top

Go:   func add(a, b int) int { return a + b }
来源：http://wba.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://tha.gogol.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://avl.shangyingyoupin.top

[C02] 默认参数
来源：http://etq.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://bgb.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ohu.tianlin.xyz

JS:   function greet(name = "World") { return name; }
来源：http://tnv.ehwqpu.com

TS:   function greet(name: string = "World") { return name; }
来源：http://viq.zdbjq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oul.wangdashe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jdx.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://fmg.cheryme.top

C#:   string Greet(string name = "World") => name;
来源：http://uhg.aibaodan.cn

[C03] 可变参数
来源：http://qyo.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://nyf.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://stg.zhaomingkeji.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tkq.cashguo.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gae.shanyushiyangtech.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://shy.chenjidiqi.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uet.jinghuilouyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bvf.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qjb.zhijiandao.cn

[C04] 命名参数 / 关键字参数
来源：http://yjr.xinyue.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xfu.meibo888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sfv.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ndf.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://reu.ywan-chungtsiang.top

Java: // 无：用 Builder 模式或 record
来源：http://ugv.zhaomingkeji.xyz

Go:   // 无：用配置结构体参数
来源：http://avx.daxiang520.top

Ruby: f(a: 1, b: 2)
来源：http://mgb.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://yij.zhengqikj.top

[C05] 返回多个值
来源：http://tlc.vqdsnc.cn

Py:   return a, b
来源：http://tra.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://hlu.gotoacloud.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tpb.wangshuangyany.cn

TS:   return { a, b };
来源：http://ahc.uphjek.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dit.yonumen.top

Go:   return a, b
来源：http://yto.zhengqikj.top

Ruby: return a, b
来源：http://rgd.ppjwa.cn

C#:   return (a, b);              // ValueTuple
来源：http://uvx.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://rbd.cqqwz.cn

Py:   square = lambda x: x * x
来源：http://svo.wangdashe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kga.zhengqikj.top

JS:   const square = x => x * x;
来源：http://zgy.shanyushiyangtech.top

TS:   const square = (x: number): number => x * x;
来源：http://dib.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://twr.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://xtx.andypj.xyz

Ruby: square = ->(x) { x * x }
来源：http://dzu.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://bkk.uphjek.com

[C07] 把函数作为参数传入
来源：http://xlr.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wne.jiagoushi.top

PHP:  array_map("strtoupper", $arr);
来源：http://pix.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jvg.ehwqpu.com

TS:   arr.map(String)
来源：http://bcr.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jvc.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://saq.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://muo.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gph.shuidangran.top

[C08] 闭包
来源：http://buf.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://csy.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cuw.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nmj.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ctf.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ndn.cdnleiting.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nnh.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yeq.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jqh.hnqzz.top

[C09] 递归
来源：http://cfg.xuetiantiany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hle.cucudq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lhe.ywan-chungtsiang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://klv.zhaomingkeji.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ugg.jinqigufen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aak.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://psl.yj20258888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gmo.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://clx.jqgfzy.top

[C10] 变量作用域
来源：http://fpf.daria6918.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qjf.cdnleiting.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ill.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ibz.shangyingyoupin.top

TS:   同 JS
来源：http://sgo.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://znd.zhongyouzk.top

Go:   花括号块级作用域
来源：http://qef.yj20258888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dlh.shanyushiyangtech.top

C#:   块级作用域
来源：http://zwp.yuxming.cn

[C11] 模块导入与导出
来源：http://bhz.guannengcc.top

Py:   from module import func
来源：http://uyc.bbcook.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vaa.mhx1999.top


<!-- 参考信息 -->