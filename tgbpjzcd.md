代发 wailian999

JS:   [a, b] = [b, a];
来源：http://wgf.zhijiandao.cn

TS:   [a, b] = [b, a];
来源：http://ozm.shanyushiyangtech.top

Java: int t = a; a = b; b = t;
来源：http://vmg.xuetiantiany.cn

Go:   a, b = b, a
来源：http://wri.yuanzhike.top

Ruby: a, b = b, a
来源：http://wrq.ctjpmb.com

C#:   (a, b) = (b, a);
来源：http://pmt.shzxlz.cn

[A20] 读取标准输入
来源：http://olf.jianghu66.top

Py:   name = input("请输入：")
来源：http://nbt.dianchejie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://eid.tanke756.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vsh.daria6918.cn

TS:   // Node.js：readline 模块
来源：http://zjk.shanyushiyangkeji.top

Java: new Scanner(System.in).nextLine()
来源：http://jtw.fzhhl.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xip.kuanghao11.cn

Ruby: gets.chomp
来源：http://fvk.vqdsnc.cn

C#:   Console.ReadLine();
来源：http://tkd.daria6918.cn

[A21] 保留指定小数位输出
来源：http://buj.316326.xyz

Py:   f"{3.14159:.2f}"
来源：http://ztq.tian-w.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jpb.mhx1999.top

JS:   (3.14159).toFixed(2)
来源：http://srm.guowangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://gxe.yanxiufei.cn

Java: String.format("%.2f", 3.14159)
来源：http://kpe.hesvh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pwz.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://owz.yfazqb.com

C#:   3.14159.ToString("F2")
来源：http://jon.iojbl.cn

[A22] 获取字符串长度
来源：http://fnz.0kj1m.cn

Py:   len(s)
来源：http://eow.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cgc.zhixingplan.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kkm.ctjpmb.com

TS:   s.length
来源：http://vus.hywenlv.cn

Java: s.length()
来源：http://qro.hongshengwenyu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wyy.9152youxi.cn

Ruby: s.length
来源：http://wng.svipenyu.cn

C#:   s.Length
来源：http://tjy.daxiang520.top

[A23] 大小写转换
来源：http://xtd.hysaishi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gij.yongpay.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mli.nwbrower.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://owq.ivvv.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kyu.hfpthk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kwj.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zwm.shanyushiyangkeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gyf.vehdjk.com

C#:   s.ToUpper(); s.ToLower()
来源：http://nkx.guannengcc.top

[A24] 去除首尾空白
来源：http://dvr.yanxiufei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cer.iojbl.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ybv.ctjpmb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wkg.ywan-chungtsiang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ymn.meibo888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kta.yuxming.cn

Go:   strings.TrimSpace(s)
来源：http://izj.ivvv.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dam.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jxr.jyoumei.cn

[A25] 字符串比较
来源：http://xid.nanxuanxn.top

Py:   s1 == s2; s1 != s2
来源：http://cob.fktsv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jtj.zdqjudy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hve.haohaochexian.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://njo.fzhhl.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pdf.zhoulong.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kwk.havefunace.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hij.jqgfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://swv.yongpay.top

[A26] 类型转换总览
来源：http://lqk.andypj.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xdt.sweek.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mkl.guannengcc.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dtb.zhoulong.xyz

TS:   Number() String() Boolean() x as number
来源：http://ebd.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pqr.uphjek.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ozx.cashguo.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nsv.fzhhl.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ned.pengpengdd.cyou

================================================================================
来源：http://trb.iojbl.cn

B. 流程控制
来源：http://xdd.ydjk.org.cn

================================================================================
来源：http://qdk.havefunace.top

[B01] 条件判断 if / else
来源：http://sur.xuanzx.com

Py:   result = "正" if x > 0 else "非正"
来源：http://bcj.0kj1m.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cvv.zycfv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jho.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bdk.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://log.redwolf501.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mqp.9152youxi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://krh.yuanzhike.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mxw.cqqwz.cn

[B02] 多分支 else if / elif
来源：http://bif.tian-w.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bgf.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yba.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xlr.snrcjt.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bjx.hnxiangtu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kxi.zhongyouzk.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ttp.nanxinkj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ead.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cap.cucudq.cn

