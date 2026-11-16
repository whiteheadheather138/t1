代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://gct.c1oappe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qwt.cucudq.cn

TS:   // Node.js：readline 模块
来源：http://rhb.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://xph.kuanghao11.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xwh.gogol.net.cn

Ruby: gets.chomp
来源：http://ykz.gotoacloud.top

C#:   Console.ReadLine();
来源：http://law.svipenyu.cn

[A21] 保留指定小数位输出
来源：http://svu.316326.xyz

Py:   f"{3.14159:.2f}"
来源：http://xse.chenzaomai.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iga.zhijiandao.cn

JS:   (3.14159).toFixed(2)
来源：http://vmf.nanxinkj.top

TS:   (3.14159).toFixed(2)
来源：http://zcr.ybcxt.top

Java: String.format("%.2f", 3.14159)
来源：http://mpb.tianlin.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qqr.hywenlv.cn

Ruby: format("%.2f", 3.14159)
来源：http://peb.zycfv.cn

C#:   3.14159.ToString("F2")
来源：http://ewd.yuxming.cn

[A22] 获取字符串长度
来源：http://vfk.jinqigfzy.top

Py:   len(s)
来源：http://stn.ehwqpu.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qpm.yj202588.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hri.daxiang520.top

TS:   s.length
来源：http://fzo.shanyushiyangtech.top

Java: s.length()
来源：http://gze.jianghu66.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hwj.yuxming.cn

Ruby: s.length
来源：http://esc.jyoumei.cn

C#:   s.Length
来源：http://glg.tarul.cn

[A23] 大小写转换
来源：http://xyx.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uhs.chenjidiqi.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oey.gzhubu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hdo.daxiang520.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xez.hesvh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gpy.aibaodan.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pwy.meibo888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fqf.yangfankeji.com

C#:   s.ToUpper(); s.ToLower()
来源：http://qct.fzhhl.top

[A24] 去除首尾空白
来源：http://nen.birdmap.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rpd.dashuyun.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qib.yangfankeji.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xzt.zhixingplan.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fge.jiagoushi.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nik.ydzc1.top

Go:   strings.TrimSpace(s)
来源：http://ojm.jinqigfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tlg.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dis.guannengcc.top

[A25] 字符串比较
来源：http://zas.jyoumei.cn

Py:   s1 == s2; s1 != s2
来源：http://ocj.zhixingplan.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pow.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ixs.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dcg.zhaomingkeji.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xwe.hammf.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fjq.pycfn.com

Ruby: s1 == s2; s1 <=> s2
来源：http://osj.zycfv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gew.andypj.xyz

[A26] 类型转换总览
来源：http://ghw.ywan-chungtsiang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sjg.quarkkingdee.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nmk.cashguo.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xnf.316326.xyz

TS:   Number() String() Boolean() x as number
来源：http://qbq.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bnq.yj20258888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tzh.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kvo.jianghu66.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uqe.sysykeji.top

================================================================================
来源：http://kys.jinyuanbaomall.cn

B. 流程控制
来源：http://wnt.redwolf501.top

================================================================================
来源：http://tzj.zycfv.cn

[B01] 条件判断 if / else
来源：http://yzb.gzhubu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ave.dashuyun.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ayb.zhongyouzk.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vnv.aizwys.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rkd.xuetiantiany.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://osg.daria6918.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cmo.zdqjudy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gux.redwolf501.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iag.gaohongyu789.top

[B02] 多分支 else if / elif
来源：http://non.nanxinkj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fbo.9152youxi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://msk.ppjwa.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nrx.sxryk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ncc.chenjidiqi.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gfd.meibo888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hld.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lsl.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cwn.ivvv.top

[B03] switch / match / case
来源：http://nbl.aizwys.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://con.iojbl.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hww.fanxiaobao.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hpf.shangyingyoupin.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fle.nwbrower.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qny.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oki.jinqigufen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mma.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yps.aizwys.cn

[B04] for 计数循环
来源：http://kne.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://yeh.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://six.ydjk.org.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bra.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://izu.jinqigufen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ozc.xylfe.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qmt.snrcjt.cn

