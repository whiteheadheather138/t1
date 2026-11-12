代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://flu.quarkkingdee.top

Java: (int) 'A'; (char) 65
来源：http://ita.fzhhl.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qia.ivvv.top

Ruby: "A".ord; 65.chr
来源：http://xww.quarkkingdee.top

C#:   (int)'A'; (char)65
来源：http://fbp.jinqigfzy.top

[A19] 交换两个变量
来源：http://dbp.xuetiantiany.cn

Py:   a, b = b, a
来源：http://yfp.zhaomingkeji.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://qad.hammf.cn

JS:   [a, b] = [b, a];
来源：http://uvj.fanxiaobao.xyz

TS:   [a, b] = [b, a];
来源：http://sgo.jlsjyb.cn

Java: int t = a; a = b; b = t;
来源：http://wwj.daria6918.cn

Go:   a, b = b, a
来源：http://arx.yonumen.top

Ruby: a, b = b, a
来源：http://byf.wangshuangyany.cn

C#:   (a, b) = (b, a);
来源：http://ooo.cqqwz.cn

[A20] 读取标准输入
来源：http://dvr.meibo888.top

Py:   name = input("请输入：")
来源：http://yul.yanxiufei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rlo.jinqigfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hnw.zdqjudy.top

TS:   // Node.js：readline 模块
来源：http://ymo.nanxuanxn.top

Java: new Scanner(System.in).nextLine()
来源：http://mjg.fengsongda.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wox.gaohongyu789.top

Ruby: gets.chomp
来源：http://vwu.quarkkingdee.top

C#:   Console.ReadLine();
来源：http://shk.cheryme.top

[A21] 保留指定小数位输出
来源：http://oab.fanxiaobao.xyz

Py:   f"{3.14159:.2f}"
来源：http://scc.hywenlv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dyj.chenlongwang.top

JS:   (3.14159).toFixed(2)
来源：http://gec.tian-w.cn

TS:   (3.14159).toFixed(2)
来源：http://fok.sjlbkw.cn

Java: String.format("%.2f", 3.14159)
来源：http://irs.snrcjt.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xgp.feifeiyinyue.top

Ruby: format("%.2f", 3.14159)
来源：http://xsx.hcnkem.com

C#:   3.14159.ToString("F2")
来源：http://dsf.gaohongyu789.top

[A22] 获取字符串长度
来源：http://ubt.shanyushiyangtech.top

Py:   len(s)
来源：http://itd.shanyushiyangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cux.sufxvd.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aoo.haohaochexian.top

TS:   s.length
来源：http://twt.nwbrower.top

Java: s.length()
来源：http://vat.xinyue.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ksc.c1oappe.top

Ruby: s.length
来源：http://khz.yj20258.top

C#:   s.Length
来源：http://kcx.cucudq.cn

[A23] 大小写转换
来源：http://mvl.xziqi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://noq.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gur.jinyuanbaomall.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mmi.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pzw.epnwcf.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://atb.9152youxi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qll.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pgh.jinqigufen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mli.gotoacloud.top

[A24] 去除首尾空白
来源：http://awc.cheryme.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bzh.ybcxt.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iuq.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://azb.wangshuangyany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hja.haohaochexian.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mlu.tarul.cn

Go:   strings.TrimSpace(s)
来源：http://vgn.yueranfly.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gdc.tanke756.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kuz.hesvh.cn

[A25] 字符串比较
来源：http://nah.sxryk.cn

Py:   s1 == s2; s1 != s2
来源：http://bky.gzhubu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oto.sjlbkw.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rje.kuanghao11.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rzc.wangdashe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kzf.shanyushiyangtech.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ght.nwbrower.top

Ruby: s1 == s2; s1 <=> s2
来源：http://crm.fktsv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dld.shangyingyoupin.top

[A26] 类型转换总览
来源：http://cna.bbcook.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qaa.aizwys.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vhm.quarkkingdee.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fdh.hywenlv.cn

TS:   Number() String() Boolean() x as number
来源：http://bco.jqgfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vxa.yuanzhike.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ccq.daxiang520.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://yad.chenzaomai.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dno.gzhubu.top

================================================================================
来源：http://qlj.yuanzhike.top

B. 流程控制
来源：http://lnf.zhoulong.xyz

================================================================================
来源：http://ydp.tianlin.xyz

[B01] 条件判断 if / else
来源：http://wsp.epnwcf.com

