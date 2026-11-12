代发 wailian999

TS:   s.length
来源：http://yto.shangyingyoupin.top

Java: s.length()
来源：http://muo.cdnleiting.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hfb.jinyuanbaomall.cn

Ruby: s.length
来源：http://eck.0kj1m.cn

C#:   s.Length
来源：http://mpd.zhijiandao.cn

[A23] 大小写转换
来源：http://sfv.ywan-chungtsiang.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bof.cheryme.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bxp.aibaodan.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tnv.shzxlz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pyt.jqgfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ocz.fengsongda.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://azv.yonumen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cdb.cdnleiting.top

C#:   s.ToUpper(); s.ToLower()
来源：http://tvk.sufxvd.cn

[A24] 去除首尾空白
来源：http://aau.svipenyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ktg.andypj.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ehh.chenjidiqi.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ebx.havefunace.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bkp.zhixingplan.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qeq.bbcook.cn

Go:   strings.TrimSpace(s)
来源：http://yzw.vqdsnc.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://acv.zdqjudy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cmi.jyoumei.cn

[A25] 字符串比较
来源：http://prc.gotoacloud.top

Py:   s1 == s2; s1 != s2
来源：http://hne.tianlin.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mow.nwbrower.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://twd.hywenlv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ffx.smart0.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hem.yj202588.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dbu.fktsv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://spt.smart0.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jjb.birdmap.top

[A26] 类型转换总览
来源：http://dhw.dianchejie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ggx.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tut.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cos.shuidangran.top

TS:   Number() String() Boolean() x as number
来源：http://eoq.chenjidiqi.icu

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tmk.shanyushiyangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://odm.nanxuanxn.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gic.fzhhl.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wlr.cheryme.top

================================================================================
来源：http://zgk.snrcjt.cn

B. 流程控制
来源：http://vmq.mhx1999.top

================================================================================
来源：http://bfl.yanxiufei.cn

[B01] 条件判断 if / else
来源：http://qho.ppjwa.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wew.fzhhl.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gue.gogol.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yhs.52xcode.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lyv.havefunace.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://oos.fanxiaobao.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yhk.chenzaomai.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://emi.jinyuanbaomall.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://osl.hammf.cn

[B02] 多分支 else if / elif
来源：http://amb.bjfxy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gfc.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hpn.pengpengdd.cyou

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://voe.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zli.hnxiangtu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://khy.smart0.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://egh.ybcxt.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bub.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tav.aibaodan.cn

[B03] switch / match / case
来源：http://npo.9152youxi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tli.wangdashe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nwb.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tws.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kda.redwolf501.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://csj.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xju.gogol.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uib.vehdjk.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dgw.xylfe.cn

[B04] for 计数循环
来源：http://zlo.cqqwz.cn

Py:   for i in range(10): print(i)
来源：http://spc.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fuc.snrcjt.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://glo.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blh.yvedp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rtq.zdbjq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zic.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://zxn.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zfp.hammf.cn

[B05] 遍历数组 / 列表
来源：http://onv.redwolf501.top

Py:   for item in arr: print(item)
来源：http://djx.sjlbkw.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qdb.tianlin.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://ggi.cdnleiting.top

TS:   for (const item of arr) { console.log(item); }
来源：http://spf.vehdjk.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://lyj.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kuu.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://ckw.yj20258.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jod.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://krp.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://upg.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cse.bbcook.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ykv.yueranfly.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fqm.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://anl.sxryk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wrl.chenjidiqi.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zkw.yj202588.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mjn.zdbjq.cn

[B07] while 循环
来源：http://sfo.cheryme.top

Py:   while i < 10: i += 1
来源：http://uyk.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://ziz.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://luc.gaohongyu789.top

TS:   while (i < 10) { i++; }
来源：http://zmj.shanyushiyangkeji.top

Java: while (i < 10) { i++; }
来源：http://gzj.tianlin.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qdl.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://usp.jianghu66.top

C#:   while (i < 10) { i++; }
来源：http://klq.hnqzz.top