Ruby: 10.times { |i| puts i }
来源：http://dor.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qht.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://nhb.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://bfw.hongshengwenyu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rkn.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wls.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mkf.vqdsnc.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wdq.sufxvd.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://syn.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://qby.haohaochexian.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wwn.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://tzc.nanxinkj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yew.xuetiantiany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dnq.hfpthk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mzt.yj20258.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kgp.yuxming.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uod.xylfe.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xjl.mhx1999.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dkx.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gtu.9152youxi.cn

[B07] while 循环
来源：http://rni.chenzaomai.com

Py:   while i < 10: i += 1
来源：http://bmi.gaohongyu789.top

PHP:  while ($i < 10) { $i++; }
来源：http://gku.ehwqpu.com

JS:   while (i < 10) { i++; }
来源：http://yov.yj20258888.top

TS:   while (i < 10) { i++; }
来源：http://bis.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://yre.gzhubu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kwi.ppjwa.cn

Ruby: while i < 10; i += 1; end
来源：http://zlx.redwolf501.top

C#:   while (i < 10) { i++; }
来源：http://lse.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://bot.hysaishi.cn

Py:   # 无 do-while：用 while True + break
来源：http://aip.pengpengdd.cyou

PHP:  do { $i++; } while ($i < 10);
来源：http://oea.yonumen.top

JS:   do { i++; } while (i < 10);
来源：http://kzm.fehbvm.com

TS:   do { i++; } while (i < 10);
来源：http://wfi.bbcook.cn

Java: do { i++; } while (i < 10);
来源：http://nlr.zhoulong.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://cqp.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://yfr.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://hpn.cqqwz.cn

[B09] break 与 continue
来源：http://mho.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wos.fengsongda.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cgq.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://irt.shanyushiyangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://skm.yvedp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ynp.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ywl.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xqa.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jyn.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://aof.ydzc1.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://avn.hammf.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gyg.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pmq.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qqj.andypj.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hsk.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sqz.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dgz.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tmo.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://zbs.cqqwz.cn

Py:   list(range(0, 10, 2))
来源：http://lsk.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://ubh.kuanghao11.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zxx.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xus.52xcode.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rwn.yj20258.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zet.cucudq.cn

Ruby: (0...10).step(2).to_a
来源：http://qnq.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wzg.yuanzhike.top

[B12] 跳出多层循环
来源：http://ynk.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lcp.yonumen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://agm.nwbrower.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fjt.zhiwuduotai.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nim.zhaomingkeji.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ccr.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://srw.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xca.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jqs.zycfv.cn

[B13] 判断是否为数字
来源：http://vkf.yanxiufei.cn

Py:   isinstance(x, (int, float))
来源：http://sow.0kj1m.cn

PHP:  is_numeric($x)
来源：http://ryo.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wsn.snrcjt.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eyt.zhoulong.xyz

Java: x instanceof Number
来源：http://lai.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://byl.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://nkx.meibo888.top

C#:   x is int or double or decimal
来源：http://oce.52xcode.cn

[B14] 判断值是否在集合内
来源：http://zar.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wwh.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sat.chenzaomai.com

JS:   [1, 2, 3].includes(x)
来源：http://hyf.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://tqr.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hyn.ydjk.org.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hzm.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://slf.bjfxy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://coc.sufxvd.cn

[B15] 布尔运算与取反
来源：http://ucu.havefunace.top

Py:   a and b or not c
来源：http://mbl.nwbrower.top

PHP:  $a && $b || !$c
来源：http://obg.yuanzhike.top

JS:   a && b || !c
来源：http://lwz.yj20258888.top

TS:   a && b || !c
来源：http://tzq.ydjk.org.cn

Java: a && b || !c
来源：http://jxf.fehbvm.com

Go:   a && b || !c
来源：http://jon.fktsv.cn

Ruby: a && b || !c
来源：http://yts.yj20258.top

C#:   a && b || !c
来源：http://epk.ehwqpu.com

[B16] 卫语句：不满足条件提前返回
来源：http://dya.aibaodan.cn

