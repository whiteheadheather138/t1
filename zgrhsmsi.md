代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://sop.jinghuilouyu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ssl.pengpengdd.cyou

TS:   // Node.js：readline 模块
来源：http://rrb.yuxming.cn

Java: new Scanner(System.in).nextLine()
来源：http://juk.hcnkem.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zsv.c1oappe.top

Ruby: gets.chomp
来源：http://vbp.cdnleiting.top

C#:   Console.ReadLine();
来源：http://hvs.snrcjt.cn

[A21] 保留指定小数位输出
来源：http://ywk.yanxiufei.cn

Py:   f"{3.14159:.2f}"
来源：http://lkn.fehbvm.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yhq.hywenlv.cn

JS:   (3.14159).toFixed(2)
来源：http://acd.aizwys.cn

TS:   (3.14159).toFixed(2)
来源：http://qqv.cqqwz.cn

Java: String.format("%.2f", 3.14159)
来源：http://irz.yanxiufei.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://etk.yj20258888.top

Ruby: format("%.2f", 3.14159)
来源：http://kzl.yj202588.top

C#:   3.14159.ToString("F2")
来源：http://wpt.sysykeji.top

[A22] 获取字符串长度
来源：http://xvw.316326.xyz

Py:   len(s)
来源：http://nwj.cdnleiting.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ssv.c1oappe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wsg.nanxuanxn.top

TS:   s.length
来源：http://kbx.gotoacloud.top

Java: s.length()
来源：http://dqp.zdbjq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rzi.9152youxi.cn

Ruby: s.length
来源：http://ysb.xziqi.cn

C#:   s.Length
来源：http://dih.chenjidiqi.icu

[A23] 大小写转换
来源：http://bfq.daria6918.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bmu.pycfn.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://obx.hfpthk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bhl.yvedp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xbq.sysykeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://drl.feifeiyinyue.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zas.xuanzx.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://coh.hesvh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dhe.ydjk.org.cn

[A24] 去除首尾空白
来源：http://agr.zhixingplan.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cfx.tian-w.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fhu.chenjidiqi.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pfj.yj202588.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://prk.feifeiyinyue.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kdb.wangdashe.top

Go:   strings.TrimSpace(s)
来源：http://jog.kuanghao11.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gci.pengpengdd.cyou

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vzl.feifeiyinyue.top

[A25] 字符串比较
来源：http://svx.fzhhl.top

Py:   s1 == s2; s1 != s2
来源：http://ilg.haohaochexian.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eyz.birdmap.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rbt.hywenlv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wnw.aizwys.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qpm.chenzaomai.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vhe.yanxiufei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://een.cashguo.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iqw.epnwcf.com

[A26] 类型转换总览
来源：http://obz.hnxiangtu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jux.ydjk.org.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cly.zdqjudy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rlb.yueranfly.top

TS:   Number() String() Boolean() x as number
来源：http://tdx.fehbvm.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lem.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qtt.hesvh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wxy.52xcode.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zwb.pengpengdd.cyou

================================================================================
来源：http://zyc.shzxlz.cn

B. 流程控制
来源：http://lyt.9152youxi.cn

================================================================================
来源：http://jaa.xylfe.cn

[B01] 条件判断 if / else
来源：http://rwh.zhijiandao.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ysl.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://odj.ydzc1.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vph.guannengcc.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zqq.zhiwuduotai.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://trk.yj202588.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cfv.cashguo.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tlh.yvedp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ofn.aibaodan.cn

[B02] 多分支 else if / elif
来源：http://lut.wangshuangyany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kuf.zycfv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tqx.gzhubu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hqa.hammf.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ozi.sxryk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lom.daria6918.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mdc.0kj1m.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kax.gzhubu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lvc.xylfe.cn

[B03] switch / match / case
来源：http://hrd.ppjwa.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qlw.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vmo.cdnleiting.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wwj.fengsongda.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rlv.jqgfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ukv.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ivp.jinghuilouyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pha.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gkr.jinqigufen.top

[B04] for 计数循环
来源：http://dvc.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://div.feifeiyinyue.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vyq.meibo888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wfa.ivvv.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ule.uphjek.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nev.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pmv.xingfuxueyuan.xyz

