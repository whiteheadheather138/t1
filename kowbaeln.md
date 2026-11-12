代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vzv.ydjk.org.cn

Ruby: gets.chomp
来源：http://ukt.feifeiyinyue.top

C#:   Console.ReadLine();
来源：http://urm.zhoulong.xyz

[A21] 保留指定小数位输出
来源：http://ppm.haohaochexian.top

Py:   f"{3.14159:.2f}"
来源：http://xto.sjlbkw.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bca.yongpay.top

JS:   (3.14159).toFixed(2)
来源：http://myr.uphjek.com

TS:   (3.14159).toFixed(2)
来源：http://wcs.pycfn.com

Java: String.format("%.2f", 3.14159)
来源：http://cpq.shanyushiyangkeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ful.hcnkem.com

Ruby: format("%.2f", 3.14159)
来源：http://hby.yangfankeji.com

C#:   3.14159.ToString("F2")
来源：http://lgp.yj20258.top

[A22] 获取字符串长度
来源：http://rfn.zhaomingkeji.xyz

Py:   len(s)
来源：http://dwg.daria6918.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ciu.xuanzx.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://iuz.jiagoushi.top

TS:   s.length
来源：http://pbw.jinqigfzy.top

Java: s.length()
来源：http://cnr.vehdjk.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://obr.ydzc1.top

Ruby: s.length
来源：http://ulm.xuetiantiany.cn

C#:   s.Length
来源：http://fhk.nanxinkj.top

[A23] 大小写转换
来源：http://kpy.tian-w.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://taz.gaohongyu789.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://abq.yuxming.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hug.zhongyouzk.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nle.zhongyouzk.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ing.cdnleiting.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xmw.9152youxi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ufa.hnxiangtu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kdk.tanke756.top

[A24] 去除首尾空白
来源：http://wnj.yuxming.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wym.hesvh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://evm.jinqigfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uwy.nanxuanxn.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ztk.shuidangran.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lyk.52xcode.cn

Go:   strings.TrimSpace(s)
来源：http://rav.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tps.gaohongyu789.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dop.sweek.top

[A25] 字符串比较
来源：http://met.hnxiangtu.top

Py:   s1 == s2; s1 != s2
来源：http://kbx.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rgn.gotoacloud.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pup.nwbrower.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lrk.cheryme.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wmw.zdqjudy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yud.yj20258888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rxl.hesvh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bqk.52xcode.cn

[A26] 类型转换总览
来源：http://kvt.shuidangran.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cqw.dianchejie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kfm.vqdsnc.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nak.shanyushiyangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://ztj.zhiwuduotai.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ohd.xinyue.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bfp.chenlongwang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hur.xylfe.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ceq.0kj1m.cn

================================================================================
来源：http://pfo.sxryk.cn

B. 流程控制
来源：http://iah.0kj1m.cn

================================================================================
来源：http://vme.gogol.net.cn

[B01] 条件判断 if / else
来源：http://vpt.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dhi.jinqigfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qub.ppjwa.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xup.cashguo.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://btp.0kj1m.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tbm.gotoacloud.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kgg.xylfe.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qjx.0kj1m.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kla.cucudq.cn

[B02] 多分支 else if / elif
来源：http://lwp.ivvv.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://enq.sweek.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rdy.zhengqikj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zsf.sjlbkw.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ldl.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ifp.ctjpmb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lfo.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ays.bjfxy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gfk.ywan-chungtsiang.top

[B03] switch / match / case
来源：http://qtw.zdbjq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hrq.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fzk.jinqigfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fbp.bbcook.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://seq.ydjk.org.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zcq.redwolf501.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mye.tianlin.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ywx.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wfg.jinyuanbaomall.cn

[B04] for 计数循环
来源：http://oik.tian-w.cn

Py:   for i in range(10): print(i)
来源：http://sbi.jinqigfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://svl.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://azx.daria6918.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gja.xziqi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rfz.nanxinkj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gkk.yongpay.top

Ruby: 10.times { |i| puts i }
来源：http://dny.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ibw.birdmap.top

[B05] 遍历数组 / 列表
来源：http://vle.zhoulong.xyz

