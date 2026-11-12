代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://auc.nwbrower.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iwg.jlsjyb.cn

TS:   // Node.js：readline 模块
来源：http://xsn.fengsongda.top

Java: new Scanner(System.in).nextLine()
来源：http://nyx.yangfankeji.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bqn.fktsv.cn

Ruby: gets.chomp
来源：http://jxu.hfpthk.cn

C#:   Console.ReadLine();
来源：http://frg.316326.xyz

[A21] 保留指定小数位输出
来源：http://mxt.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://eyh.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xgq.chenjidiqi.icu

JS:   (3.14159).toFixed(2)
来源：http://vav.mhx1999.top

TS:   (3.14159).toFixed(2)
来源：http://tfv.daria6918.cn

Java: String.format("%.2f", 3.14159)
来源：http://nvx.zhoulong.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kwa.jqgufenzy.top

Ruby: format("%.2f", 3.14159)
来源：http://ani.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://ano.mhx1999.top

[A22] 获取字符串长度
来源：http://npf.jinqigufen.top

Py:   len(s)
来源：http://mcr.ybcxt.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jxb.daxiang520.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tch.cdnleiting.top

TS:   s.length
来源：http://czs.havefunace.top

Java: s.length()
来源：http://myh.yj20258888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pbv.hongshengwenyu.top

Ruby: s.length
来源：http://trj.xuetiantiany.cn

C#:   s.Length
来源：http://skq.cashguo.top

[A23] 大小写转换
来源：http://cxu.jinqigufen.top

Py:   s.upper(); s.lower(); s.title()
来源：http://awj.fehbvm.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pwi.bbcook.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bxi.guannengcc.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vpp.jqgufenzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://asi.zdbjq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://joa.hysaishi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ssb.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yeg.yj202588.top

[A24] 去除首尾空白
来源：http://nrt.cucudq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zsn.tian-w.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lsw.jlsjyb.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xlc.pengpengdd.cyou

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zej.smart0.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ncx.mhx1999.top

Go:   strings.TrimSpace(s)
来源：http://itn.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ybq.hfpthk.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zpk.yj202588.top

[A25] 字符串比较
来源：http://ozt.hesvh.cn

Py:   s1 == s2; s1 != s2
来源：http://htk.gaohongyu789.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dpc.wangdashe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hii.yonumen.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zrd.wangshuangyany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://crh.svipenyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://piy.vqdsnc.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fkc.yfazqb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xuj.smart0.xyz

[A26] 类型转换总览
来源：http://thc.xuanzx.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ryd.snrcjt.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hep.yanxiufei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vln.cucudq.cn

TS:   Number() String() Boolean() x as number
来源：http://vdo.hongshengwenyu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gft.hesvh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mea.nwbrower.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ovv.yfazqb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qti.316326.xyz

================================================================================
来源：http://jnm.mhx1999.top

B. 流程控制
来源：http://msq.gaohongyu789.top

================================================================================
来源：http://sya.yueranfly.top

[B01] 条件判断 if / else
来源：http://pjw.bbcook.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aiy.hongshengwenyu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ajr.hnxiangtu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hrc.epnwcf.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ntr.fzhhl.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yiv.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sfe.daxiang520.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://npz.dashuyun.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ywq.hfpthk.cn

[B02] 多分支 else if / elif
来源：http://rtw.vqdsnc.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qtp.haohaochexian.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rqn.gzhubu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vdh.jqgufenzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pmt.bjfxy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iua.zhoulong.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fmk.chenjidiqi.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wpd.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://boq.nanxuanxn.top

[B03] switch / match / case
来源：http://evr.fktsv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vhc.cashguo.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://udp.xziqi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fmr.svipenyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://otg.ctjpmb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ppr.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pqt.52xcode.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fcq.hnqzz.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dtt.yvedp.cn

[B04] for 计数循环
来源：http://obv.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://uwp.jlsjyb.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zvc.ywan-chungtsiang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xfr.birdmap.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jqd.fktsv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://quj.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lqs.hnqzz.top