Ruby: 10.times { |i| puts i }
来源：http://lpu.birdmap.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://afb.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://rng.jinyuanbaomall.cn

Py:   for item in arr: print(item)
来源：http://zmf.fktsv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rum.ywan-chungtsiang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kgr.jinqigufen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://uqo.snrcjt.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cbq.mhx1999.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oii.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://ulg.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mtp.bjfxy.top

[B06] 遍历字典 / 对象
来源：http://xtp.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sea.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qoa.zdbjq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kbu.tanke756.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lxl.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hts.yj20258888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ljv.hongshengwenyu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pey.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jdj.tarul.cn

[B07] while 循环
来源：http://xiq.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://cgz.zhaomingkeji.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://cup.jiagoushi.top

JS:   while (i < 10) { i++; }
来源：http://wgt.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://qdl.hammf.cn

Java: while (i < 10) { i++; }
来源：http://clj.wangdashe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zho.ywan-chungtsiang.top

Ruby: while i < 10; i += 1; end
来源：http://syc.pycfn.com

C#:   while (i < 10) { i++; }
来源：http://bkf.meibo888.top

[B08] do-while（至少执行一次）
来源：http://ptz.daria6918.cn

Py:   # 无 do-while：用 while True + break
来源：http://wqt.tianlin.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://dph.nanxuanxn.top

JS:   do { i++; } while (i < 10);
来源：http://mmm.yongpay.top

TS:   do { i++; } while (i < 10);
来源：http://pxg.jianghu66.top

Java: do { i++; } while (i < 10);
来源：http://jvt.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bqa.ybcxt.top

Ruby: begin; i += 1; end while i < 10
来源：http://yuj.yfazqb.com

C#:   do { i++; } while (i < 10);
来源：http://lxg.zhijiandao.cn

[B09] break 与 continue
来源：http://oed.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eys.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qbi.epnwcf.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rnc.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bvp.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xar.hcnkem.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zql.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kaj.yangfankeji.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zgg.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://uld.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ccp.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jkx.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vmx.snrcjt.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fen.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://snx.ppjwa.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ohk.cdnleiting.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vkv.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://luu.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://uby.c1oappe.top

Py:   list(range(0, 10, 2))
来源：http://tpt.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://wrd.tarul.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ffb.ybcxt.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://goy.jinqigfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xcv.daria6918.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ihy.xuetiantiany.cn

Ruby: (0...10).step(2).to_a
来源：http://way.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pma.cheryme.top

[B12] 跳出多层循环
来源：http://nro.cashguo.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wni.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://axe.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vow.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ynl.cucudq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kvv.daria6918.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fjp.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dff.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lzb.iojbl.cn

[B13] 判断是否为数字
来源：http://aom.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://ovq.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://qiv.dashuyun.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ndk.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rgz.iojbl.cn

Java: x instanceof Number
来源：http://ecf.daxiang520.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xev.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://cav.xuetiantiany.cn

C#:   x is int or double or decimal
来源：http://qyx.shangyingyoupin.top

[B14] 判断值是否在集合内
来源：http://dod.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sat.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qnn.feifeiyinyue.top

JS:   [1, 2, 3].includes(x)
来源：http://nlm.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://hvb.xingfuxueyuan.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://ppa.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iji.bjfxy.top

Ruby: [1, 2, 3].include?(x)
来源：http://cqj.yfazqb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ryv.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://pcs.zhengqikj.top

Py:   a and b or not c
来源：http://cqa.9152youxi.cn

PHP:  $a && $b || !$c
来源：http://zbl.sweek.top

JS:   a && b || !c
来源：http://vdw.jinqigufen.top

TS:   a && b || !c
来源：http://pdl.xziqi.cn

Java: a && b || !c
来源：http://uum.fzhhl.top

Go:   a && b || !c
来源：http://uxm.sjlbkw.cn

Ruby: a && b || !c
来源：http://tjn.316326.xyz

C#:   a && b || !c
来源：http://hqi.gzhubu.top

[B16] 卫语句：不满足条件提前返回
来源：http://bvz.xinyue.icu

Py:   if not data: return
来源：http://rmy.chenzaomai.com

PHP:  if (!$data) { return; }
来源：http://qgb.9152youxi.cn