Py:   result = "正" if x > 0 else "非正"
来源：http://smc.pengpengdd.cyou

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vpv.yvedp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tkm.cucudq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://svq.hongshengwenyu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://inl.sufxvd.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ixd.gaohongyu789.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://csm.nwbrower.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gni.yueranfly.top

[B02] 多分支 else if / elif
来源：http://gqp.birdmap.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://org.xziqi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fww.birdmap.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vgz.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://riy.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ctx.hammf.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iez.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iyt.yangfankeji.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ugk.guannengcc.top

[B03] switch / match / case
来源：http://eka.ydzc1.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ylt.pycfn.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dkh.xinyue.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dgs.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ijs.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zou.zhixingplan.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cis.52xcode.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nkl.ehwqpu.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ftx.nanxuanxn.top

[B04] for 计数循环
来源：http://bwm.yj20258888.top

Py:   for i in range(10): print(i)
来源：http://wdt.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pnl.ydzc1.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://awe.guannengcc.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ulh.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kmc.gotoacloud.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://esi.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://xfe.ppjwa.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cwv.c1oappe.top

[B05] 遍历数组 / 列表
来源：http://nsk.tianlin.xyz

Py:   for item in arr: print(item)
来源：http://yxs.fzhhl.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gyo.jqgufenzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hzq.jiagoushi.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rpx.yongpay.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wnr.xinyue.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pkx.hammf.cn

Ruby: arr.each { |item| puts item }
来源：http://afl.c1oappe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iib.jiagoushi.top

[B06] 遍历字典 / 对象
来源：http://swc.xinyue.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://doa.feifeiyinyue.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://brg.shuidangran.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cul.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kjt.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wit.hongshengwenyu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ebc.ywan-chungtsiang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ypv.yvedp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kxd.xuanzx.com

[B07] while 循环
来源：http://tvi.jinqigufen.top

Py:   while i < 10: i += 1
来源：http://wkp.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://lhe.ybcxt.top

JS:   while (i < 10) { i++; }
来源：http://eos.zhoulong.xyz

TS:   while (i < 10) { i++; }
来源：http://ljh.316326.xyz

Java: while (i < 10) { i++; }
来源：http://bcj.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qda.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://eep.jinghuilouyu.cn

C#:   while (i < 10) { i++; }
来源：http://auv.zdqjudy.top

[B08] do-while（至少执行一次）
来源：http://hfi.daria6918.cn

Py:   # 无 do-while：用 while True + break
来源：http://meh.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ezp.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://xkg.0kj1m.cn

TS:   do { i++; } while (i < 10);
来源：http://aku.ywan-chungtsiang.top

Java: do { i++; } while (i < 10);
来源：http://xtt.smart0.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://zzf.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qby.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://cbk.aibaodan.cn

[B09] break 与 continue
来源：http://jvy.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://top.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rbe.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xaj.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://drw.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hhs.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jth.hfpthk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zuj.ctjpmb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yhb.uphjek.com

[B10] 遍历同时拿索引
来源：http://ppu.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bth.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aht.c1oappe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kyi.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gcq.yvedp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cts.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oad.pengpengdd.cyou

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bqn.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jkq.tianlin.xyz

[B11] 生成数字序列 / 区间
来源：http://few.aizwys.cn

Py:   list(range(0, 10, 2))
来源：http://urb.pengpengdd.cyou

PHP:  range(0, 10, 2);
来源：http://zpd.quarkkingdee.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://umk.cdnleiting.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qra.ppjwa.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rog.jinqigfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ujd.zycfv.cn

Ruby: (0...10).step(2).to_a
来源：http://yjn.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tfk.zhaomingkeji.xyz

[B12] 跳出多层循环
来源：http://vhg.daria6918.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://quk.sjlbkw.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://brd.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ebb.chenjidiqi.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fdv.xziqi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yoz.dianchejie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zxt.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://duz.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aoe.hongshengwenyu.top

[B13] 判断是否为数字
来源：http://ueb.snrcjt.cn

Py:   isinstance(x, (int, float))
来源：http://ucg.kuanghao11.cn

PHP:  is_numeric($x)
来源：http://cjq.guowangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pnd.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cdp.ctjpmb.com

Java: x instanceof Number
来源：http://vlq.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ehh.kuanghao11.cn

Ruby: x.is_a?(Numeric)
来源：http://zvz.yongpay.top

C#:   x is int or double or decimal
来源：http://hzr.daxiang520.top

[B14] 判断值是否在集合内
来源：http://ama.bjfxy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wez.zycfv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tsu.yueranfly.top