[B08] do-while（至少执行一次）
来源：http://ibr.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://vsf.52xcode.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ojr.birdmap.top

JS:   do { i++; } while (i < 10);
来源：http://iuz.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://its.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://xvs.ivvv.top

Go:   for { i++; if i >= 10 { break } }
来源：http://afj.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://kev.tian-w.cn

C#:   do { i++; } while (i < 10);
来源：http://yvh.hammf.cn

[B09] break 与 continue
来源：http://zjt.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gbg.yj202588.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cul.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hii.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yxq.meibo888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wah.xylfe.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qcy.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://abe.guowangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bsc.guowangkeji.top

[B10] 遍历同时拿索引
来源：http://drc.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yoa.hcnkem.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lvk.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cua.smart0.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://omy.tianlin.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sno.bbcook.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://klu.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bhs.hnxiangtu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xiv.kuanghao11.cn

[B11] 生成数字序列 / 区间
来源：http://rho.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://buk.ywan-chungtsiang.top

PHP:  range(0, 10, 2);
来源：http://ktl.cdnleiting.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bgv.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dao.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lkv.pengpengdd.cyou

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ubp.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://jek.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lwy.gogol.net.cn

[B12] 跳出多层循环
来源：http://rqb.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wsm.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://crf.yuanzhike.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jwy.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pib.xuanzx.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vds.zhiwuduotai.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zae.52xcode.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wgz.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gvi.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://prp.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://xaw.chenzaomai.com

PHP:  is_numeric($x)
来源：http://fls.fktsv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lst.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ans.uphjek.com

Java: x instanceof Number
来源：http://inz.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://snr.gzhubu.top

Ruby: x.is_a?(Numeric)
来源：http://hsl.jinqigufen.top

C#:   x is int or double or decimal
来源：http://zzj.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://zht.gaohongyu789.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://loz.redwolf501.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vvn.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://qdq.svipenyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://ljw.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ewb.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bqz.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://chu.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jud.ctjpmb.com

[B15] 布尔运算与取反
来源：http://tfs.dashuyun.cn

Py:   a and b or not c
来源：http://tnf.yueranfly.top

PHP:  $a && $b || !$c
来源：http://vgr.gzhubu.top

JS:   a && b || !c
来源：http://cpk.yonumen.top

TS:   a && b || !c
来源：http://qhp.ctjpmb.com

Java: a && b || !c
来源：http://mqg.quarkkingdee.top

Go:   a && b || !c
来源：http://uit.zhaomingkeji.xyz

Ruby: a && b || !c
来源：http://kna.shuidangran.top

C#:   a && b || !c
来源：http://ffu.ivvv.top

[B16] 卫语句：不满足条件提前返回
来源：http://hho.yanxiufei.cn

Py:   if not data: return
来源：http://qwk.haohaochexian.top

PHP:  if (!$data) { return; }
来源：http://efj.chenjidiqi.icu

JS:   if (!data) return;
来源：http://pkv.guowangkeji.top

TS:   if (!data) return;
来源：http://gks.zhoulong.xyz

Java: if (data == null) return;
来源：http://uoz.smart0.xyz

Go:   if data == nil { return }
来源：http://ptx.tianlin.xyz

Ruby: return if data.nil?
来源：http://bog.cashguo.top

C#:   if (data == null) return;
来源：http://mpi.tianlin.xyz

================================================================================
来源：http://jdm.kuanghao11.cn

C. 函数与作用域
来源：http://pap.dashuyun.cn

================================================================================
来源：http://rmq.zycfv.cn

[C01] 定义函数
来源：http://fka.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://rje.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zkc.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://psc.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://him.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://spj.gotoacloud.top

Go:   func add(a, b int) int { return a + b }
来源：http://euu.zdbjq.cn

Ruby: def add(a, b); a + b; end
来源：http://fyy.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qfl.meibo888.top

[C02] 默认参数
来源：http://nnq.xuetiantiany.cn

