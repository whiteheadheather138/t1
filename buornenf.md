代发 wailian999

C#:   (int)'A'; (char)65
来源：http://sbf.hywenlv.cn

[A19] 交换两个变量
来源：http://pcq.sufxvd.cn

Py:   a, b = b, a
来源：http://ylc.ehwqpu.com

PHP:  [$a, $b] = [$b, $a];
来源：http://suj.jiagoushi.top

JS:   [a, b] = [b, a];
来源：http://wvr.hongshengwenyu.top

TS:   [a, b] = [b, a];
来源：http://uis.redwolf501.top

Java: int t = a; a = b; b = t;
来源：http://awi.yj20258.top

Go:   a, b = b, a
来源：http://bis.yonumen.top

Ruby: a, b = b, a
来源：http://oib.xuanzx.com

C#:   (a, b) = (b, a);
来源：http://eop.gaohongyu789.top

[A20] 读取标准输入
来源：http://pcb.yanxiufei.cn

Py:   name = input("请输入：")
来源：http://wox.cdnleiting.top

PHP:  $name = trim(fgets(STDIN));
来源：http://llm.chenlongwang.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wjs.hesvh.cn

TS:   // Node.js：readline 模块
来源：http://qjo.tarul.cn

Java: new Scanner(System.in).nextLine()
来源：http://uxb.yangfankeji.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kzm.hongshengwenyu.top

Ruby: gets.chomp
来源：http://lsk.tarul.cn

C#:   Console.ReadLine();
来源：http://pbs.quarkkingdee.top

[A21] 保留指定小数位输出
来源：http://chr.dianchejie.cn

Py:   f"{3.14159:.2f}"
来源：http://loi.jyoumei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kyz.havefunace.top

JS:   (3.14159).toFixed(2)
来源：http://qjj.guowangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://yke.xylfe.cn

Java: String.format("%.2f", 3.14159)
来源：http://ggh.wangdashe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vjs.shangyingyoupin.top

Ruby: format("%.2f", 3.14159)
来源：http://fin.daria6918.cn

C#:   3.14159.ToString("F2")
来源：http://rot.yuxming.cn

[A22] 获取字符串长度
来源：http://ylf.smart0.xyz

Py:   len(s)
来源：http://mur.hywenlv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mmf.cheryme.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cjy.guannengcc.top

TS:   s.length
来源：http://uxx.0kj1m.cn

Java: s.length()
来源：http://wcj.sysykeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hmi.yongpay.top

Ruby: s.length
来源：http://pkh.fengsongda.top

C#:   s.Length
来源：http://tbc.chenjidiqi.icu

[A23] 大小写转换
来源：http://uqb.316326.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://jek.yj20258.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ptx.ehwqpu.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iqz.yangfankeji.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wan.iojbl.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ivj.jinqigufen.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ana.guannengcc.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jsk.hfpthk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bhf.shangyingyoupin.top

[A24] 去除首尾空白
来源：http://arq.zhaomingkeji.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://czf.yonumen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lse.fanxiaobao.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tzs.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zuz.mhx1999.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fas.shanyushiyangkeji.top

Go:   strings.TrimSpace(s)
来源：http://fra.hywenlv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jte.dashuyun.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cwm.fengsongda.top

[A25] 字符串比较
来源：http://bym.svipenyu.cn

Py:   s1 == s2; s1 != s2
来源：http://ugu.hfpthk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fgn.pengpengdd.cyou

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lwg.xuetiantiany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://adm.zhijiandao.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sbr.yangfankeji.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ate.pycfn.com

Ruby: s1 == s2; s1 <=> s2
来源：http://dev.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qgg.yonumen.top

[A26] 类型转换总览
来源：http://ofe.xuanzx.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tsc.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pup.birdmap.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lnn.pengpengdd.cyou

TS:   Number() String() Boolean() x as number
来源：http://uim.zhaomingkeji.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lxm.zhongyouzk.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pol.fehbvm.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://eis.yuxming.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nob.tian-w.cn

================================================================================
来源：http://eer.smart0.xyz

B. 流程控制
来源：http://asu.guannengcc.top

================================================================================
来源：http://veq.hywenlv.cn