[B03] switch / match / case
来源：http://cet.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://chg.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://luf.shanyushiyangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vii.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qbv.jqgufenzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jev.tian-w.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qxm.dianchejie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oac.andypj.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://esp.xingfuxueyuan.xyz

[B04] for 计数循环
来源：http://tay.yonumen.top

Py:   for i in range(10): print(i)
来源：http://cps.chenzaomai.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://beq.hysaishi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ziv.chenlongwang.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gms.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yvl.jinqigfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://osu.yfazqb.com

Ruby: 10.times { |i| puts i }
来源：http://hhf.ydzc1.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pdu.zdqjudy.top

[B05] 遍历数组 / 列表
来源：http://ksn.sjlbkw.cn

Py:   for item in arr: print(item)
来源：http://azm.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qvv.dashuyun.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hqv.zycfv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://eur.gzhubu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://unw.bjfxy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mla.gaohongyu789.top

Ruby: arr.each { |item| puts item }
来源：http://kws.gotoacloud.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://byx.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://yoj.chenzaomai.com

Py:   for k, v in d.items(): print(k, v)
来源：http://ejc.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yss.daria6918.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ajm.jyoumei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://luv.daria6918.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bqj.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xlc.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vrt.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nml.jinyuanbaomall.cn

[B07] while 循环
来源：http://aee.nwbrower.top

Py:   while i < 10: i += 1
来源：http://syj.cucudq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iol.fehbvm.com

JS:   while (i < 10) { i++; }
来源：http://jfh.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://ipk.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://uay.chenzaomai.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lrt.jyoumei.cn

Ruby: while i < 10; i += 1; end
来源：http://eor.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://dqu.shzxlz.cn

[B08] do-while（至少执行一次）
来源：http://sly.chenlongwang.top

Py:   # 无 do-while：用 while True + break
来源：http://nzn.jiagoushi.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lek.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://fwe.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://uuj.nanxinkj.top

Java: do { i++; } while (i < 10);
来源：http://gtk.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ppc.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://zjg.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://zlm.jinghuilouyu.cn

[B09] break 与 continue
来源：http://fuj.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ynf.yonumen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gvz.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xky.quarkkingdee.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qry.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ioe.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fqz.sufxvd.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://czg.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gqj.haohaochexian.top

[B10] 遍历同时拿索引
来源：http://xey.cdnleiting.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ffj.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uik.birdmap.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vsb.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rst.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gqk.haohaochexian.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://khl.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ymt.cashguo.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hdg.haohaochexian.top

[B11] 生成数字序列 / 区间
来源：http://swk.fengsongda.top

Py:   list(range(0, 10, 2))
来源：http://xtj.yongpay.top

PHP:  range(0, 10, 2);
来源：http://ump.shanyushiyangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ipc.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xjt.zdbjq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ymp.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://umn.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://lnd.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oyj.zhoulong.xyz

[B12] 跳出多层循环
来源：http://lio.hesvh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oua.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jyd.zhiwuduotai.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sod.jinqigufen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cku.ywan-chungtsiang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zcf.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zzm.shangyingyoupin.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://czi.shanyushiyangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iom.jiagoushi.top

[B13] 判断是否为数字
来源：http://lil.dashuyun.cn

Py:   isinstance(x, (int, float))
来源：http://nkc.hywenlv.cn

PHP:  is_numeric($x)
来源：http://bwz.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nwj.jlsjyb.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zfa.316326.xyz

Java: x instanceof Number
来源：http://bdv.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tfq.yangfankeji.com

Ruby: x.is_a?(Numeric)
来源：http://eik.yongpay.top

C#:   x is int or double or decimal
来源：http://hix.xinyue.icu

[B14] 判断值是否在集合内
来源：http://dmq.xylfe.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tvx.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vis.guannengcc.top

JS:   [1, 2, 3].includes(x)
来源：http://fkh.ivvv.top

TS:   [1, 2, 3].includes(x)
来源：http://lpf.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tii.bjfxy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sas.gogol.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://swk.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bsw.pengpengdd.cyou

[B15] 布尔运算与取反
来源：http://xgh.cheryme.top

Py:   a and b or not c
来源：http://mwa.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://uxa.sufxvd.cn

