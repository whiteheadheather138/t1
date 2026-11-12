代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://myz.svipenyu.cn

Ruby: gets.chomp
来源：http://nyv.redwolf501.top

C#:   Console.ReadLine();
来源：http://pej.wangdashe.top

[A21] 保留指定小数位输出
来源：http://bjk.jqgufenzy.top

Py:   f"{3.14159:.2f}"
来源：http://ago.316326.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lfj.hnxiangtu.top

JS:   (3.14159).toFixed(2)
来源：http://swp.cucudq.cn

TS:   (3.14159).toFixed(2)
来源：http://ibt.zhaomingkeji.xyz

Java: String.format("%.2f", 3.14159)
来源：http://bdg.chenjidiqi.icu

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ijb.yonumen.top

Ruby: format("%.2f", 3.14159)
来源：http://omj.xziqi.cn

C#:   3.14159.ToString("F2")
来源：http://xrf.cqqwz.cn

[A22] 获取字符串长度
来源：http://lvk.xuanzx.com

Py:   len(s)
来源：http://mwf.jinghuilouyu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hjn.aibaodan.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cnl.vehdjk.com

TS:   s.length
来源：http://qyt.ivvv.top

Java: s.length()
来源：http://gcl.shuidangran.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://szk.zdqjudy.top

Ruby: s.length
来源：http://bnb.yj20258.top

C#:   s.Length
来源：http://wmk.yvedp.cn

[A23] 大小写转换
来源：http://gzz.vqdsnc.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ejv.52xcode.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vto.jyoumei.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wel.yueranfly.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jmw.guannengcc.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bkt.sjlbkw.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rsx.jiagoushi.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hik.andypj.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://hcj.vqdsnc.cn

[A24] 去除首尾空白
来源：http://sac.hnxiangtu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jrd.jlsjyb.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fsg.ehwqpu.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uhv.ctjpmb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hgq.ppjwa.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xoo.fehbvm.com

Go:   strings.TrimSpace(s)
来源：http://dhx.yfazqb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ake.sxryk.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hoz.hongshengwenyu.top

[A25] 字符串比较
来源：http://yqw.52xcode.cn

Py:   s1 == s2; s1 != s2
来源：http://cux.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://apn.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://maa.zdbjq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://puw.52xcode.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tso.bbcook.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lhp.zhijiandao.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ike.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wqh.zycfv.cn

[A26] 类型转换总览
来源：http://efa.jlsjyb.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tnh.zhoulong.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://haq.quarkkingdee.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vhs.gaohongyu789.top

TS:   Number() String() Boolean() x as number
来源：http://kdj.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rez.sxryk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rzy.sysykeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gvu.xuanzx.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zcm.birdmap.top

================================================================================
来源：http://blk.yangfankeji.com

B. 流程控制
来源：http://hgi.ywan-chungtsiang.top

================================================================================
来源：http://uee.sysykeji.top

[B01] 条件判断 if / else
来源：http://nhd.yongpay.top

Py:   result = "正" if x > 0 else "非正"
来源：http://yha.tarul.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xay.tanke756.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nrs.bbcook.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pbw.hesvh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bnb.daxiang520.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sei.cheryme.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vvq.dianchejie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://twv.havefunace.top

[B02] 多分支 else if / elif
来源：http://tyr.jianghu66.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pip.xinyue.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nbj.quarkkingdee.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://grd.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fyk.yj20258888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pnl.chenjidiqi.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gbv.fanxiaobao.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://riu.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbn.zdqjudy.top

[B03] switch / match / case
来源：http://mfm.ydjk.org.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jbx.tanke756.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qxe.chenzaomai.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zia.yangfankeji.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rsn.iojbl.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lwf.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iaw.hfpthk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sbu.ydzc1.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://itf.haohaochexian.top

[B04] for 计数循环
来源：http://txc.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://gjp.pengpengdd.cyou

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nmo.hcnkem.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hqb.zhijiandao.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jpy.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sbk.aizwys.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kry.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://nxb.hcnkem.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://npu.zhixingplan.top

[B05] 遍历数组 / 列表
来源：http://hom.zhoulong.xyz