Py:   def greet(name="World"): return name
来源：http://uxq.jlsjyb.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://msa.hesvh.cn

JS:   function greet(name = "World") { return name; }
来源：http://wpo.316326.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://dpt.cashguo.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qzr.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://los.shzxlz.cn

Ruby: def greet(name = "World") = name
来源：http://scv.svipenyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://pea.chenjidiqi.icu

[C03] 可变参数
来源：http://ufu.wangdashe.top

Py:   def total(*args): return sum(args)
来源：http://zpl.vqdsnc.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qlb.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jrq.guowangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cjp.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iqe.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lbv.tianlin.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://gdc.jinyuanbaomall.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ukf.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://pcz.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://snu.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uar.yangfankeji.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fpz.meibo888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kpf.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://saa.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://pba.feifeiyinyue.top

Ruby: f(a: 1, b: 2)
来源：http://bsa.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://ubg.jlsjyb.cn

[C05] 返回多个值
来源：http://gqz.hcnkem.com

Py:   return a, b
来源：http://ucg.316326.xyz

PHP:  return [$a, $b];
来源：http://ryl.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tni.gaohongyu789.top

TS:   return { a, b };
来源：http://tza.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ape.jinqigfzy.top

Go:   return a, b
来源：http://nuj.snrcjt.cn

Ruby: return a, b
来源：http://rur.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://mdv.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://fnv.snrcjt.cn

Py:   square = lambda x: x * x
来源：http://fmm.yuanzhike.top

PHP:  $square = fn($x) => $x * $x;
来源：http://imr.uphjek.com

JS:   const square = x => x * x;
来源：http://dln.fehbvm.com

TS:   const square = (x: number): number => x * x;
来源：http://lze.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vri.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wpt.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://fkv.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://fyo.iojbl.cn

[C07] 把函数作为参数传入
来源：http://jcu.jinghuilouyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://guh.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://gez.aizwys.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xyw.52xcode.cn

TS:   arr.map(String)
来源：http://ivj.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cwj.yvedp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://exg.andypj.xyz

Ruby: arr.map(&:upcase)
来源：http://gmg.ctjpmb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://vlu.yj202588.top

[C08] 闭包
来源：http://dcx.chenjidiqi.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zzg.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ebh.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://red.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://npv.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jye.jyoumei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gjc.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bzw.jqgufenzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yhr.yj202588.top

[C09] 递归
来源：http://wxw.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qgk.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vtx.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wgp.aizwys.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gbf.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://scz.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://udc.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pfx.dashuyun.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iwv.hcnkem.com

[C10] 变量作用域
来源：http://npo.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mmr.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fqn.hongshengwenyu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wlt.hcnkem.com

TS:   同 JS
来源：http://dbl.fehbvm.com

Java: 方法内为块级作用域
来源：http://qgf.dianchejie.cn

Go:   花括号块级作用域
来源：http://vtn.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kti.zdbjq.cn

C#:   块级作用域
来源：http://ysd.yj20258888.top

[C11] 模块导入与导出
来源：http://sfd.52xcode.cn

Py:   from module import func
来源：http://cxg.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://jmb.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tce.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yzu.shuidangran.top

Java: import java.util.List;
来源：http://noc.fengsongda.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bgi.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ftw.cashguo.top

C#:   using System.Text;
来源：http://ndz.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://fke.nanxinkj.top

Py:   (lambda: print("run"))()
来源：http://jvp.wangshuangyany.cn

PHP:  (function () { echo "run"; })();
来源：http://acr.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://ekn.zhoulong.xyz

TS:   (() => { console.log("run"); })();
来源：http://bms.hnxiangtu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bxj.feifeiyinyue.top

Go:   func() { fmt.Println("run") }()
来源：http://jlf.mhx1999.top

Ruby: -> { puts "run" }.call
来源：http://mje.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fbe.zhongyouzk.top

[C13] 类型声明 / 类型注解
来源：http://yms.shangyingyoupin.top


<!-- 参考信息 -->