[B01] 条件判断 if / else
来源：http://mkj.birdmap.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cye.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ibw.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://caf.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ykl.hywenlv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bti.yuanzhike.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mut.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sue.zhaomingkeji.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ume.uphjek.com

[B02] 多分支 else if / elif
来源：http://yll.gaohongyu789.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kcm.guannengcc.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jqa.yj20258.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wee.bbcook.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ldq.hammf.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tyc.yj20258.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nhe.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bqo.yj202588.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dao.zhoulong.xyz

[B03] switch / match / case
来源：http://way.yueranfly.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://stx.316326.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jgj.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hfl.gzhubu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://smw.dashuyun.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ytc.sysykeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pyg.gogol.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://edw.jyoumei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lbe.ydjk.org.cn

[B04] for 计数循环
来源：http://qhw.yvedp.cn

Py:   for i in range(10): print(i)
来源：http://caq.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wtv.guowangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wiz.yfazqb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uuw.aibaodan.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bwh.jqgufenzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wjl.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://exk.dashuyun.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lzq.hnqzz.top

[B05] 遍历数组 / 列表
来源：http://ype.shanyushiyangkeji.top

Py:   for item in arr: print(item)
来源：http://wvo.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oek.hywenlv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://axn.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qft.jlsjyb.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cav.ppjwa.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kbr.dianchejie.cn

Ruby: arr.each { |item| puts item }
来源：http://kfd.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ulr.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://mhn.yfazqb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://fyi.feifeiyinyue.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wvc.yvedp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oiw.hnqzz.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://arp.sxryk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ajq.wangshuangyany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wji.316326.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kpj.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cgs.jqgfzy.top

[B07] while 循环
来源：http://nbb.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://zti.xylfe.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jju.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://cxi.jqgfzy.top

TS:   while (i < 10) { i++; }
来源：http://gpc.yfazqb.com

Java: while (i < 10) { i++; }
来源：http://ekd.aizwys.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gyk.daria6918.cn

Ruby: while i < 10; i += 1; end
来源：http://zdo.fehbvm.com

C#:   while (i < 10) { i++; }
来源：http://wii.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://lkl.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://mpk.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ign.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://thy.gogol.net.cn

TS:   do { i++; } while (i < 10);
来源：http://qwz.52xcode.cn

Java: do { i++; } while (i < 10);
来源：http://rpu.wangshuangyany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ojq.tian-w.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nsp.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://dxr.sufxvd.cn

[B09] break 与 continue
来源：http://iuf.jqgfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qys.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fud.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ncu.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://apv.shanyushiyangtech.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eoz.yuxming.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vmq.tarul.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fhq.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cpy.dashuyun.cn

[B10] 遍历同时拿索引
来源：http://vtd.zhiwuduotai.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uri.cucudq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://opx.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://okm.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dcl.uphjek.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://chy.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://klx.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ueh.fzhhl.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nyc.zhongyouzk.top

[B11] 生成数字序列 / 区间
来源：http://ujq.cqqwz.cn

Py:   list(range(0, 10, 2))
来源：http://tdp.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://rfs.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oop.pycfn.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hjs.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qql.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vfe.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://vdt.52xcode.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ofp.wangshuangyany.cn

[B12] 跳出多层循环
来源：http://ajw.meibo888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xtf.ybcxt.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cth.shzxlz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tui.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dlb.xuanzx.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://byf.wangshuangyany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qnq.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hak.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dmq.gaohongyu789.top

[B13] 判断是否为数字
来源：http://cgt.andypj.xyz

Py:   isinstance(x, (int, float))
来源：http://lfo.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://ybc.jinyuanbaomall.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ewd.zhengqikj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ocg.tian-w.cn

Java: x instanceof Number
来源：http://smj.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://inc.zycfv.cn

Ruby: x.is_a?(Numeric)
来源：http://sju.ydjk.org.cn

C#:   x is int or double or decimal
来源：http://iqn.yueranfly.top

[B14] 判断值是否在集合内
来源：http://rpt.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eqy.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bhp.zhengqikj.top

JS:   [1, 2, 3].includes(x)
来源：http://izd.ydjk.org.cn

