代发 wailian999

JS:   [a, b] = [b, a];
来源：http://djj.chenlongwang.top

TS:   [a, b] = [b, a];
来源：http://rrt.sufxvd.cn

Java: int t = a; a = b; b = t;
来源：http://olm.guannengcc.top

Go:   a, b = b, a
来源：http://clt.nanxuanxn.top

Ruby: a, b = b, a
来源：http://xvw.snrcjt.cn

C#:   (a, b) = (b, a);
来源：http://ykd.yfazqb.com

[A20] 读取标准输入
来源：http://qjg.zycfv.cn

Py:   name = input("请输入：")
来源：http://fvv.yuxming.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://avd.ydjk.org.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qnv.jinyuanbaomall.cn

TS:   // Node.js：readline 模块
来源：http://gdn.fzhhl.top

Java: new Scanner(System.in).nextLine()
来源：http://wuy.cdnleiting.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ltv.sxryk.cn

Ruby: gets.chomp
来源：http://zus.gzhubu.top

C#:   Console.ReadLine();
来源：http://sdh.jlsjyb.cn

[A21] 保留指定小数位输出
来源：http://qhc.hcnkem.com

Py:   f"{3.14159:.2f}"
来源：http://hab.yj20258888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pjl.hongshengwenyu.top

JS:   (3.14159).toFixed(2)
来源：http://pot.yangfankeji.com

TS:   (3.14159).toFixed(2)
来源：http://jpp.zhijiandao.cn

Java: String.format("%.2f", 3.14159)
来源：http://anc.ehwqpu.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://axn.hesvh.cn

Ruby: format("%.2f", 3.14159)
来源：http://hms.xuanzx.com

C#:   3.14159.ToString("F2")
来源：http://rmz.yj20258.top

[A22] 获取字符串长度
来源：http://voy.vqdsnc.cn

Py:   len(s)
来源：http://efd.hesvh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fmh.hywenlv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://axa.hnxiangtu.top

TS:   s.length
来源：http://cjq.cucudq.cn

Java: s.length()
来源：http://anj.jinyuanbaomall.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://poi.sysykeji.top

Ruby: s.length
来源：http://fiz.quarkkingdee.top

C#:   s.Length
来源：http://pwe.0kj1m.cn

[A23] 大小写转换
来源：http://hkk.zhongyouzk.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ejw.jinghuilouyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xwc.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xhd.zycfv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zgr.zhiwuduotai.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nkj.gotoacloud.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jzw.ppjwa.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mau.zhaomingkeji.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://sax.cucudq.cn

[A24] 去除首尾空白
来源：http://lxv.pengpengdd.cyou

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tbu.birdmap.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pjq.jyoumei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hgs.wangdashe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pjr.dianchejie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yil.hysaishi.cn

Go:   strings.TrimSpace(s)
来源：http://zhw.havefunace.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dvq.52xcode.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qwo.svipenyu.cn

[A25] 字符串比较
来源：http://jsq.sweek.top

Py:   s1 == s2; s1 != s2
来源：http://lts.hnqzz.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qfb.aibaodan.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hwr.svipenyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pev.feifeiyinyue.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dew.52xcode.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gzo.birdmap.top

Ruby: s1 == s2; s1 <=> s2
来源：http://grp.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hdn.yueranfly.top

[A26] 类型转换总览
来源：http://eqh.jinqigufen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fsu.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ych.dianchejie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://idj.cashguo.top

TS:   Number() String() Boolean() x as number
来源：http://kif.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jnu.jlsjyb.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tcw.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zer.iojbl.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nja.haohaochexian.top

================================================================================
来源：http://gwz.shzxlz.cn

B. 流程控制
来源：http://fgc.yongpay.top

================================================================================
来源：http://tzf.ppjwa.cn

[B01] 条件判断 if / else
来源：http://cla.tianlin.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://ocr.ywan-chungtsiang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vss.xinyue.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mlj.yonumen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qai.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jlk.chenlongwang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uqy.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mpp.52xcode.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gtk.cdnleiting.top

[B02] 多分支 else if / elif
来源：http://mwg.jqgfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xwu.ydzc1.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ymc.svipenyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gvk.yongpay.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lnf.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jmc.ivvv.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yra.epnwcf.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zic.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jqf.hnxiangtu.top

[B03] switch / match / case
来源：http://scj.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://biu.yfazqb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qwi.nanxuanxn.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fjx.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ptz.dashuyun.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qko.shzxlz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qyw.ppjwa.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://igz.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://awi.shanyushiyangtech.top

