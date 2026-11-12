代发 wailian999

Ruby: a, b = b, a
来源：http://uco.shangyingyoupin.top

C#:   (a, b) = (b, a);
来源：http://baa.yuanzhike.top

[A20] 读取标准输入
来源：http://ama.shanyushiyangtech.top

Py:   name = input("请输入：")
来源：http://ixt.gotoacloud.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bkc.wangshuangyany.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rpt.cashguo.top

TS:   // Node.js：readline 模块
来源：http://owq.chenjidiqi.icu

Java: new Scanner(System.in).nextLine()
来源：http://wwq.shanyushiyangkeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bma.yanxiufei.cn

Ruby: gets.chomp
来源：http://kwh.fanxiaobao.xyz

C#:   Console.ReadLine();
来源：http://vou.bjfxy.top

[A21] 保留指定小数位输出
来源：http://tgv.gzhubu.top

Py:   f"{3.14159:.2f}"
来源：http://ahj.jyoumei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ald.birdmap.top

JS:   (3.14159).toFixed(2)
来源：http://mfn.52xcode.cn

TS:   (3.14159).toFixed(2)
来源：http://zpg.tarul.cn

Java: String.format("%.2f", 3.14159)
来源：http://ogc.ydjk.org.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://aqd.gaohongyu789.top

Ruby: format("%.2f", 3.14159)
来源：http://mad.ehwqpu.com

C#:   3.14159.ToString("F2")
来源：http://kqh.daria6918.cn

[A22] 获取字符串长度
来源：http://gay.shuidangran.top

Py:   len(s)
来源：http://wgf.9152youxi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fqt.yangfankeji.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bbx.cashguo.top

TS:   s.length
来源：http://rvg.yj202588.top

Java: s.length()
来源：http://cnl.ehwqpu.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jyl.316326.xyz

Ruby: s.length
来源：http://wgy.tanke756.top

C#:   s.Length
来源：http://frq.hysaishi.cn

[A23] 大小写转换
来源：http://mmr.yangfankeji.com

Py:   s.upper(); s.lower(); s.title()
来源：http://icr.vehdjk.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xae.daria6918.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mbc.tianlin.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lyi.pengpengdd.cyou

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sen.jqgfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hnr.fanxiaobao.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ayr.xziqi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pts.nanxuanxn.top

[A24] 去除首尾空白
来源：http://rlg.svipenyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jcr.meibo888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uqs.zhiwuduotai.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://skv.sweek.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://klp.haohaochexian.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gnh.birdmap.top

Go:   strings.TrimSpace(s)
来源：http://jem.xuanzx.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ysy.tanke756.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sur.redwolf501.top

[A25] 字符串比较
来源：http://ukt.redwolf501.top

Py:   s1 == s2; s1 != s2
来源：http://ntg.bbcook.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xwq.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zhx.vehdjk.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fsf.epnwcf.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mgo.yanxiufei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jxx.tanke756.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qdw.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://shy.smart0.xyz

[A26] 类型转换总览
来源：http://svp.shuidangran.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zxi.316326.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zfz.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ybk.cheryme.top

TS:   Number() String() Boolean() x as number
来源：http://ktt.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bpr.zhoulong.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tfb.iojbl.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yki.hywenlv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://haj.guannengcc.top

================================================================================
来源：http://pvx.pengpengdd.cyou

B. 流程控制
来源：http://xzy.bbcook.cn

================================================================================
来源：http://zem.yangfankeji.com

[B01] 条件判断 if / else
来源：http://uqv.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ukt.yvedp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oxz.316326.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uiw.hfpthk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sfu.zhixingplan.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hfu.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ijx.gogol.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yvw.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zlm.fehbvm.com

[B02] 多分支 else if / elif
来源：http://dac.zycfv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cac.yj20258.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zyr.c1oappe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://azu.fehbvm.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tpt.feifeiyinyue.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kwn.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://efj.havefunace.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dqh.cdnleiting.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://igy.haohaochexian.top

