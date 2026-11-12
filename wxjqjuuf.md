代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zei.52xcode.cn

Java: (int) 'A'; (char) 65
来源：http://kjc.zhijiandao.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://grl.shangyingyoupin.top

Ruby: "A".ord; 65.chr
来源：http://ngy.jinqigufen.top

C#:   (int)'A'; (char)65
来源：http://bkb.jianghu66.top

[A19] 交换两个变量
来源：http://uwa.tian-w.cn

Py:   a, b = b, a
来源：http://kjo.ywan-chungtsiang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ywg.shanyushiyangkeji.top

JS:   [a, b] = [b, a];
来源：http://dxt.shanyushiyangtech.top

TS:   [a, b] = [b, a];
来源：http://miz.yangfankeji.com

Java: int t = a; a = b; b = t;
来源：http://pne.pengpengdd.cyou

Go:   a, b = b, a
来源：http://gnw.yuanzhike.top

Ruby: a, b = b, a
来源：http://ybn.quarkkingdee.top

C#:   (a, b) = (b, a);
来源：http://hur.nanxinkj.top

[A20] 读取标准输入
来源：http://jkp.shangyingyoupin.top

Py:   name = input("请输入：")
来源：http://xoj.fktsv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ofj.hesvh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ylz.wangshuangyany.cn

TS:   // Node.js：readline 模块
来源：http://zso.yj202588.top

Java: new Scanner(System.in).nextLine()
来源：http://ivc.kuanghao11.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vih.zhiwuduotai.top

Ruby: gets.chomp
来源：http://iib.tianlin.xyz

C#:   Console.ReadLine();
来源：http://agd.zhengqikj.top

[A21] 保留指定小数位输出
来源：http://ejy.zhongyouzk.top

Py:   f"{3.14159:.2f}"
来源：http://wcy.yj20258.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bkn.ywan-chungtsiang.top

JS:   (3.14159).toFixed(2)
来源：http://nhv.yfazqb.com

TS:   (3.14159).toFixed(2)
来源：http://ttc.sxryk.cn

Java: String.format("%.2f", 3.14159)
来源：http://xpl.c1oappe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yzx.c1oappe.top

Ruby: format("%.2f", 3.14159)
来源：http://akt.fktsv.cn

C#:   3.14159.ToString("F2")
来源：http://wzx.cashguo.top

[A22] 获取字符串长度
来源：http://uqa.cdnleiting.top

Py:   len(s)
来源：http://gna.dianchejie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rzx.hongshengwenyu.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wtm.pycfn.com

TS:   s.length
来源：http://wqm.vehdjk.com

Java: s.length()
来源：http://bzn.sjlbkw.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jsb.ydjk.org.cn

Ruby: s.length
来源：http://gqy.yj20258888.top

C#:   s.Length
来源：http://tbs.havefunace.top

[A23] 大小写转换
来源：http://kfl.cheryme.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gvl.xylfe.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://foi.c1oappe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ojf.zhijiandao.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vyz.yongpay.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fqo.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://efr.hammf.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://knh.sjlbkw.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lus.52xcode.cn

[A24] 去除首尾空白
来源：http://ukm.epnwcf.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cdc.tian-w.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ekp.gzhubu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lxw.shanyushiyangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jsj.316326.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nhl.c1oappe.top

Go:   strings.TrimSpace(s)
来源：http://apl.redwolf501.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lay.yongpay.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://urq.havefunace.top

[A25] 字符串比较
来源：http://wur.sweek.top

Py:   s1 == s2; s1 != s2
来源：http://gim.pycfn.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vjg.jlsjyb.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hov.hnxiangtu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pmf.zhijiandao.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gmm.shanyushiyangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kgs.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://sja.haohaochexian.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tdg.pengpengdd.cyou

[A26] 类型转换总览
来源：http://pnl.zycfv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sar.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ulq.gzhubu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jzc.ctjpmb.com

TS:   Number() String() Boolean() x as number
来源：http://ijy.shanyushiyangtech.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wsa.redwolf501.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hvs.gogol.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qiz.gogol.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rbs.nanxinkj.top

================================================================================
来源：http://iwd.snrcjt.cn

B. 流程控制
来源：http://loq.gzhubu.top

================================================================================
来源：http://rbo.jinghuilouyu.cn

