代发 wailian999

Ruby: a, b = b, a
来源：http://zom.ybcxt.top

C#:   (a, b) = (b, a);
来源：http://htt.vehdjk.com

[A20] 读取标准输入
来源：http://aey.gotoacloud.top

Py:   name = input("请输入：")
来源：http://jox.meibo888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qbi.jqgufenzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vvo.shanyushiyangkeji.top

TS:   // Node.js：readline 模块
来源：http://eaq.jianghu66.top

Java: new Scanner(System.in).nextLine()
来源：http://pcb.shanyushiyangtech.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://abt.snrcjt.cn

Ruby: gets.chomp
来源：http://gqk.shanyushiyangkeji.top

C#:   Console.ReadLine();
来源：http://ftu.daxiang520.top

[A21] 保留指定小数位输出
来源：http://mpo.fanxiaobao.xyz

Py:   f"{3.14159:.2f}"
来源：http://agg.9152youxi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pez.ehwqpu.com

JS:   (3.14159).toFixed(2)
来源：http://vao.jianghu66.top

TS:   (3.14159).toFixed(2)
来源：http://lan.dianchejie.cn

Java: String.format("%.2f", 3.14159)
来源：http://rkh.cucudq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qoe.jqgufenzy.top

Ruby: format("%.2f", 3.14159)
来源：http://spr.hcnkem.com

C#:   3.14159.ToString("F2")
来源：http://nzh.pycfn.com

[A22] 获取字符串长度
来源：http://pqx.tarul.cn

Py:   len(s)
来源：http://rft.sufxvd.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fkp.jiagoushi.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://raa.zhijiandao.cn

TS:   s.length
来源：http://ytt.jqgufenzy.top

Java: s.length()
来源：http://uqt.hnqzz.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vtc.jyoumei.cn

Ruby: s.length
来源：http://vfg.jinyuanbaomall.cn

C#:   s.Length
来源：http://gyj.cashguo.top

[A23] 大小写转换
来源：http://uhd.jyoumei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gbu.chenzaomai.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qcd.epnwcf.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xon.yueranfly.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://igj.vqdsnc.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jmt.ywan-chungtsiang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tpt.ehwqpu.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hdq.jqgufenzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://goc.jianghu66.top

[A24] 去除首尾空白
来源：http://rix.havefunace.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mgk.yj202588.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xkk.nanxuanxn.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xyv.cqqwz.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wcg.jianghu66.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ffa.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://qhn.c1oappe.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wet.aibaodan.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uwf.yj20258888.top

[A25] 字符串比较
来源：http://lif.xylfe.cn

Py:   s1 == s2; s1 != s2
来源：http://jgu.smart0.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ews.yuxming.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kov.feifeiyinyue.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aom.hysaishi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xxh.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xwu.sweek.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fcc.jqgufenzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wqg.zhaomingkeji.xyz

[A26] 类型转换总览
来源：http://qgm.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://npm.tianlin.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jth.cheryme.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sfb.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://olq.sysykeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nya.jqgfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://erc.jianghu66.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ifo.sjlbkw.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cwl.cashguo.top

================================================================================
来源：http://wxr.gotoacloud.top

B. 流程控制
来源：http://fou.sufxvd.cn

================================================================================
来源：http://cvh.feifeiyinyue.top

[B01] 条件判断 if / else
来源：http://psj.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://gtx.redwolf501.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://anz.shanyushiyangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xgh.xziqi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://coe.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://hya.aibaodan.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cbp.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://das.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qlb.snrcjt.cn

[B02] 多分支 else if / elif
来源：http://lyj.smart0.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fww.daria6918.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pxd.shangyingyoupin.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://swv.52xcode.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aby.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hdr.yj20258888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mfh.nwbrower.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qgt.zhaomingkeji.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kpr.sysykeji.top

[B03] switch / match / case
来源：http://pxt.tanke756.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fzc.yj202588.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xxg.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lhd.ivvv.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xzm.ivvv.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xpn.pycfn.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dje.jqgfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sih.wangshuangyany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://azb.zhongyouzk.top

