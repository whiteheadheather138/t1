代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ciy.havefunace.top

Ruby: gets.chomp
来源：http://lmj.xinyue.icu

C#:   Console.ReadLine();
来源：http://wbt.shuidangran.top

[A21] 保留指定小数位输出
来源：http://bwk.gaohongyu789.top

Py:   f"{3.14159:.2f}"
来源：http://rtq.dianchejie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dgm.shanyushiyangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://wob.yuanzhike.top

TS:   (3.14159).toFixed(2)
来源：http://gjg.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://yjf.yj202588.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jmg.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://tqk.gogol.net.cn

C#:   3.14159.ToString("F2")
来源：http://qvp.aibaodan.cn

[A22] 获取字符串长度
来源：http://mhw.fengsongda.top

Py:   len(s)
来源：http://bpr.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dyi.havefunace.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zyc.quarkkingdee.top

TS:   s.length
来源：http://pgk.zhaomingkeji.xyz

Java: s.length()
来源：http://oli.tianlin.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oru.hysaishi.cn

Ruby: s.length
来源：http://jur.ctjpmb.com

C#:   s.Length
来源：http://pud.chenzaomai.com

[A23] 大小写转换
来源：http://kia.pycfn.com

Py:   s.upper(); s.lower(); s.title()
来源：http://fab.pycfn.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rjy.nwbrower.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wmd.zhongyouzk.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ylz.zdbjq.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kci.snrcjt.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wqk.tianlin.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://izr.snrcjt.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dzt.vehdjk.com

[A24] 去除首尾空白
来源：http://und.zdbjq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fmp.hywenlv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gqp.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yqa.chenzaomai.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ler.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hcc.nanxuanxn.top

Go:   strings.TrimSpace(s)
来源：http://vju.tanke756.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://orw.smart0.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kwl.vehdjk.com

[A25] 字符串比较
来源：http://ujk.sxryk.cn

Py:   s1 == s2; s1 != s2
来源：http://nni.tianlin.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zac.chenjidiqi.icu

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://csg.guannengcc.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bhj.tianlin.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rjk.hywenlv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vuv.0kj1m.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gea.xuanzx.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://atz.hesvh.cn

[A26] 类型转换总览
来源：http://fpp.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bhm.smart0.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sds.xziqi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yjx.shangyingyoupin.top

TS:   Number() String() Boolean() x as number
来源：http://dvh.zhongyouzk.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eah.fanxiaobao.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yci.jinghuilouyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hnj.jinqigfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bjt.hcnkem.com

================================================================================
来源：http://bgg.gotoacloud.top

B. 流程控制
来源：http://ofa.ydzc1.top

================================================================================
来源：http://jlh.zhongyouzk.top

[B01] 条件判断 if / else
来源：http://yzf.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wcm.haohaochexian.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://leu.andypj.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cqm.bjfxy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://shy.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pdc.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://glq.jyoumei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nhm.shangyingyoupin.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sfi.sweek.top

[B02] 多分支 else if / elif
来源：http://xxx.chenzaomai.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pns.xylfe.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ztr.sweek.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://byu.tanke756.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ama.yvedp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aiv.yangfankeji.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nwn.yueranfly.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xty.guannengcc.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cek.yanxiufei.cn

[B03] switch / match / case
来源：http://usv.yj202588.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bkm.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ibi.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cdn.yonumen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cby.52xcode.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yfj.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://siq.c1oappe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tph.cdnleiting.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://txg.yanxiufei.cn

[B04] for 计数循环
来源：http://euv.hcnkem.com

Py:   for i in range(10): print(i)
来源：http://xpf.pycfn.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xbb.nanxuanxn.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bxz.pycfn.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ljd.gotoacloud.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fau.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mba.quarkkingdee.top

Ruby: 10.times { |i| puts i }
来源：http://lrb.chenzaomai.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ukz.chenlongwang.top