[B01] 条件判断 if / else
来源：http://kcn.xylfe.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pok.jyoumei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://stq.jiagoushi.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oye.havefunace.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qer.bjfxy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zyi.vqdsnc.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xla.jinqigufen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oyp.ctjpmb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jkw.feifeiyinyue.top

[B02] 多分支 else if / elif
来源：http://mfk.jqgufenzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qbr.aibaodan.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mec.dashuyun.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dcw.zhengqikj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qab.wangdashe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://egf.52xcode.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://etg.shuidangran.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yfl.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://srg.cucudq.cn

[B03] switch / match / case
来源：http://emg.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://moq.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://klw.cucudq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gbt.xuanzx.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tnh.zdqjudy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oos.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ttt.zhaomingkeji.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ykb.quarkkingdee.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ogk.hywenlv.cn

[B04] for 计数循环
来源：http://yyt.fktsv.cn

Py:   for i in range(10): print(i)
来源：http://cvp.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rey.fehbvm.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hrf.daria6918.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://prt.fehbvm.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oin.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ewj.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://jiu.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mwq.bbcook.cn

[B05] 遍历数组 / 列表
来源：http://ilc.ehwqpu.com

Py:   for item in arr: print(item)
来源：http://kgz.hnxiangtu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jgj.havefunace.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zrd.havefunace.top

TS:   for (const item of arr) { console.log(item); }
来源：http://eyu.tarul.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hzm.jianghu66.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lup.hfpthk.cn

Ruby: arr.each { |item| puts item }
来源：http://low.tanke756.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ytx.jqgfzy.top

[B06] 遍历字典 / 对象
来源：http://rla.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dki.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zdc.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xus.zdqjudy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tgv.vehdjk.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ghx.wangdashe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yxq.tianlin.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wyg.nwbrower.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gkw.yj20258.top

[B07] while 循环
来源：http://yur.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://ell.gzhubu.top

PHP:  while ($i < 10) { $i++; }
来源：http://trc.nanxuanxn.top

JS:   while (i < 10) { i++; }
来源：http://ikv.aibaodan.cn

TS:   while (i < 10) { i++; }
来源：http://tuj.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://euv.vehdjk.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ekx.quarkkingdee.top

Ruby: while i < 10; i += 1; end
来源：http://ymt.jlsjyb.cn

C#:   while (i < 10) { i++; }
来源：http://drz.bjfxy.top

[B08] do-while（至少执行一次）
来源：http://uys.xinyue.icu

Py:   # 无 do-while：用 while True + break
来源：http://max.hcnkem.com

PHP:  do { $i++; } while ($i < 10);
来源：http://bnx.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://mey.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://xfu.meibo888.top

Java: do { i++; } while (i < 10);
来源：http://cfc.tarul.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://inf.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://rfl.jianghu66.top

C#:   do { i++; } while (i < 10);
来源：http://lfq.wangdashe.top

[B09] break 与 continue
来源：http://hdl.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://two.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uzw.guannengcc.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ydt.cheryme.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://olf.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wal.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://trm.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gxy.hysaishi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ywu.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://ais.guowangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wiu.gotoacloud.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nkd.kuanghao11.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aar.zdqjudy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jyp.snrcjt.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://plq.sjlbkw.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jnb.gotoacloud.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zau.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nmo.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://xpo.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://kun.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://yir.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cgp.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://neo.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fgw.yj202588.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hmt.xinyue.icu

Ruby: (0...10).step(2).to_a
来源：http://uap.ctjpmb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lkb.chenzaomai.com

[B12] 跳出多层循环
来源：http://siz.yuxming.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bjp.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cdn.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ogu.chenjidiqi.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bzj.fehbvm.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://upv.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vuf.ctjpmb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zlf.wangshuangyany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yvm.tian-w.cn

[B13] 判断是否为数字
来源：http://gqk.xziqi.cn

Py:   isinstance(x, (int, float))
来源：http://ktu.fzhhl.top

PHP:  is_numeric($x)
来源：http://lyo.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pvs.tanke756.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mru.ydjk.org.cn

Java: x instanceof Number
来源：http://iqk.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dvy.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://knl.316326.xyz

C#:   x is int or double or decimal
来源：http://fls.tarul.cn

[B14] 判断值是否在集合内
来源：http://kya.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eqg.chenlongwang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gvp.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://sqe.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://kgp.andypj.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://vil.cqqwz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://miw.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://xnk.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ovf.cucudq.cn

[B15] 布尔运算与取反
来源：http://ucd.sysykeji.top