Py:   for item in arr: print(item)
来源：http://yds.yuanzhike.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rtv.havefunace.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gbp.ehwqpu.com

TS:   for (const item of arr) { console.log(item); }
来源：http://nqd.sjlbkw.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sis.pengpengdd.cyou

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oko.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://rra.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kkd.xziqi.cn

[B06] 遍历字典 / 对象
来源：http://rzy.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://igl.iojbl.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vms.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mvd.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xwc.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mql.xuanzx.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vof.epnwcf.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eqj.jiagoushi.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sst.tian-w.cn

[B07] while 循环
来源：http://fui.hnqzz.top

Py:   while i < 10: i += 1
来源：http://eyx.fengsongda.top

PHP:  while ($i < 10) { $i++; }
来源：http://rab.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://twx.shzxlz.cn

TS:   while (i < 10) { i++; }
来源：http://zxm.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://yur.xziqi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nxk.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://ufp.nanxinkj.top

C#:   while (i < 10) { i++; }
来源：http://dbh.gotoacloud.top

[B08] do-while（至少执行一次）
来源：http://kmi.daria6918.cn

Py:   # 无 do-while：用 while True + break
来源：http://qby.xinyue.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://zdn.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://bxw.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://rqp.fzhhl.top

Java: do { i++; } while (i < 10);
来源：http://cgg.hesvh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://amv.uphjek.com

Ruby: begin; i += 1; end while i < 10
来源：http://zws.zhengqikj.top

C#:   do { i++; } while (i < 10);
来源：http://adi.gaohongyu789.top

[B09] break 与 continue
来源：http://bak.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ijj.jinqigufen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nss.zdqjudy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zmn.epnwcf.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hes.smart0.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xxp.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://htq.feifeiyinyue.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://alz.xziqi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pbf.hcnkem.com

[B10] 遍历同时拿索引
来源：http://zfg.dashuyun.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://add.nanxuanxn.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xmj.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nbm.ctjpmb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wdq.sweek.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://evd.snrcjt.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://taj.meibo888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rmo.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://urk.daxiang520.top

[B11] 生成数字序列 / 区间
来源：http://hfo.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://vay.yj202588.top

PHP:  range(0, 10, 2);
来源：http://kkk.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ozl.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://izg.wangshuangyany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vah.yj20258.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lhr.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://kfe.chenjidiqi.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xph.iojbl.cn

[B12] 跳出多层循环
来源：http://ieo.aibaodan.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gmu.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://moo.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xsk.ppjwa.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ivk.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pxp.hesvh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nnh.birdmap.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xia.sweek.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rnn.bbcook.cn

[B13] 判断是否为数字
来源：http://dqe.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://iwp.hesvh.cn

PHP:  is_numeric($x)
来源：http://etq.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nsd.yonumen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xne.kuanghao11.cn

Java: x instanceof Number
来源：http://jks.yongpay.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eic.yvedp.cn

Ruby: x.is_a?(Numeric)
来源：http://jtr.fktsv.cn

C#:   x is int or double or decimal
来源：http://gea.uphjek.com

[B14] 判断值是否在集合内
来源：http://hlt.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://afd.shzxlz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fal.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://okv.andypj.xyz

TS:   [1, 2, 3].includes(x)
来源：http://gsq.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ojn.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xmu.zhoulong.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://kzj.aizwys.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gec.c1oappe.top

[B15] 布尔运算与取反
来源：http://knn.jqgufenzy.top

Py:   a and b or not c
来源：http://wpo.jiagoushi.top

PHP:  $a && $b || !$c
来源：http://cwd.xuetiantiany.cn

JS:   a && b || !c
来源：http://lxy.jinyuanbaomall.cn

TS:   a && b || !c
来源：http://ufw.wangshuangyany.cn

Java: a && b || !c
来源：http://kum.ehwqpu.com

Go:   a && b || !c
来源：http://uio.xziqi.cn

Ruby: a && b || !c
来源：http://nym.ivvv.top

C#:   a && b || !c
来源：http://yuc.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gyu.jianghu66.top

Py:   if not data: return
来源：http://hdt.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://auz.sxryk.cn

JS:   if (!data) return;
来源：http://yty.ywan-chungtsiang.top