[B03] switch / match / case
来源：http://uvh.tianlin.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ytr.ydjk.org.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wvo.jinghuilouyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qws.zhixingplan.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ehm.yj202588.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ewk.snrcjt.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nze.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ouv.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dre.birdmap.top

[B04] for 计数循环
来源：http://bhg.gaohongyu789.top

Py:   for i in range(10): print(i)
来源：http://mxd.hfpthk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rsq.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hvz.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yzh.smart0.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vlk.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wku.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://ymp.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://djc.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://awh.yj20258888.top

Py:   for item in arr: print(item)
来源：http://biz.sufxvd.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yzl.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://skr.ywan-chungtsiang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xex.52xcode.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rqr.jqgfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tsj.uphjek.com

Ruby: arr.each { |item| puts item }
来源：http://gsf.gogol.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dir.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://tde.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ecw.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://erf.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://znj.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gps.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://afb.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dfu.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jei.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gfm.dashuyun.cn

[B07] while 循环
来源：http://ayq.hongshengwenyu.top

Py:   while i < 10: i += 1
来源：http://qlo.yfazqb.com

PHP:  while ($i < 10) { $i++; }
来源：http://xlk.zycfv.cn

JS:   while (i < 10) { i++; }
来源：http://ifq.wangdashe.top

TS:   while (i < 10) { i++; }
来源：http://fkd.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://prx.nanxinkj.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fnw.cheryme.top

Ruby: while i < 10; i += 1; end
来源：http://dyp.zycfv.cn

C#:   while (i < 10) { i++; }
来源：http://sws.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://zdk.cdnleiting.top

Py:   # 无 do-while：用 while True + break
来源：http://oxg.zycfv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://swh.jqgufenzy.top

JS:   do { i++; } while (i < 10);
来源：http://sgu.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://xkg.fengsongda.top

Java: do { i++; } while (i < 10);
来源：http://mph.quarkkingdee.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jkq.daria6918.cn

Ruby: begin; i += 1; end while i < 10
来源：http://imf.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://lae.zhengqikj.top

[B09] break 与 continue
来源：http://fkv.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://knl.snrcjt.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gid.meibo888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uvn.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ayq.snrcjt.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gzv.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yqt.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mwg.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nvv.tian-w.cn

[B10] 遍历同时拿索引
来源：http://pkb.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xda.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tvg.yanxiufei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://djk.havefunace.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://axq.bjfxy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nof.haohaochexian.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zyr.yonumen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://isw.shzxlz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nkq.havefunace.top

[B11] 生成数字序列 / 区间
来源：http://vmw.hywenlv.cn

Py:   list(range(0, 10, 2))
来源：http://fdp.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://zld.vqdsnc.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gvl.gotoacloud.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dfp.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://frm.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://erp.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://wwr.jinqigfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oxo.quarkkingdee.top

[B12] 跳出多层循环
来源：http://osk.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://grz.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jxg.yuxming.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://znp.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qdw.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yvb.zhongyouzk.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://msj.xuetiantiany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sle.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ebg.ehwqpu.com

[B13] 判断是否为数字
来源：http://gqh.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://uhn.zhaomingkeji.xyz

PHP:  is_numeric($x)
来源：http://iri.cdnleiting.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dsg.jyoumei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ttq.tarul.cn

Java: x instanceof Number
来源：http://zlz.vehdjk.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ahn.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://mij.jqgfzy.top

C#:   x is int or double or decimal
来源：http://ove.jianghu66.top

[B14] 判断值是否在集合内
来源：http://plq.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jmz.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mso.uphjek.com

JS:   [1, 2, 3].includes(x)
来源：http://iln.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://hea.chenjidiqi.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://qyz.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://afc.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://our.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://urw.chenjidiqi.icu

[B15] 布尔运算与取反
来源：http://omr.shzxlz.cn

Py:   a and b or not c
来源：http://vpq.chenzaomai.com

PHP:  $a && $b || !$c
来源：http://qkm.hywenlv.cn

JS:   a && b || !c
来源：http://itd.yangfankeji.com

