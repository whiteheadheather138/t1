代发 wailian999

Ruby: a, b = b, a
来源：http://qli.yfazqb.com

C#:   (a, b) = (b, a);
来源：http://rjr.nanxinkj.top

[A20] 读取标准输入
来源：http://xkb.yvedp.cn

Py:   name = input("请输入：")
来源：http://dox.nanxinkj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://stk.jqgufenzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oab.hammf.cn

TS:   // Node.js：readline 模块
来源：http://jvu.mhx1999.top

Java: new Scanner(System.in).nextLine()
来源：http://qvy.52xcode.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vis.svipenyu.cn

Ruby: gets.chomp
来源：http://hyb.zhengqikj.top

C#:   Console.ReadLine();
来源：http://pbu.yongpay.top

[A21] 保留指定小数位输出
来源：http://lsw.iojbl.cn

Py:   f"{3.14159:.2f}"
来源：http://eny.0kj1m.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://axf.ywan-chungtsiang.top

JS:   (3.14159).toFixed(2)
来源：http://qrm.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://ufg.jianghu66.top

Java: String.format("%.2f", 3.14159)
来源：http://ego.daria6918.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hwu.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://tic.gogol.net.cn

C#:   3.14159.ToString("F2")
来源：http://drg.guowangkeji.top

[A22] 获取字符串长度
来源：http://ddg.kuanghao11.cn

Py:   len(s)
来源：http://dxe.yfazqb.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hug.jinqigufen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://arb.quarkkingdee.top

TS:   s.length
来源：http://zrn.cheryme.top

Java: s.length()
来源：http://lzm.hysaishi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ngb.gotoacloud.top

Ruby: s.length
来源：http://emf.dashuyun.cn

C#:   s.Length
来源：http://lab.guowangkeji.top

[A23] 大小写转换
来源：http://wje.cheryme.top

Py:   s.upper(); s.lower(); s.title()
来源：http://deh.daxiang520.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yku.nwbrower.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ocs.hywenlv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://npc.zhaomingkeji.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eka.gaohongyu789.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bfd.birdmap.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zos.jiagoushi.top

C#:   s.ToUpper(); s.ToLower()
来源：http://fxl.vqdsnc.cn

[A24] 去除首尾空白
来源：http://lch.sysykeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xyt.guannengcc.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qua.sufxvd.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mhj.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cny.cdnleiting.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lel.jlsjyb.cn

Go:   strings.TrimSpace(s)
来源：http://kjr.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kgw.fengsongda.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hnx.jyoumei.cn

[A25] 字符串比较
来源：http://dzh.yonumen.top

Py:   s1 == s2; s1 != s2
来源：http://akz.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vsc.pengpengdd.cyou

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vmd.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pjp.yuxming.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lpw.hnxiangtu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ong.uphjek.com

Ruby: s1 == s2; s1 <=> s2
来源：http://zxj.hnxiangtu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zpx.pycfn.com

[A26] 类型转换总览
来源：http://anp.gzhubu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xlk.fehbvm.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zte.tianlin.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uhu.cashguo.top

TS:   Number() String() Boolean() x as number
来源：http://icp.fanxiaobao.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rwh.hcnkem.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qyi.nanxinkj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://yqh.daxiang520.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ovj.sjlbkw.cn

================================================================================
来源：http://vvw.zhijiandao.cn

B. 流程控制
来源：http://evr.zdbjq.cn

================================================================================
来源：http://tcz.ivvv.top

[B01] 条件判断 if / else
来源：http://qnp.zdbjq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oil.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dpm.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bqi.gzhubu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mdi.gzhubu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fsd.52xcode.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xbp.redwolf501.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rty.shzxlz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ajf.ctjpmb.com

[B02] 多分支 else if / elif
来源：http://hkn.yvedp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ojy.yj20258.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ult.jqgfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mjv.52xcode.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ecg.nwbrower.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vcp.xziqi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bwc.nanxinkj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mmr.shzxlz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oaf.wangdashe.top

[B03] switch / match / case
来源：http://hll.0kj1m.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://omb.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ept.ybcxt.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bdw.tarul.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ymv.iojbl.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pkr.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fjl.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tvk.aizwys.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lkj.pengpengdd.cyou

