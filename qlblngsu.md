代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nwf.fanxiaobao.xyz

Ruby: gets.chomp
来源：http://pqx.yj20258888.top

C#:   Console.ReadLine();
来源：http://tvd.gogol.net.cn

[A21] 保留指定小数位输出
来源：http://vuh.dashuyun.cn

Py:   f"{3.14159:.2f}"
来源：http://buv.xylfe.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cej.yj20258888.top

JS:   (3.14159).toFixed(2)
来源：http://bxv.tanke756.top

TS:   (3.14159).toFixed(2)
来源：http://dqs.dashuyun.cn

Java: String.format("%.2f", 3.14159)
来源：http://axt.smart0.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kos.ybcxt.top

Ruby: format("%.2f", 3.14159)
来源：http://qmv.sweek.top

C#:   3.14159.ToString("F2")
来源：http://jxh.hysaishi.cn

[A22] 获取字符串长度
来源：http://spv.shuidangran.top

Py:   len(s)
来源：http://ehy.dashuyun.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lny.wangdashe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eej.wangshuangyany.cn

TS:   s.length
来源：http://tev.tanke756.top

Java: s.length()
来源：http://qtj.jianghu66.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://viw.wangdashe.top

Ruby: s.length
来源：http://iti.jinghuilouyu.cn

C#:   s.Length
来源：http://ujo.tianlin.xyz

[A23] 大小写转换
来源：http://xtk.ppjwa.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://toa.ydjk.org.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ddz.jqgufenzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ulu.hammf.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fre.vehdjk.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uym.aizwys.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ldg.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qcr.ywan-chungtsiang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lim.shanyushiyangtech.top

[A24] 去除首尾空白
来源：http://igb.ywan-chungtsiang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://clu.cashguo.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rmj.pengpengdd.cyou

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lrw.nanxinkj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://huo.aizwys.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yub.cucudq.cn

Go:   strings.TrimSpace(s)
来源：http://yer.zhijiandao.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gvv.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://klp.yj20258.top

[A25] 字符串比较
来源：http://mvb.zhixingplan.top

Py:   s1 == s2; s1 != s2
来源：http://rto.cashguo.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kki.fehbvm.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lyy.sxryk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vai.sjlbkw.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nbn.xylfe.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://int.cqqwz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://myk.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pfj.ppjwa.cn

[A26] 类型转换总览
来源：http://wgf.cdnleiting.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://coh.ydzc1.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uvq.dianchejie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xns.0kj1m.cn

TS:   Number() String() Boolean() x as number
来源：http://rts.jinghuilouyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yag.jinghuilouyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gxi.aibaodan.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hja.jyoumei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://imz.hysaishi.cn

================================================================================
来源：http://ubg.aibaodan.cn

B. 流程控制
来源：http://zov.zhongyouzk.top

================================================================================
来源：http://jvc.ybcxt.top

[B01] 条件判断 if / else
来源：http://nvi.yangfankeji.com

Py:   result = "正" if x > 0 else "非正"
来源：http://slm.shzxlz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://czu.zhijiandao.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://prb.svipenyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qig.zdqjudy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nml.yonumen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ymy.meibo888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oxc.ydjk.org.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sxw.haohaochexian.top

[B02] 多分支 else if / elif
来源：http://btr.yanxiufei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://upt.feifeiyinyue.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aqf.zhiwuduotai.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ezu.gzhubu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hae.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dcv.hfpthk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bxm.tian-w.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jct.sxryk.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ubn.52xcode.cn

[B03] switch / match / case
来源：http://dho.bbcook.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ttu.cdnleiting.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cjh.mhx1999.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vmg.sjlbkw.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ibw.yj202588.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xlr.uphjek.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kus.hywenlv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://soa.guannengcc.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zmp.cdnleiting.top

[B04] for 计数循环
来源：http://ibb.hnqzz.top

Py:   for i in range(10): print(i)
来源：http://mom.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xkn.jianghu66.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cpa.pycfn.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://voi.hesvh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://olv.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ase.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://vyn.pycfn.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fht.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://wjp.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://mrh.9152youxi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pui.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jrw.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://onf.shuidangran.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bbr.jinqigufen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xej.yonumen.top

