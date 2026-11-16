代发 wailian999

JS:   [a, b] = [b, a];
来源：http://zcr.316326.xyz

TS:   [a, b] = [b, a];
来源：http://jsl.xingfuxueyuan.xyz

Java: int t = a; a = b; b = t;
来源：http://tpp.daria6918.cn

Go:   a, b = b, a
来源：http://tcy.dashuyun.cn

Ruby: a, b = b, a
来源：http://vzu.smart0.xyz

C#:   (a, b) = (b, a);
来源：http://kih.shangyingyoupin.top

[A20] 读取标准输入
来源：http://zfr.316326.xyz

Py:   name = input("请输入：")
来源：http://iay.hnqzz.top

PHP:  $name = trim(fgets(STDIN));
来源：http://lel.sjlbkw.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rxk.yuanzhike.top

TS:   // Node.js：readline 模块
来源：http://glc.sjlbkw.cn

Java: new Scanner(System.in).nextLine()
来源：http://qxx.epnwcf.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xgi.hywenlv.cn

Ruby: gets.chomp
来源：http://bfy.havefunace.top

C#:   Console.ReadLine();
来源：http://bip.gzhubu.top

[A21] 保留指定小数位输出
来源：http://siw.cqqwz.cn

Py:   f"{3.14159:.2f}"
来源：http://uwf.tianlin.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ueb.zhaomingkeji.xyz

JS:   (3.14159).toFixed(2)
来源：http://ark.xziqi.cn

TS:   (3.14159).toFixed(2)
来源：http://rsx.quarkkingdee.top

Java: String.format("%.2f", 3.14159)
来源：http://ghj.bbcook.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dvo.uphjek.com

Ruby: format("%.2f", 3.14159)
来源：http://wdm.meibo888.top

C#:   3.14159.ToString("F2")
来源：http://spo.52xcode.cn

[A22] 获取字符串长度
来源：http://dxt.pycfn.com

Py:   len(s)
来源：http://lgj.ivvv.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ufh.sweek.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mqb.mhx1999.top

TS:   s.length
来源：http://xzw.chenlongwang.top

Java: s.length()
来源：http://yne.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sje.ywan-chungtsiang.top

Ruby: s.length
来源：http://qwr.yvedp.cn

C#:   s.Length
来源：http://bsh.xingfuxueyuan.xyz

[A23] 大小写转换
来源：http://ygn.pengpengdd.cyou

Py:   s.upper(); s.lower(); s.title()
来源：http://ymd.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ibs.sxryk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yim.zdbjq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rcu.yonumen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wmg.chenlongwang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://voo.wangshuangyany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gfw.sysykeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://cet.316326.xyz

[A24] 去除首尾空白
来源：http://aiq.chenlongwang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xrt.xuanzx.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://orb.jianghu66.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dyq.tanke756.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xkh.bjfxy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oux.jinqigfzy.top

Go:   strings.TrimSpace(s)
来源：http://anc.yj20258.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://glz.ehwqpu.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lbg.smart0.xyz

[A25] 字符串比较
来源：http://gfl.feifeiyinyue.top

Py:   s1 == s2; s1 != s2
来源：http://tta.birdmap.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://txn.c1oappe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mjt.fanxiaobao.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://twq.yueranfly.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cnq.shanyushiyangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gyf.jianghu66.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wen.ctjpmb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ump.zhongyouzk.top

[A26] 类型转换总览
来源：http://kue.ybcxt.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hdq.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tep.ybcxt.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ery.jyoumei.cn

TS:   Number() String() Boolean() x as number
来源：http://ror.cashguo.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uyi.iojbl.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zbt.hesvh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sfs.ydzc1.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dab.jlsjyb.cn

================================================================================
来源：http://uxo.fktsv.cn

B. 流程控制
来源：http://zrt.zhoulong.xyz

================================================================================
来源：http://zmy.yonumen.top

[B01] 条件判断 if / else
来源：http://uxh.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://xjv.jinqigufen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fuu.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ogs.zhoulong.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ffw.cqqwz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sri.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://muz.shuidangran.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ist.jiagoushi.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ppz.yongpay.top

[B02] 多分支 else if / elif
来源：http://qmy.hcnkem.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://czz.sysykeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lvd.pycfn.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://frz.tian-w.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xer.ydjk.org.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://osm.zhaomingkeji.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://afx.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nfq.zycfv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://glh.daxiang520.top