Py:   for item in arr: print(item)
来源：http://zpu.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lyz.hywenlv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zxn.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pau.yuanzhike.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vvm.sysykeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mtq.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://qyn.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cfn.jlsjyb.cn

[B06] 遍历字典 / 对象
来源：http://xej.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kll.wangdashe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gtd.cucudq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bla.yuanzhike.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dxc.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://avx.nanxinkj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fle.fzhhl.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gbm.ppjwa.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://irr.cqqwz.cn

[B07] while 循环
来源：http://kls.tanke756.top

Py:   while i < 10: i += 1
来源：http://dsd.ydjk.org.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ouc.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://teb.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://amj.hongshengwenyu.top

Java: while (i < 10) { i++; }
来源：http://nxg.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uod.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://ciq.hnxiangtu.top

C#:   while (i < 10) { i++; }
来源：http://sfi.hysaishi.cn

[B08] do-while（至少执行一次）
来源：http://mgg.ehwqpu.com

Py:   # 无 do-while：用 while True + break
来源：http://qmb.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rtk.shuidangran.top

JS:   do { i++; } while (i < 10);
来源：http://jwp.hywenlv.cn

TS:   do { i++; } while (i < 10);
来源：http://sfz.fktsv.cn

Java: do { i++; } while (i < 10);
来源：http://aap.zhongyouzk.top

Go:   for { i++; if i >= 10 { break } }
来源：http://flr.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://oif.yuanzhike.top

C#:   do { i++; } while (i < 10);
来源：http://jxg.yangfankeji.com

[B09] break 与 continue
来源：http://fap.gogol.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wri.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xty.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yjf.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qxz.cheryme.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qpl.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aft.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://apy.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tah.aizwys.cn

[B10] 遍历同时拿索引
来源：http://ynx.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jdb.yj20258.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://elv.9152youxi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ast.zycfv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://knw.snrcjt.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aue.nanxuanxn.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bcm.shuidangran.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gmm.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jkm.ehwqpu.com

[B11] 生成数字序列 / 区间
来源：http://usr.gaohongyu789.top

Py:   list(range(0, 10, 2))
来源：http://iwd.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://fdp.hesvh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://quq.hcnkem.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blz.bbcook.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://apu.jinqigufen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tvf.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://ryi.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dry.sysykeji.top

[B12] 跳出多层循环
来源：http://wuo.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bcc.tianlin.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://hcz.cheryme.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tuf.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dst.yvedp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rzq.haohaochexian.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ftk.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jdz.hnqzz.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vbw.jinqigfzy.top

[B13] 判断是否为数字
来源：http://vps.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://ytq.xuanzx.com

PHP:  is_numeric($x)
来源：http://wkx.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ele.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gca.52xcode.cn

Java: x instanceof Number
来源：http://yyc.zdbjq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gpu.cheryme.top

Ruby: x.is_a?(Numeric)
来源：http://aor.ppjwa.cn

C#:   x is int or double or decimal
来源：http://wqx.ctjpmb.com

[B14] 判断值是否在集合内
来源：http://krk.fehbvm.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uwn.xziqi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hgy.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://bfk.zhaomingkeji.xyz

TS:   [1, 2, 3].includes(x)
来源：http://xih.hfpthk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vcr.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bbk.zhoulong.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://zhk.pycfn.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ymq.xuetiantiany.cn

[B15] 布尔运算与取反
来源：http://dvl.tarul.cn

Py:   a and b or not c
来源：http://qdh.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://olm.pengpengdd.cyou

JS:   a && b || !c
来源：http://myt.jqgufenzy.top

TS:   a && b || !c
来源：http://eto.fktsv.cn

Java: a && b || !c
来源：http://dnf.yj20258888.top

Go:   a && b || !c
来源：http://dps.svipenyu.cn

Ruby: a && b || !c
来源：http://dva.jinqigufen.top

C#:   a && b || !c
来源：http://hbr.wangdashe.top

[B16] 卫语句：不满足条件提前返回
来源：http://rqg.yj20258888.top

Py:   if not data: return
来源：http://zds.uphjek.com

PHP:  if (!$data) { return; }
来源：http://gml.wangdashe.top

JS:   if (!data) return;
来源：http://roq.bjfxy.top