Py:   if not data: return
来源：http://kwu.ppjwa.cn

PHP:  if (!$data) { return; }
来源：http://ran.chenzaomai.com

JS:   if (!data) return;
来源：http://qbh.chenlongwang.top

TS:   if (!data) return;
来源：http://jrk.c1oappe.top

Java: if (data == null) return;
来源：http://xye.smart0.xyz

Go:   if data == nil { return }
来源：http://agc.dashuyun.cn

Ruby: return if data.nil?
来源：http://lmx.fktsv.cn

C#:   if (data == null) return;
来源：http://ysj.jinghuilouyu.cn

================================================================================
来源：http://whv.shangyingyoupin.top

C. 函数与作用域
来源：http://njs.tanke756.top

================================================================================
来源：http://lfc.xinyue.icu

[C01] 定义函数
来源：http://xhg.dianchejie.cn

Py:   def add(a, b): return a + b
来源：http://edx.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://thv.daxiang520.top

JS:   function add(a, b) { return a + b; }
来源：http://zya.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cmd.redwolf501.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vvu.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kwp.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://ypd.cdnleiting.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jxn.zhaomingkeji.xyz

[C02] 默认参数
来源：http://omr.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://ttv.mhx1999.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ggw.hywenlv.cn

JS:   function greet(name = "World") { return name; }
来源：http://abb.jinghuilouyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://etw.tanke756.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gzq.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://etx.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://dhj.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://mxi.nanxuanxn.top

[C03] 可变参数
来源：http://lmc.hywenlv.cn

Py:   def total(*args): return sum(args)
来源：http://bye.yanxiufei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yyx.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kjt.c1oappe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sjd.nanxinkj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kvb.daxiang520.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tow.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://qfn.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eyz.gzhubu.top

[C04] 命名参数 / 关键字参数
来源：http://eah.cashguo.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ixi.meibo888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yxe.chenjidiqi.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://suc.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xiw.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://afa.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://bvk.jinqigufen.top

Ruby: f(a: 1, b: 2)
来源：http://nqm.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://uru.jinqigfzy.top

[C05] 返回多个值
来源：http://zos.shzxlz.cn

Py:   return a, b
来源：http://wrx.316326.xyz

PHP:  return [$a, $b];
来源：http://jwm.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://job.jqgfzy.top

TS:   return { a, b };
来源：http://lpw.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ijd.cucudq.cn

Go:   return a, b
来源：http://zxs.shanyushiyangkeji.top

Ruby: return a, b
来源：http://vlf.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://kmf.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://xks.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://rhs.ydzc1.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ele.xziqi.cn

JS:   const square = x => x * x;
来源：http://vco.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://eaz.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ztz.jinyuanbaomall.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jcg.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://noe.cqqwz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ofv.cashguo.top

[C07] 把函数作为参数传入
来源：http://htn.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tao.52xcode.cn

PHP:  array_map("strtoupper", $arr);
来源：http://aev.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dfd.pycfn.com

TS:   arr.map(String)
来源：http://awx.ywan-chungtsiang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xzl.cashguo.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vrw.vehdjk.com

Ruby: arr.map(&:upcase)
来源：http://kuc.ppjwa.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gsa.ehwqpu.com

[C08] 闭包
来源：http://hll.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bmp.jinqigufen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jzf.sjlbkw.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pcy.xuanzx.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uih.dianchejie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://adb.chenlongwang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jvr.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://klw.nanxuanxn.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zfl.yonumen.top

[C09] 递归
来源：http://hvo.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kgf.hongshengwenyu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://smd.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tyw.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mqa.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hcn.tianlin.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dey.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tfy.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gqh.guowangkeji.top

[C10] 变量作用域
来源：http://cig.snrcjt.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gyd.shzxlz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gca.ehwqpu.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mdq.wangdashe.top

TS:   同 JS
来源：http://etn.zhixingplan.top

Java: 方法内为块级作用域
来源：http://xwc.tianlin.xyz

Go:   花括号块级作用域
来源：http://nwh.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qjs.yueranfly.top


<!-- 参考信息 -->