TS:   if (!data) return;
来源：http://ick.jinghuilouyu.cn

Java: if (data == null) return;
来源：http://moz.zhoulong.xyz

Go:   if data == nil { return }
来源：http://aez.cdnleiting.top

Ruby: return if data.nil?
来源：http://igz.hywenlv.cn

C#:   if (data == null) return;
来源：http://mcz.hnxiangtu.top

================================================================================
来源：http://wsb.haohaochexian.top

C. 函数与作用域
来源：http://zit.zhoulong.xyz

================================================================================
来源：http://zgd.shuidangran.top

[C01] 定义函数
来源：http://cpu.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://ink.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wau.shangyingyoupin.top

JS:   function add(a, b) { return a + b; }
来源：http://rov.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zhd.fehbvm.com

Java: static int add(int a, int b) { return a + b; }
来源：http://axq.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://coy.hammf.cn

Ruby: def add(a, b); a + b; end
来源：http://bct.hywenlv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dbd.zycfv.cn

[C02] 默认参数
来源：http://mal.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://fqe.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://oei.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://fif.0kj1m.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ohq.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nno.quarkkingdee.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yia.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://nzo.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://jnd.ppjwa.cn

[C03] 可变参数
来源：http://vzs.jinqigfzy.top

Py:   def total(*args): return sum(args)
来源：http://hyq.daria6918.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tir.jlsjyb.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dwi.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://adx.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://boy.dianchejie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dfm.zdqjudy.top

Ruby: def total(*nums); nums.sum; end
来源：http://xob.fehbvm.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ylj.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://lcf.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mwb.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kag.yfazqb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xji.xingfuxueyuan.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zlm.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://vba.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://aey.zhoulong.xyz

Ruby: f(a: 1, b: 2)
来源：http://snf.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://cfw.gotoacloud.top

[C05] 返回多个值
来源：http://gau.sweek.top

Py:   return a, b
来源：http://jgv.tianlin.xyz

PHP:  return [$a, $b];
来源：http://tbv.yonumen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kla.hnqzz.top

TS:   return { a, b };
来源：http://kct.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://whq.xuanzx.com

Go:   return a, b
来源：http://mck.yongpay.top

Ruby: return a, b
来源：http://taz.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://dnw.jinqigufen.top

[C06] 匿名函数 / lambda
来源：http://hvs.haohaochexian.top

Py:   square = lambda x: x * x
来源：http://xjn.tianlin.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://bwj.yonumen.top

JS:   const square = x => x * x;
来源：http://iwc.bjfxy.top

TS:   const square = (x: number): number => x * x;
来源：http://syk.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://muh.daxiang520.top

Go:   sq := func(x int) int { return x * x }
来源：http://ifp.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://vpz.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://edx.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://wmc.jinqigufen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rut.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ouh.jinghuilouyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jlb.jqgfzy.top

TS:   arr.map(String)
来源：http://qjc.nwbrower.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://adu.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zew.bjfxy.top

Ruby: arr.map(&:upcase)
来源：http://dhv.kuanghao11.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ccz.quarkkingdee.top

[C08] 闭包
来源：http://gol.feifeiyinyue.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://clk.dashuyun.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uil.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://trf.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lno.smart0.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zid.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aln.zycfv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ayq.quarkkingdee.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uzn.yfazqb.com

[C09] 递归
来源：http://qui.dianchejie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://shc.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ffw.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://psy.aibaodan.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bmv.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kvj.jlsjyb.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://you.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lkk.tianlin.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zgv.ydzc1.top

[C10] 变量作用域
来源：http://hem.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lkl.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yry.hnxiangtu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mwv.iojbl.cn

TS:   同 JS
来源：http://oiw.quarkkingdee.top

Java: 方法内为块级作用域
来源：http://mwm.yj20258888.top

Go:   花括号块级作用域
来源：http://ezf.zhoulong.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wgm.jinqigufen.top

C#:   块级作用域
来源：http://piq.cashguo.top

[C11] 模块导入与导出
来源：http://hkm.gogol.net.cn

Py:   from module import func
来源：http://cnm.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rge.meibo888.top


<!-- 参考信息 -->