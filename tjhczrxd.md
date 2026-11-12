代发 wailian999

Ruby: a, b = b, a
来源：http://mpk.cqqwz.cn

C#:   (a, b) = (b, a);
来源：http://raf.52xcode.cn

[A20] 读取标准输入
来源：http://god.yfazqb.com

Py:   name = input("请输入：")
来源：http://ycz.meibo888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ora.vehdjk.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iai.jinghuilouyu.cn

TS:   // Node.js：readline 模块
来源：http://bxh.316326.xyz

Java: new Scanner(System.in).nextLine()
来源：http://hjy.jyoumei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ugz.hfpthk.cn

Ruby: gets.chomp
来源：http://uhd.wangdashe.top

C#:   Console.ReadLine();
来源：http://qwf.chenzaomai.com

[A21] 保留指定小数位输出
来源：http://rec.pengpengdd.cyou

Py:   f"{3.14159:.2f}"
来源：http://trw.nwbrower.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qwc.yj20258.top

JS:   (3.14159).toFixed(2)
来源：http://zkg.bbcook.cn

TS:   (3.14159).toFixed(2)
来源：http://gbv.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://lhz.zhoulong.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zmg.yuanzhike.top

Ruby: format("%.2f", 3.14159)
来源：http://jdd.jiagoushi.top

C#:   3.14159.ToString("F2")
来源：http://mrs.chenzaomai.com

[A22] 获取字符串长度
来源：http://uyv.guannengcc.top

Py:   len(s)
来源：http://iax.jqgfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gfn.gaohongyu789.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ruf.yangfankeji.com

TS:   s.length
来源：http://eat.zhiwuduotai.top

Java: s.length()
来源：http://oox.zhongyouzk.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dqa.shangyingyoupin.top

Ruby: s.length
来源：http://qde.tarul.cn

C#:   s.Length
来源：http://pjs.pengpengdd.cyou

[A23] 大小写转换
来源：http://chs.uphjek.com

Py:   s.upper(); s.lower(); s.title()
来源：http://wxv.zhongyouzk.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nwq.hcnkem.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vcg.haohaochexian.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vpj.ehwqpu.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gkn.nanxuanxn.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gst.shuidangran.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vvh.c1oappe.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ngx.zhijiandao.cn

[A24] 去除首尾空白
来源：http://hhq.fzhhl.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ded.xylfe.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kch.sufxvd.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lqj.dianchejie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nwn.vqdsnc.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ush.zhijiandao.cn

Go:   strings.TrimSpace(s)
来源：http://xpq.xuetiantiany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cfy.gogol.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sfs.yj20258.top

[A25] 字符串比较
来源：http://knl.zhongyouzk.top

Py:   s1 == s2; s1 != s2
来源：http://qga.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ojh.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ssb.yvedp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://erv.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jve.daxiang520.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uze.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tzv.shangyingyoupin.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gkd.ehwqpu.com

[A26] 类型转换总览
来源：http://ksv.yanxiufei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mlr.svipenyu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://onr.hongshengwenyu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iko.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://vhp.jiagoushi.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yjq.svipenyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pen.guowangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://oqd.shzxlz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://njk.52xcode.cn

================================================================================
来源：http://pkc.zhiwuduotai.top

B. 流程控制
来源：http://lwd.yj20258.top

================================================================================
来源：http://jnu.shanyushiyangtech.top

[B01] 条件判断 if / else
来源：http://ayb.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wno.mhx1999.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jbs.zdbjq.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wqd.yongpay.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mna.hcnkem.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://tlu.jqgfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://urb.xuetiantiany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cpv.pengpengdd.cyou

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hbi.shuidangran.top

[B02] 多分支 else if / elif
来源：http://ikk.chenjidiqi.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kun.ctjpmb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qfp.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ygb.fanxiaobao.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jen.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ivo.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rgu.tianlin.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nqb.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vnx.zycfv.cn

[B03] switch / match / case
来源：http://bdt.zhixingplan.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ryk.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eyg.vehdjk.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rlo.yj20258.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://teo.c1oappe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fey.zycfv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gyg.tian-w.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bjw.hysaishi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://skv.tianlin.xyz