[B04] for 计数循环
来源：http://rxu.tian-w.cn

Py:   for i in range(10): print(i)
来源：http://esl.ctjpmb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zpj.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jvs.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nwp.jlsjyb.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sgn.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bky.gotoacloud.top

Ruby: 10.times { |i| puts i }
来源：http://aai.xinyue.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cez.havefunace.top

[B05] 遍历数组 / 列表
来源：http://mvb.iojbl.cn

Py:   for item in arr: print(item)
来源：http://dvv.jqgufenzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gxi.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pdy.jiagoushi.top

TS:   for (const item of arr) { console.log(item); }
来源：http://scz.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rji.yueranfly.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ekp.gaohongyu789.top

Ruby: arr.each { |item| puts item }
来源：http://vki.iojbl.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baq.birdmap.top

[B06] 遍历字典 / 对象
来源：http://tyf.hfpthk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rol.sjlbkw.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fig.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://opb.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kmn.yuanzhike.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xyi.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ria.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zow.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pmd.epnwcf.com

[B07] while 循环
来源：http://jlk.zhiwuduotai.top

Py:   while i < 10: i += 1
来源：http://bdo.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://feq.jqgfzy.top

JS:   while (i < 10) { i++; }
来源：http://ybd.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://sks.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://jqf.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jaz.snrcjt.cn

Ruby: while i < 10; i += 1; end
来源：http://irj.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://lyz.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://gcl.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://nvv.yongpay.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yjv.chenlongwang.top

JS:   do { i++; } while (i < 10);
来源：http://gqc.xingfuxueyuan.xyz

TS:   do { i++; } while (i < 10);
来源：http://gic.hongshengwenyu.top

Java: do { i++; } while (i < 10);
来源：http://lkv.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rlf.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://sef.pycfn.com

C#:   do { i++; } while (i < 10);
来源：http://ygq.gogol.net.cn

[B09] break 与 continue
来源：http://vty.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ufh.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ckc.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://atv.ywan-chungtsiang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ppu.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bip.ppjwa.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cjg.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://etb.snrcjt.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qju.meibo888.top

[B10] 遍历同时拿索引
来源：http://ofc.yj202588.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ocb.nwbrower.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uel.guannengcc.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ffz.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yyr.cheryme.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wzt.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hkf.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eko.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rio.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://ahf.yfazqb.com

Py:   list(range(0, 10, 2))
来源：http://xzj.bjfxy.top

PHP:  range(0, 10, 2);
来源：http://mbj.fktsv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ett.wangshuangyany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yuz.nwbrower.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ivv.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cwk.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://oth.xinyue.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dll.zhoulong.xyz

[B12] 跳出多层循环
来源：http://rgf.zhiwuduotai.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vqj.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hyj.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cyg.cdnleiting.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mel.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jzo.yonumen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fmj.sufxvd.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uxt.yuxming.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vfa.9152youxi.cn

[B13] 判断是否为数字
来源：http://zun.andypj.xyz

Py:   isinstance(x, (int, float))
来源：http://qkt.c1oappe.top

PHP:  is_numeric($x)
来源：http://bnw.zhengqikj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qot.gogol.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lol.cashguo.top

Java: x instanceof Number
来源：http://wed.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fww.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://hdk.gzhubu.top

C#:   x is int or double or decimal
来源：http://oef.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://dyx.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wmn.jinqigfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kor.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://iqv.xziqi.cn

TS:   [1, 2, 3].includes(x)
来源：http://fxs.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://xqh.aibaodan.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ffz.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yne.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://odu.hysaishi.cn

[B15] 布尔运算与取反
来源：http://lvw.xuanzx.com

Py:   a and b or not c
来源：http://qvm.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://vvr.hongshengwenyu.top

JS:   a && b || !c
来源：http://ail.pengpengdd.cyou

TS:   a && b || !c
来源：http://qkv.jinqigfzy.top

Java: a && b || !c
来源：http://sxl.zhijiandao.cn

Go:   a && b || !c
来源：http://clf.fehbvm.com