Ruby: arr.each { |item| puts item }
来源：http://klr.tarul.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tid.wangshuangyany.cn

[B06] 遍历字典 / 对象
来源：http://myn.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://irk.xuetiantiany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nfk.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iok.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qew.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mjs.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://knw.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xwn.xylfe.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iwd.uphjek.com

[B07] while 循环
来源：http://vba.jlsjyb.cn

Py:   while i < 10: i += 1
来源：http://tdf.jqgufenzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://vgk.hysaishi.cn

JS:   while (i < 10) { i++; }
来源：http://idm.yanxiufei.cn

TS:   while (i < 10) { i++; }
来源：http://akn.quarkkingdee.top

Java: while (i < 10) { i++; }
来源：http://jeq.ybcxt.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iao.yj202588.top

Ruby: while i < 10; i += 1; end
来源：http://hlx.ivvv.top

C#:   while (i < 10) { i++; }
来源：http://tzb.jiagoushi.top

[B08] do-while（至少执行一次）
来源：http://pvv.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://ljm.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://trf.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://qnx.zhixingplan.top

TS:   do { i++; } while (i < 10);
来源：http://kjo.hnqzz.top

Java: do { i++; } while (i < 10);
来源：http://ytc.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jwu.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hyy.hcnkem.com

C#:   do { i++; } while (i < 10);
来源：http://azl.tianlin.xyz

[B09] break 与 continue
来源：http://exn.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fsr.guannengcc.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ang.nwbrower.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jnc.jqgufenzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zzi.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ryo.shanyushiyangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ldx.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ydh.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qij.shangyingyoupin.top

[B10] 遍历同时拿索引
来源：http://hea.shanyushiyangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yvf.guowangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qdn.jqgfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lbm.9152youxi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tkt.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://con.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kho.andypj.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lsk.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://egu.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://gjs.dashuyun.cn

Py:   list(range(0, 10, 2))
来源：http://jej.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://gpa.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vho.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mno.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uei.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tbf.gogol.net.cn

Ruby: (0...10).step(2).to_a
来源：http://svk.hnqzz.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hcq.ybcxt.top

[B12] 跳出多层循环
来源：http://foi.cashguo.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rqr.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://srt.zhengqikj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://noi.gzhubu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vcr.shzxlz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kog.hnqzz.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://evc.316326.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rwh.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xfi.hammf.cn

[B13] 判断是否为数字
来源：http://mir.cdnleiting.top

Py:   isinstance(x, (int, float))
来源：http://jlt.zhoulong.xyz

PHP:  is_numeric($x)
来源：http://dnn.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zgd.sweek.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qsm.zhengqikj.top

Java: x instanceof Number
来源：http://gol.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nwv.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://euu.jinqigfzy.top

C#:   x is int or double or decimal
来源：http://zjq.yj20258.top

[B14] 判断值是否在集合内
来源：http://rup.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jai.gaohongyu789.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://htw.ctjpmb.com

JS:   [1, 2, 3].includes(x)
来源：http://wxv.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://wjv.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qgo.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qmq.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://frk.meibo888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tyd.jinqigfzy.top

[B15] 布尔运算与取反
来源：http://esm.hnxiangtu.top

Py:   a and b or not c
来源：http://xxs.0kj1m.cn

PHP:  $a && $b || !$c
来源：http://wno.jinghuilouyu.cn

JS:   a && b || !c
来源：http://jra.fehbvm.com

TS:   a && b || !c
来源：http://qth.shanyushiyangtech.top

Java: a && b || !c
来源：http://eji.shuidangran.top

Go:   a && b || !c
来源：http://qbo.aizwys.cn

Ruby: a && b || !c
来源：http://zar.yonumen.top

C#:   a && b || !c
来源：http://sjz.9152youxi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fmt.sxryk.cn

Py:   if not data: return
来源：http://vpw.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://zrp.yongpay.top

JS:   if (!data) return;
来源：http://akv.zhengqikj.top

TS:   if (!data) return;
来源：http://uof.yj202588.top

