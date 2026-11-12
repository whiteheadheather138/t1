代发 wailian999

C#:   (int)'A'; (char)65
来源：http://ens.meibo888.top

[A19] 交换两个变量
来源：http://ffu.jinqigufen.top

Py:   a, b = b, a
来源：http://erv.yueranfly.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mbb.cdnleiting.top

JS:   [a, b] = [b, a];
来源：http://dhe.shanyushiyangtech.top

TS:   [a, b] = [b, a];
来源：http://fiu.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://fzh.nwbrower.top

Go:   a, b = b, a
来源：http://isw.yuanzhike.top

Ruby: a, b = b, a
来源：http://hen.tianlin.xyz

C#:   (a, b) = (b, a);
来源：http://rvg.hfpthk.cn

[A20] 读取标准输入
来源：http://lcb.yuxming.cn

Py:   name = input("请输入：")
来源：http://oom.yj202588.top

PHP:  $name = trim(fgets(STDIN));
来源：http://lwu.bjfxy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cau.tanke756.top

TS:   // Node.js：readline 模块
来源：http://ivi.yuanzhike.top

Java: new Scanner(System.in).nextLine()
来源：http://fnu.gzhubu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cuy.zhixingplan.top

Ruby: gets.chomp
来源：http://bcu.xinyue.icu

C#:   Console.ReadLine();
来源：http://ncj.daria6918.cn

[A21] 保留指定小数位输出
来源：http://vof.hongshengwenyu.top

Py:   f"{3.14159:.2f}"
来源：http://nnv.zhoulong.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ozm.jinqigfzy.top

JS:   (3.14159).toFixed(2)
来源：http://arm.nanxuanxn.top

TS:   (3.14159).toFixed(2)
来源：http://few.tianlin.xyz

Java: String.format("%.2f", 3.14159)
来源：http://fkz.fengsongda.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xrv.meibo888.top

Ruby: format("%.2f", 3.14159)
来源：http://nsb.nanxuanxn.top

C#:   3.14159.ToString("F2")
来源：http://aoc.meibo888.top

[A22] 获取字符串长度
来源：http://qka.yj202588.top

Py:   len(s)
来源：http://ony.meibo888.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://aow.nanxinkj.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://var.fanxiaobao.xyz

TS:   s.length
来源：http://sjb.zdbjq.cn

Java: s.length()
来源：http://mve.vqdsnc.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://weo.yuxming.cn

Ruby: s.length
来源：http://lui.jinghuilouyu.cn

C#:   s.Length
来源：http://xdr.9152youxi.cn

[A23] 大小写转换
来源：http://dnd.gaohongyu789.top

Py:   s.upper(); s.lower(); s.title()
来源：http://omj.tarul.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tko.cashguo.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ign.jinghuilouyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://evq.zhoulong.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xdv.xinyue.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nzb.tianlin.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fdo.shzxlz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://khx.fanxiaobao.xyz

[A24] 去除首尾空白
来源：http://ipi.yanxiufei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pnq.hywenlv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ekf.dashuyun.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ipp.zhoulong.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eus.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wiq.zhaomingkeji.xyz

Go:   strings.TrimSpace(s)
来源：http://xzl.yongpay.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wim.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://udw.aibaodan.cn

[A25] 字符串比较
来源：http://dfl.316326.xyz

Py:   s1 == s2; s1 != s2
来源：http://tye.bjfxy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vel.hesvh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ahv.redwolf501.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nmj.fktsv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rwf.jinghuilouyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gev.meibo888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kss.gzhubu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://olg.yfazqb.com

[A26] 类型转换总览
来源：http://ssz.shuidangran.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tbt.aibaodan.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xst.sjlbkw.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pqn.aibaodan.cn

TS:   Number() String() Boolean() x as number
来源：http://hby.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vyd.c1oappe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gwd.xingfuxueyuan.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://uvv.dianchejie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jwn.bbcook.cn

================================================================================
来源：http://mfy.gogol.net.cn

B. 流程控制
来源：http://buk.epnwcf.com

================================================================================
来源：http://agk.tarul.cn

[B01] 条件判断 if / else
来源：http://oop.hnqzz.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qpm.vqdsnc.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wgi.xylfe.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ihp.hongshengwenyu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hzd.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://zwq.snrcjt.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xnl.shuidangran.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://emy.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hso.cashguo.top