Ruby: a && b || !c
来源：http://xhi.cheryme.top

C#:   a && b || !c
来源：http://ajj.jqgufenzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://ilh.shuidangran.top

Py:   if not data: return
来源：http://meg.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://vdz.aizwys.cn

JS:   if (!data) return;
来源：http://aoj.316326.xyz

TS:   if (!data) return;
来源：http://gpk.smart0.xyz

Java: if (data == null) return;
来源：http://scs.tarul.cn

Go:   if data == nil { return }
来源：http://ksv.gaohongyu789.top

Ruby: return if data.nil?
来源：http://fvf.daria6918.cn

C#:   if (data == null) return;
来源：http://sof.hywenlv.cn

================================================================================
来源：http://ldm.cheryme.top

C. 函数与作用域
来源：http://mcx.cqqwz.cn

================================================================================
来源：http://wnv.epnwcf.com

[C01] 定义函数
来源：http://qyb.fengsongda.top

Py:   def add(a, b): return a + b
来源：http://ejf.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xax.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://hmu.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jxc.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gjs.zhengqikj.top

Go:   func add(a, b int) int { return a + b }
来源：http://wdh.fehbvm.com

Ruby: def add(a, b); a + b; end
来源：http://tcq.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://whn.jinqigufen.top

[C02] 默认参数
来源：http://rnf.zhixingplan.top

Py:   def greet(name="World"): return name
来源：http://foo.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://shn.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://wjr.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tbs.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ijl.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nbq.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://jzx.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://iuj.daria6918.cn

[C03] 可变参数
来源：http://dff.xinyue.icu

Py:   def total(*args): return sum(args)
来源：http://nyp.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eji.shzxlz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zhd.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yra.ctjpmb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mdk.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yle.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://eyy.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://emg.hfpthk.cn

[C04] 命名参数 / 关键字参数
来源：http://ylt.bjfxy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fem.meibo888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wtw.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qso.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wok.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://wun.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://mod.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://kwl.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://jvq.xuetiantiany.cn

[C05] 返回多个值
来源：http://kao.nwbrower.top

Py:   return a, b
来源：http://wex.ppjwa.cn

PHP:  return [$a, $b];
来源：http://evk.pengpengdd.cyou

JS:   return [a, b];             // 或 return { a, b };
来源：http://mdb.pengpengdd.cyou

TS:   return { a, b };
来源：http://pfy.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pss.gotoacloud.top

Go:   return a, b
来源：http://waa.yonumen.top

Ruby: return a, b
来源：http://yhq.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://lwm.fktsv.cn

[C06] 匿名函数 / lambda
来源：http://eay.meibo888.top

Py:   square = lambda x: x * x
来源：http://pry.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yri.tarul.cn

JS:   const square = x => x * x;
来源：http://dkx.nanxinkj.top

TS:   const square = (x: number): number => x * x;
来源：http://had.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://neb.shanyushiyangtech.top

Go:   sq := func(x int) int { return x * x }
来源：http://cdz.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://smx.aibaodan.cn

C#:   Func<int, int> square = x => x * x;
来源：http://imq.dashuyun.cn

[C07] 把函数作为参数传入
来源：http://uor.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dnq.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vts.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ewn.c1oappe.top

TS:   arr.map(String)
来源：http://rkw.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uvk.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://etk.yvedp.cn

Ruby: arr.map(&:upcase)
来源：http://fyj.tarul.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fey.zhongyouzk.top

[C08] 闭包
来源：http://rpq.hesvh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lla.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wfz.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mqn.cucudq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dwx.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dwa.gaohongyu789.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rna.guowangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jrt.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dzq.kuanghao11.cn

[C09] 递归
来源：http://upd.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ngz.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zjw.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xxe.quarkkingdee.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://awg.shuidangran.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mca.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tcc.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gkb.shanyushiyangtech.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vhx.sufxvd.cn

[C10] 变量作用域
来源：http://ajd.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wzv.hywenlv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xmh.haohaochexian.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vhd.vehdjk.com


<!-- 参考信息 -->