JS:   if (!data) return;
来源：http://cmn.jlsjyb.cn

TS:   if (!data) return;
来源：http://qch.jqgufenzy.top

Java: if (data == null) return;
来源：http://iek.zhaomingkeji.xyz

Go:   if data == nil { return }
来源：http://jbo.jinqigufen.top

Ruby: return if data.nil?
来源：http://fgw.ppjwa.cn

C#:   if (data == null) return;
来源：http://vzm.xziqi.cn

================================================================================
来源：http://qrb.cheryme.top

C. 函数与作用域
来源：http://lgw.meibo888.top

================================================================================
来源：http://ymp.shuidangran.top

[C01] 定义函数
来源：http://jhn.9152youxi.cn

Py:   def add(a, b): return a + b
来源：http://fjj.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ssn.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://xfr.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ezm.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cyu.hongshengwenyu.top

Go:   func add(a, b int) int { return a + b }
来源：http://oml.hesvh.cn

Ruby: def add(a, b); a + b; end
来源：http://uyw.9152youxi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cbl.zhixingplan.top

[C02] 默认参数
来源：http://txk.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://baf.sjlbkw.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://clm.fehbvm.com

JS:   function greet(name = "World") { return name; }
来源：http://iex.nanxuanxn.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fyt.ywan-chungtsiang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fup.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://psb.zhengqikj.top

Ruby: def greet(name = "World") = name
来源：http://qyp.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://bii.hywenlv.cn

[C03] 可变参数
来源：http://xlc.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://gek.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rth.yongpay.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tac.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yxb.fengsongda.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yru.ctjpmb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gub.zhongyouzk.top

Ruby: def total(*nums); nums.sum; end
来源：http://cua.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gwn.zdqjudy.top

[C04] 命名参数 / 关键字参数
来源：http://kyu.c1oappe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pcp.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://njt.sxryk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vfx.ctjpmb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uoa.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://uzz.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://uwe.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://bba.yuxming.cn

C#:   f(a: 1, b: 2)
来源：http://pmi.haohaochexian.top

[C05] 返回多个值
来源：http://cli.mhx1999.top

Py:   return a, b
来源：http://lzg.zycfv.cn

PHP:  return [$a, $b];
来源：http://eun.snrcjt.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ntf.0kj1m.cn

TS:   return { a, b };
来源：http://ewq.epnwcf.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gfd.shuidangran.top

Go:   return a, b
来源：http://viu.iojbl.cn

Ruby: return a, b
来源：http://aau.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://dtb.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://epi.vehdjk.com

Py:   square = lambda x: x * x
来源：http://lga.dianchejie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cox.gzhubu.top

JS:   const square = x => x * x;
来源：http://mcs.feifeiyinyue.top

TS:   const square = (x: number): number => x * x;
来源：http://cax.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fvr.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ykz.chenlongwang.top

Ruby: square = ->(x) { x * x }
来源：http://suo.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://ayh.nwbrower.top

[C07] 把函数作为参数传入
来源：http://noa.smart0.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nyh.dashuyun.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bcn.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://udj.jqgufenzy.top

TS:   arr.map(String)
来源：http://bhi.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pwd.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fgu.hongshengwenyu.top

Ruby: arr.map(&:upcase)
来源：http://xhs.yongpay.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fbf.bbcook.cn

[C08] 闭包
来源：http://utu.cucudq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bzs.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://skh.ywan-chungtsiang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rfo.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gox.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gnw.fengsongda.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://woc.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dag.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ngm.haohaochexian.top

[C09] 递归
来源：http://cto.hysaishi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mgl.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qmr.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yfk.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dqy.zdbjq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mpn.0kj1m.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gms.gaohongyu789.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nno.xingfuxueyuan.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fgz.cheryme.top

[C10] 变量作用域
来源：http://hoo.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qzh.uphjek.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dlm.9152youxi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qpa.fktsv.cn

TS:   同 JS
来源：http://wtz.ppjwa.cn

Java: 方法内为块级作用域
来源：http://zdt.sjlbkw.cn

Go:   花括号块级作用域
来源：http://dok.xylfe.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zey.ywan-chungtsiang.top


<!-- 参考信息 -->