TS:   a && b || !c
来源：http://ugr.redwolf501.top

Java: a && b || !c
来源：http://fep.chenzaomai.com

Go:   a && b || !c
来源：http://zyj.jqgfzy.top

Ruby: a && b || !c
来源：http://tqr.0kj1m.cn

C#:   a && b || !c
来源：http://zye.cdnleiting.top

[B16] 卫语句：不满足条件提前返回
来源：http://uip.yuanzhike.top

Py:   if not data: return
来源：http://tzb.sweek.top

PHP:  if (!$data) { return; }
来源：http://ylu.cashguo.top

JS:   if (!data) return;
来源：http://efb.hcnkem.com

TS:   if (!data) return;
来源：http://oui.xuetiantiany.cn

Java: if (data == null) return;
来源：http://vbu.vehdjk.com

Go:   if data == nil { return }
来源：http://twy.shuidangran.top

Ruby: return if data.nil?
来源：http://ppw.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://xrc.jqgufenzy.top

================================================================================
来源：http://llw.dashuyun.cn

C. 函数与作用域
来源：http://gla.meibo888.top

================================================================================
来源：http://wdb.zhaomingkeji.xyz

[C01] 定义函数
来源：http://htn.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://hlj.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sdw.jqgufenzy.top

JS:   function add(a, b) { return a + b; }
来源：http://wix.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mkx.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://biu.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://oav.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://kxo.jinyuanbaomall.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ude.kuanghao11.cn

[C02] 默认参数
来源：http://ihq.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://dpb.ybcxt.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kie.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://vng.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gvn.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://osy.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nia.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://itu.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://slb.andypj.xyz

[C03] 可变参数
来源：http://aci.gaohongyu789.top

Py:   def total(*args): return sum(args)
来源：http://amm.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jun.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xqb.yuxming.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://onh.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kfi.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ldw.aizwys.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lks.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eqs.dianchejie.cn

[C04] 命名参数 / 关键字参数
来源：http://bdk.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ybn.vqdsnc.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ete.xingfuxueyuan.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qfo.fzhhl.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hqx.ehwqpu.com

Java: // 无：用 Builder 模式或 record
来源：http://apn.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://ybo.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://bhm.redwolf501.top

C#:   f(a: 1, b: 2)
来源：http://afq.dashuyun.cn

[C05] 返回多个值
来源：http://jrk.mhx1999.top

Py:   return a, b
来源：http://ztq.zhoulong.xyz

PHP:  return [$a, $b];
来源：http://chv.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mdb.yangfankeji.com

TS:   return { a, b };
来源：http://onm.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bpz.yj20258.top

Go:   return a, b
来源：http://rsb.vqdsnc.cn

Ruby: return a, b
来源：http://bix.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://qeg.chenlongwang.top

[C06] 匿名函数 / lambda
来源：http://ytz.zdqjudy.top

Py:   square = lambda x: x * x
来源：http://fsh.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dud.zdbjq.cn

JS:   const square = x => x * x;
来源：http://hrw.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://zta.nanxuanxn.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hkg.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://akk.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://ddg.iojbl.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hpa.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://lwc.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://skm.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://jty.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mvu.fengsongda.top

TS:   arr.map(String)
来源：http://lhg.nanxinkj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pfi.shangyingyoupin.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jen.xuanzx.com

Ruby: arr.map(&:upcase)
来源：http://chw.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gji.chenjidiqi.icu

[C08] 闭包
来源：http://jwf.shzxlz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ttf.xuanzx.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ykt.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xdj.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cqq.ydjk.org.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zmd.guannengcc.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kqi.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oph.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xbj.yongpay.top

[C09] 递归
来源：http://ayk.hongshengwenyu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kmm.jinyuanbaomall.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pke.zhixingplan.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://red.xziqi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zqv.0kj1m.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://syk.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jvw.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vzk.hnxiangtu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mpc.pengpengdd.cyou

[C10] 变量作用域
来源：http://tuv.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ilp.jyoumei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fyl.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://scd.guannengcc.top


<!-- 参考信息 -->