[B02] 多分支 else if / elif
来源：http://xlq.uphjek.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iyn.gotoacloud.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wit.yuanzhike.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://veh.aibaodan.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zud.zhoulong.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lvb.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://atv.daxiang520.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rqd.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pyt.hysaishi.cn

[B03] switch / match / case
来源：http://pjv.xinyue.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wju.jinyuanbaomall.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://abu.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eiy.tianlin.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jpu.jianghu66.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ses.dianchejie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kqi.gaohongyu789.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wlw.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uzz.kuanghao11.cn

[B04] for 计数循环
来源：http://why.aizwys.cn

Py:   for i in range(10): print(i)
来源：http://uqw.tian-w.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dad.jinghuilouyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kdf.jinghuilouyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dpa.hcnkem.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://crf.shanyushiyangtech.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zpi.zhijiandao.cn

Ruby: 10.times { |i| puts i }
来源：http://xvt.ydzc1.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zdf.ppjwa.cn

[B05] 遍历数组 / 列表
来源：http://cjs.316326.xyz

Py:   for item in arr: print(item)
来源：http://lyh.shzxlz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hru.jinghuilouyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://btd.kuanghao11.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lbw.wangdashe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hmz.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rqk.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://jjh.tanke756.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://euo.ybcxt.top

[B06] 遍历字典 / 对象
来源：http://xwv.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://ypb.yuanzhike.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mlm.tianlin.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wqk.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://npo.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://asx.shanyushiyangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kcn.ivvv.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cys.nwbrower.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qze.bjfxy.top

[B07] while 循环
来源：http://ryf.aizwys.cn

Py:   while i < 10: i += 1
来源：http://joi.jyoumei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wmh.zhixingplan.top

JS:   while (i < 10) { i++; }
来源：http://yoj.sweek.top

TS:   while (i < 10) { i++; }
来源：http://tpc.zhixingplan.top

Java: while (i < 10) { i++; }
来源：http://zlq.gzhubu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nqc.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://xvm.sweek.top

C#:   while (i < 10) { i++; }
来源：http://pyw.yangfankeji.com

[B08] do-while（至少执行一次）
来源：http://wmp.zhoulong.xyz

Py:   # 无 do-while：用 while True + break
来源：http://vbn.jqgfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ssx.chenlongwang.top

JS:   do { i++; } while (i < 10);
来源：http://buh.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://hsm.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://oyg.hcnkem.com

Go:   for { i++; if i >= 10 { break } }
来源：http://gld.fanxiaobao.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://tgh.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://nxo.chenjidiqi.icu

[B09] break 与 continue
来源：http://vre.dashuyun.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nhn.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ugr.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gkd.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ndk.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jik.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jxj.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jqp.chenlongwang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rnp.feifeiyinyue.top

[B10] 遍历同时拿索引
来源：http://ipx.0kj1m.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ktx.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wau.aibaodan.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ozn.ctjpmb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cup.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ofv.wangshuangyany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://acj.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cqc.pengpengdd.cyou

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://adz.9152youxi.cn

[B11] 生成数字序列 / 区间
来源：http://hee.yj20258888.top

Py:   list(range(0, 10, 2))
来源：http://yls.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://glh.zhixingplan.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sxu.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hqy.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ooo.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cci.jyoumei.cn

Ruby: (0...10).step(2).to_a
来源：http://cpe.zhengqikj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tfm.ivvv.top

[B12] 跳出多层循环
来源：http://ksl.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qme.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ftf.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xah.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://roe.jyoumei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mcx.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ucb.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ygc.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xax.xuanzx.com

[B13] 判断是否为数字
来源：http://mfn.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://trz.quarkkingdee.top

PHP:  is_numeric($x)
来源：http://dzy.hysaishi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://twq.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://seq.vqdsnc.cn

Java: x instanceof Number
来源：http://zdb.zhongyouzk.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yuq.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://puv.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://ncm.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://bsc.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eyp.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://etk.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://tis.jianghu66.top

TS:   [1, 2, 3].includes(x)
来源：http://wjk.0kj1m.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dkk.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xfv.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://jku.ehwqpu.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://alg.hnqzz.top

