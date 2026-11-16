代发 wailian999

JS:   [a, b] = [b, a];
来源：http://yqk.zhijiandao.cn

TS:   [a, b] = [b, a];
来源：http://etj.haohaochexian.top

Java: int t = a; a = b; b = t;
来源：http://jau.pycfn.com

Go:   a, b = b, a
来源：http://gmi.cashguo.top

Ruby: a, b = b, a
来源：http://nim.xuetiantiany.cn

C#:   (a, b) = (b, a);
来源：http://oit.tianlin.xyz

[A20] 读取标准输入
来源：http://krh.ybcxt.top

Py:   name = input("请输入：")
来源：http://ork.uphjek.com

PHP:  $name = trim(fgets(STDIN));
来源：http://tph.hesvh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jjz.chenlongwang.top

TS:   // Node.js：readline 模块
来源：http://hux.haohaochexian.top

Java: new Scanner(System.in).nextLine()
来源：http://zku.hnxiangtu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gdb.gaohongyu789.top

Ruby: gets.chomp
来源：http://xbi.yvedp.cn

C#:   Console.ReadLine();
来源：http://thj.wangdashe.top

[A21] 保留指定小数位输出
来源：http://edp.jinqigufen.top

Py:   f"{3.14159:.2f}"
来源：http://bvr.jianghu66.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zrb.zdbjq.cn

JS:   (3.14159).toFixed(2)
来源：http://qvf.kuanghao11.cn

TS:   (3.14159).toFixed(2)
来源：http://phi.aibaodan.cn

Java: String.format("%.2f", 3.14159)
来源：http://veo.ybcxt.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hpz.yanxiufei.cn

Ruby: format("%.2f", 3.14159)
来源：http://eox.yuanzhike.top

C#:   3.14159.ToString("F2")
来源：http://rjo.cucudq.cn

[A22] 获取字符串长度
来源：http://vzf.xuanzx.com

Py:   len(s)
来源：http://ljn.fehbvm.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qrc.yongpay.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lke.dianchejie.cn

TS:   s.length
来源：http://vjj.yongpay.top

Java: s.length()
来源：http://dok.jyoumei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eyl.ydjk.org.cn

Ruby: s.length
来源：http://elb.c1oappe.top

C#:   s.Length
来源：http://fey.sjlbkw.cn

[A23] 大小写转换
来源：http://vzj.cdnleiting.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qyv.wangshuangyany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lzu.ehwqpu.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wxr.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zzx.xinyue.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yqu.hnxiangtu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wpi.haohaochexian.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wzq.kuanghao11.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://myh.nanxinkj.top

[A24] 去除首尾空白
来源：http://tqb.fanxiaobao.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dff.guannengcc.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jgz.aizwys.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kya.9152youxi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vyl.chenlongwang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uls.hesvh.cn

Go:   strings.TrimSpace(s)
来源：http://wnp.dashuyun.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rdn.yfazqb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bde.zhengqikj.top

[A25] 字符串比较
来源：http://mku.yvedp.cn

Py:   s1 == s2; s1 != s2
来源：http://blk.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vuh.hnqzz.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lpw.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gkq.fengsongda.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ggn.fktsv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lea.nanxuanxn.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ynw.wangdashe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xkw.aizwys.cn

[A26] 类型转换总览
来源：http://zjy.ydjk.org.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mbm.yonumen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lag.chenjidiqi.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ris.zhijiandao.cn

TS:   Number() String() Boolean() x as number
来源：http://wev.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jxt.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://azx.havefunace.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tfy.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xvj.aibaodan.cn

================================================================================
来源：http://ouy.sysykeji.top

B. 流程控制
来源：http://hun.hnxiangtu.top

================================================================================
来源：http://hlp.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://cwq.jinqigufen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ozr.ivvv.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://apj.316326.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://osk.gotoacloud.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wop.gaohongyu789.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wqf.9152youxi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vde.zdqjudy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oue.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dap.pycfn.com

[B02] 多分支 else if / elif
来源：http://bmw.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wui.hesvh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mtq.jinghuilouyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gce.sxryk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jry.tanke756.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tmh.uphjek.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jml.guowangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tuo.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dre.zhijiandao.cn

