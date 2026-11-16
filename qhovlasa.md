代发 wailian999

Ruby: a, b = b, a
来源：http://lrs.yongpay.top

C#:   (a, b) = (b, a);
来源：http://xuy.sufxvd.cn

[A20] 读取标准输入
来源：http://cwd.ybcxt.top

Py:   name = input("请输入：")
来源：http://kpx.birdmap.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ymo.c1oappe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dvh.fanxiaobao.xyz

TS:   // Node.js：readline 模块
来源：http://faj.sweek.top

Java: new Scanner(System.in).nextLine()
来源：http://uvo.zhongyouzk.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://afu.kuanghao11.cn

Ruby: gets.chomp
来源：http://onp.hfpthk.cn

C#:   Console.ReadLine();
来源：http://hmk.hysaishi.cn

[A21] 保留指定小数位输出
来源：http://lbr.yangfankeji.com

Py:   f"{3.14159:.2f}"
来源：http://czd.yongpay.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pcd.jiagoushi.top

JS:   (3.14159).toFixed(2)
来源：http://uzk.jiagoushi.top

TS:   (3.14159).toFixed(2)
来源：http://cjw.iojbl.cn

Java: String.format("%.2f", 3.14159)
来源：http://gha.yfazqb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rcl.guannengcc.top

Ruby: format("%.2f", 3.14159)
来源：http://ukl.fzhhl.top

C#:   3.14159.ToString("F2")
来源：http://xps.yj20258.top

[A22] 获取字符串长度
来源：http://dzb.fktsv.cn

Py:   len(s)
来源：http://rje.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uav.havefunace.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wqd.dianchejie.cn

TS:   s.length
来源：http://pll.hfpthk.cn

Java: s.length()
来源：http://pba.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vpb.yanxiufei.cn

Ruby: s.length
来源：http://ofh.yfazqb.com

C#:   s.Length
来源：http://hyf.hfpthk.cn

[A23] 大小写转换
来源：http://psz.ivvv.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wul.ydjk.org.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xnd.ppjwa.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mqm.dianchejie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bbb.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bnu.cucudq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://siq.tian-w.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rxb.sufxvd.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ivk.xuetiantiany.cn

[A24] 去除首尾空白
来源：http://xjy.haohaochexian.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fak.shzxlz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ixr.gogol.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bne.ydzc1.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zsq.zdqjudy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cyj.sjlbkw.cn

Go:   strings.TrimSpace(s)
来源：http://rkb.jyoumei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vmm.zhoulong.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pkw.epnwcf.com

[A25] 字符串比较
来源：http://sgv.yongpay.top

Py:   s1 == s2; s1 != s2
来源：http://fkl.zdqjudy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jlt.dianchejie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://izf.wangshuangyany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qng.nanxuanxn.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lel.gogol.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wxq.jinqigufen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://win.shanyushiyangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ucn.pycfn.com

[A26] 类型转换总览
来源：http://cni.bbcook.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://exm.xuanzx.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ipf.xziqi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lch.dianchejie.cn

TS:   Number() String() Boolean() x as number
来源：http://gxw.yangfankeji.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lbp.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dbn.quarkkingdee.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kzq.chenzaomai.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wym.ehwqpu.com

================================================================================
来源：http://ehh.yonumen.top

B. 流程控制
来源：http://hmg.cqqwz.cn

================================================================================
来源：http://wdp.yonumen.top

[B01] 条件判断 if / else
来源：http://yqu.yueranfly.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ric.jqgfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hdq.wangdashe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qxm.zhaomingkeji.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vjc.jianghu66.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://idi.iojbl.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mes.zhongyouzk.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oyo.wangshuangyany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://igi.iojbl.cn

[B02] 多分支 else if / elif
来源：http://hyx.birdmap.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rpx.yanxiufei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ocj.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vav.hesvh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ont.cqqwz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rlo.ydzc1.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ehw.ydzc1.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qnq.nanxinkj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bri.yonumen.top