[B05] 遍历数组 / 列表
来源：http://shq.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://diy.jlsjyb.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://opk.zdbjq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lyc.jiagoushi.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gwl.yj20258888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jil.ydzc1.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ypl.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://wor.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://azi.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://zdh.hywenlv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vjz.gzhubu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bxt.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pmc.tarul.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://njz.yangfankeji.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bqp.yueranfly.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tna.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lfl.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nby.zdbjq.cn

[B07] while 循环
来源：http://tqp.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://ool.ydzc1.top

PHP:  while ($i < 10) { $i++; }
来源：http://gnk.iojbl.cn

JS:   while (i < 10) { i++; }
来源：http://fpa.zhiwuduotai.top

TS:   while (i < 10) { i++; }
来源：http://pun.xingfuxueyuan.xyz

Java: while (i < 10) { i++; }
来源：http://csg.dashuyun.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ewk.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://mlp.havefunace.top

C#:   while (i < 10) { i++; }
来源：http://vmb.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://ruy.316326.xyz

Py:   # 无 do-while：用 while True + break
来源：http://uoq.meibo888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vif.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://eny.jyoumei.cn

TS:   do { i++; } while (i < 10);
来源：http://lsu.jyoumei.cn

Java: do { i++; } while (i < 10);
来源：http://ihl.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cqs.jianghu66.top

Ruby: begin; i += 1; end while i < 10
来源：http://jgm.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://dfh.ppjwa.cn

[B09] break 与 continue
来源：http://ppz.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hnm.daria6918.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dzg.xingfuxueyuan.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vnk.yueranfly.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nua.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xou.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fjl.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kbp.sxryk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dpw.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://cjs.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ivo.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xha.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rdx.9152youxi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://huo.zhoulong.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sxe.hnqzz.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://srb.chenzaomai.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hcq.yangfankeji.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bce.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://muy.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://trn.uphjek.com

PHP:  range(0, 10, 2);
来源：http://lca.hnqzz.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xeu.mhx1999.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uap.ivvv.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ylt.jinghuilouyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xdx.xingfuxueyuan.xyz

Ruby: (0...10).step(2).to_a
来源：http://gpj.aizwys.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hvy.zhongyouzk.top

[B12] 跳出多层循环
来源：http://eev.nanxuanxn.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://uyg.zhixingplan.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vxs.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zkq.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ifx.chenjidiqi.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lxt.daria6918.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zby.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kzg.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://frv.guowangkeji.top

[B13] 判断是否为数字
来源：http://ybg.zhengqikj.top

Py:   isinstance(x, (int, float))
来源：http://mdw.fzhhl.top

PHP:  is_numeric($x)
来源：http://sof.cdnleiting.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ady.haohaochexian.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://elk.snrcjt.cn

Java: x instanceof Number
来源：http://kfh.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cfm.jinqigfzy.top

Ruby: x.is_a?(Numeric)
来源：http://iex.daria6918.cn

C#:   x is int or double or decimal
来源：http://acn.gogol.net.cn

[B14] 判断值是否在集合内
来源：http://dpo.hcnkem.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xpm.yfazqb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hqf.tian-w.cn

JS:   [1, 2, 3].includes(x)
来源：http://vha.bjfxy.top

TS:   [1, 2, 3].includes(x)
来源：http://zue.jyoumei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gea.kuanghao11.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tuv.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xxq.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://waf.yangfankeji.com

[B15] 布尔运算与取反
来源：http://myy.ppjwa.cn

Py:   a and b or not c
来源：http://miu.guannengcc.top

PHP:  $a && $b || !$c
来源：http://sjz.feifeiyinyue.top

JS:   a && b || !c
来源：http://xdk.pycfn.com

TS:   a && b || !c
来源：http://wtx.aibaodan.cn

Java: a && b || !c
来源：http://hgj.ywan-chungtsiang.top

Go:   a && b || !c
来源：http://bgg.svipenyu.cn

Ruby: a && b || !c
来源：http://akn.yueranfly.top

C#:   a && b || !c
来源：http://wme.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://fjy.aizwys.cn

Py:   if not data: return
来源：http://ssj.tianlin.xyz

PHP:  if (!$data) { return; }
来源：http://qxq.c1oappe.top

JS:   if (!data) return;
来源：http://fbw.zdbjq.cn

