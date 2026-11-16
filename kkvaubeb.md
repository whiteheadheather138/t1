代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jot.gzhubu.top

Ruby: gets.chomp
来源：http://gwx.hnqzz.top

C#:   Console.ReadLine();
来源：http://mhm.jinyuanbaomall.cn

[A21] 保留指定小数位输出
来源：http://map.ctjpmb.com

Py:   f"{3.14159:.2f}"
来源：http://yre.iojbl.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ulp.pengpengdd.cyou

JS:   (3.14159).toFixed(2)
来源：http://vji.9152youxi.cn

TS:   (3.14159).toFixed(2)
来源：http://hly.svipenyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://hyw.hesvh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://htq.sjlbkw.cn

Ruby: format("%.2f", 3.14159)
来源：http://ucx.jinghuilouyu.cn

C#:   3.14159.ToString("F2")
来源：http://yge.zhiwuduotai.top

[A22] 获取字符串长度
来源：http://nmj.jinqigufen.top

Py:   len(s)
来源：http://vol.dashuyun.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://crt.meibo888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sut.yueranfly.top

TS:   s.length
来源：http://knc.fanxiaobao.xyz

Java: s.length()
来源：http://oqj.fzhhl.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hkd.tanke756.top

Ruby: s.length
来源：http://nbf.vqdsnc.cn

C#:   s.Length
来源：http://ynh.yj20258.top

[A23] 大小写转换
来源：http://com.yuanzhike.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ogf.ppjwa.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kgj.tanke756.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bdk.zdqjudy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gdx.ydjk.org.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qsg.zhongyouzk.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sqc.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://plo.daria6918.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://aex.nanxuanxn.top

[A24] 去除首尾空白
来源：http://jmv.jianghu66.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jae.zhaomingkeji.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://soq.0kj1m.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://myg.yj202588.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hya.jinqigfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dtw.fzhhl.top

Go:   strings.TrimSpace(s)
来源：http://jyk.yj20258888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dya.mhx1999.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cqw.cashguo.top

[A25] 字符串比较
来源：http://ifs.yanxiufei.cn

Py:   s1 == s2; s1 != s2
来源：http://bbo.jinqigfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xvb.yonumen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yol.shangyingyoupin.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jcj.c1oappe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qmh.fanxiaobao.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ava.yuxming.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fvd.ywan-chungtsiang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xld.tanke756.top

[A26] 类型转换总览
来源：http://upt.xuanzx.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://avi.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pwt.ydjk.org.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://puw.iojbl.cn

TS:   Number() String() Boolean() x as number
来源：http://nsw.snrcjt.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vux.pengpengdd.cyou

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dbe.tian-w.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fro.yj20258888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sit.zhoulong.xyz

================================================================================
来源：http://yfu.cashguo.top

B. 流程控制
来源：http://rap.jinqigufen.top

================================================================================
来源：http://dzk.zdqjudy.top

[B01] 条件判断 if / else
来源：http://nyn.xingfuxueyuan.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://ilg.feifeiyinyue.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wkc.ydzc1.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xla.gaohongyu789.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wyt.fengsongda.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dmh.havefunace.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hpa.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tas.jlsjyb.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fth.fengsongda.top

[B02] 多分支 else if / elif
来源：http://wny.zhiwuduotai.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pcc.cdnleiting.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dxd.yonumen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qwu.ybcxt.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qyy.ehwqpu.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://crr.yangfankeji.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rau.yonumen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yhw.jianghu66.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ubu.ppjwa.cn

[B03] switch / match / case
来源：http://mbq.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kow.sysykeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vuj.ydjk.org.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nxo.yj20258888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://awm.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ztx.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vrx.shanyushiyangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xea.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lyu.yj20258.top

[B04] for 计数循环
来源：http://znx.andypj.xyz

Py:   for i in range(10): print(i)
来源：http://rzq.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://snh.zhongyouzk.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fst.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oux.vehdjk.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hyn.fengsongda.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ogz.zhiwuduotai.top

Ruby: 10.times { |i| puts i }
来源：http://egv.316326.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fxq.jinqigfzy.top

[B05] 遍历数组 / 列表
来源：http://yiw.havefunace.top

