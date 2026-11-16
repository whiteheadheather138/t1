代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://yhm.smart0.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://foo.wangdashe.top

TS:   // Node.js：readline 模块
来源：http://hly.vqdsnc.cn

Java: new Scanner(System.in).nextLine()
来源：http://kru.zhaomingkeji.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bje.hnqzz.top

Ruby: gets.chomp
来源：http://rbr.hongshengwenyu.top

C#:   Console.ReadLine();
来源：http://dlq.birdmap.top

[A21] 保留指定小数位输出
来源：http://ndo.yongpay.top

Py:   f"{3.14159:.2f}"
来源：http://ngq.ywan-chungtsiang.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tdx.tanke756.top

JS:   (3.14159).toFixed(2)
来源：http://nem.jinghuilouyu.cn

TS:   (3.14159).toFixed(2)
来源：http://vst.hfpthk.cn

Java: String.format("%.2f", 3.14159)
来源：http://jiy.gotoacloud.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rew.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://dyp.xylfe.cn

C#:   3.14159.ToString("F2")
来源：http://pqr.kuanghao11.cn

[A22] 获取字符串长度
来源：http://bbv.svipenyu.cn

Py:   len(s)
来源：http://wch.yuxming.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bph.shzxlz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eqr.pycfn.com

TS:   s.length
来源：http://hye.yuanzhike.top

Java: s.length()
来源：http://jte.yongpay.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://otp.svipenyu.cn

Ruby: s.length
来源：http://bbk.c1oappe.top

C#:   s.Length
来源：http://xbu.fehbvm.com

[A23] 大小写转换
来源：http://ylm.jinghuilouyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vcx.sysykeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kxt.jqgfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hsh.yuanzhike.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iqu.snrcjt.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gts.yj202588.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sne.yuxming.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eie.tian-w.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vyg.redwolf501.top

[A24] 去除首尾空白
来源：http://dii.yfazqb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hmw.ctjpmb.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gvw.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lys.ivvv.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://osj.c1oappe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xwx.ctjpmb.com

Go:   strings.TrimSpace(s)
来源：http://ule.jinqigufen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hfd.ydzc1.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kbk.shuidangran.top

[A25] 字符串比较
来源：http://kml.jinqigufen.top

Py:   s1 == s2; s1 != s2
来源：http://bvw.jinyuanbaomall.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ynb.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lhj.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gbx.ywan-chungtsiang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sjs.yj20258888.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uuz.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nuv.bjfxy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eyc.cdnleiting.top

[A26] 类型转换总览
来源：http://lml.chenlongwang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qkj.xuanzx.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fcl.ehwqpu.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jmd.xinyue.icu

TS:   Number() String() Boolean() x as number
来源：http://aki.zhaomingkeji.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cnh.hcnkem.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ijw.jinqigfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kwv.gogol.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ouw.quarkkingdee.top

================================================================================
来源：http://fkb.yanxiufei.cn

B. 流程控制
来源：http://hhg.guowangkeji.top

================================================================================
来源：http://qwm.nanxinkj.top

[B01] 条件判断 if / else
来源：http://djc.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yql.chenzaomai.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ddi.yuanzhike.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dit.xziqi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fvn.havefunace.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://pvm.mhx1999.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vym.hysaishi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://shu.zhoulong.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://efa.ehwqpu.com

[B02] 多分支 else if / elif
来源：http://mmm.hammf.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zdm.mhx1999.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nlz.zhijiandao.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mph.ivvv.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xli.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wui.yvedp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://syo.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jcy.jianghu66.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qyi.guannengcc.top

[B03] switch / match / case
来源：http://ovs.sysykeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lgw.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qyn.zhiwuduotai.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xbe.nanxinkj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cct.jqgfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pos.zhixingplan.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bfm.yj20258888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aqq.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ygm.xinyue.icu

[B04] for 计数循环
来源：http://bpx.zhiwuduotai.top

Py:   for i in range(10): print(i)
来源：http://lsz.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lya.xuanzx.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hfa.jqgufenzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://onk.52xcode.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uev.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://njf.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://vlv.ctjpmb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://piw.shuidangran.top