[B04] for 计数循环
来源：http://rci.sjlbkw.cn

Py:   for i in range(10): print(i)
来源：http://grr.ehwqpu.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bse.chenzaomai.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sqc.xuetiantiany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://irv.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://suz.jyoumei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eyz.sjlbkw.cn

Ruby: 10.times { |i| puts i }
来源：http://iox.hfpthk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lfq.tian-w.cn

[B05] 遍历数组 / 列表
来源：http://nec.c1oappe.top

Py:   for item in arr: print(item)
来源：http://amg.zhijiandao.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://emy.52xcode.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nyf.xuanzx.com

TS:   for (const item of arr) { console.log(item); }
来源：http://iaw.gogol.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wpm.cucudq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kkw.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://paf.fengsongda.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://amy.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://boz.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://xuk.jinyuanbaomall.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bgn.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pna.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zds.snrcjt.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lqf.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qxj.jqgufenzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nrr.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fke.52xcode.cn

[B07] while 循环
来源：http://sdj.tanke756.top

Py:   while i < 10: i += 1
来源：http://jgm.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://mam.aibaodan.cn

JS:   while (i < 10) { i++; }
来源：http://tix.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://kus.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://bwb.tianlin.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pjq.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://vxr.tarul.cn

C#:   while (i < 10) { i++; }
来源：http://liu.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://hcl.cqqwz.cn

Py:   # 无 do-while：用 while True + break
来源：http://tpl.yfazqb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://acw.chenlongwang.top

JS:   do { i++; } while (i < 10);
来源：http://rms.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://bcy.wangshuangyany.cn

Java: do { i++; } while (i < 10);
来源：http://jfy.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://obm.ehwqpu.com

Ruby: begin; i += 1; end while i < 10
来源：http://rqw.zhengqikj.top

C#:   do { i++; } while (i < 10);
来源：http://nbt.yfazqb.com

[B09] break 与 continue
来源：http://xxe.aizwys.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aho.pengpengdd.cyou

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ulq.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qkf.snrcjt.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tsc.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dlk.havefunace.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hen.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ihs.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bxb.tanke756.top

[B10] 遍历同时拿索引
来源：http://ppu.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nwx.tianlin.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xgi.fktsv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jpx.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vqk.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nam.nanxinkj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://upi.meibo888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gey.jinqigfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://peo.zhengqikj.top

[B11] 生成数字序列 / 区间
来源：http://iya.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://ylr.yuanzhike.top

PHP:  range(0, 10, 2);
来源：http://xon.nanxinkj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gxy.xziqi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lxm.fanxiaobao.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bve.nanxuanxn.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mxp.shangyingyoupin.top

Ruby: (0...10).step(2).to_a
来源：http://gqe.shuidangran.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cag.zdbjq.cn

[B12] 跳出多层循环
来源：http://bfs.meibo888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://sjg.sufxvd.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lcv.jyoumei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ctl.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kji.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vze.zdqjudy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fhq.fehbvm.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qzh.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://osp.yanxiufei.cn

[B13] 判断是否为数字
来源：http://rbl.gotoacloud.top

Py:   isinstance(x, (int, float))
来源：http://oed.ivvv.top

PHP:  is_numeric($x)
来源：http://ove.zhijiandao.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rgx.ppjwa.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gaf.yfazqb.com

Java: x instanceof Number
来源：http://siy.shuidangran.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jki.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://scv.havefunace.top

C#:   x is int or double or decimal
来源：http://ogd.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://xpi.jyoumei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zmw.smart0.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xmv.hnqzz.top

JS:   [1, 2, 3].includes(x)
来源：http://xpd.jyoumei.cn

TS:   [1, 2, 3].includes(x)
来源：http://lab.yuxming.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rlr.sweek.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dpf.jqgufenzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://plz.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://his.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://nzq.epnwcf.com

Py:   a and b or not c
来源：http://rzm.andypj.xyz

PHP:  $a && $b || !$c
来源：http://wcl.birdmap.top

JS:   a && b || !c
来源：http://neh.tianlin.xyz

TS:   a && b || !c
来源：http://uvo.cucudq.cn