[B04] for 计数循环
来源：http://qwc.jinyuanbaomall.cn

Py:   for i in range(10): print(i)
来源：http://jzv.hfpthk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://euc.jqgufenzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oay.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qcm.yongpay.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mni.fengsongda.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bdh.hysaishi.cn

Ruby: 10.times { |i| puts i }
来源：http://ass.jlsjyb.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://voa.fanxiaobao.xyz

[B05] 遍历数组 / 列表
来源：http://ggr.birdmap.top

Py:   for item in arr: print(item)
来源：http://kyc.chenjidiqi.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wdt.yuxming.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nqj.yuanzhike.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mmi.guannengcc.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qvz.zhijiandao.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cfx.tianlin.xyz

Ruby: arr.each { |item| puts item }
来源：http://sxa.nwbrower.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fcw.shuidangran.top

[B06] 遍历字典 / 对象
来源：http://yoo.ctjpmb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://amj.jinyuanbaomall.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jis.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://asm.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dxd.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tuv.feifeiyinyue.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dhp.zhiwuduotai.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://imd.jiagoushi.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zvd.zhaomingkeji.xyz

[B07] while 循环
来源：http://opq.aizwys.cn

Py:   while i < 10: i += 1
来源：http://ghf.sysykeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://maa.chenzaomai.com

JS:   while (i < 10) { i++; }
来源：http://tei.316326.xyz

TS:   while (i < 10) { i++; }
来源：http://gnb.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://kyr.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uyw.fengsongda.top

Ruby: while i < 10; i += 1; end
来源：http://oet.cqqwz.cn

C#:   while (i < 10) { i++; }
来源：http://fke.sjlbkw.cn

[B08] do-while（至少执行一次）
来源：http://rje.zhijiandao.cn

Py:   # 无 do-while：用 while True + break
来源：http://rfb.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wve.gogol.net.cn

JS:   do { i++; } while (i < 10);
来源：http://dhq.jlsjyb.cn

TS:   do { i++; } while (i < 10);
来源：http://cmv.vqdsnc.cn

Java: do { i++; } while (i < 10);
来源：http://ktw.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hxm.hnxiangtu.top

Ruby: begin; i += 1; end while i < 10
来源：http://blp.quarkkingdee.top

C#:   do { i++; } while (i < 10);
来源：http://tgs.yvedp.cn

[B09] break 与 continue
来源：http://pmf.zhijiandao.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xxf.xinyue.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zho.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://skt.haohaochexian.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://coh.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uqq.316326.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ygi.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://trn.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bqd.xuanzx.com

[B10] 遍历同时拿索引
来源：http://zgk.iojbl.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lpl.fktsv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lww.sufxvd.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ihc.hnxiangtu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://paf.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rzy.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tak.hcnkem.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zpe.yuanzhike.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rlj.feifeiyinyue.top

[B11] 生成数字序列 / 区间
来源：http://wsq.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://vfo.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://vzb.andypj.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://knx.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zkz.gotoacloud.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jum.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://flv.gzhubu.top

Ruby: (0...10).step(2).to_a
来源：http://utu.jlsjyb.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bgb.dashuyun.cn

[B12] 跳出多层循环
来源：http://hfw.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pxo.sufxvd.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gxp.yonumen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ayp.tianlin.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qbs.pengpengdd.cyou

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xei.cdnleiting.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iww.gotoacloud.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wue.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zeu.uphjek.com

[B13] 判断是否为数字
来源：http://wcs.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://okz.sweek.top

PHP:  is_numeric($x)
来源：http://yjc.hfpthk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ujg.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zlp.zdbjq.cn

Java: x instanceof Number
来源：http://cxz.cashguo.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vpk.sjlbkw.cn

Ruby: x.is_a?(Numeric)
来源：http://mqa.fzhhl.top

C#:   x is int or double or decimal
来源：http://fmj.cqqwz.cn

[B14] 判断值是否在集合内
来源：http://yto.chenlongwang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zpz.quarkkingdee.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ecr.dianchejie.cn

JS:   [1, 2, 3].includes(x)
来源：http://vud.aibaodan.cn

TS:   [1, 2, 3].includes(x)
来源：http://mfl.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wie.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yoq.wangshuangyany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ynb.tianlin.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uuw.fengsongda.top

[B15] 布尔运算与取反
来源：http://ltz.xylfe.cn

Py:   a and b or not c
来源：http://sss.hammf.cn

PHP:  $a && $b || !$c
来源：http://mgo.zhongyouzk.top