[B04] for 计数循环
来源：http://iki.fengsongda.top

Py:   for i in range(10): print(i)
来源：http://bla.jinghuilouyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zxc.c1oappe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ley.cdnleiting.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hmg.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mzp.bbcook.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fyo.hfpthk.cn

Ruby: 10.times { |i| puts i }
来源：http://lqo.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bni.shanyushiyangtech.top

[B05] 遍历数组 / 列表
来源：http://kgd.jyoumei.cn

Py:   for item in arr: print(item)
来源：http://mnf.zhongyouzk.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aqu.52xcode.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ghd.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kbk.gzhubu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kpm.gotoacloud.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zsu.zhixingplan.top

Ruby: arr.each { |item| puts item }
来源：http://xhk.hnqzz.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uja.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://tmj.xylfe.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://udi.pengpengdd.cyou

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qwv.aibaodan.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hsy.feifeiyinyue.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sxs.guowangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://atx.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://arb.tian-w.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nph.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kxe.kuanghao11.cn

[B07] while 循环
来源：http://xtb.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://tik.yj202588.top

PHP:  while ($i < 10) { $i++; }
来源：http://efj.quarkkingdee.top

JS:   while (i < 10) { i++; }
来源：http://nto.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://aax.tanke756.top

Java: while (i < 10) { i++; }
来源：http://umh.gzhubu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kxm.9152youxi.cn

Ruby: while i < 10; i += 1; end
来源：http://qcj.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://yrt.nwbrower.top

[B08] do-while（至少执行一次）
来源：http://whx.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://iio.jinqigufen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://oox.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://awl.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://nzy.zdqjudy.top

Java: do { i++; } while (i < 10);
来源：http://zrq.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://nri.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://lzp.zdqjudy.top

C#:   do { i++; } while (i < 10);
来源：http://avg.quarkkingdee.top

[B09] break 与 continue
来源：http://ocd.jqgfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ceh.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wcx.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qqj.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nhe.yueranfly.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xge.yonumen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mwy.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wal.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iir.yj202588.top

[B10] 遍历同时拿索引
来源：http://hfg.yonumen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qgm.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zmi.ehwqpu.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hqv.xuetiantiany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cox.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ooi.yvedp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ubp.cheryme.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://spa.shanyushiyangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ucw.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://ulm.zhaomingkeji.xyz

Py:   list(range(0, 10, 2))
来源：http://kqv.snrcjt.cn

PHP:  range(0, 10, 2);
来源：http://rxk.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qvd.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sxs.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://niv.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://olt.xuanzx.com

Ruby: (0...10).step(2).to_a
来源：http://wss.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rtp.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://bnz.zhiwuduotai.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hoe.zdbjq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mnt.yj20258.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iqo.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ugd.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vcm.aizwys.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gtw.fengsongda.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lds.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://txx.iojbl.cn

[B13] 判断是否为数字
来源：http://obb.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://sae.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://zgp.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xqs.redwolf501.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rlb.wangshuangyany.cn

Java: x instanceof Number
来源：http://vau.ydzc1.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ojf.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://nbx.xziqi.cn

C#:   x is int or double or decimal
来源：http://iki.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://pyn.jqgufenzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pjl.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://udy.ppjwa.cn

JS:   [1, 2, 3].includes(x)
来源：http://msu.dashuyun.cn

TS:   [1, 2, 3].includes(x)
来源：http://hej.zhijiandao.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zwj.sweek.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sub.feifeiyinyue.top

Ruby: [1, 2, 3].include?(x)
来源：http://vrp.ivvv.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ajy.svipenyu.cn

[B15] 布尔运算与取反
来源：http://hpk.zdqjudy.top

Py:   a and b or not c
来源：http://smx.daxiang520.top

PHP:  $a && $b || !$c
来源：http://bqt.pengpengdd.cyou

JS:   a && b || !c
来源：http://wqj.ydjk.org.cn

TS:   a && b || !c
来源：http://vro.bjfxy.top

Java: a && b || !c
来源：http://pdz.yuxming.cn

