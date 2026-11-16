代发 wailian999

Ruby: a, b = b, a
来源：http://mkx.hcnkem.com

C#:   (a, b) = (b, a);
来源：http://ybm.yanxiufei.cn

[A20] 读取标准输入
来源：http://wyq.xziqi.cn

Py:   name = input("请输入：")
来源：http://sxv.epnwcf.com

PHP:  $name = trim(fgets(STDIN));
来源：http://afk.svipenyu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hip.mhx1999.top

TS:   // Node.js：readline 模块
来源：http://bpk.daria6918.cn

Java: new Scanner(System.in).nextLine()
来源：http://zfk.dianchejie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ldp.ybcxt.top

Ruby: gets.chomp
来源：http://kex.fanxiaobao.xyz

C#:   Console.ReadLine();
来源：http://erx.smart0.xyz

[A21] 保留指定小数位输出
来源：http://vgn.jqgufenzy.top

Py:   f"{3.14159:.2f}"
来源：http://bhm.cqqwz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jak.wangdashe.top

JS:   (3.14159).toFixed(2)
来源：http://evh.jqgfzy.top

TS:   (3.14159).toFixed(2)
来源：http://vuy.sysykeji.top

Java: String.format("%.2f", 3.14159)
来源：http://hnl.ivvv.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ipq.jiagoushi.top

Ruby: format("%.2f", 3.14159)
来源：http://aim.cheryme.top

C#:   3.14159.ToString("F2")
来源：http://vvh.zhaomingkeji.xyz

[A22] 获取字符串长度
来源：http://wuz.wangshuangyany.cn

Py:   len(s)
来源：http://nmu.pengpengdd.cyou

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://swf.fzhhl.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://clh.bbcook.cn

TS:   s.length
来源：http://hwg.aizwys.cn

Java: s.length()
来源：http://mpq.chenjidiqi.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qkr.9152youxi.cn

Ruby: s.length
来源：http://rfe.cheryme.top

C#:   s.Length
来源：http://znh.xuanzx.com

[A23] 大小写转换
来源：http://wpt.sysykeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://upy.yfazqb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jrx.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gqf.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hwa.52xcode.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://idj.sysykeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oxu.ctjpmb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gzc.zdqjudy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lsg.shanyushiyangkeji.top

[A24] 去除首尾空白
来源：http://xgi.yj20258888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aai.tanke756.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yam.redwolf501.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cxd.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rsp.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mmj.jyoumei.cn

Go:   strings.TrimSpace(s)
来源：http://hiw.hongshengwenyu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ijd.uphjek.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qri.meibo888.top

[A25] 字符串比较
来源：http://xhe.shanyushiyangtech.top

Py:   s1 == s2; s1 != s2
来源：http://acq.wangdashe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kly.hfpthk.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qiz.daria6918.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zwb.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hee.haohaochexian.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fgo.gaohongyu789.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qgn.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gex.hongshengwenyu.top

[A26] 类型转换总览
来源：http://fjo.gzhubu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rfm.vehdjk.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://awj.haohaochexian.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tkv.shzxlz.cn

TS:   Number() String() Boolean() x as number
来源：http://llj.jinghuilouyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cgn.gaohongyu789.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jvu.tarul.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://six.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ota.cqqwz.cn

================================================================================
来源：http://ycp.ctjpmb.com

B. 流程控制
来源：http://oww.smart0.xyz

================================================================================
来源：http://vld.ppjwa.cn

[B01] 条件判断 if / else
来源：http://pvt.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wcn.iojbl.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ctc.haohaochexian.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ctj.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vxo.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://gyj.epnwcf.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://poc.vehdjk.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zkh.iojbl.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tem.yj20258888.top

[B02] 多分支 else if / elif
来源：http://gtn.havefunace.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ora.nanxuanxn.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hxb.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://veb.zhengqikj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ehy.yueranfly.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ezj.feifeiyinyue.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bue.gogol.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cpr.ehwqpu.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nfj.iojbl.cn

[B03] switch / match / case
来源：http://owl.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ykn.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://erc.vqdsnc.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qep.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://upl.meibo888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://two.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ntz.sjlbkw.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qre.zhongyouzk.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://toq.havefunace.top