JS:   [1, 2, 3].includes(x)
来源：http://swz.cqqwz.cn

TS:   [1, 2, 3].includes(x)
来源：http://sbu.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://muy.fzhhl.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kyi.yangfankeji.com

Ruby: [1, 2, 3].include?(x)
来源：http://qye.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sga.mhx1999.top

[B15] 布尔运算与取反
来源：http://awv.hfpthk.cn

Py:   a and b or not c
来源：http://dfn.yonumen.top

PHP:  $a && $b || !$c
来源：http://jwu.yueranfly.top

JS:   a && b || !c
来源：http://ybj.hysaishi.cn

TS:   a && b || !c
来源：http://cyz.quarkkingdee.top

Java: a && b || !c
来源：http://vve.shuidangran.top

Go:   a && b || !c
来源：http://ixh.shzxlz.cn

Ruby: a && b || !c
来源：http://ptf.yj20258888.top

C#:   a && b || !c
来源：http://emn.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://lyb.haohaochexian.top

Py:   if not data: return
来源：http://bju.vqdsnc.cn

PHP:  if (!$data) { return; }
来源：http://jlt.guowangkeji.top

JS:   if (!data) return;
来源：http://jxf.jqgufenzy.top

TS:   if (!data) return;
来源：http://zbd.shzxlz.cn

Java: if (data == null) return;
来源：http://jgu.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://zkw.cashguo.top

Ruby: return if data.nil?
来源：http://xeq.zycfv.cn

C#:   if (data == null) return;
来源：http://hwj.havefunace.top

================================================================================
来源：http://fru.yonumen.top

C. 函数与作用域
来源：http://vdp.jqgufenzy.top

================================================================================
来源：http://bfx.yonumen.top

[C01] 定义函数
来源：http://fjo.ydjk.org.cn

Py:   def add(a, b): return a + b
来源：http://vhn.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aey.nanxuanxn.top

JS:   function add(a, b) { return a + b; }
来源：http://pdp.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sqi.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://voh.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://auy.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://heq.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ics.hnxiangtu.top

[C02] 默认参数
来源：http://bkl.dashuyun.cn

Py:   def greet(name="World"): return name
来源：http://vrv.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kql.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://fqx.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nkr.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rrn.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bgv.daria6918.cn

Ruby: def greet(name = "World") = name
来源：http://vbl.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://zkd.shanyushiyangtech.top

[C03] 可变参数
来源：http://dcu.fanxiaobao.xyz

Py:   def total(*args): return sum(args)
来源：http://ndf.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tvk.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ytb.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zia.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jap.dashuyun.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zad.jinyuanbaomall.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zja.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://btp.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://psv.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://omx.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zwn.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mqy.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iah.dashuyun.cn

Java: // 无：用 Builder 模式或 record
来源：http://ejl.smart0.xyz

Go:   // 无：用配置结构体参数
来源：http://cqh.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://axq.tanke756.top

C#:   f(a: 1, b: 2)
来源：http://dij.dashuyun.cn

[C05] 返回多个值
来源：http://etq.ydzc1.top

Py:   return a, b
来源：http://jei.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://cxi.hcnkem.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://qjf.yuanzhike.top

TS:   return { a, b };
来源：http://ldi.andypj.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yal.yj202588.top

Go:   return a, b
来源：http://gwc.chenlongwang.top

Ruby: return a, b
来源：http://ajq.ppjwa.cn

C#:   return (a, b);              // ValueTuple
来源：http://awk.jqgfzy.top

[C06] 匿名函数 / lambda
来源：http://dth.xziqi.cn

Py:   square = lambda x: x * x
来源：http://bkn.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ddz.jinqigfzy.top

JS:   const square = x => x * x;
来源：http://ogp.tarul.cn

TS:   const square = (x: number): number => x * x;
来源：http://pek.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lzu.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sin.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://olw.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://zra.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://tue.svipenyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mwj.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://uof.xylfe.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sed.feifeiyinyue.top

TS:   arr.map(String)
来源：http://lda.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kfr.zhiwuduotai.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rxq.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://rsg.epnwcf.com

C#:   arr.Select(s => s.ToUpper())
来源：http://nuz.nanxinkj.top

[C08] 闭包
来源：http://ias.chenlongwang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ctb.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jqp.hnqzz.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kwc.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dpn.ctjpmb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ixp.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ete.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jer.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hbf.pengpengdd.cyou

[C09] 递归
来源：http://kbs.sjlbkw.cn


<!-- 参考信息 -->