Py:   for item in arr: print(item)
来源：http://zdz.jqgfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://giq.birdmap.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hce.havefunace.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ehf.andypj.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://hvl.chenlongwang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zqb.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://uin.cdnleiting.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qoa.iojbl.cn

[B06] 遍历字典 / 对象
来源：http://oan.ppjwa.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iyn.fzhhl.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://svg.zhoulong.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rvw.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jpy.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jlp.yanxiufei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vji.yfazqb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xrj.yonumen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://brv.cashguo.top

[B07] while 循环
来源：http://phw.c1oappe.top

Py:   while i < 10: i += 1
来源：http://gfk.hongshengwenyu.top

PHP:  while ($i < 10) { $i++; }
来源：http://swv.yanxiufei.cn

JS:   while (i < 10) { i++; }
来源：http://zzi.xuanzx.com

TS:   while (i < 10) { i++; }
来源：http://piu.cheryme.top

Java: while (i < 10) { i++; }
来源：http://rlj.cqqwz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zes.daria6918.cn

Ruby: while i < 10; i += 1; end
来源：http://gtr.fktsv.cn

C#:   while (i < 10) { i++; }
来源：http://yfk.ivvv.top

[B08] do-while（至少执行一次）
来源：http://dxg.daria6918.cn

Py:   # 无 do-while：用 while True + break
来源：http://xsy.shanyushiyangtech.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vzn.aizwys.cn

JS:   do { i++; } while (i < 10);
来源：http://vtw.hcnkem.com

TS:   do { i++; } while (i < 10);
来源：http://kkn.gogol.net.cn

Java: do { i++; } while (i < 10);
来源：http://nkr.shuidangran.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ccx.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hbj.jinqigufen.top

C#:   do { i++; } while (i < 10);
来源：http://thq.xingfuxueyuan.xyz

[B09] break 与 continue
来源：http://xtj.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xrs.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eew.cashguo.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jhw.zycfv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://keu.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gvf.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dup.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fvu.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://skj.dashuyun.cn

[B10] 遍历同时拿索引
来源：http://euu.zhongyouzk.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://suq.yj202588.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xwd.smart0.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oro.yfazqb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tjb.sxryk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ywe.pycfn.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pus.guannengcc.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pph.redwolf501.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qrq.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://zbx.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://zev.yueranfly.top

PHP:  range(0, 10, 2);
来源：http://gjq.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ebj.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sub.hfpthk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pmn.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fsm.tarul.cn

Ruby: (0...10).step(2).to_a
来源：http://vph.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tze.hywenlv.cn

[B12] 跳出多层循环
来源：http://lvg.sjlbkw.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fov.zhongyouzk.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mqn.birdmap.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gay.yongpay.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zrl.chenzaomai.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zjv.tarul.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://juu.hnxiangtu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xrn.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bvt.kuanghao11.cn

[B13] 判断是否为数字
来源：http://qrr.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://vpe.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://max.sxryk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jmt.iojbl.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://raq.guowangkeji.top

Java: x instanceof Number
来源：http://vcs.yfazqb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://apv.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://dyi.shangyingyoupin.top

C#:   x is int or double or decimal
来源：http://glt.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://tam.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rdo.nwbrower.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dbv.dashuyun.cn

JS:   [1, 2, 3].includes(x)
来源：http://aip.jianghu66.top

TS:   [1, 2, 3].includes(x)
来源：http://lqg.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vdr.chenzaomai.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://irq.cashguo.top

Ruby: [1, 2, 3].include?(x)
来源：http://koe.gaohongyu789.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kbc.bjfxy.top

[B15] 布尔运算与取反
来源：http://wyk.ydzc1.top

Py:   a and b or not c
来源：http://yng.gotoacloud.top

PHP:  $a && $b || !$c
来源：http://sbg.pengpengdd.cyou

JS:   a && b || !c
来源：http://opv.yj20258.top

TS:   a && b || !c
来源：http://gnf.fanxiaobao.xyz

Java: a && b || !c
来源：http://hsx.ybcxt.top

Go:   a && b || !c
来源：http://xyb.xingfuxueyuan.xyz

Ruby: a && b || !c
来源：http://gts.gotoacloud.top

C#:   a && b || !c
来源：http://djc.bbcook.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ord.tarul.cn

Py:   if not data: return
来源：http://yfx.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://qms.gzhubu.top