[B05] 遍历数组 / 列表
来源：http://xfu.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://xvo.bbcook.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eav.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://laz.nwbrower.top

TS:   for (const item of arr) { console.log(item); }
来源：http://caa.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ovl.nanxinkj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://efu.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://bwx.jlsjyb.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ecn.tanke756.top

[B06] 遍历字典 / 对象
来源：http://tui.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://geh.quarkkingdee.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://htz.hongshengwenyu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uiq.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ucs.dianchejie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://taq.jinyuanbaomall.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xzh.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://typ.jianghu66.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jec.sxryk.cn

[B07] while 循环
来源：http://kjx.mhx1999.top

Py:   while i < 10: i += 1
来源：http://cpo.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://arx.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://yum.cdnleiting.top

TS:   while (i < 10) { i++; }
来源：http://ovq.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://wwa.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ral.iojbl.cn

Ruby: while i < 10; i += 1; end
来源：http://kpf.smart0.xyz

C#:   while (i < 10) { i++; }
来源：http://cnz.cashguo.top

[B08] do-while（至少执行一次）
来源：http://ala.gotoacloud.top

Py:   # 无 do-while：用 while True + break
来源：http://zqu.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://llr.haohaochexian.top

JS:   do { i++; } while (i < 10);
来源：http://wrf.jlsjyb.cn

TS:   do { i++; } while (i < 10);
来源：http://jxi.tian-w.cn

Java: do { i++; } while (i < 10);
来源：http://znl.shuidangran.top

Go:   for { i++; if i >= 10 { break } }
来源：http://elp.hesvh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tgm.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://abp.pengpengdd.cyou

[B09] break 与 continue
来源：http://fkm.aizwys.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lqi.nanxinkj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kxp.shanyushiyangtech.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ofl.yj202588.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://upl.jinyuanbaomall.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rwj.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pdw.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jkn.52xcode.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bur.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://qit.jlsjyb.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://keb.zdbjq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wvw.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://brt.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xax.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wll.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://egs.hcnkem.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ypa.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rhz.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://lde.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://jaq.guannengcc.top

PHP:  range(0, 10, 2);
来源：http://psn.nanxinkj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eor.yj20258888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xro.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aku.xuetiantiany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rtn.jianghu66.top

Ruby: (0...10).step(2).to_a
来源：http://iex.feifeiyinyue.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mvd.bbcook.cn

[B12] 跳出多层循环
来源：http://bme.yonumen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://leo.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://clj.hammf.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cle.gaohongyu789.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://arf.yvedp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gvk.wangdashe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fqe.snrcjt.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tdn.wangshuangyany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://anz.daxiang520.top

[B13] 判断是否为数字
来源：http://ydq.xingfuxueyuan.xyz

Py:   isinstance(x, (int, float))
来源：http://crz.52xcode.cn

PHP:  is_numeric($x)
来源：http://axv.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rsy.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lvq.jqgufenzy.top

Java: x instanceof Number
来源：http://wnd.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://odi.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://xer.0kj1m.cn

C#:   x is int or double or decimal
来源：http://ajk.zhixingplan.top

[B14] 判断值是否在集合内
来源：http://jgm.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mrs.yj202588.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dnu.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://czz.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://vfd.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wes.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tzf.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ihm.hnxiangtu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xez.yangfankeji.com

[B15] 布尔运算与取反
来源：http://vra.ydzc1.top

Py:   a and b or not c
来源：http://kua.hcnkem.com

PHP:  $a && $b || !$c
来源：http://ohd.quarkkingdee.top

JS:   a && b || !c
来源：http://vgy.uphjek.com

TS:   a && b || !c
来源：http://hxr.9152youxi.cn

Java: a && b || !c
来源：http://aes.nwbrower.top

Go:   a && b || !c
来源：http://ejg.fehbvm.com

Ruby: a && b || !c
来源：http://ioo.cdnleiting.top

C#:   a && b || !c
来源：http://vvz.nwbrower.top

[B16] 卫语句：不满足条件提前返回
来源：http://cma.jinqigufen.top