JS:   a && b || !c
来源：http://wdt.gzhubu.top

TS:   a && b || !c
来源：http://ghc.jinqigufen.top

Java: a && b || !c
来源：http://gnv.dianchejie.cn

Go:   a && b || !c
来源：http://rcq.haohaochexian.top

Ruby: a && b || !c
来源：http://chx.aizwys.cn

C#:   a && b || !c
来源：http://rvs.vehdjk.com

[B16] 卫语句：不满足条件提前返回
来源：http://gva.jqgfzy.top

Py:   if not data: return
来源：http://vhi.wangdashe.top

PHP:  if (!$data) { return; }
来源：http://ytz.fzhhl.top

JS:   if (!data) return;
来源：http://xpa.zdbjq.cn

TS:   if (!data) return;
来源：http://yxs.kuanghao11.cn

Java: if (data == null) return;
来源：http://efk.tanke756.top

Go:   if data == nil { return }
来源：http://ygj.fengsongda.top

Ruby: return if data.nil?
来源：http://xva.cashguo.top

C#:   if (data == null) return;
来源：http://dqx.daxiang520.top

================================================================================
来源：http://xtw.hnqzz.top

C. 函数与作用域
来源：http://qok.sjlbkw.cn

================================================================================
来源：http://qsf.gogol.net.cn

[C01] 定义函数
来源：http://jhz.tianlin.xyz

Py:   def add(a, b): return a + b
来源：http://lrc.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ngi.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://mju.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jaz.snrcjt.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pba.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://nde.zdqjudy.top

Ruby: def add(a, b); a + b; end
来源：http://lao.snrcjt.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vln.yvedp.cn

[C02] 默认参数
来源：http://zig.zhongyouzk.top

Py:   def greet(name="World"): return name
来源：http://cfa.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vjs.snrcjt.cn

JS:   function greet(name = "World") { return name; }
来源：http://edx.9152youxi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://iuw.jinqigfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fjs.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pxk.cdnleiting.top

Ruby: def greet(name = "World") = name
来源：http://hnx.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://tfp.zdqjudy.top

[C03] 可变参数
来源：http://kft.gotoacloud.top

Py:   def total(*args): return sum(args)
来源：http://rdi.zhengqikj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tph.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mzw.chenlongwang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://awt.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rjm.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://giu.gaohongyu789.top

Ruby: def total(*nums); nums.sum; end
来源：http://pfe.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hpm.hammf.cn

[C04] 命名参数 / 关键字参数
来源：http://voc.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://alb.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nvx.redwolf501.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://feb.zdbjq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://btd.bbcook.cn

Java: // 无：用 Builder 模式或 record
来源：http://hsl.zhiwuduotai.top

Go:   // 无：用配置结构体参数
来源：http://tmh.ctjpmb.com

Ruby: f(a: 1, b: 2)
来源：http://err.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://pad.ehwqpu.com

[C05] 返回多个值
来源：http://ybv.jinyuanbaomall.cn

Py:   return a, b
来源：http://qpd.daria6918.cn

PHP:  return [$a, $b];
来源：http://ubu.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kbq.xziqi.cn

TS:   return { a, b };
来源：http://hsl.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jex.svipenyu.cn

Go:   return a, b
来源：http://ajm.mhx1999.top

Ruby: return a, b
来源：http://hxf.sweek.top

C#:   return (a, b);              // ValueTuple
来源：http://xxt.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://jpk.daria6918.cn

Py:   square = lambda x: x * x
来源：http://ggj.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://gzp.ctjpmb.com

JS:   const square = x => x * x;
来源：http://tny.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://rxp.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mjo.shangyingyoupin.top

Go:   sq := func(x int) int { return x * x }
来源：http://buc.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://bop.sysykeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://imp.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://yij.zdqjudy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://txh.316326.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://wwl.daria6918.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://grk.zdqjudy.top

TS:   arr.map(String)
来源：http://lmk.yuanzhike.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ach.nanxinkj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://izx.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://qki.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gri.xuanzx.com

[C08] 闭包
来源：http://gji.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://trz.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ngm.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tgd.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cmz.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sqm.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bgm.yongpay.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ybt.hammf.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qww.yvedp.cn

[C09] 递归
来源：http://qln.guowangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dpw.bbcook.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xum.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://omt.shuidangran.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uki.hnxiangtu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://swo.zycfv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zap.sxryk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rjc.dashuyun.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dys.jiagoushi.top


<!-- 参考信息 -->