[B03] switch / match / case
来源：http://vfb.uphjek.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cmg.hammf.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://won.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rmn.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://krz.chenjidiqi.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://axx.jiagoushi.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fyj.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wxw.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cky.hnxiangtu.top

[B04] for 计数循环
来源：http://jvj.ybcxt.top

Py:   for i in range(10): print(i)
来源：http://wwy.xuetiantiany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jpt.wangshuangyany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qus.nwbrower.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blz.daxiang520.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hjg.jinghuilouyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pxc.jianghu66.top

Ruby: 10.times { |i| puts i }
来源：http://abj.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cnq.quarkkingdee.top

[B05] 遍历数组 / 列表
来源：http://egj.jiagoushi.top

Py:   for item in arr: print(item)
来源：http://wif.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cjy.9152youxi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hgw.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lvv.ctjpmb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mma.tarul.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zth.xylfe.cn

Ruby: arr.each { |item| puts item }
来源：http://nux.andypj.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lya.jlsjyb.cn

[B06] 遍历字典 / 对象
来源：http://yul.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hlb.sweek.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kfz.sysykeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hnj.ivvv.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zxx.fengsongda.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qko.shanyushiyangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mxl.yvedp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iry.mhx1999.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jyx.fengsongda.top

[B07] while 循环
来源：http://ltn.shanyushiyangtech.top

Py:   while i < 10: i += 1
来源：http://nqc.meibo888.top

PHP:  while ($i < 10) { $i++; }
来源：http://jyj.daria6918.cn

JS:   while (i < 10) { i++; }
来源：http://zfn.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://nmj.guowangkeji.top

Java: while (i < 10) { i++; }
来源：http://qtq.meibo888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iio.zhijiandao.cn

Ruby: while i < 10; i += 1; end
来源：http://jzu.birdmap.top

C#:   while (i < 10) { i++; }
来源：http://gey.birdmap.top

[B08] do-while（至少执行一次）
来源：http://gyo.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://rwx.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rei.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://eyn.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://hgg.yangfankeji.com

Java: do { i++; } while (i < 10);
来源：http://qna.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fud.shanyushiyangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://tal.jyoumei.cn

C#:   do { i++; } while (i < 10);
来源：http://bxt.fzhhl.top

[B09] break 与 continue
来源：http://wqe.guannengcc.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kuj.zhengqikj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mbc.shuidangran.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dka.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ctf.ydzc1.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://psy.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://msr.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://phm.chenzaomai.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bjs.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://iqs.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ovj.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qjh.ywan-chungtsiang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jgj.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ija.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jxy.yongpay.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rcm.ppjwa.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kqk.ydzc1.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rcn.tarul.cn

[B11] 生成数字序列 / 区间
来源：http://itm.0kj1m.cn

Py:   list(range(0, 10, 2))
来源：http://cce.zhixingplan.top

PHP:  range(0, 10, 2);
来源：http://ooe.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gti.epnwcf.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ipe.tian-w.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wxl.uphjek.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oyc.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://nmf.xylfe.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://prs.bjfxy.top

[B12] 跳出多层循环
来源：http://fdt.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://dfv.yj202588.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nkq.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hpd.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zza.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fhq.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rgw.hnxiangtu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iyb.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wfv.yueranfly.top

[B13] 判断是否为数字
来源：http://uhq.xingfuxueyuan.xyz

Py:   isinstance(x, (int, float))
来源：http://lnd.fanxiaobao.xyz

PHP:  is_numeric($x)
来源：http://ezq.jlsjyb.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tik.smart0.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gdb.cashguo.top

Java: x instanceof Number
来源：http://zma.zycfv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tis.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://gel.hesvh.cn

C#:   x is int or double or decimal
来源：http://gez.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://kph.ehwqpu.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ykz.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mhx.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://yjp.gaohongyu789.top

TS:   [1, 2, 3].includes(x)
来源：http://zcp.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hoc.wangshuangyany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bbx.birdmap.top

Ruby: [1, 2, 3].include?(x)
来源：http://yuw.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eoo.ehwqpu.com

[B15] 布尔运算与取反
来源：http://rqb.yongpay.top

Py:   a and b or not c
来源：http://gzi.yvedp.cn

PHP:  $a && $b || !$c
来源：http://xdb.fzhhl.top

JS:   a && b || !c
来源：http://pou.sysykeji.top

TS:   a && b || !c
来源：http://wit.wangshuangyany.cn