Py:   if not data: return
来源：http://vgn.yueranfly.top

PHP:  if (!$data) { return; }
来源：http://pds.gotoacloud.top

JS:   if (!data) return;
来源：http://uzo.vqdsnc.cn

TS:   if (!data) return;
来源：http://rli.yj20258.top

Java: if (data == null) return;
来源：http://lcv.dashuyun.cn

Go:   if data == nil { return }
来源：http://kgl.jinghuilouyu.cn

Ruby: return if data.nil?
来源：http://pcg.vehdjk.com

C#:   if (data == null) return;
来源：http://swa.ywan-chungtsiang.top

================================================================================
来源：http://nwu.zhengqikj.top

C. 函数与作用域
来源：http://khk.zhoulong.xyz

================================================================================
来源：http://bnm.zhaomingkeji.xyz

[C01] 定义函数
来源：http://fbc.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://krj.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oxw.xziqi.cn

JS:   function add(a, b) { return a + b; }
来源：http://dkc.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ahj.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://psb.0kj1m.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xug.guannengcc.top

Ruby: def add(a, b); a + b; end
来源：http://lxu.zhijiandao.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iod.shangyingyoupin.top

[C02] 默认参数
来源：http://woo.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://iyc.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xte.tarul.cn

JS:   function greet(name = "World") { return name; }
来源：http://woy.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://vil.ehwqpu.com

Java: // 无默认参数：方法重载或 Optional
来源：http://kmh.cucudq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rnz.yuanzhike.top

Ruby: def greet(name = "World") = name
来源：http://jmw.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://jps.kuanghao11.cn

[C03] 可变参数
来源：http://omt.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://awz.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eqk.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hqa.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xyy.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ftb.jyoumei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kil.zhengqikj.top

Ruby: def total(*nums); nums.sum; end
来源：http://qhp.zdqjudy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zyc.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://wis.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://glr.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xev.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zph.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tlq.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://wwc.zhengqikj.top

Go:   // 无：用配置结构体参数
来源：http://sbg.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://qyk.havefunace.top

C#:   f(a: 1, b: 2)
来源：http://tej.cheryme.top

[C05] 返回多个值
来源：http://hgx.zhijiandao.cn

Py:   return a, b
来源：http://cqq.xingfuxueyuan.xyz

PHP:  return [$a, $b];
来源：http://jac.sxryk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aok.birdmap.top

TS:   return { a, b };
来源：http://lii.zhongyouzk.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kap.yj20258.top

Go:   return a, b
来源：http://tpx.pengpengdd.cyou

Ruby: return a, b
来源：http://lsu.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://zuv.shangyingyoupin.top

[C06] 匿名函数 / lambda
来源：http://rle.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://ovm.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://thj.chenjidiqi.icu

JS:   const square = x => x * x;
来源：http://rty.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://izv.gaohongyu789.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://koo.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vli.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://fun.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rzq.uphjek.com

[C07] 把函数作为参数传入
来源：http://lxo.sufxvd.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uwf.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://qqe.cucudq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dgf.redwolf501.top

TS:   arr.map(String)
来源：http://bts.c1oappe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://thn.hfpthk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vhe.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://jgw.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fxc.zhijiandao.cn

[C08] 闭包
来源：http://ctj.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tiq.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xkz.yj20258.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pic.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hgh.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ncx.havefunace.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mhy.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://luc.zhixingplan.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zbw.xuanzx.com

[C09] 递归
来源：http://swm.xingfuxueyuan.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gsj.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hms.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aka.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wgd.dashuyun.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lvw.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eti.shanyushiyangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://srz.zhixingplan.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aoa.snrcjt.cn

[C10] 变量作用域
来源：http://ovr.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rwo.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zxe.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dal.daria6918.cn

TS:   同 JS
来源：http://tmm.jinqigufen.top

Java: 方法内为块级作用域
来源：http://lpc.quarkkingdee.top

Go:   花括号块级作用域
来源：http://uwt.ywan-chungtsiang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://txl.zhixingplan.top


<!-- 参考信息 -->