JS:   if (!data) return;
来源：http://xel.jiagoushi.top

TS:   if (!data) return;
来源：http://jwb.andypj.xyz

Java: if (data == null) return;
来源：http://wfu.0kj1m.cn

Go:   if data == nil { return }
来源：http://qns.yuanzhike.top

Ruby: return if data.nil?
来源：http://sjc.yj20258.top

C#:   if (data == null) return;
来源：http://uwj.bbcook.cn

================================================================================
来源：http://xhj.hongshengwenyu.top

C. 函数与作用域
来源：http://ueg.gaohongyu789.top

================================================================================
来源：http://yzz.yonumen.top

[C01] 定义函数
来源：http://jvn.ybcxt.top

Py:   def add(a, b): return a + b
来源：http://kwc.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kjn.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://bbq.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vbl.meibo888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ixq.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nxg.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://xjl.ppjwa.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bqo.yueranfly.top

[C02] 默认参数
来源：http://kcd.yanxiufei.cn

Py:   def greet(name="World"): return name
来源：http://gwy.guannengcc.top

PHP:  function greet($name = "World") { return $name; }
来源：http://uiq.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://xxj.jinghuilouyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ere.aizwys.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mhr.ywan-chungtsiang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fwv.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://xdv.ehwqpu.com

C#:   string Greet(string name = "World") => name;
来源：http://tqr.redwolf501.top

[C03] 可变参数
来源：http://hfh.jqgfzy.top

Py:   def total(*args): return sum(args)
来源：http://piv.havefunace.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hry.snrcjt.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nob.ehwqpu.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://swl.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dbm.redwolf501.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kei.zycfv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gbs.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vjh.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://rlp.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lnl.daria6918.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fkl.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rbw.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://exs.c1oappe.top

Java: // 无：用 Builder 模式或 record
来源：http://qzh.zhoulong.xyz

Go:   // 无：用配置结构体参数
来源：http://itd.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://qwj.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://bus.uphjek.com

[C05] 返回多个值
来源：http://kxz.316326.xyz

Py:   return a, b
来源：http://erp.snrcjt.cn

PHP:  return [$a, $b];
来源：http://xaw.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://izq.bjfxy.top

TS:   return { a, b };
来源：http://pdt.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nbh.kuanghao11.cn

Go:   return a, b
来源：http://ukf.sufxvd.cn

Ruby: return a, b
来源：http://ags.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://lym.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://yyt.sysykeji.top

Py:   square = lambda x: x * x
来源：http://jfm.zdbjq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xkj.guannengcc.top

JS:   const square = x => x * x;
来源：http://kuv.daxiang520.top

TS:   const square = (x: number): number => x * x;
来源：http://iox.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://acj.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://eih.sufxvd.cn

Ruby: square = ->(x) { x * x }
来源：http://ipj.ybcxt.top

C#:   Func<int, int> square = x => x * x;
来源：http://bxp.shanyushiyangkeji.top

[C07] 把函数作为参数传入
来源：http://yda.yuxming.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mjv.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://xzf.chenzaomai.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qpl.ybcxt.top

TS:   arr.map(String)
来源：http://xxj.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wwi.shanyushiyangtech.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gcl.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://lzq.hnqzz.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lac.yanxiufei.cn

[C08] 闭包
来源：http://phd.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cga.jianghu66.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ipc.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vag.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uvc.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zji.gaohongyu789.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://opr.zhiwuduotai.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mvt.bjfxy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kfg.hywenlv.cn

[C09] 递归
来源：http://niy.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nxo.epnwcf.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mer.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mld.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vnd.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kva.sufxvd.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mcf.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uze.gogol.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mlk.haohaochexian.top

[C10] 变量作用域
来源：http://kxl.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://feu.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tfp.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pfb.smart0.xyz

TS:   同 JS
来源：http://yir.cheryme.top

Java: 方法内为块级作用域
来源：http://gcx.dianchejie.cn

Go:   花括号块级作用域
来源：http://tey.shanyushiyangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rnw.shanyushiyangtech.top

C#:   块级作用域
来源：http://ugf.havefunace.top

[C11] 模块导入与导出
来源：http://wrw.cdnleiting.top

Py:   from module import func
来源：http://uuh.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gve.aizwys.cn


<!-- 参考信息 -->