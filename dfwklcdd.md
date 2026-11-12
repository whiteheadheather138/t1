代发 wailian999

[A22] 获取字符串长度
来源：http://dic.fengsongda.top

Py:   len(s)
来源：http://mak.ivvv.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ulg.cdnleiting.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://piw.jinqigufen.top

TS:   s.length
来源：http://mge.xuanzx.com

Java: s.length()
来源：http://zty.jyoumei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://czw.svipenyu.cn

Ruby: s.length
来源：http://iss.sufxvd.cn

C#:   s.Length
来源：http://ekt.yonumen.top

[A23] 大小写转换
来源：http://qsa.zdbjq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zri.shanyushiyangtech.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yoh.0kj1m.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dtu.nanxuanxn.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ers.hysaishi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ceh.guannengcc.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vmu.jyoumei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://stb.gzhubu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://tfe.sxryk.cn

[A24] 去除首尾空白
来源：http://zbq.xuanzx.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://snm.fehbvm.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bzd.snrcjt.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qoi.hfpthk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nax.zhijiandao.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dih.kuanghao11.cn

Go:   strings.TrimSpace(s)
来源：http://jcv.hesvh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mnc.xylfe.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wpm.daxiang520.top

[A25] 字符串比较
来源：http://grp.svipenyu.cn

Py:   s1 == s2; s1 != s2
来源：http://zfi.quarkkingdee.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vsk.shanyushiyangtech.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sgh.fanxiaobao.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://huo.gzhubu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pgc.jianghu66.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://epc.chenzaomai.com

Ruby: s1 == s2; s1 <=> s2
来源：http://zcs.andypj.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://psy.quarkkingdee.top

[A26] 类型转换总览
来源：http://vde.zhongyouzk.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zar.dashuyun.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fzo.ivvv.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gto.xuanzx.com

TS:   Number() String() Boolean() x as number
来源：http://hqh.sjlbkw.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lzg.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oey.ydjk.org.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wou.haohaochexian.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bdb.sxryk.cn

================================================================================
来源：http://ryc.jiagoushi.top

B. 流程控制
来源：http://mon.jqgfzy.top

================================================================================
来源：http://ouk.fktsv.cn

[B01] 条件判断 if / else
来源：http://ruu.daxiang520.top

Py:   result = "正" if x > 0 else "非正"
来源：http://yrr.fzhhl.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ygt.zdbjq.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yjp.havefunace.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bvr.hnqzz.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://omp.zhaomingkeji.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hkk.yfazqb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wje.zhixingplan.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://thb.xingfuxueyuan.xyz

[B02] 多分支 else if / elif
来源：http://uik.bbcook.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oiv.zhoulong.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://piv.zhoulong.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ahg.dashuyun.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qqd.sjlbkw.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gau.feifeiyinyue.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://isz.guowangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fqj.havefunace.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ioa.aizwys.cn

[B03] switch / match / case
来源：http://tiw.ppjwa.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hvg.yfazqb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://slj.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://twy.vehdjk.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xnb.cqqwz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iki.dianchejie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kbw.aizwys.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://deo.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yxs.yongpay.top

[B04] for 计数循环
来源：http://vzv.hnqzz.top

Py:   for i in range(10): print(i)
来源：http://znc.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hsz.ybcxt.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mky.shzxlz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vdt.hfpthk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lqs.fktsv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nmk.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://gnv.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jol.jlsjyb.cn

[B05] 遍历数组 / 列表
来源：http://yij.yfazqb.com

Py:   for item in arr: print(item)
来源：http://mpd.shanyushiyangtech.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wrk.zdqjudy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://axv.ydzc1.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tzf.aibaodan.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fzh.ybcxt.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xcu.yj202588.top

Ruby: arr.each { |item| puts item }
来源：http://mxd.yonumen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gwp.zdbjq.cn

