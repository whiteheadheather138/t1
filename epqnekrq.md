代发 wailian999

[A22] 获取字符串长度
来源：http://sou.yangfankeji.com

Py:   len(s)
来源：http://gww.chenjidiqi.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://scy.bbcook.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sis.yj20258888.top

TS:   s.length
来源：http://puk.daria6918.cn

Java: s.length()
来源：http://isk.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nuq.havefunace.top

Ruby: s.length
来源：http://ezw.epnwcf.com

C#:   s.Length
来源：http://eea.zhengqikj.top

[A23] 大小写转换
来源：http://nlp.cucudq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ruo.redwolf501.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jtj.yj202588.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vlu.haohaochexian.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uvz.iojbl.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cfe.zdqjudy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://abr.havefunace.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zxj.aizwys.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gjm.yonumen.top

[A24] 去除首尾空白
来源：http://fvm.ehwqpu.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sln.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gtd.c1oappe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hfy.nwbrower.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://upp.snrcjt.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pch.uphjek.com

Go:   strings.TrimSpace(s)
来源：http://vmh.fktsv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ftu.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cup.meibo888.top

[A25] 字符串比较
来源：http://ufn.hammf.cn

Py:   s1 == s2; s1 != s2
来源：http://grp.yonumen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://joo.vqdsnc.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yih.gotoacloud.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lwt.yanxiufei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pvb.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://urs.9152youxi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oji.haohaochexian.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dqw.xylfe.cn

[A26] 类型转换总览
来源：http://hjk.hongshengwenyu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yil.nanxinkj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yrm.hfpthk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bks.jiagoushi.top

TS:   Number() String() Boolean() x as number
来源：http://ztv.redwolf501.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oug.wangdashe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qou.sufxvd.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tte.yj202588.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lwf.gotoacloud.top

================================================================================
来源：http://rbh.chenzaomai.com

B. 流程控制
来源：http://dyh.zdbjq.cn

================================================================================
来源：http://oeb.fengsongda.top

[B01] 条件判断 if / else
来源：http://ydg.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xwp.ybcxt.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hbo.yuxming.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jvt.jianghu66.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blo.yueranfly.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uzp.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zmr.meibo888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://usu.dashuyun.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://taf.sjlbkw.cn

[B02] 多分支 else if / elif
来源：http://nss.guannengcc.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cti.0kj1m.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vat.birdmap.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vvv.c1oappe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rea.gaohongyu789.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fxj.jlsjyb.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tsg.wangdashe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gnm.wangshuangyany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fsg.svipenyu.cn

[B03] switch / match / case
来源：http://ish.dianchejie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kgk.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kcl.zhijiandao.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zds.kuanghao11.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wof.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pct.sysykeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fjf.hfpthk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qfg.ppjwa.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://olk.vehdjk.com

[B04] for 计数循环
来源：http://qet.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://otl.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ukf.0kj1m.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iwe.tian-w.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ipa.chenlongwang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kel.zdbjq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qju.cqqwz.cn

Ruby: 10.times { |i| puts i }
来源：http://avd.aibaodan.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vjt.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://usk.yonumen.top

Py:   for item in arr: print(item)
来源：http://erq.cheryme.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ztk.cucudq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yml.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kvf.jlsjyb.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tzv.jlsjyb.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tbs.guowangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://hpf.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yte.hysaishi.cn

[B06] 遍历字典 / 对象
来源：http://mlk.ivvv.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xgn.shanyushiyangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gff.fengsongda.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xne.jinyuanbaomall.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://adu.svipenyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jza.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ihh.sweek.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ecx.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fto.hywenlv.cn

[B07] while 循环
来源：http://uyb.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://whn.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jzf.redwolf501.top

JS:   while (i < 10) { i++; }
来源：http://pzk.jinyuanbaomall.cn

TS:   while (i < 10) { i++; }
来源：http://sin.guowangkeji.top

Java: while (i < 10) { i++; }
来源：http://tzv.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kgp.tarul.cn