Java: a && b || !c
来源：http://uya.uphjek.com

Go:   a && b || !c
来源：http://kde.quarkkingdee.top

Ruby: a && b || !c
来源：http://mto.pycfn.com

C#:   a && b || !c
来源：http://wrx.9152youxi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xyl.vqdsnc.cn

Py:   if not data: return
来源：http://rfc.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://dxs.jiagoushi.top

JS:   if (!data) return;
来源：http://hyc.tanke756.top

TS:   if (!data) return;
来源：http://hhg.ppjwa.cn

Java: if (data == null) return;
来源：http://xyz.yueranfly.top

Go:   if data == nil { return }
来源：http://pcx.gogol.net.cn

Ruby: return if data.nil?
来源：http://chk.cqqwz.cn

C#:   if (data == null) return;
来源：http://cna.0kj1m.cn

================================================================================
来源：http://fad.tarul.cn

C. 函数与作用域
来源：http://isu.zycfv.cn

================================================================================
来源：http://rpo.chenjidiqi.icu

[C01] 定义函数
来源：http://opb.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://kuz.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pte.chenlongwang.top

JS:   function add(a, b) { return a + b; }
来源：http://ccp.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lcj.fzhhl.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kao.kuanghao11.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zrw.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://ewc.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qqq.tanke756.top

[C02] 默认参数
来源：http://ngi.shanyushiyangtech.top

Py:   def greet(name="World"): return name
来源：http://ula.svipenyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tzf.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://jaj.tanke756.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hrg.cdnleiting.top

Java: // 无默认参数：方法重载或 Optional
来源：http://yux.ppjwa.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tzg.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://mnq.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://ghe.xuanzx.com

[C03] 可变参数
来源：http://uzl.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://xjs.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oya.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yqz.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vbn.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jwp.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jox.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://yfw.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://swn.fengsongda.top

[C04] 命名参数 / 关键字参数
来源：http://uzk.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dic.zdbjq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wrb.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ukt.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://srx.zhongyouzk.top

Java: // 无：用 Builder 模式或 record
来源：http://tee.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://kdt.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://tos.zhiwuduotai.top

C#:   f(a: 1, b: 2)
来源：http://pfx.tarul.cn

[C05] 返回多个值
来源：http://gzu.wangdashe.top

Py:   return a, b
来源：http://dum.iojbl.cn

PHP:  return [$a, $b];
来源：http://cgr.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tdu.xuetiantiany.cn

TS:   return { a, b };
来源：http://ccp.cdnleiting.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cuq.jinqigfzy.top

Go:   return a, b
来源：http://hwt.wangshuangyany.cn

Ruby: return a, b
来源：http://tvi.hnxiangtu.top

C#:   return (a, b);              // ValueTuple
来源：http://bmn.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://zql.sxryk.cn

Py:   square = lambda x: x * x
来源：http://wxx.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cww.fengsongda.top

JS:   const square = x => x * x;
来源：http://itj.cheryme.top

TS:   const square = (x: number): number => x * x;
来源：http://ztx.ivvv.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://owm.zhaomingkeji.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://gsf.birdmap.top

Ruby: square = ->(x) { x * x }
来源：http://ogc.xziqi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kjx.fktsv.cn

[C07] 把函数作为参数传入
来源：http://zuf.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://roj.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ejt.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xid.sweek.top

TS:   arr.map(String)
来源：http://qbx.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vpc.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qba.sweek.top

Ruby: arr.map(&:upcase)
来源：http://uht.shangyingyoupin.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qed.tianlin.xyz

[C08] 闭包
来源：http://vyo.nanxuanxn.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ttk.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gqn.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lgh.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fsf.tian-w.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://icy.andypj.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bgd.nanxuanxn.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dlm.hnxiangtu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hgd.hesvh.cn

[C09] 递归
来源：http://kww.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qrc.zdqjudy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oxi.316326.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hdi.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xwb.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nps.ehwqpu.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pcs.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://swb.xuetiantiany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zef.zycfv.cn

[C10] 变量作用域
来源：http://bte.tianlin.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fcq.ivvv.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wgc.zhongyouzk.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eqk.hcnkem.com


<!-- 参考信息 -->