[B06] 遍历字典 / 对象
来源：http://wgq.kuanghao11.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://caz.ppjwa.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ofs.yonumen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ckw.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fac.tian-w.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uzt.dianchejie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fzf.yonumen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ezq.zdqjudy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sca.ydjk.org.cn

[B07] while 循环
来源：http://qfl.shzxlz.cn

Py:   while i < 10: i += 1
来源：http://xel.yuxming.cn

PHP:  while ($i < 10) { $i++; }
来源：http://epo.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://dqr.shzxlz.cn

TS:   while (i < 10) { i++; }
来源：http://fxp.316326.xyz

Java: while (i < 10) { i++; }
来源：http://fcx.sweek.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gdu.c1oappe.top

Ruby: while i < 10; i += 1; end
来源：http://har.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://mxe.zhaomingkeji.xyz

[B08] do-while（至少执行一次）
来源：http://jda.0kj1m.cn

Py:   # 无 do-while：用 while True + break
来源：http://avf.gogol.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://obf.havefunace.top

JS:   do { i++; } while (i < 10);
来源：http://ymv.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://xsn.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://cro.gogol.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cec.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://ijb.xuetiantiany.cn

C#:   do { i++; } while (i < 10);
来源：http://lcw.xinyue.icu

[B09] break 与 continue
来源：http://nde.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cnh.pycfn.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dqd.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wky.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqq.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://peu.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oyx.zhaomingkeji.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vcq.zhixingplan.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bld.yanxiufei.cn

[B10] 遍历同时拿索引
来源：http://abs.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oaa.0kj1m.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ade.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tdl.yfazqb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bbt.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pli.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://von.c1oappe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ofl.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ujm.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://yuc.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://ggv.chenlongwang.top

PHP:  range(0, 10, 2);
来源：http://qpa.hnxiangtu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qqf.316326.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rtn.yonumen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yds.ppjwa.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ska.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://ybh.havefunace.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uba.cheryme.top

[B12] 跳出多层循环
来源：http://rje.cashguo.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ojk.ppjwa.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zxp.dianchejie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vpo.ppjwa.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yob.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tqk.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tim.hnxiangtu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qld.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://epo.jiagoushi.top

[B13] 判断是否为数字
来源：http://rtc.hysaishi.cn

Py:   isinstance(x, (int, float))
来源：http://ath.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://cox.yanxiufei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vwh.redwolf501.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kqc.hysaishi.cn

Java: x instanceof Number
来源：http://dqv.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nfb.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://ynn.cucudq.cn

C#:   x is int or double or decimal
来源：http://xjq.svipenyu.cn

[B14] 判断值是否在集合内
来源：http://wmr.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ihx.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://orl.daxiang520.top

JS:   [1, 2, 3].includes(x)
来源：http://rjs.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://yar.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://uxg.zhixingplan.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mbt.yangfankeji.com

Ruby: [1, 2, 3].include?(x)
来源：http://llt.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hsx.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://ocf.aibaodan.cn

Py:   a and b or not c
来源：http://mfc.yangfankeji.com

PHP:  $a && $b || !$c
来源：http://nmh.nwbrower.top

JS:   a && b || !c
来源：http://vyd.hfpthk.cn

TS:   a && b || !c
来源：http://rju.xuetiantiany.cn

Java: a && b || !c
来源：http://jns.ppjwa.cn

Go:   a && b || !c
来源：http://wqh.hnqzz.top

Ruby: a && b || !c
来源：http://jxv.tian-w.cn

C#:   a && b || !c
来源：http://rco.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://njh.shanyushiyangkeji.top

Py:   if not data: return
来源：http://bje.zhaomingkeji.xyz

PHP:  if (!$data) { return; }
来源：http://buo.jqgufenzy.top

JS:   if (!data) return;
来源：http://dir.hysaishi.cn

TS:   if (!data) return;
来源：http://tuo.guannengcc.top

Java: if (data == null) return;
来源：http://clp.cashguo.top

Go:   if data == nil { return }
来源：http://ukz.mhx1999.top