Ruby: while i < 10; i += 1; end
来源：http://lkd.tian-w.cn

C#:   while (i < 10) { i++; }
来源：http://qax.shanyushiyangtech.top

[B08] do-while（至少执行一次）
来源：http://kqo.9152youxi.cn

Py:   # 无 do-while：用 while True + break
来源：http://vzz.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://sra.zdbjq.cn

JS:   do { i++; } while (i < 10);
来源：http://fog.hcnkem.com

TS:   do { i++; } while (i < 10);
来源：http://bvi.cucudq.cn

Java: do { i++; } while (i < 10);
来源：http://obe.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://iox.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://dby.zdqjudy.top

C#:   do { i++; } while (i < 10);
来源：http://cff.ybcxt.top

[B09] break 与 continue
来源：http://djk.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fii.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ihj.yvedp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mxl.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zsq.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kkb.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wgy.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wok.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bfp.shuidangran.top

[B10] 遍历同时拿索引
来源：http://zsu.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://huy.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xzt.fehbvm.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sfb.tarul.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ukk.daria6918.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hoj.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fxa.chenlongwang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qrg.52xcode.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eww.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://vgx.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://rfv.gzhubu.top

PHP:  range(0, 10, 2);
来源：http://qnt.shanyushiyangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fye.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qxx.jinghuilouyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pfw.fzhhl.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mvr.daria6918.cn

Ruby: (0...10).step(2).to_a
来源：http://yrr.hywenlv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oiy.yfazqb.com

[B12] 跳出多层循环
来源：http://bas.ehwqpu.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://xih.kuanghao11.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yby.hesvh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://esy.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://byr.dashuyun.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://srq.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mgy.havefunace.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://win.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://trv.nanxinkj.top

[B13] 判断是否为数字
来源：http://drn.zhengqikj.top

Py:   isinstance(x, (int, float))
来源：http://ldc.smart0.xyz

PHP:  is_numeric($x)
来源：http://xxk.svipenyu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pto.316326.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nmu.zhengqikj.top

Java: x instanceof Number
来源：http://jbq.feifeiyinyue.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gel.jyoumei.cn

Ruby: x.is_a?(Numeric)
来源：http://lpn.chenzaomai.com

C#:   x is int or double or decimal
来源：http://dgp.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://hul.yuxming.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zxn.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gry.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://wfh.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://adw.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qam.ctjpmb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qaf.bbcook.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cqm.52xcode.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qpf.sweek.top

[B15] 布尔运算与取反
来源：http://gyo.shuidangran.top

Py:   a and b or not c
来源：http://plk.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://uqj.gotoacloud.top

JS:   a && b || !c
来源：http://xby.svipenyu.cn

TS:   a && b || !c
来源：http://hak.guannengcc.top

Java: a && b || !c
来源：http://kha.guannengcc.top

Go:   a && b || !c
来源：http://rrc.hnxiangtu.top

Ruby: a && b || !c
来源：http://sal.gotoacloud.top

C#:   a && b || !c
来源：http://vta.jinyuanbaomall.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fna.yuxming.cn

Py:   if not data: return
来源：http://hkl.smart0.xyz

PHP:  if (!$data) { return; }
来源：http://qsw.jiagoushi.top

JS:   if (!data) return;
来源：http://lko.yuxming.cn

TS:   if (!data) return;
来源：http://mga.xinyue.icu

Java: if (data == null) return;
来源：http://gei.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://dvd.ybcxt.top

Ruby: return if data.nil?
来源：http://bek.cashguo.top

C#:   if (data == null) return;
来源：http://sen.cdnleiting.top

================================================================================
来源：http://tpg.jinyuanbaomall.cn

C. 函数与作用域
来源：http://uhd.chenzaomai.com

================================================================================
来源：http://vfz.jlsjyb.cn

[C01] 定义函数
来源：http://lzb.hnxiangtu.top

Py:   def add(a, b): return a + b
来源：http://zce.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ujl.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://ldx.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hxo.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dmd.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://kjb.sjlbkw.cn