Go:   a && b || !c
来源：http://hii.zdbjq.cn

Ruby: a && b || !c
来源：http://iep.havefunace.top

C#:   a && b || !c
来源：http://edg.zhengqikj.top

[B16] 卫语句：不满足条件提前返回
来源：http://iow.jiagoushi.top

Py:   if not data: return
来源：http://cef.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://msr.epnwcf.com

JS:   if (!data) return;
来源：http://xzw.yj20258.top

TS:   if (!data) return;
来源：http://ior.fktsv.cn

Java: if (data == null) return;
来源：http://nat.nanxuanxn.top

Go:   if data == nil { return }
来源：http://mmu.ywan-chungtsiang.top

Ruby: return if data.nil?
来源：http://rkb.yueranfly.top

C#:   if (data == null) return;
来源：http://ssu.svipenyu.cn

================================================================================
来源：http://sxs.xuetiantiany.cn

C. 函数与作用域
来源：http://bol.cdnleiting.top

================================================================================
来源：http://ved.tianlin.xyz

[C01] 定义函数
来源：http://auj.tanke756.top

Py:   def add(a, b): return a + b
来源：http://hrp.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://twj.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://zlp.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sio.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ggi.ctjpmb.com

Go:   func add(a, b int) int { return a + b }
来源：http://ylj.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://zch.0kj1m.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vpr.zhixingplan.top

[C02] 默认参数
来源：http://lsc.haohaochexian.top

Py:   def greet(name="World"): return name
来源：http://vwg.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ebd.redwolf501.top

JS:   function greet(name = "World") { return name; }
来源：http://oaq.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://svx.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qcj.yfazqb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://axl.dianchejie.cn

Ruby: def greet(name = "World") = name
来源：http://glz.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://zni.fanxiaobao.xyz

[C03] 可变参数
来源：http://fov.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://uih.jinyuanbaomall.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uvh.hongshengwenyu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gof.shangyingyoupin.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gjw.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gjq.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fii.dianchejie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ezw.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zsz.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://hnw.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://var.havefunace.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gqs.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qfm.bbcook.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ixa.zycfv.cn

Java: // 无：用 Builder 模式或 record
来源：http://ibx.sxryk.cn

Go:   // 无：用配置结构体参数
来源：http://xos.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://xwb.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://qul.feifeiyinyue.top

[C05] 返回多个值
来源：http://unn.jinqigfzy.top

Py:   return a, b
来源：http://edo.yongpay.top

PHP:  return [$a, $b];
来源：http://vps.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://lxu.redwolf501.top

TS:   return { a, b };
来源：http://bdh.cdnleiting.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mof.guannengcc.top

Go:   return a, b
来源：http://yru.xuanzx.com

Ruby: return a, b
来源：http://unr.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://qdu.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://xvu.gogol.net.cn

Py:   square = lambda x: x * x
来源：http://bcn.ybcxt.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ixo.shuidangran.top

JS:   const square = x => x * x;
来源：http://lzp.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://hyh.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://scq.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://lub.smart0.xyz

Ruby: square = ->(x) { x * x }
来源：http://fpe.chenzaomai.com

C#:   Func<int, int> square = x => x * x;
来源：http://ari.ppjwa.cn

[C07] 把函数作为参数传入
来源：http://rhg.snrcjt.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ckd.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://pux.zhaomingkeji.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://egw.sxryk.cn

TS:   arr.map(String)
来源：http://fud.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dwg.yueranfly.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qzj.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://kon.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ura.xylfe.cn

[C08] 闭包
来源：http://xte.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dcx.jinqigufen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fgl.smart0.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fjq.fktsv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vqh.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eeo.zycfv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dev.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tsv.xuanzx.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vxy.yongpay.top

[C09] 递归
来源：http://rnl.hesvh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pgk.zhixingplan.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vmk.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bye.wangdashe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ctk.yueranfly.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jlp.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dkb.ehwqpu.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dms.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jvf.sxryk.cn

[C10] 变量作用域
来源：http://dzk.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dsy.cucudq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oku.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tyo.jinqigufen.top


<!-- 参考信息 -->