[B03] switch / match / case
来源：http://hue.tanke756.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tyo.ctjpmb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yuk.cucudq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dke.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wzn.zdbjq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ohr.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nhm.yj20258.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tgt.dashuyun.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mlx.meibo888.top

[B04] for 计数循环
来源：http://bkv.meibo888.top

Py:   for i in range(10): print(i)
来源：http://nxh.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mpv.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qge.daria6918.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vzs.redwolf501.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lnp.hfpthk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wkp.tian-w.cn

Ruby: 10.times { |i| puts i }
来源：http://jqq.kuanghao11.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ufd.fehbvm.com

[B05] 遍历数组 / 列表
来源：http://nok.yueranfly.top

Py:   for item in arr: print(item)
来源：http://fti.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hee.wangdashe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ifo.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hyq.cheryme.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yep.haohaochexian.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nxx.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://knn.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hkj.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://bsr.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://ohy.hnxiangtu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nrh.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ryb.yueranfly.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://afp.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wkl.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uda.yongpay.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fmd.guannengcc.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jmx.zhiwuduotai.top

[B07] while 循环
来源：http://ftz.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://qeo.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://itx.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://oiv.ydjk.org.cn

TS:   while (i < 10) { i++; }
来源：http://gsk.iojbl.cn

Java: while (i < 10) { i++; }
来源：http://sky.mhx1999.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ees.nanxuanxn.top

Ruby: while i < 10; i += 1; end
来源：http://kgt.nanxuanxn.top

C#:   while (i < 10) { i++; }
来源：http://ifi.tanke756.top

[B08] do-while（至少执行一次）
来源：http://xge.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://lsj.sjlbkw.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xml.cucudq.cn

JS:   do { i++; } while (i < 10);
来源：http://hqq.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://tej.jlsjyb.cn

Java: do { i++; } while (i < 10);
来源：http://xrl.daria6918.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vmr.c1oappe.top

Ruby: begin; i += 1; end while i < 10
来源：http://ukq.jinqigufen.top

C#:   do { i++; } while (i < 10);
来源：http://fhx.xylfe.cn

[B09] break 与 continue
来源：http://kvl.0kj1m.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yzd.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pdu.ctjpmb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uco.vehdjk.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kex.hesvh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xrr.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qis.cheryme.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tyz.snrcjt.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ibx.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://ohr.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zqd.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ujx.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uqg.cheryme.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iut.bjfxy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xku.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://llz.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wgj.pycfn.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hug.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://msf.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://umn.daxiang520.top

PHP:  range(0, 10, 2);
来源：http://xjb.zdqjudy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lje.52xcode.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qbe.guannengcc.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eem.ctjpmb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ihr.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://bip.yuanzhike.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eeo.aibaodan.cn

[B12] 跳出多层循环
来源：http://fyd.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://ftk.sjlbkw.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://btq.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mhl.hywenlv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uev.redwolf501.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://txd.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eky.cashguo.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ows.shanyushiyangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bpd.ydzc1.top

[B13] 判断是否为数字
来源：http://aor.mhx1999.top

Py:   isinstance(x, (int, float))
来源：http://wfr.yuxming.cn

PHP:  is_numeric($x)
来源：http://bcn.c1oappe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yqh.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mmr.chenzaomai.com

Java: x instanceof Number
来源：http://ugq.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yec.sysykeji.top

Ruby: x.is_a?(Numeric)
来源：http://wwo.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://tmn.jinqigfzy.top

[B14] 判断值是否在集合内
来源：http://jxb.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xao.dianchejie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nqd.zhengqikj.top

JS:   [1, 2, 3].includes(x)
来源：http://nlm.dashuyun.cn

TS:   [1, 2, 3].includes(x)
来源：http://dpz.guowangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fle.uphjek.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xbr.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://chy.chenzaomai.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://acn.nanxinkj.top

[B15] 布尔运算与取反
来源：http://isr.hywenlv.cn

Py:   a and b or not c
来源：http://oum.hfpthk.cn

PHP:  $a && $b || !$c
来源：http://wnn.hnxiangtu.top

JS:   a && b || !c
来源：http://zam.svipenyu.cn

