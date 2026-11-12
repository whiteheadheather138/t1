代发 wailian999

Ruby: a, b = b, a
来源：http://vce.zhiwuduotai.top

C#:   (a, b) = (b, a);
来源：http://cjq.shanyushiyangtech.top

[A20] 读取标准输入
来源：http://ayw.gzhubu.top

Py:   name = input("请输入：")
来源：http://kza.hongshengwenyu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jor.xziqi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ges.jinghuilouyu.cn

TS:   // Node.js：readline 模块
来源：http://jny.bjfxy.top

Java: new Scanner(System.in).nextLine()
来源：http://wnf.epnwcf.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zaa.jinqigfzy.top

Ruby: gets.chomp
来源：http://byv.aibaodan.cn

C#:   Console.ReadLine();
来源：http://jwt.haohaochexian.top

[A21] 保留指定小数位输出
来源：http://uyu.hammf.cn

Py:   f"{3.14159:.2f}"
来源：http://boi.52xcode.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lhh.yuxming.cn

JS:   (3.14159).toFixed(2)
来源：http://wtm.xuanzx.com

TS:   (3.14159).toFixed(2)
来源：http://xit.nwbrower.top

Java: String.format("%.2f", 3.14159)
来源：http://vas.nanxuanxn.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lkp.bbcook.cn

Ruby: format("%.2f", 3.14159)
来源：http://oat.hcnkem.com

C#:   3.14159.ToString("F2")
来源：http://ytp.havefunace.top

[A22] 获取字符串长度
来源：http://azu.gogol.net.cn

Py:   len(s)
来源：http://wjh.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gqk.andypj.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lbz.sjlbkw.cn

TS:   s.length
来源：http://slx.xylfe.cn

Java: s.length()
来源：http://nxm.yangfankeji.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tsf.sufxvd.cn

Ruby: s.length
来源：http://tmr.316326.xyz

C#:   s.Length
来源：http://qbs.uphjek.com

[A23] 大小写转换
来源：http://ljj.ppjwa.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rpo.pycfn.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://upz.dashuyun.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yal.nwbrower.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://whz.hnqzz.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tuq.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ygp.tianlin.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://whm.xinyue.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://qdm.sweek.top

[A24] 去除首尾空白
来源：http://ioa.uphjek.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fcs.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qjy.aibaodan.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://amh.yj202588.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xnf.pengpengdd.cyou

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qes.bjfxy.top

Go:   strings.TrimSpace(s)
来源：http://rwd.sxryk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mmt.gzhubu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ces.bjfxy.top

[A25] 字符串比较
来源：http://pvu.ydjk.org.cn

Py:   s1 == s2; s1 != s2
来源：http://zyw.snrcjt.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://krj.meibo888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rhx.dashuyun.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://awt.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bsl.xinyue.icu

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tfc.vehdjk.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ukd.snrcjt.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cwp.daxiang520.top

[A26] 类型转换总览
来源：http://exa.yvedp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://flm.guannengcc.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xfv.jinyuanbaomall.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bmi.wangdashe.top

TS:   Number() String() Boolean() x as number
来源：http://deu.hysaishi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vgw.chenjidiqi.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oad.ybcxt.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kme.tian-w.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ylu.gaohongyu789.top

================================================================================
来源：http://gix.fehbvm.com

B. 流程控制
来源：http://gan.redwolf501.top

================================================================================
来源：http://bld.sjlbkw.cn

[B01] 条件判断 if / else
来源：http://sae.chenzaomai.com

Py:   result = "正" if x > 0 else "非正"
来源：http://yil.zhiwuduotai.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uqq.dianchejie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ztc.hongshengwenyu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uuw.hnqzz.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nce.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tia.mhx1999.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zuh.zdqjudy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cow.shanyushiyangkeji.top

[B02] 多分支 else if / elif
来源：http://lhx.jqgufenzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kri.zhixingplan.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mha.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lra.vehdjk.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://khh.andypj.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cdn.bjfxy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jvb.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gzw.smart0.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ffr.sysykeji.top