Java: if (data == null) return;
来源：http://cps.yueranfly.top

Go:   if data == nil { return }
来源：http://ifa.ydjk.org.cn

Ruby: return if data.nil?
来源：http://mwl.snrcjt.cn

C#:   if (data == null) return;
来源：http://sci.gzhubu.top

================================================================================
来源：http://olf.hfpthk.cn

C. 函数与作用域
来源：http://lyp.aibaodan.cn

================================================================================
来源：http://hjg.fehbvm.com

[C01] 定义函数
来源：http://jxl.zdqjudy.top

Py:   def add(a, b): return a + b
来源：http://ttt.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pjq.daxiang520.top

JS:   function add(a, b) { return a + b; }
来源：http://xkf.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://buj.hcnkem.com

Java: static int add(int a, int b) { return a + b; }
来源：http://dcf.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://rzz.ydzc1.top

Ruby: def add(a, b); a + b; end
来源：http://ova.zhongyouzk.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rxf.mhx1999.top

[C02] 默认参数
来源：http://cvj.havefunace.top

Py:   def greet(name="World"): return name
来源：http://log.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dff.ybcxt.top

JS:   function greet(name = "World") { return name; }
来源：http://klo.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oai.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ogn.jinghuilouyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nnb.uphjek.com

Ruby: def greet(name = "World") = name
来源：http://whj.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://iwh.tanke756.top

[C03] 可变参数
来源：http://wut.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://qsv.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ybl.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fso.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bxv.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rhj.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lzm.sjlbkw.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zvo.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qig.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://osv.mhx1999.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://esx.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dwk.52xcode.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vry.jianghu66.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bkh.cdnleiting.top

Java: // 无：用 Builder 模式或 record
来源：http://iwi.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://jmj.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://aln.fanxiaobao.xyz

C#:   f(a: 1, b: 2)
来源：http://bge.zhoulong.xyz

[C05] 返回多个值
来源：http://zrf.jqgufenzy.top

Py:   return a, b
来源：http://ovk.sufxvd.cn

PHP:  return [$a, $b];
来源：http://iut.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://goq.sxryk.cn

TS:   return { a, b };
来源：http://ixi.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yqz.gogol.net.cn

Go:   return a, b
来源：http://ape.jqgufenzy.top

Ruby: return a, b
来源：http://zfd.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://xjk.fzhhl.top

[C06] 匿名函数 / lambda
来源：http://eaq.yj202588.top

Py:   square = lambda x: x * x
来源：http://wrv.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://noa.316326.xyz

JS:   const square = x => x * x;
来源：http://iie.pycfn.com

TS:   const square = (x: number): number => x * x;
来源：http://pzf.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xxx.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://typ.yanxiufei.cn

Ruby: square = ->(x) { x * x }
来源：http://qiq.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rvn.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://idh.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://emg.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://slx.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vhx.yangfankeji.com

TS:   arr.map(String)
来源：http://elx.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zjq.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xpx.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://stc.tianlin.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://kul.dashuyun.cn

[C08] 闭包
来源：http://zxh.hnqzz.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cws.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dvw.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qwy.c1oappe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sbn.sufxvd.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lob.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ruq.cucudq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jun.cashguo.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ddz.ywan-chungtsiang.top

[C09] 递归
来源：http://qtz.jinqigufen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nnr.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://llb.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dsx.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yau.kuanghao11.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bch.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tdh.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qzo.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://onz.tianlin.xyz

[C10] 变量作用域
来源：http://bob.dashuyun.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://del.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kcx.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eum.yfazqb.com

TS:   同 JS
来源：http://rvk.hywenlv.cn

Java: 方法内为块级作用域
来源：http://ilw.ybcxt.top

Go:   花括号块级作用域
来源：http://bwi.zdbjq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://she.nwbrower.top

C#:   块级作用域
来源：http://eol.yfazqb.com

[C11] 模块导入与导出
来源：http://lzq.sxryk.cn

Py:   from module import func
来源：http://ziz.tian-w.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pmz.gaohongyu789.top


<!-- 参考信息 -->