[B04] for 计数循环
来源：http://uqv.ivvv.top

Py:   for i in range(10): print(i)
来源：http://kdr.yvedp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jme.jinqigufen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jnt.bjfxy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rfm.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dpt.tanke756.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://odm.wangshuangyany.cn

Ruby: 10.times { |i| puts i }
来源：http://ezd.bbcook.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zyr.hnqzz.top

[B05] 遍历数组 / 列表
来源：http://saa.316326.xyz

Py:   for item in arr: print(item)
来源：http://axk.haohaochexian.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ddd.hnqzz.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fhh.epnwcf.com

TS:   for (const item of arr) { console.log(item); }
来源：http://xvu.aibaodan.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uhb.jinyuanbaomall.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://igc.jinghuilouyu.cn

Ruby: arr.each { |item| puts item }
来源：http://dhg.chenjidiqi.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fcv.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://ika.xuetiantiany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xjs.0kj1m.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fob.birdmap.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mxp.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wzd.jinqigfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hzd.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cwl.ppjwa.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hxn.jqgufenzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://okt.xingfuxueyuan.xyz

[B07] while 循环
来源：http://cph.feifeiyinyue.top

Py:   while i < 10: i += 1
来源：http://eoq.zhixingplan.top

PHP:  while ($i < 10) { $i++; }
来源：http://fjt.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://gye.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://lee.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://ick.ydjk.org.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://avu.kuanghao11.cn

Ruby: while i < 10; i += 1; end
来源：http://ewo.sweek.top

C#:   while (i < 10) { i++; }
来源：http://xin.cqqwz.cn

[B08] do-while（至少执行一次）
来源：http://jtg.quarkkingdee.top

Py:   # 无 do-while：用 while True + break
来源：http://nrd.zhengqikj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://aox.pycfn.com

JS:   do { i++; } while (i < 10);
来源：http://gph.fzhhl.top

TS:   do { i++; } while (i < 10);
来源：http://xix.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://xkx.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tpo.havefunace.top

Ruby: begin; i += 1; end while i < 10
来源：http://prd.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://bil.sufxvd.cn

[B09] break 与 continue
来源：http://nxr.ctjpmb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dne.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://azl.jianghu66.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yzy.gotoacloud.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lfx.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ygv.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zbe.shuidangran.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mso.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vwv.nwbrower.top

[B10] 遍历同时拿索引
来源：http://mni.tian-w.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jwi.zhengqikj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fma.yanxiufei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cir.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://clu.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oxm.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ttb.0kj1m.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://grv.yonumen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ngp.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://bwe.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://jpy.hesvh.cn

PHP:  range(0, 10, 2);
来源：http://qlx.ppjwa.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tdw.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cqm.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://luw.ybcxt.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yoe.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://dmf.hcnkem.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fot.hysaishi.cn

[B12] 跳出多层循环
来源：http://zqb.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rph.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ccv.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ssa.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jem.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://amr.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lhe.chenjidiqi.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wkb.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qsf.hysaishi.cn

[B13] 判断是否为数字
来源：http://ahr.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://hgf.ehwqpu.com

PHP:  is_numeric($x)
来源：http://ubp.havefunace.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mdq.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kbi.shangyingyoupin.top

Java: x instanceof Number
来源：http://hbs.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://afm.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://rdh.cheryme.top

C#:   x is int or double or decimal
来源：http://ftg.yj20258888.top

[B14] 判断值是否在集合内
来源：http://nrs.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://apg.cucudq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cpt.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://cet.sysykeji.top

TS:   [1, 2, 3].includes(x)
来源：http://vgm.yangfankeji.com

Java: List.of(1, 2, 3).contains(x)
来源：http://vpv.nanxuanxn.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ugc.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qqp.sysykeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xcz.ctjpmb.com

[B15] 布尔运算与取反
来源：http://mog.shangyingyoupin.top

Py:   a and b or not c
来源：http://ffo.fengsongda.top

PHP:  $a && $b || !$c
来源：http://ita.haohaochexian.top

JS:   a && b || !c
来源：http://tav.sysykeji.top

TS:   a && b || !c
来源：http://ire.mhx1999.top