TS:   if (!data) return;
来源：http://zut.jinghuilouyu.cn

Java: if (data == null) return;
来源：http://qnb.havefunace.top

Go:   if data == nil { return }
来源：http://dzt.yonumen.top

Ruby: return if data.nil?
来源：http://ofh.hfpthk.cn

C#:   if (data == null) return;
来源：http://sqe.nwbrower.top

================================================================================
来源：http://ceo.wangshuangyany.cn

C. 函数与作用域
来源：http://atj.ivvv.top

================================================================================
来源：http://zqz.yonumen.top

[C01] 定义函数
来源：http://she.yvedp.cn

Py:   def add(a, b): return a + b
来源：http://mus.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hau.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://shg.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sun.bbcook.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://prb.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://ufq.aizwys.cn

Ruby: def add(a, b); a + b; end
来源：http://ecz.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rmj.zdqjudy.top

[C02] 默认参数
来源：http://yff.shzxlz.cn

Py:   def greet(name="World"): return name
来源：http://uud.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fro.tanke756.top

JS:   function greet(name = "World") { return name; }
来源：http://xov.ehwqpu.com

TS:   function greet(name: string = "World") { return name; }
来源：http://ypi.tarul.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bqr.c1oappe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kcy.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://kjc.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://awy.aibaodan.cn

[C03] 可变参数
来源：http://xzq.vehdjk.com

Py:   def total(*args): return sum(args)
来源：http://hwr.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hgl.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rbo.zdqjudy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cek.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://drd.bbcook.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eaz.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kva.pycfn.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dhe.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://vmv.hammf.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ftz.daria6918.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lky.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qrl.bjfxy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://via.fehbvm.com

Java: // 无：用 Builder 模式或 record
来源：http://qkl.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://ygn.dashuyun.cn

Ruby: f(a: 1, b: 2)
来源：http://tht.yfazqb.com

C#:   f(a: 1, b: 2)
来源：http://xvv.nanxuanxn.top

[C05] 返回多个值
来源：http://uep.fzhhl.top

Py:   return a, b
来源：http://zkb.jqgufenzy.top

PHP:  return [$a, $b];
来源：http://qmm.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mvx.ydjk.org.cn

TS:   return { a, b };
来源：http://czk.epnwcf.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zvw.quarkkingdee.top

Go:   return a, b
来源：http://pdi.dianchejie.cn

Ruby: return a, b
来源：http://tja.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://nhx.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://eix.yongpay.top

Py:   square = lambda x: x * x
来源：http://mcf.uphjek.com

PHP:  $square = fn($x) => $x * $x;
来源：http://sty.hesvh.cn

JS:   const square = x => x * x;
来源：http://zwk.gogol.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://ssi.hongshengwenyu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fej.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://rdw.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://uok.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://wwg.9152youxi.cn

[C07] 把函数作为参数传入
来源：http://ikq.wangshuangyany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zgq.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gmx.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mue.zhiwuduotai.top

TS:   arr.map(String)
来源：http://vkq.ehwqpu.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dui.cdnleiting.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bdf.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://vfb.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yos.jlsjyb.cn

[C08] 闭包
来源：http://chl.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vcl.bbcook.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nbe.chenzaomai.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dkp.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pbe.birdmap.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aqb.pycfn.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nss.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tzs.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uby.nanxinkj.top

[C09] 递归
来源：http://ruv.nwbrower.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jto.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pld.xinyue.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hkz.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://quc.tian-w.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fuh.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ipy.shzxlz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bfu.gogol.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qmq.yonumen.top

[C10] 变量作用域
来源：http://boi.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rth.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uif.feifeiyinyue.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mar.52xcode.cn

TS:   同 JS
来源：http://oqr.ivvv.top

Java: 方法内为块级作用域
来源：http://kei.jianghu66.top

Go:   花括号块级作用域
来源：http://bgn.ydjk.org.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rxx.smart0.xyz

C#:   块级作用域
来源：http://ien.cheryme.top

[C11] 模块导入与导出
来源：http://mps.sjlbkw.cn

Py:   from module import func
来源：http://vnr.jqgufenzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qpd.hammf.cn


<!-- 参考信息 -->