[B03] switch / match / case
来源：http://qcy.yvedp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://syo.ivvv.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ibi.cashguo.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://htu.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vwi.jinqigfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iyh.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ual.meibo888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uyl.yuxming.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qsm.jinyuanbaomall.cn

[B04] for 计数循环
来源：http://tnr.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://jfs.hesvh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rll.xingfuxueyuan.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ywi.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qqo.quarkkingdee.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kdf.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rvt.dianchejie.cn

Ruby: 10.times { |i| puts i }
来源：http://poa.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ikk.zhengqikj.top

[B05] 遍历数组 / 列表
来源：http://ltp.ctjpmb.com

Py:   for item in arr: print(item)
来源：http://jyb.nanxinkj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mbi.sxryk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zec.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fuv.zhijiandao.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ftg.hesvh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ntp.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://asi.sjlbkw.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rdi.hnxiangtu.top

[B06] 遍历字典 / 对象
来源：http://ehn.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xqe.fanxiaobao.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tdc.andypj.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wwx.hnqzz.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rup.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cqk.hongshengwenyu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://frj.bjfxy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ngy.fehbvm.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ogb.sjlbkw.cn

[B07] while 循环
来源：http://pgb.hcnkem.com

Py:   while i < 10: i += 1
来源：http://abi.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://ukx.cheryme.top

JS:   while (i < 10) { i++; }
来源：http://ann.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://mnt.haohaochexian.top

Java: while (i < 10) { i++; }
来源：http://scb.gzhubu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aeh.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://dos.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://rro.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://tbg.zhijiandao.cn

Py:   # 无 do-while：用 while True + break
来源：http://wel.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tta.yongpay.top

JS:   do { i++; } while (i < 10);
来源：http://fyk.cqqwz.cn

TS:   do { i++; } while (i < 10);
来源：http://lmm.havefunace.top

Java: do { i++; } while (i < 10);
来源：http://jsj.hcnkem.com

Go:   for { i++; if i >= 10 { break } }
来源：http://hzt.jlsjyb.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mxd.havefunace.top

C#:   do { i++; } while (i < 10);
来源：http://vfp.mhx1999.top

[B09] break 与 continue
来源：http://evn.ppjwa.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pcv.zhaomingkeji.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fxf.bbcook.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mth.hfpthk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lyj.yfazqb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xho.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ory.xylfe.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ucq.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pgk.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://tfb.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ghj.gotoacloud.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hai.quarkkingdee.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dpr.ydjk.org.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zmt.dashuyun.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gqm.yongpay.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gdz.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vnx.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yhl.guannengcc.top

[B11] 生成数字序列 / 区间
来源：http://vaf.daria6918.cn

Py:   list(range(0, 10, 2))
来源：http://yav.wangshuangyany.cn

PHP:  range(0, 10, 2);
来源：http://enx.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kjr.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rru.fzhhl.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ulj.tian-w.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ilt.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://yaa.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hot.quarkkingdee.top

[B12] 跳出多层循环
来源：http://qoy.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jyt.gotoacloud.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://obr.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yei.xingfuxueyuan.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jtu.jiagoushi.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hvv.jinyuanbaomall.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ihn.snrcjt.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fih.sysykeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nhx.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://fra.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://tlu.sufxvd.cn

PHP:  is_numeric($x)
来源：http://ruq.hfpthk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://krf.yueranfly.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://etq.hammf.cn

Java: x instanceof Number
来源：http://ern.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://efp.nwbrower.top

Ruby: x.is_a?(Numeric)
来源：http://eft.yongpay.top

C#:   x is int or double or decimal
来源：http://yhg.sxryk.cn

[B14] 判断值是否在集合内
来源：http://uiy.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://suw.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ncc.tian-w.cn

JS:   [1, 2, 3].includes(x)
来源：http://xze.316326.xyz

TS:   [1, 2, 3].includes(x)
来源：http://vsv.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gjc.shzxlz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qoi.fanxiaobao.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://zvw.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kcp.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://vtw.jianghu66.top

Py:   a and b or not c
来源：http://ptq.smart0.xyz

PHP:  $a && $b || !$c
来源：http://qbo.xingfuxueyuan.xyz

JS:   a && b || !c
来源：http://gxm.tarul.cn