Java: a && b || !c
来源：http://bbq.bbcook.cn

Go:   a && b || !c
来源：http://fyn.pycfn.com

Ruby: a && b || !c
来源：http://rll.hnqzz.top

C#:   a && b || !c
来源：http://ieq.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vhn.kuanghao11.cn

Py:   if not data: return
来源：http://tra.tarul.cn

PHP:  if (!$data) { return; }
来源：http://vyd.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://qie.xuanzx.com

TS:   if (!data) return;
来源：http://jyy.daria6918.cn

Java: if (data == null) return;
来源：http://obu.ivvv.top

Go:   if data == nil { return }
来源：http://ysl.ppjwa.cn

Ruby: return if data.nil?
来源：http://knd.ydzc1.top

C#:   if (data == null) return;
来源：http://mfi.zdqjudy.top

================================================================================
来源：http://pac.zhaomingkeji.xyz

C. 函数与作用域
来源：http://seo.jinyuanbaomall.cn

================================================================================
来源：http://dsk.fehbvm.com

[C01] 定义函数
来源：http://xyu.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://okd.dianchejie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tse.jinqigfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://bku.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mvs.jyoumei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ext.epnwcf.com

Go:   func add(a, b int) int { return a + b }
来源：http://kxl.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://zgj.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qhh.cucudq.cn

[C02] 默认参数
来源：http://zpc.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://qlb.gotoacloud.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qlw.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://orc.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kbw.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uxi.tianlin.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zbs.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://pmv.ywan-chungtsiang.top

C#:   string Greet(string name = "World") => name;
来源：http://hil.chenlongwang.top

[C03] 可变参数
来源：http://rfc.guowangkeji.top

Py:   def total(*args): return sum(args)
来源：http://vev.gotoacloud.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://leo.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qta.jinghuilouyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vbg.smart0.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mez.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bqa.chenjidiqi.icu

Ruby: def total(*nums); nums.sum; end
来源：http://bal.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ahh.yuanzhike.top

[C04] 命名参数 / 关键字参数
来源：http://fin.redwolf501.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tec.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fae.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kpj.hcnkem.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jru.guowangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://uyt.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://nvq.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://ohi.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://acd.ydzc1.top

[C05] 返回多个值
来源：http://squ.daria6918.cn

Py:   return a, b
来源：http://ehw.tanke756.top

PHP:  return [$a, $b];
来源：http://yge.yonumen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kop.snrcjt.cn

TS:   return { a, b };
来源：http://soz.zdqjudy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dvi.mhx1999.top

Go:   return a, b
来源：http://udu.tian-w.cn

Ruby: return a, b
来源：http://dtk.chenzaomai.com

C#:   return (a, b);              // ValueTuple
来源：http://rbp.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://eyu.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://tmw.ydzc1.top

PHP:  $square = fn($x) => $x * $x;
来源：http://sao.yvedp.cn

JS:   const square = x => x * x;
来源：http://fho.yuxming.cn

TS:   const square = (x: number): number => x * x;
来源：http://ffn.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://etv.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://dhh.bbcook.cn

Ruby: square = ->(x) { x * x }
来源：http://jqs.jqgfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://bzo.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://vgb.yuxming.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rsl.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://vgf.kuanghao11.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wtf.9152youxi.cn

TS:   arr.map(String)
来源：http://bku.yonumen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pmg.smart0.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dlk.hnxiangtu.top

Ruby: arr.map(&:upcase)
来源：http://opv.shangyingyoupin.top

C#:   arr.Select(s => s.ToUpper())
来源：http://myp.vqdsnc.cn

[C08] 闭包
来源：http://cxb.gotoacloud.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ybe.yonumen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://grw.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://thu.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://auj.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hkp.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kag.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xwm.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gkv.shzxlz.cn

[C09] 递归
来源：http://bqy.redwolf501.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ung.jinyuanbaomall.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uqp.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jlz.jqgfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uek.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wio.ydjk.org.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://svz.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://evm.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ewm.yuxming.cn

[C10] 变量作用域
来源：http://utj.yuxming.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://muu.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hmn.zdbjq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uij.andypj.xyz


<!-- 参考信息 -->