Py:   a and b or not c
来源：http://xpt.fktsv.cn

PHP:  $a && $b || !$c
来源：http://pju.aizwys.cn

JS:   a && b || !c
来源：http://yix.shanyushiyangtech.top

TS:   a && b || !c
来源：http://kvj.vehdjk.com

Java: a && b || !c
来源：http://icb.pycfn.com

Go:   a && b || !c
来源：http://njr.sweek.top

Ruby: a && b || !c
来源：http://kov.cucudq.cn

C#:   a && b || !c
来源：http://kbu.yj20258.top

[B16] 卫语句：不满足条件提前返回
来源：http://kgj.yfazqb.com

Py:   if not data: return
来源：http://zbl.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://awg.chenjidiqi.icu

JS:   if (!data) return;
来源：http://pel.ehwqpu.com

TS:   if (!data) return;
来源：http://utn.zhiwuduotai.top

Java: if (data == null) return;
来源：http://byr.mhx1999.top

Go:   if data == nil { return }
来源：http://ogc.yanxiufei.cn

Ruby: return if data.nil?
来源：http://scs.xinyue.icu

C#:   if (data == null) return;
来源：http://vbw.jinyuanbaomall.cn

================================================================================
来源：http://rbx.shzxlz.cn

C. 函数与作用域
来源：http://uvw.hywenlv.cn

================================================================================
来源：http://qst.chenlongwang.top

[C01] 定义函数
来源：http://rpi.nwbrower.top

Py:   def add(a, b): return a + b
来源：http://fvm.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xtg.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://ynp.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://grv.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zws.hongshengwenyu.top

Go:   func add(a, b int) int { return a + b }
来源：http://pan.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://icv.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gzv.xuanzx.com

[C02] 默认参数
来源：http://xxl.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://wgp.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fgx.ehwqpu.com

JS:   function greet(name = "World") { return name; }
来源：http://sjl.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ayu.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://lza.sjlbkw.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kys.birdmap.top

Ruby: def greet(name = "World") = name
来源：http://ocr.zhixingplan.top

C#:   string Greet(string name = "World") => name;
来源：http://xus.ydjk.org.cn

[C03] 可变参数
来源：http://jfm.yongpay.top

Py:   def total(*args): return sum(args)
来源：http://kgs.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pan.shzxlz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gcd.shangyingyoupin.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iwc.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zci.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ahn.svipenyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vpq.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jhb.gotoacloud.top

[C04] 命名参数 / 关键字参数
来源：http://ngo.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mjx.jlsjyb.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://idb.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cxv.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://huz.pycfn.com

Java: // 无：用 Builder 模式或 record
来源：http://oks.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://twr.daxiang520.top

Ruby: f(a: 1, b: 2)
来源：http://ykh.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://ikp.yfazqb.com

[C05] 返回多个值
来源：http://ikt.hysaishi.cn

Py:   return a, b
来源：http://rff.c1oappe.top

PHP:  return [$a, $b];
来源：http://saf.ydzc1.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mfg.ywan-chungtsiang.top

TS:   return { a, b };
来源：http://zyv.gotoacloud.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://seg.tarul.cn

Go:   return a, b
来源：http://lfi.xylfe.cn

Ruby: return a, b
来源：http://khc.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://tde.guannengcc.top

[C06] 匿名函数 / lambda
来源：http://qbk.hnqzz.top

Py:   square = lambda x: x * x
来源：http://tcy.guannengcc.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kaa.gzhubu.top

JS:   const square = x => x * x;
来源：http://oby.chenlongwang.top

TS:   const square = (x: number): number => x * x;
来源：http://brj.jiagoushi.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zcv.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://fgk.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://das.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ktg.tarul.cn

[C07] 把函数作为参数传入
来源：http://leo.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xnt.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://hno.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://urx.zhengqikj.top

TS:   arr.map(String)
来源：http://jow.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zfa.wangshuangyany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://viv.iojbl.cn

Ruby: arr.map(&:upcase)
来源：http://xwt.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bqz.bbcook.cn

[C08] 闭包
来源：http://vwi.jqgfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hcz.fehbvm.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wuh.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yiu.jinyuanbaomall.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bhh.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vaa.aizwys.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://svh.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kbd.aibaodan.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bcl.hnxiangtu.top

[C09] 递归
来源：http://kce.zdqjudy.top


<!-- 参考信息 -->