Ruby: 10.times { |i| puts i }
来源：http://kju.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rtk.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://umt.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://xgh.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qyj.uphjek.com

JS:   for (const item of arr) { console.log(item); }
来源：http://dms.chenjidiqi.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://etz.cheryme.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uqz.ivvv.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ggn.dashuyun.cn

Ruby: arr.each { |item| puts item }
来源：http://jot.uphjek.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rcj.aizwys.cn

[B06] 遍历字典 / 对象
来源：http://fwu.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fzk.gaohongyu789.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tgw.fktsv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dzo.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://scu.andypj.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bey.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nqd.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rzw.wangshuangyany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lhv.gzhubu.top

[B07] while 循环
来源：http://ouf.daria6918.cn

Py:   while i < 10: i += 1
来源：http://yio.daria6918.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hjd.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://pvz.xingfuxueyuan.xyz

TS:   while (i < 10) { i++; }
来源：http://mvt.yfazqb.com

Java: while (i < 10) { i++; }
来源：http://koi.hcnkem.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bgn.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://miv.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://vfb.sweek.top

[B08] do-while（至少执行一次）
来源：http://ppc.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://fqf.jiagoushi.top

PHP:  do { $i++; } while ($i < 10);
来源：http://tqr.gaohongyu789.top

JS:   do { i++; } while (i < 10);
来源：http://boe.xuetiantiany.cn

TS:   do { i++; } while (i < 10);
来源：http://zfj.quarkkingdee.top

Java: do { i++; } while (i < 10);
来源：http://vnl.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://sqr.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://rqm.zhengqikj.top

C#:   do { i++; } while (i < 10);
来源：http://zky.svipenyu.cn

[B09] break 与 continue
来源：http://ljs.jlsjyb.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rdp.zdqjudy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://byr.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hrr.ivvv.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qta.gotoacloud.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eoh.svipenyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wrw.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jhh.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aaq.zdbjq.cn

[B10] 遍历同时拿索引
来源：http://rxw.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wqv.yanxiufei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fej.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yqd.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rkf.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cqw.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mry.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fom.quarkkingdee.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pns.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://oqh.tianlin.xyz

Py:   list(range(0, 10, 2))
来源：http://dil.yuxming.cn

PHP:  range(0, 10, 2);
来源：http://juc.chenjidiqi.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zwz.xylfe.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zws.ydzc1.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gwz.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qat.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://lvw.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kcs.chenzaomai.com

[B12] 跳出多层循环
来源：http://yai.zycfv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://imw.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xoy.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tne.hnxiangtu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://usj.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rbc.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://elu.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xmt.gzhubu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blc.jlsjyb.cn

[B13] 判断是否为数字
来源：http://sio.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://hfq.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://edi.gaohongyu789.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mfs.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dou.haohaochexian.top

Java: x instanceof Number
来源：http://lvx.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hup.cucudq.cn

Ruby: x.is_a?(Numeric)
来源：http://ajn.mhx1999.top

C#:   x is int or double or decimal
来源：http://krd.gzhubu.top

[B14] 判断值是否在集合内
来源：http://agx.sysykeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://txz.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kaz.shuidangran.top

JS:   [1, 2, 3].includes(x)
来源：http://flc.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://oml.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://giw.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eub.bbcook.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nkc.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uwt.cashguo.top

[B15] 布尔运算与取反
来源：http://sud.316326.xyz

Py:   a and b or not c
来源：http://mad.havefunace.top

PHP:  $a && $b || !$c
来源：http://qox.yuxming.cn

JS:   a && b || !c
来源：http://tba.yj202588.top

TS:   a && b || !c
来源：http://iqt.svipenyu.cn

Java: a && b || !c
来源：http://fto.birdmap.top

Go:   a && b || !c
来源：http://zlq.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://mrr.tanke756.top