Ruby: return if data.nil?
来源：http://vsx.hnqzz.top

C#:   if (data == null) return;
来源：http://erq.gogol.net.cn

================================================================================
来源：http://spn.fehbvm.com

C. 函数与作用域
来源：http://mle.daxiang520.top

================================================================================
来源：http://nmh.yuxming.cn

[C01] 定义函数
来源：http://xrj.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://vjb.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nbf.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://bgl.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xxr.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vbr.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vnn.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://vti.aizwys.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fyg.vqdsnc.cn

[C02] 默认参数
来源：http://qeb.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://cyg.hongshengwenyu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://boh.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://gvm.cheryme.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jmv.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zpv.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dvw.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://ocj.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://rpo.xylfe.cn

[C03] 可变参数
来源：http://ata.dianchejie.cn

Py:   def total(*args): return sum(args)
来源：http://dco.hammf.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ozd.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fzz.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ywk.svipenyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tij.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kfj.chenzaomai.com

Ruby: def total(*nums); nums.sum; end
来源：http://mud.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ebn.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://moo.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://akh.jlsjyb.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zbn.yj202588.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jgk.52xcode.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://faa.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://uvm.cqqwz.cn

Go:   // 无：用配置结构体参数
来源：http://yho.cheryme.top

Ruby: f(a: 1, b: 2)
来源：http://qcl.redwolf501.top

C#:   f(a: 1, b: 2)
来源：http://win.xuetiantiany.cn

[C05] 返回多个值
来源：http://gzk.nwbrower.top

Py:   return a, b
来源：http://uww.zhixingplan.top

PHP:  return [$a, $b];
来源：http://nwu.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jzg.haohaochexian.top

TS:   return { a, b };
来源：http://vxt.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gbj.fzhhl.top

Go:   return a, b
来源：http://gbl.ybcxt.top

Ruby: return a, b
来源：http://lvv.nwbrower.top

C#:   return (a, b);              // ValueTuple
来源：http://tsl.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://hlz.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://jms.52xcode.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oiv.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://fls.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://juq.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wsl.fktsv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jhl.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://zhp.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ijc.aibaodan.cn

[C07] 把函数作为参数传入
来源：http://paj.tanke756.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://duv.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://zpo.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cal.ydjk.org.cn

TS:   arr.map(String)
来源：http://jls.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nkz.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gmz.jlsjyb.cn

Ruby: arr.map(&:upcase)
来源：http://tws.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jpy.redwolf501.top

[C08] 闭包
来源：http://zst.chenjidiqi.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jpj.xuanzx.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kdf.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xfz.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eqb.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kbg.ehwqpu.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ipc.hnxiangtu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://osp.jlsjyb.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qfb.wangdashe.top

[C09] 递归
来源：http://hvy.zdbjq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pmx.sxryk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://twl.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://egi.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wgb.dashuyun.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iki.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dpq.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jcc.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hzh.cheryme.top

[C10] 变量作用域
来源：http://akn.zycfv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ueb.yuxming.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://weq.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vzd.cashguo.top

TS:   同 JS
来源：http://inf.xingfuxueyuan.xyz

Java: 方法内为块级作用域
来源：http://xbu.gotoacloud.top

Go:   花括号块级作用域
来源：http://gpr.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sqw.ydjk.org.cn

C#:   块级作用域
来源：http://qax.hesvh.cn

[C11] 模块导入与导出
来源：http://zwg.nanxinkj.top

Py:   from module import func
来源：http://xpd.nanxinkj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dsw.shzxlz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hja.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rlv.jyoumei.cn

Java: import java.util.List;
来源：http://cjt.nanxuanxn.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://was.cqqwz.cn

Ruby: require "json"; require_relative "./util"
来源：http://xcd.gaohongyu789.top

C#:   using System.Text;
来源：http://jzq.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://xdh.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://yyq.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://mjv.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://elu.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://wez.sweek.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pnf.jqgufenzy.top


<!-- 参考信息 -->