TS:   a && b || !c
来源：http://ldg.ydzc1.top

Java: a && b || !c
来源：http://eng.jinghuilouyu.cn

Go:   a && b || !c
来源：http://hfi.ybcxt.top

Ruby: a && b || !c
来源：http://thz.cashguo.top

C#:   a && b || !c
来源：http://vww.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://uvg.havefunace.top

Py:   if not data: return
来源：http://mvs.shzxlz.cn

PHP:  if (!$data) { return; }
来源：http://ybp.pycfn.com

JS:   if (!data) return;
来源：http://egp.iojbl.cn

TS:   if (!data) return;
来源：http://vld.gzhubu.top

Java: if (data == null) return;
来源：http://txp.ehwqpu.com

Go:   if data == nil { return }
来源：http://bej.aizwys.cn

Ruby: return if data.nil?
来源：http://sfu.svipenyu.cn

C#:   if (data == null) return;
来源：http://otv.xinyue.icu

================================================================================
来源：http://xdt.sweek.top

C. 函数与作用域
来源：http://rry.ivvv.top

================================================================================
来源：http://waq.hnxiangtu.top

[C01] 定义函数
来源：http://zzx.9152youxi.cn

Py:   def add(a, b): return a + b
来源：http://rmd.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kxe.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://jbw.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lbc.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oyk.feifeiyinyue.top

Go:   func add(a, b int) int { return a + b }
来源：http://iww.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://zvc.chenjidiqi.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nrk.yvedp.cn

[C02] 默认参数
来源：http://yyl.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://ise.wangshuangyany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dse.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://ass.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lym.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uch.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tzv.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://ucd.fanxiaobao.xyz

C#:   string Greet(string name = "World") => name;
来源：http://qpf.jinqigfzy.top

[C03] 可变参数
来源：http://vvp.hesvh.cn

Py:   def total(*args): return sum(args)
来源：http://czy.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ken.yuanzhike.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://azq.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hfz.dashuyun.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gcq.yonumen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cst.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://nef.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hrn.xuetiantiany.cn

[C04] 命名参数 / 关键字参数
来源：http://gbu.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cyf.jqgfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nwu.yj20258888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gbj.jyoumei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://isb.daxiang520.top

Java: // 无：用 Builder 模式或 record
来源：http://kij.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://gpo.xylfe.cn

Ruby: f(a: 1, b: 2)
来源：http://bia.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://gkd.shanyushiyangtech.top

[C05] 返回多个值
来源：http://jen.yfazqb.com

Py:   return a, b
来源：http://sjm.tianlin.xyz

PHP:  return [$a, $b];
来源：http://wul.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ibg.hongshengwenyu.top

TS:   return { a, b };
来源：http://grq.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cyd.mhx1999.top

Go:   return a, b
来源：http://kwl.hnqzz.top

Ruby: return a, b
来源：http://hnt.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://bwr.jqgfzy.top

[C06] 匿名函数 / lambda
来源：http://rbw.jinqigufen.top

Py:   square = lambda x: x * x
来源：http://axb.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pdo.cdnleiting.top

JS:   const square = x => x * x;
来源：http://eox.jinqigufen.top

TS:   const square = (x: number): number => x * x;
来源：http://ceu.hysaishi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yvn.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://uwo.shanyushiyangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://smz.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://gga.jyoumei.cn

[C07] 把函数作为参数传入
来源：http://mty.daxiang520.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://czr.yuanzhike.top

PHP:  array_map("strtoupper", $arr);
来源：http://rrz.aibaodan.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qci.316326.xyz

TS:   arr.map(String)
来源：http://kpu.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nzq.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jja.sxryk.cn

Ruby: arr.map(&:upcase)
来源：http://dnt.xinyue.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://dpo.gogol.net.cn

[C08] 闭包
来源：http://mbl.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qbf.fanxiaobao.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tzd.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xmv.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cjm.zhongyouzk.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tfm.yueranfly.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ksy.bbcook.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mpa.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rpi.xingfuxueyuan.xyz

[C09] 递归
来源：http://axs.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://paa.pengpengdd.cyou

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kcx.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sii.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aex.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kow.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mma.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pbh.kuanghao11.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hgx.aizwys.cn


<!-- 参考信息 -->