C#:   a && b || !c
来源：http://igp.fktsv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ayy.fanxiaobao.xyz

Py:   if not data: return
来源：http://dar.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://vvn.tianlin.xyz

JS:   if (!data) return;
来源：http://xij.uphjek.com

TS:   if (!data) return;
来源：http://oul.yfazqb.com

Java: if (data == null) return;
来源：http://dxf.fktsv.cn

Go:   if data == nil { return }
来源：http://dsr.yanxiufei.cn

Ruby: return if data.nil?
来源：http://qnf.wangdashe.top

C#:   if (data == null) return;
来源：http://hja.xziqi.cn

================================================================================
来源：http://btr.jinyuanbaomall.cn

C. 函数与作用域
来源：http://rmx.havefunace.top

================================================================================
来源：http://idh.ywan-chungtsiang.top

[C01] 定义函数
来源：http://aqw.smart0.xyz

Py:   def add(a, b): return a + b
来源：http://uhx.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jri.guannengcc.top

JS:   function add(a, b) { return a + b; }
来源：http://dkl.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jkd.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://sit.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://akt.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://ply.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oau.shuidangran.top

[C02] 默认参数
来源：http://tob.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://gas.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vbj.0kj1m.cn

JS:   function greet(name = "World") { return name; }
来源：http://uwy.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://cyy.cucudq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tip.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sxe.guannengcc.top

Ruby: def greet(name = "World") = name
来源：http://fgd.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://xef.sysykeji.top

[C03] 可变参数
来源：http://aph.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://jut.cucudq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://doc.zhaomingkeji.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yro.cheryme.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ntq.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ubl.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zsa.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://wcm.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zrv.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://rql.aibaodan.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://agb.daria6918.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cxv.yj20258888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wzh.fengsongda.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bub.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://mzk.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://dqx.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://hdk.kuanghao11.cn

C#:   f(a: 1, b: 2)
来源：http://uky.pycfn.com

[C05] 返回多个值
来源：http://pja.gogol.net.cn

Py:   return a, b
来源：http://dyu.jiagoushi.top

PHP:  return [$a, $b];
来源：http://coz.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yed.aizwys.cn

TS:   return { a, b };
来源：http://max.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://env.nwbrower.top

Go:   return a, b
来源：http://apo.shanyushiyangtech.top

Ruby: return a, b
来源：http://zti.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://exx.zhijiandao.cn

[C06] 匿名函数 / lambda
来源：http://uir.chenjidiqi.icu

Py:   square = lambda x: x * x
来源：http://mzk.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://csk.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://gpw.jinqigufen.top

TS:   const square = (x: number): number => x * x;
来源：http://ryi.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gfj.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ydv.zhongyouzk.top

Ruby: square = ->(x) { x * x }
来源：http://asg.hfpthk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kkh.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://gpn.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ckp.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://env.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jiw.jlsjyb.cn

TS:   arr.map(String)
来源：http://ysi.yanxiufei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pdv.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://adb.pycfn.com

Ruby: arr.map(&:upcase)
来源：http://mfd.yfazqb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://jcl.fktsv.cn

[C08] 闭包
来源：http://knd.birdmap.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yta.snrcjt.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yfm.xingfuxueyuan.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://biy.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xud.wangdashe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hki.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tnt.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://itl.jinyuanbaomall.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yhx.vqdsnc.cn

[C09] 递归
来源：http://nyp.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://azx.gzhubu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://los.pycfn.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://izy.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ncm.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rzr.xylfe.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rre.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xwj.vqdsnc.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pth.yongpay.top

[C10] 变量作用域
来源：http://din.guowangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fgq.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gcb.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cps.gzhubu.top

TS:   同 JS
来源：http://ovv.snrcjt.cn

Java: 方法内为块级作用域
来源：http://rie.cheryme.top

Go:   花括号块级作用域
来源：http://ljk.zhijiandao.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://edg.tarul.cn


<!-- 参考信息 -->