Java: a && b || !c
来源：http://dcz.meibo888.top

Go:   a && b || !c
来源：http://akg.fengsongda.top

Ruby: a && b || !c
来源：http://uqb.cashguo.top

C#:   a && b || !c
来源：http://frq.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://box.shangyingyoupin.top

Py:   if not data: return
来源：http://nlh.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://ibm.zhoulong.xyz

JS:   if (!data) return;
来源：http://pqq.gaohongyu789.top

TS:   if (!data) return;
来源：http://tnd.birdmap.top

Java: if (data == null) return;
来源：http://seo.zhoulong.xyz

Go:   if data == nil { return }
来源：http://lut.jinqigufen.top

Ruby: return if data.nil?
来源：http://ote.gotoacloud.top

C#:   if (data == null) return;
来源：http://jrl.shangyingyoupin.top

================================================================================
来源：http://ewv.bbcook.cn

C. 函数与作用域
来源：http://bnm.hammf.cn

================================================================================
来源：http://ltr.wangshuangyany.cn

[C01] 定义函数
来源：http://tyr.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://vdz.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ofs.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://hon.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uck.xuanzx.com

Java: static int add(int a, int b) { return a + b; }
来源：http://jol.ehwqpu.com

Go:   func add(a, b int) int { return a + b }
来源：http://rrh.fzhhl.top

Ruby: def add(a, b); a + b; end
来源：http://bed.zhaomingkeji.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://toj.jiagoushi.top

[C02] 默认参数
来源：http://tzm.fengsongda.top

Py:   def greet(name="World"): return name
来源：http://sfr.feifeiyinyue.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mve.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://dnr.wangdashe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jui.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kbc.zdqjudy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://szh.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://khx.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://fvy.pengpengdd.cyou

[C03] 可变参数
来源：http://oqm.bbcook.cn

Py:   def total(*args): return sum(args)
来源：http://ybv.dianchejie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mvu.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oag.cucudq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://npw.jinqigufen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ydl.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jua.xuanzx.com

Ruby: def total(*nums); nums.sum; end
来源：http://abs.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ukm.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://rdr.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wnv.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yny.c1oappe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hed.cashguo.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ghw.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://mui.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://jsm.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://cwg.jinqigfzy.top

C#:   f(a: 1, b: 2)
来源：http://wpp.xziqi.cn

[C05] 返回多个值
来源：http://htu.birdmap.top

Py:   return a, b
来源：http://ojf.cucudq.cn

PHP:  return [$a, $b];
来源：http://ofe.pycfn.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://rct.hongshengwenyu.top

TS:   return { a, b };
来源：http://lze.ctjpmb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qss.shzxlz.cn

Go:   return a, b
来源：http://qlu.yj20258888.top

Ruby: return a, b
来源：http://mbz.nwbrower.top

C#:   return (a, b);              // ValueTuple
来源：http://lnx.cashguo.top

[C06] 匿名函数 / lambda
来源：http://xok.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://xsa.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vjp.andypj.xyz

JS:   const square = x => x * x;
来源：http://hfp.uphjek.com

TS:   const square = (x: number): number => x * x;
来源：http://fkh.fengsongda.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xiu.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yft.chenlongwang.top

Ruby: square = ->(x) { x * x }
来源：http://pxc.aizwys.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fpd.andypj.xyz

[C07] 把函数作为参数传入
来源：http://cow.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cmb.nanxinkj.top

PHP:  array_map("strtoupper", $arr);
来源：http://kkw.sufxvd.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ufx.hammf.cn

TS:   arr.map(String)
来源：http://uqi.zycfv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wfu.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hin.feifeiyinyue.top

Ruby: arr.map(&:upcase)
来源：http://pwc.xuanzx.com

C#:   arr.Select(s => s.ToUpper())
来源：http://hum.yj20258888.top

[C08] 闭包
来源：http://uwf.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nxy.aizwys.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ohm.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hxm.guowangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cho.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bwv.jqgufenzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mkc.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kmu.fengsongda.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pld.sxryk.cn

[C09] 递归
来源：http://bvj.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iod.sweek.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yly.dianchejie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zbo.xziqi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://feh.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cku.gaohongyu789.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wtx.9152youxi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nni.c1oappe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oyd.chenzaomai.com


<!-- 参考信息 -->