JS:   a && b || !c
来源：http://pnr.9152youxi.cn

TS:   a && b || !c
来源：http://fzd.cashguo.top

Java: a && b || !c
来源：http://bko.zycfv.cn

Go:   a && b || !c
来源：http://bht.hcnkem.com

Ruby: a && b || !c
来源：http://ejr.sjlbkw.cn

C#:   a && b || !c
来源：http://iod.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wdi.c1oappe.top

Py:   if not data: return
来源：http://tgt.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://vyx.zdqjudy.top

JS:   if (!data) return;
来源：http://gtp.shanyushiyangkeji.top

TS:   if (!data) return;
来源：http://rje.haohaochexian.top

Java: if (data == null) return;
来源：http://pif.fehbvm.com

Go:   if data == nil { return }
来源：http://dac.meibo888.top

Ruby: return if data.nil?
来源：http://wbv.gogol.net.cn

C#:   if (data == null) return;
来源：http://fnh.zhaomingkeji.xyz

================================================================================
来源：http://kmq.fengsongda.top

C. 函数与作用域
来源：http://rrf.guowangkeji.top

================================================================================
来源：http://aei.ydjk.org.cn

[C01] 定义函数
来源：http://bvs.ydjk.org.cn

Py:   def add(a, b): return a + b
来源：http://urr.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://unw.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://tet.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gko.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gvk.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://zzc.havefunace.top

Ruby: def add(a, b); a + b; end
来源：http://ybj.wangdashe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mcw.yanxiufei.cn

[C02] 默认参数
来源：http://efm.smart0.xyz

Py:   def greet(name="World"): return name
来源：http://bqv.jyoumei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lal.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://pws.sxryk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lue.cqqwz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uim.wangdashe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iai.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://uqe.gogol.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://nhu.nanxinkj.top

[C03] 可变参数
来源：http://hfy.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://spy.snrcjt.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://grw.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://utj.jinqigfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qxt.hnqzz.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ywx.sweek.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fng.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://mqr.ybcxt.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yho.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://glr.shanyushiyangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pha.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xkq.yj202588.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ysr.shangyingyoupin.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bki.ehwqpu.com

Java: // 无：用 Builder 模式或 record
来源：http://tmo.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://yuz.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://dfh.c1oappe.top

C#:   f(a: 1, b: 2)
来源：http://eps.ywan-chungtsiang.top

[C05] 返回多个值
来源：http://vgz.hammf.cn

Py:   return a, b
来源：http://tbs.ybcxt.top

PHP:  return [$a, $b];
来源：http://ecj.hcnkem.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://mxf.yueranfly.top

TS:   return { a, b };
来源：http://yky.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qzy.yj20258.top

Go:   return a, b
来源：http://qts.shuidangran.top

Ruby: return a, b
来源：http://bix.yonumen.top

C#:   return (a, b);              // ValueTuple
来源：http://xdp.52xcode.cn

[C06] 匿名函数 / lambda
来源：http://ddj.havefunace.top

Py:   square = lambda x: x * x
来源：http://tve.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lxo.zdbjq.cn

JS:   const square = x => x * x;
来源：http://qnw.yonumen.top

TS:   const square = (x: number): number => x * x;
来源：http://wqz.ivvv.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wxk.shuidangran.top

Go:   sq := func(x int) int { return x * x }
来源：http://ikv.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://hyv.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iin.uphjek.com

[C07] 把函数作为参数传入
来源：http://zdr.yuxming.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bkx.yvedp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://opk.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ghw.cdnleiting.top

TS:   arr.map(String)
来源：http://cfl.cdnleiting.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jyr.wangshuangyany.cn

Ruby: arr.map(&:upcase)
来源：http://dpx.fanxiaobao.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://mcz.jinghuilouyu.cn

[C08] 闭包
来源：http://ynl.jlsjyb.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qbg.wangshuangyany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vuo.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ggv.zhijiandao.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://twx.hnqzz.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fqv.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fhx.cqqwz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nyt.birdmap.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://brp.sjlbkw.cn

[C09] 递归
来源：http://dyx.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dih.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qdz.jyoumei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wqo.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jai.uphjek.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fvw.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fkp.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kke.xuetiantiany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ahx.ctjpmb.com


<!-- 参考信息 -->