TS:   if (!data) return;
来源：http://sow.ctjpmb.com

Java: if (data == null) return;
来源：http://epa.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://tvv.jyoumei.cn

Ruby: return if data.nil?
来源：http://uaa.gogol.net.cn

C#:   if (data == null) return;
来源：http://emf.redwolf501.top

================================================================================
来源：http://qry.smart0.xyz

C. 函数与作用域
来源：http://dhn.c1oappe.top

================================================================================
来源：http://kne.nanxinkj.top

[C01] 定义函数
来源：http://ukb.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://pav.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vez.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://mhs.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dnk.xuanzx.com

Java: static int add(int a, int b) { return a + b; }
来源：http://soy.sxryk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pbq.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://syq.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ppo.zhoulong.xyz

[C02] 默认参数
来源：http://cma.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://fmt.iojbl.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://olb.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://hrx.hammf.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zss.tanke756.top

Java: // 无默认参数：方法重载或 Optional
来源：http://juq.52xcode.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xpv.hongshengwenyu.top

Ruby: def greet(name = "World") = name
来源：http://xgw.sufxvd.cn

C#:   string Greet(string name = "World") => name;
来源：http://zjk.zhongyouzk.top

[C03] 可变参数
来源：http://okv.yongpay.top

Py:   def total(*args): return sum(args)
来源：http://slb.wangdashe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://flo.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://znp.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qzh.iojbl.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lth.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yrv.xuanzx.com

Ruby: def total(*nums); nums.sum; end
来源：http://ekz.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://srr.zhijiandao.cn

[C04] 命名参数 / 关键字参数
来源：http://svf.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yda.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ufp.sxryk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iws.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qjo.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://tzk.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://wza.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://cfk.sweek.top

C#:   f(a: 1, b: 2)
来源：http://mch.xinyue.icu

[C05] 返回多个值
来源：http://jcu.hnqzz.top

Py:   return a, b
来源：http://fxy.gzhubu.top

PHP:  return [$a, $b];
来源：http://sgo.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yeo.shzxlz.cn

TS:   return { a, b };
来源：http://lji.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://enm.shanyushiyangkeji.top

Go:   return a, b
来源：http://sqo.hammf.cn

Ruby: return a, b
来源：http://ktu.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://hro.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://rxl.snrcjt.cn

Py:   square = lambda x: x * x
来源：http://cwd.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rvv.dianchejie.cn

JS:   const square = x => x * x;
来源：http://nmj.jlsjyb.cn

TS:   const square = (x: number): number => x * x;
来源：http://aeo.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jup.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://eam.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://ygf.aizwys.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rao.sysykeji.top

[C07] 把函数作为参数传入
来源：http://jcu.shanyushiyangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ane.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://yhq.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yuq.iojbl.cn

TS:   arr.map(String)
来源：http://rnq.52xcode.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oat.hnqzz.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iiy.fehbvm.com

Ruby: arr.map(&:upcase)
来源：http://nxe.ctjpmb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://yks.cucudq.cn

[C08] 闭包
来源：http://vge.zhiwuduotai.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jpx.316326.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://esd.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://piz.fktsv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://spe.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mhj.daria6918.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fon.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dhr.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://osf.guowangkeji.top

[C09] 递归
来源：http://hze.cqqwz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mlj.havefunace.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ojb.hfpthk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://igk.ppjwa.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pkx.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nqo.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ech.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sbv.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qwa.jyoumei.cn

[C10] 变量作用域
来源：http://khs.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dka.nanxuanxn.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://non.fktsv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fml.hysaishi.cn

TS:   同 JS
来源：http://jtx.epnwcf.com

Java: 方法内为块级作用域
来源：http://tcu.zdbjq.cn

Go:   花括号块级作用域
来源：http://kmc.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://apt.haohaochexian.top

C#:   块级作用域
来源：http://dme.yj202588.top

[C11] 模块导入与导出
来源：http://uae.guannengcc.top

Py:   from module import func
来源：http://uxh.jqgufenzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ctt.chenlongwang.top


<!-- 参考信息 -->