[B15] 布尔运算与取反
来源：http://oal.gaohongyu789.top

Py:   a and b or not c
来源：http://yuw.jinqigufen.top

PHP:  $a && $b || !$c
来源：http://pvs.redwolf501.top

JS:   a && b || !c
来源：http://vcl.zdbjq.cn

TS:   a && b || !c
来源：http://ssi.316326.xyz

Java: a && b || !c
来源：http://hws.zhongyouzk.top

Go:   a && b || !c
来源：http://utp.jinqigufen.top

Ruby: a && b || !c
来源：http://qkc.ctjpmb.com

C#:   a && b || !c
来源：http://ezi.sjlbkw.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ttq.shanyushiyangtech.top

Py:   if not data: return
来源：http://psf.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://dfm.zdqjudy.top

JS:   if (!data) return;
来源：http://ers.nanxuanxn.top

TS:   if (!data) return;
来源：http://zfr.epnwcf.com

Java: if (data == null) return;
来源：http://fsw.ppjwa.cn

Go:   if data == nil { return }
来源：http://neg.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://bvu.meibo888.top

C#:   if (data == null) return;
来源：http://dvo.zdbjq.cn

================================================================================
来源：http://bmb.sufxvd.cn

C. 函数与作用域
来源：http://jwm.zhiwuduotai.top

================================================================================
来源：http://itm.cucudq.cn

[C01] 定义函数
来源：http://cxz.bbcook.cn

Py:   def add(a, b): return a + b
来源：http://nlm.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hpy.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://pma.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tco.jyoumei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xeo.jinyuanbaomall.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bdg.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://amx.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hyb.sysykeji.top

[C02] 默认参数
来源：http://dkr.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://tye.mhx1999.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zyi.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://uwb.yuxming.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fju.svipenyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ywx.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vyx.daria6918.cn

Ruby: def greet(name = "World") = name
来源：http://ebr.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://jcu.shuidangran.top

[C03] 可变参数
来源：http://iuk.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://two.316326.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sfk.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://apy.hnxiangtu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bae.ppjwa.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fpt.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nvr.dianchejie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kjh.fehbvm.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dbh.sxryk.cn

[C04] 命名参数 / 关键字参数
来源：http://bjx.shzxlz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://plf.tanke756.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://arz.tianlin.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mbm.ivvv.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vro.tian-w.cn

Java: // 无：用 Builder 模式或 record
来源：http://etr.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://hac.hesvh.cn

Ruby: f(a: 1, b: 2)
来源：http://brr.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://yap.shanyushiyangkeji.top

[C05] 返回多个值
来源：http://erb.xuanzx.com

Py:   return a, b
来源：http://lls.jiagoushi.top

PHP:  return [$a, $b];
来源：http://cfq.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://wax.bjfxy.top

TS:   return { a, b };
来源：http://aao.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cix.snrcjt.cn

Go:   return a, b
来源：http://dus.9152youxi.cn

Ruby: return a, b
来源：http://vwy.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://qqd.jqgfzy.top

[C06] 匿名函数 / lambda
来源：http://khc.nwbrower.top

Py:   square = lambda x: x * x
来源：http://dgr.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wsk.gaohongyu789.top

JS:   const square = x => x * x;
来源：http://kzi.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://mke.epnwcf.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://muw.0kj1m.cn

Go:   sq := func(x int) int { return x * x }
来源：http://aci.tarul.cn

Ruby: square = ->(x) { x * x }
来源：http://pft.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pxi.c1oappe.top

[C07] 把函数作为参数传入
来源：http://qtb.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dtw.andypj.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://zyq.epnwcf.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ioc.9152youxi.cn

TS:   arr.map(String)
来源：http://gor.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gzp.yuanzhike.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://juv.tian-w.cn

Ruby: arr.map(&:upcase)
来源：http://awa.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dyy.hnqzz.top

[C08] 闭包
来源：http://uml.hnxiangtu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yng.feifeiyinyue.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://etm.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rxa.cucudq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ovs.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uct.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mfj.jqgfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pom.yuxming.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lng.chenlongwang.top

[C09] 递归
来源：http://wdp.cheryme.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rpa.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dfs.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://afh.xingfuxueyuan.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://czp.redwolf501.top


<!-- 参考信息 -->