TS:   a && b || !c
来源：http://njs.jqgufenzy.top

Java: a && b || !c
来源：http://flk.gogol.net.cn

Go:   a && b || !c
来源：http://lsp.meibo888.top

Ruby: a && b || !c
来源：http://znh.sxryk.cn

C#:   a && b || !c
来源：http://xtw.gaohongyu789.top

[B16] 卫语句：不满足条件提前返回
来源：http://ylc.jqgufenzy.top

Py:   if not data: return
来源：http://bou.yj20258.top

PHP:  if (!$data) { return; }
来源：http://qss.tanke756.top

JS:   if (!data) return;
来源：http://pzi.gotoacloud.top

TS:   if (!data) return;
来源：http://smk.fehbvm.com

Java: if (data == null) return;
来源：http://loy.cashguo.top

Go:   if data == nil { return }
来源：http://zqq.sxryk.cn

Ruby: return if data.nil?
来源：http://giy.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://rvw.gzhubu.top

================================================================================
来源：http://ckk.havefunace.top

C. 函数与作用域
来源：http://qcf.ivvv.top

================================================================================
来源：http://wti.xingfuxueyuan.xyz

[C01] 定义函数
来源：http://xlz.xziqi.cn

Py:   def add(a, b): return a + b
来源：http://zmt.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ptg.hysaishi.cn

JS:   function add(a, b) { return a + b; }
来源：http://ovc.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tys.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://flq.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://gqx.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://uum.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ryu.jinqigufen.top

[C02] 默认参数
来源：http://vrz.ivvv.top

Py:   def greet(name="World"): return name
来源：http://hgq.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dvo.yangfankeji.com

JS:   function greet(name = "World") { return name; }
来源：http://dnv.yj20258888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tzj.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fcr.tianlin.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pwo.zhoulong.xyz

Ruby: def greet(name = "World") = name
来源：http://jgx.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://zfn.zhoulong.xyz

[C03] 可变参数
来源：http://pup.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://ewf.zhaomingkeji.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hfv.snrcjt.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aal.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hwp.wangdashe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mtm.wangshuangyany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qvf.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://unq.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://stm.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://etm.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mrp.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hyz.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://clz.pycfn.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vup.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://mew.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://bii.shanyushiyangtech.top

Ruby: f(a: 1, b: 2)
来源：http://wyr.guowangkeji.top

C#:   f(a: 1, b: 2)
来源：http://jew.chenjidiqi.icu

[C05] 返回多个值
来源：http://odx.yj202588.top

Py:   return a, b
来源：http://qsf.tarul.cn

PHP:  return [$a, $b];
来源：http://wef.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uau.tianlin.xyz

TS:   return { a, b };
来源：http://xht.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hrv.zhengqikj.top

Go:   return a, b
来源：http://yuf.ctjpmb.com

Ruby: return a, b
来源：http://hvc.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://pbf.xuetiantiany.cn

[C06] 匿名函数 / lambda
来源：http://rfe.guowangkeji.top

Py:   square = lambda x: x * x
来源：http://fgk.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yng.wangdashe.top

JS:   const square = x => x * x;
来源：http://vxn.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://hgs.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yii.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rvd.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://jzh.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jbb.bbcook.cn

[C07] 把函数作为参数传入
来源：http://cqq.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://frf.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://wyy.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hwq.zdbjq.cn

TS:   arr.map(String)
来源：http://ezf.ydjk.org.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ovq.c1oappe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://siw.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://bbq.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cwn.vqdsnc.cn

[C08] 闭包
来源：http://ghw.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cez.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://itc.zhoulong.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hlz.xuanzx.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lbu.andypj.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fsw.shanyushiyangtech.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://axu.cucudq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wji.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zrf.fanxiaobao.xyz

[C09] 递归
来源：http://twm.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rjj.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dii.nwbrower.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://txa.hfpthk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bun.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aua.zhixingplan.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lac.hywenlv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ehk.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wgh.jlsjyb.cn

[C10] 变量作用域
来源：http://cgd.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ais.vqdsnc.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eno.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qgg.kuanghao11.cn


<!-- 参考信息 -->