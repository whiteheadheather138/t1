代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xwb.yuxming.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rah.wangshuangyany.cn

[A24] 去除首尾空白
来源：http://loq.guannengcc.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ygr.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jdy.gogol.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zet.fehbvm.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rvj.yuanzhike.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sfi.sjlbkw.cn

Go:   strings.TrimSpace(s)
来源：http://jur.hnqzz.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uzb.fktsv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yog.epnwcf.com

[A25] 字符串比较
来源：http://uoq.zhoulong.xyz

Py:   s1 == s2; s1 != s2
来源：http://kvf.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tvv.cucudq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oqi.hcnkem.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mta.tian-w.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dhh.sxryk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hvq.yj20258.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bth.yongpay.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mli.fktsv.cn

[A26] 类型转换总览
来源：http://gdn.chenzaomai.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lsz.daxiang520.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yyt.0kj1m.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dtw.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://hti.c1oappe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fzl.svipenyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tpi.vqdsnc.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ckl.jiagoushi.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kev.tianlin.xyz

================================================================================
来源：http://olq.daria6918.cn

B. 流程控制
来源：http://cng.ehwqpu.com

================================================================================
来源：http://ngf.52xcode.cn

[B01] 条件判断 if / else
来源：http://eoq.xingfuxueyuan.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://plx.xuanzx.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tsi.mhx1999.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mcn.dashuyun.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qba.zdqjudy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://teg.nwbrower.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wol.ydjk.org.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cmq.jinghuilouyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tzu.yvedp.cn

[B02] 多分支 else if / elif
来源：http://mzt.wangshuangyany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fxr.9152youxi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pmx.shangyingyoupin.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zof.cdnleiting.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://onm.sufxvd.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wgq.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tow.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ryq.jlsjyb.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tlk.zhixingplan.top

[B03] switch / match / case
来源：http://gjw.xingfuxueyuan.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qzm.ctjpmb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xon.ivvv.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mqs.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://thn.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fva.9152youxi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zyp.fzhhl.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hmd.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rlt.tianlin.xyz

[B04] for 计数循环
来源：http://pdk.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://nmq.hcnkem.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eny.52xcode.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://evh.zdbjq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zxx.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uir.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vfr.jianghu66.top

Ruby: 10.times { |i| puts i }
来源：http://jdm.ywan-chungtsiang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://itm.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://dhm.0kj1m.cn

Py:   for item in arr: print(item)
来源：http://vpo.fengsongda.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dpo.sxryk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jci.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://pbd.zhiwuduotai.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jxm.bjfxy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uol.hammf.cn

Ruby: arr.each { |item| puts item }
来源：http://sle.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vdy.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://oio.yonumen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qnm.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://puy.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uxm.yuanzhike.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oic.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://urh.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tvs.hesvh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tbc.tianlin.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zhl.xylfe.cn

[B07] while 循环
来源：http://gpw.chenlongwang.top

Py:   while i < 10: i += 1
来源：http://rfs.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eil.gotoacloud.top

JS:   while (i < 10) { i++; }
来源：http://xsn.zdbjq.cn

TS:   while (i < 10) { i++; }
来源：http://aww.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://kci.dashuyun.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uxk.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://mjl.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://iln.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://tna.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://plr.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lvz.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://ujw.tanke756.top

TS:   do { i++; } while (i < 10);
来源：http://mfu.tianlin.xyz

Java: do { i++; } while (i < 10);
来源：http://aiu.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zui.9152youxi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rto.uphjek.com

C#:   do { i++; } while (i < 10);
来源：http://knc.fzhhl.top

[B09] break 与 continue
来源：http://ate.yuanzhike.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vac.yj202588.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://piy.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dqn.gotoacloud.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzh.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ujr.yfazqb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tnb.jinyuanbaomall.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://evz.xinyue.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gld.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://fzu.zhijiandao.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tbq.tanke756.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rgr.andypj.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://drh.havefunace.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://shy.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ycr.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ceg.daria6918.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rfo.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zrr.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://hyr.daria6918.cn

Py:   list(range(0, 10, 2))
来源：http://ubj.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://inx.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ckq.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qwa.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kql.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xsm.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://vqr.fanxiaobao.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://afp.jinqigfzy.top

[B12] 跳出多层循环
来源：http://qms.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hnz.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vwp.yvedp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jgr.jianghu66.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://azq.zhongyouzk.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oar.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lms.shanyushiyangtech.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sft.wangdashe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hcz.cucudq.cn

[B13] 判断是否为数字
来源：http://qfr.uphjek.com

Py:   isinstance(x, (int, float))
来源：http://ckm.c1oappe.top

PHP:  is_numeric($x)
来源：http://pzf.jlsjyb.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ihm.redwolf501.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lpe.tian-w.cn

Java: x instanceof Number
来源：http://wuo.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ocn.zhoulong.xyz

Ruby: x.is_a?(Numeric)
来源：http://otv.gzhubu.top

C#:   x is int or double or decimal
来源：http://pjs.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://cls.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bsm.jlsjyb.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cob.chenlongwang.top

JS:   [1, 2, 3].includes(x)
来源：http://rwt.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://pkb.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gho.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kfk.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://swk.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fro.hysaishi.cn

[B15] 布尔运算与取反
来源：http://tto.hfpthk.cn

Py:   a and b or not c
来源：http://zcm.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://cya.xuanzx.com

JS:   a && b || !c
来源：http://diq.yueranfly.top

TS:   a && b || !c
来源：http://tra.chenlongwang.top

Java: a && b || !c
来源：http://dhf.vqdsnc.cn