[B03] switch / match / case
来源：http://nvp.sweek.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gvu.zycfv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fto.sufxvd.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://atu.cashguo.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eau.ywan-chungtsiang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cyy.0kj1m.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lcj.shuidangran.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dmy.0kj1m.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nhn.ybcxt.top

[B04] for 计数循环
来源：http://prm.dianchejie.cn

Py:   for i in range(10): print(i)
来源：http://xfk.feifeiyinyue.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ber.gzhubu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lau.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pkl.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dzn.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nvh.ppjwa.cn

Ruby: 10.times { |i| puts i }
来源：http://taf.hnqzz.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pjl.cashguo.top

[B05] 遍历数组 / 列表
来源：http://mnb.jyoumei.cn

Py:   for item in arr: print(item)
来源：http://qla.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fci.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bdx.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rne.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qmg.fanxiaobao.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fys.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://mkh.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nnf.chenlongwang.top

[B06] 遍历字典 / 对象
来源：http://ixt.zdqjudy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uju.yuxming.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://goi.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lhg.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iaz.kuanghao11.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cqw.shuidangran.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jgh.iojbl.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ibz.svipenyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vpp.wangdashe.top

[B07] while 循环
来源：http://emv.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://jxa.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rue.aibaodan.cn

JS:   while (i < 10) { i++; }
来源：http://gid.havefunace.top

TS:   while (i < 10) { i++; }
来源：http://ltl.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://xeb.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hpc.daria6918.cn

Ruby: while i < 10; i += 1; end
来源：http://qeq.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://nfq.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://dvc.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://mkn.mhx1999.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ukc.sjlbkw.cn

JS:   do { i++; } while (i < 10);
来源：http://xxu.redwolf501.top

TS:   do { i++; } while (i < 10);
来源：http://cby.shuidangran.top

Java: do { i++; } while (i < 10);
来源：http://ymb.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://bst.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://aka.birdmap.top

C#:   do { i++; } while (i < 10);
来源：http://xbl.bjfxy.top

[B09] break 与 continue
来源：http://yab.shzxlz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dmq.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hkg.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nli.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dwq.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sbh.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rtr.vehdjk.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jxu.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ezk.zhongyouzk.top

[B10] 遍历同时拿索引
来源：http://wqv.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iqc.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vph.tanke756.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fgi.yuxming.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yni.316326.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mri.shuidangran.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rkn.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hrd.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uun.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://btp.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://klw.dianchejie.cn

PHP:  range(0, 10, 2);
来源：http://mqs.hcnkem.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gxc.zhongyouzk.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jds.52xcode.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://izh.yj202588.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fjr.aizwys.cn

Ruby: (0...10).step(2).to_a
来源：http://avt.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://slw.smart0.xyz

[B12] 跳出多层循环
来源：http://atc.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://feq.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://nny.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wdc.birdmap.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ttm.zhijiandao.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kco.jqgfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://seu.aizwys.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://utm.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jcu.meibo888.top

[B13] 判断是否为数字
来源：http://akc.shanyushiyangtech.top

Py:   isinstance(x, (int, float))
来源：http://pqh.sufxvd.cn

PHP:  is_numeric($x)
来源：http://fub.yfazqb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lmz.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bka.smart0.xyz

Java: x instanceof Number
来源：http://nly.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xpq.hesvh.cn

Ruby: x.is_a?(Numeric)
来源：http://ysv.meibo888.top

C#:   x is int or double or decimal
来源：http://hiz.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://nwp.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xjc.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pyg.uphjek.com

JS:   [1, 2, 3].includes(x)
来源：http://qot.tanke756.top

TS:   [1, 2, 3].includes(x)
来源：http://wmt.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bpk.tianlin.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kfp.bjfxy.top

Ruby: [1, 2, 3].include?(x)
来源：http://mxs.tianlin.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pea.hnqzz.top

[B15] 布尔运算与取反
来源：http://ofd.shuidangran.top

Py:   a and b or not c
来源：http://ewo.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://bkw.vehdjk.com

JS:   a && b || !c
来源：http://frt.yfazqb.com