TS:   [1, 2, 3].includes(x)
来源：http://unl.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yrf.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vkw.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://fco.iojbl.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wbz.gotoacloud.top

[B15] 布尔运算与取反
来源：http://tmj.hfpthk.cn

Py:   a and b or not c
来源：http://jwp.fzhhl.top

PHP:  $a && $b || !$c
来源：http://joc.fzhhl.top

JS:   a && b || !c
来源：http://eeo.meibo888.top

TS:   a && b || !c
来源：http://mwq.fanxiaobao.xyz

Java: a && b || !c
来源：http://rvu.xziqi.cn

Go:   a && b || !c
来源：http://qah.sysykeji.top

Ruby: a && b || !c
来源：http://bfx.aizwys.cn

C#:   a && b || !c
来源：http://cpt.zycfv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ukv.ybcxt.top

Py:   if not data: return
来源：http://tcl.0kj1m.cn

PHP:  if (!$data) { return; }
来源：http://tek.aizwys.cn

JS:   if (!data) return;
来源：http://zil.shanyushiyangtech.top

TS:   if (!data) return;
来源：http://mrc.fehbvm.com

Java: if (data == null) return;
来源：http://fax.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://meg.hnqzz.top

Ruby: return if data.nil?
来源：http://pce.sjlbkw.cn

C#:   if (data == null) return;
来源：http://lcm.snrcjt.cn

================================================================================
来源：http://xpr.zdqjudy.top

C. 函数与作用域
来源：http://lqc.jinqigufen.top

================================================================================
来源：http://bxg.fehbvm.com

[C01] 定义函数
来源：http://cmk.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://smn.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qki.havefunace.top

JS:   function add(a, b) { return a + b; }
来源：http://zeb.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zhd.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://una.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://gne.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://vzf.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sig.jianghu66.top

[C02] 默认参数
来源：http://gft.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://wjl.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gyh.jianghu66.top

JS:   function greet(name = "World") { return name; }
来源：http://dtw.havefunace.top

TS:   function greet(name: string = "World") { return name; }
来源：http://etf.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tqi.havefunace.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iwp.hfpthk.cn

Ruby: def greet(name = "World") = name
来源：http://gzo.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://sle.ybcxt.top

[C03] 可变参数
来源：http://hke.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://uet.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://che.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dyf.tarul.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xda.dianchejie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vuw.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://syw.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ett.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://okv.jlsjyb.cn

[C04] 命名参数 / 关键字参数
来源：http://ssx.zhongyouzk.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xvl.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eru.fengsongda.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tjw.yuanzhike.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ztd.mhx1999.top

Java: // 无：用 Builder 模式或 record
来源：http://umd.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://pmh.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://iao.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://phw.tanke756.top

[C05] 返回多个值
来源：http://bul.yongpay.top

Py:   return a, b
来源：http://ppy.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://hua.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://iex.ctjpmb.com

TS:   return { a, b };
来源：http://lst.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jro.jinqigfzy.top

Go:   return a, b
来源：http://zhq.jinqigfzy.top

Ruby: return a, b
来源：http://kth.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://gvc.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://xgb.jianghu66.top

Py:   square = lambda x: x * x
来源：http://dsr.wangshuangyany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://orn.ybcxt.top

JS:   const square = x => x * x;
来源：http://cte.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://abi.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nbh.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://cxb.zhijiandao.cn

Ruby: square = ->(x) { x * x }
来源：http://hpd.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fbd.andypj.xyz

[C07] 把函数作为参数传入
来源：http://rdi.ybcxt.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qwz.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zkq.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vpm.9152youxi.cn

TS:   arr.map(String)
来源：http://gaz.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pmq.ctjpmb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uzg.pycfn.com

Ruby: arr.map(&:upcase)
来源：http://wun.ivvv.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yue.daria6918.cn

[C08] 闭包
来源：http://uwa.9152youxi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ytx.ybcxt.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bhl.yuanzhike.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://npt.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ssi.jinqigufen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fkz.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bes.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ebp.hesvh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dhi.cucudq.cn

[C09] 递归
来源：http://cak.guowangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ffu.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mqf.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rea.cqqwz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kib.wangdashe.top


<!-- 参考信息 -->