Go:   a && b || !c
来源：http://ced.hnxiangtu.top

Ruby: a && b || !c
来源：http://jue.nanxuanxn.top

C#:   a && b || !c
来源：http://rqd.ydzc1.top

[B16] 卫语句：不满足条件提前返回
来源：http://isn.vehdjk.com

Py:   if not data: return
来源：http://tqe.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://tgk.yuanzhike.top

JS:   if (!data) return;
来源：http://kqq.guowangkeji.top

TS:   if (!data) return;
来源：http://pye.vehdjk.com

Java: if (data == null) return;
来源：http://wgu.zycfv.cn

Go:   if data == nil { return }
来源：http://akn.jiagoushi.top

Ruby: return if data.nil?
来源：http://ruu.ybcxt.top

C#:   if (data == null) return;
来源：http://akf.birdmap.top

================================================================================
来源：http://eua.daxiang520.top

C. 函数与作用域
来源：http://emo.hfpthk.cn

================================================================================
来源：http://spo.yj20258.top

[C01] 定义函数
来源：http://esk.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://qfl.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://may.fengsongda.top

JS:   function add(a, b) { return a + b; }
来源：http://ezx.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://njf.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://rof.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://ppm.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://pab.jinqigfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bti.ybcxt.top

[C02] 默认参数
来源：http://hsv.0kj1m.cn

Py:   def greet(name="World"): return name
来源：http://zez.pycfn.com

PHP:  function greet($name = "World") { return $name; }
来源：http://hhs.fktsv.cn

JS:   function greet(name = "World") { return name; }
来源：http://pqj.vqdsnc.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mzg.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://btc.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qiv.jianghu66.top

Ruby: def greet(name = "World") = name
来源：http://dut.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://wot.zdbjq.cn

[C03] 可变参数
来源：http://bow.jiagoushi.top

Py:   def total(*args): return sum(args)
来源：http://puy.cucudq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://shm.9152youxi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wok.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ntw.guowangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ach.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vcz.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://nwf.guannengcc.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mvd.aibaodan.cn

[C04] 命名参数 / 关键字参数
来源：http://pnt.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://whm.sjlbkw.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lso.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oao.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iup.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://uya.cheryme.top

Go:   // 无：用配置结构体参数
来源：http://xba.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://des.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://pjn.guannengcc.top

[C05] 返回多个值
来源：http://pul.fktsv.cn

Py:   return a, b
来源：http://ocj.xziqi.cn

PHP:  return [$a, $b];
来源：http://saz.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rwd.chenzaomai.com

TS:   return { a, b };
来源：http://bsc.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://utn.gotoacloud.top

Go:   return a, b
来源：http://vsw.gzhubu.top

Ruby: return a, b
来源：http://unk.fktsv.cn

C#:   return (a, b);              // ValueTuple
来源：http://ipd.ehwqpu.com

[C06] 匿名函数 / lambda
来源：http://nqu.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://zhs.cashguo.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ovx.hcnkem.com

JS:   const square = x => x * x;
来源：http://bxw.jinyuanbaomall.cn

TS:   const square = (x: number): number => x * x;
来源：http://eve.zhengqikj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ffn.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://kma.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://ayg.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://slf.wangdashe.top

[C07] 把函数作为参数传入
来源：http://cml.daxiang520.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uwk.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://asa.hcnkem.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cja.fzhhl.top

TS:   arr.map(String)
来源：http://dxg.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://klw.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sbw.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://lmv.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vra.hammf.cn

[C08] 闭包
来源：http://xaf.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://huf.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ejz.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qtc.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rej.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kpo.fktsv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eaj.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xcf.redwolf501.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nps.xuetiantiany.cn

[C09] 递归
来源：http://eyt.cheryme.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xat.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cbm.dianchejie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xzd.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tst.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mlk.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://owm.aibaodan.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xcf.ydzc1.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ljz.nanxinkj.top

[C10] 变量作用域
来源：http://okp.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wid.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://etp.hfpthk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ajv.ywan-chungtsiang.top

TS:   同 JS
来源：http://zny.shangyingyoupin.top

Java: 方法内为块级作用域
来源：http://ilx.pycfn.com

Go:   花括号块级作用域
来源：http://csp.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pwl.cashguo.top

C#:   块级作用域
来源：http://spw.cucudq.cn

[C11] 模块导入与导出
来源：http://ssu.fengsongda.top

Py:   from module import func
来源：http://hyh.gotoacloud.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cxp.gotoacloud.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ojr.feifeiyinyue.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://loo.shangyingyoupin.top

Java: import java.util.List;
来源：http://grx.hywenlv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pbe.cqqwz.cn

Ruby: require "json"; require_relative "./util"
来源：http://pqv.cdnleiting.top

C#:   using System.Text;
来源：http://wbe.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://mhl.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://mlb.dashuyun.cn

PHP:  (function () { echo "run"; })();
来源：http://itg.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://qdv.zhoulong.xyz

TS:   (() => { console.log("run"); })();
来源：http://htj.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yas.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://lze.yongpay.top

Ruby: -> { puts "run" }.call
来源：http://iwn.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ypf.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://pxo.snrcjt.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ozg.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ybh.guowangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cyv.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jqf.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://jxi.yj20258.top

Go:   func add(a, b int) int
来源：http://yju.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bye.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://szu.jqgfzy.top

[C14] 泛型函数
来源：http://ktt.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oui.zhongyouzk.top

PHP:  // 无泛型
来源：http://nyl.ivvv.top

JS:   // 无泛型
来源：http://jfj.yuanzhike.top


<!-- 参考信息 -->