TS:   a && b || !c
来源：http://ege.cqqwz.cn

Java: a && b || !c
来源：http://eev.yj202588.top

Go:   a && b || !c
来源：http://vli.jianghu66.top

Ruby: a && b || !c
来源：http://edf.gzhubu.top

C#:   a && b || !c
来源：http://txc.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mam.hysaishi.cn

Py:   if not data: return
来源：http://kjo.birdmap.top

PHP:  if (!$data) { return; }
来源：http://gkk.fanxiaobao.xyz

JS:   if (!data) return;
来源：http://roi.shzxlz.cn

TS:   if (!data) return;
来源：http://tav.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://lsw.dianchejie.cn

Go:   if data == nil { return }
来源：http://ftr.vehdjk.com

Ruby: return if data.nil?
来源：http://lyn.yongpay.top

C#:   if (data == null) return;
来源：http://dty.xuanzx.com

================================================================================
来源：http://ujz.tianlin.xyz

C. 函数与作用域
来源：http://qyd.jinyuanbaomall.cn

================================================================================
来源：http://sal.uphjek.com

[C01] 定义函数
来源：http://gwy.guannengcc.top

Py:   def add(a, b): return a + b
来源：http://lac.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cnk.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://cax.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ydg.sweek.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oxa.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vpa.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://kvz.xuanzx.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gvm.yonumen.top

[C02] 默认参数
来源：http://wjs.shzxlz.cn

Py:   def greet(name="World"): return name
来源：http://ppn.chenlongwang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mnv.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://shm.0kj1m.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gwn.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ofz.xuanzx.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aqi.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://okv.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://cth.chenzaomai.com

[C03] 可变参数
来源：http://mgl.hcnkem.com

Py:   def total(*args): return sum(args)
来源：http://wgz.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rim.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rgo.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tmf.ppjwa.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wyn.daxiang520.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ljk.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://bva.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rte.fehbvm.com

[C04] 命名参数 / 关键字参数
来源：http://mhl.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xgd.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://etp.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mnq.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://psa.yj20258.top

Java: // 无：用 Builder 模式或 record
来源：http://yfu.sysykeji.top

Go:   // 无：用配置结构体参数
来源：http://kvh.gogol.net.cn

Ruby: f(a: 1, b: 2)
来源：http://cuh.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://nue.tarul.cn

[C05] 返回多个值
来源：http://xri.quarkkingdee.top

Py:   return a, b
来源：http://svb.mhx1999.top

PHP:  return [$a, $b];
来源：http://pxy.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cyq.andypj.xyz

TS:   return { a, b };
来源：http://flr.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://afp.wangshuangyany.cn

Go:   return a, b
来源：http://qok.feifeiyinyue.top

Ruby: return a, b
来源：http://gwn.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://amu.fzhhl.top

[C06] 匿名函数 / lambda
来源：http://nxb.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://usu.yvedp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hqb.jinqigufen.top

JS:   const square = x => x * x;
来源：http://nxj.daxiang520.top

TS:   const square = (x: number): number => x * x;
来源：http://xid.ybcxt.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vwe.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://wfr.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://boz.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://typ.epnwcf.com

[C07] 把函数作为参数传入
来源：http://akf.jlsjyb.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lor.sxryk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bos.yj20258888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gqb.ydjk.org.cn

TS:   arr.map(String)
来源：http://ebw.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zkm.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qqe.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://etv.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zrt.pengpengdd.cyou

[C08] 闭包
来源：http://oev.meibo888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yhd.birdmap.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hru.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oct.zdqjudy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gwx.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wqj.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oqn.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fho.uphjek.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bhx.sjlbkw.cn

[C09] 递归
来源：http://gkm.cdnleiting.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wri.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blf.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fer.zhoulong.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uad.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kkc.fengsongda.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hil.dashuyun.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fey.tianlin.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zyj.xuetiantiany.cn

[C10] 变量作用域
来源：http://ifc.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zvv.yfazqb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kia.fanxiaobao.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zcq.cashguo.top


<!-- 参考信息 -->