Ruby: def add(a, b); a + b; end
来源：http://apm.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ais.dashuyun.cn

[C02] 默认参数
来源：http://wvi.epnwcf.com

Py:   def greet(name="World"): return name
来源：http://jxx.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://olz.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://ahy.haohaochexian.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xkv.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fgk.guannengcc.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rxe.ctjpmb.com

Ruby: def greet(name = "World") = name
来源：http://crj.hesvh.cn

C#:   string Greet(string name = "World") => name;
来源：http://sac.yangfankeji.com

[C03] 可变参数
来源：http://crf.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://mxq.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fmz.hongshengwenyu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tms.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ezz.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wug.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fff.cheryme.top

Ruby: def total(*nums); nums.sum; end
来源：http://llr.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vnt.fehbvm.com

[C04] 命名参数 / 关键字参数
来源：http://qdy.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ude.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://frk.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lpt.zdbjq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wvw.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://aar.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://lyx.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://ujv.xziqi.cn

C#:   f(a: 1, b: 2)
来源：http://cgo.yongpay.top

[C05] 返回多个值
来源：http://dar.shuidangran.top

Py:   return a, b
来源：http://wot.guowangkeji.top

PHP:  return [$a, $b];
来源：http://pis.sysykeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lqn.ctjpmb.com

TS:   return { a, b };
来源：http://ggq.yfazqb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pch.vehdjk.com

Go:   return a, b
来源：http://ypx.jlsjyb.cn

Ruby: return a, b
来源：http://yqi.fzhhl.top

C#:   return (a, b);              // ValueTuple
来源：http://cei.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://efx.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://rkm.fanxiaobao.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://wqp.gaohongyu789.top

JS:   const square = x => x * x;
来源：http://ari.aibaodan.cn

TS:   const square = (x: number): number => x * x;
来源：http://bxj.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oct.zhiwuduotai.top

Go:   sq := func(x int) int { return x * x }
来源：http://lyt.hongshengwenyu.top

Ruby: square = ->(x) { x * x }
来源：http://pad.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://vig.andypj.xyz

[C07] 把函数作为参数传入
来源：http://exr.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aqr.hnxiangtu.top

PHP:  array_map("strtoupper", $arr);
来源：http://lmf.wangdashe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gcj.zdbjq.cn

TS:   arr.map(String)
来源：http://njj.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dvp.jinyuanbaomall.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://swy.hongshengwenyu.top

Ruby: arr.map(&:upcase)
来源：http://oil.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://jvu.sysykeji.top

[C08] 闭包
来源：http://jro.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qqj.zhaomingkeji.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ccw.uphjek.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://plu.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://epu.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qer.zhengqikj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zto.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://exa.vqdsnc.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vgv.hongshengwenyu.top

[C09] 递归
来源：http://cvs.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hrh.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sih.ydzc1.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lvy.yangfankeji.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fwo.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sat.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baz.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zzo.shangyingyoupin.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cub.yvedp.cn

[C10] 变量作用域
来源：http://whl.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://slj.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://owl.vqdsnc.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://svg.yuxming.cn

TS:   同 JS
来源：http://kof.xylfe.cn

Java: 方法内为块级作用域
来源：http://nyu.zhengqikj.top

Go:   花括号块级作用域
来源：http://kkj.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yeo.hywenlv.cn

C#:   块级作用域
来源：http://ecj.mhx1999.top

[C11] 模块导入与导出
来源：http://adq.nanxuanxn.top

Py:   from module import func
来源：http://uid.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://aqg.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jvw.hywenlv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nsy.aibaodan.cn

Java: import java.util.List;
来源：http://gqv.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dsm.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://sky.shuidangran.top

C#:   using System.Text;
来源：http://zpp.ybcxt.top

[C12] 立即执行函数 IIFE
来源：http://lqf.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://ofx.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://spq.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://lkj.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://lts.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kbj.jianghu66.top


<!-- 参考信息 -->