代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vrh.vehdjk.com

Java: (int) 'A'; (char) 65
来源：http://qrj.shanyushiyangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gwb.hesvh.cn

Ruby: "A".ord; 65.chr
来源：http://zjm.shanyushiyangkeji.top

C#:   (int)'A'; (char)65
来源：http://wzx.epnwcf.com

[A19] 交换两个变量
来源：http://zdy.wangshuangyany.cn

Py:   a, b = b, a
来源：http://ewu.zdbjq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sxq.birdmap.top

JS:   [a, b] = [b, a];
来源：http://dbp.ywan-chungtsiang.top

TS:   [a, b] = [b, a];
来源：http://vhp.tian-w.cn

Java: int t = a; a = b; b = t;
来源：http://bpg.cashguo.top

Go:   a, b = b, a
来源：http://rhk.ctjpmb.com

Ruby: a, b = b, a
来源：http://bll.cucudq.cn

C#:   (a, b) = (b, a);
来源：http://bcr.shanyushiyangkeji.top

[A20] 读取标准输入
来源：http://ver.jiagoushi.top

Py:   name = input("请输入：")
来源：http://ctl.birdmap.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ywc.jinqigufen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gkr.316326.xyz

TS:   // Node.js：readline 模块
来源：http://ims.jqgfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://wpw.meibo888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://npj.bjfxy.top

Ruby: gets.chomp
来源：http://nfu.hnxiangtu.top

C#:   Console.ReadLine();
来源：http://ryx.yuxming.cn

[A21] 保留指定小数位输出
来源：http://mvg.yj20258888.top

Py:   f"{3.14159:.2f}"
来源：http://nbx.dashuyun.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jkb.quarkkingdee.top

JS:   (3.14159).toFixed(2)
来源：http://omi.mhx1999.top

TS:   (3.14159).toFixed(2)
来源：http://hca.jinqigfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://sgh.tian-w.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yyh.birdmap.top

Ruby: format("%.2f", 3.14159)
来源：http://rey.ydjk.org.cn

C#:   3.14159.ToString("F2")
来源：http://lxj.jianghu66.top

[A22] 获取字符串长度
来源：http://kls.yj20258.top

Py:   len(s)
来源：http://pnh.ywan-chungtsiang.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nky.jqgufenzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vbd.xylfe.cn

TS:   s.length
来源：http://wyx.feifeiyinyue.top

Java: s.length()
来源：http://elw.vqdsnc.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hmr.ywan-chungtsiang.top

Ruby: s.length
来源：http://aau.yvedp.cn

C#:   s.Length
来源：http://tdp.ctjpmb.com

[A23] 大小写转换
来源：http://hds.wangshuangyany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vtv.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vzu.nanxinkj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kgi.ehwqpu.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lgi.shanyushiyangkeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gju.sysykeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://msg.hfpthk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ptj.fengsongda.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bgl.jlsjyb.cn

[A24] 去除首尾空白
来源：http://fwt.zhengqikj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://phi.mhx1999.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://srr.xuetiantiany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nho.fehbvm.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://amy.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dkm.jinghuilouyu.cn

Go:   strings.TrimSpace(s)
来源：http://yww.ehwqpu.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rvy.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://suv.hfpthk.cn

[A25] 字符串比较
来源：http://ohy.ydjk.org.cn

Py:   s1 == s2; s1 != s2
来源：http://llw.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://slw.yj20258.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kkm.cashguo.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pam.jqgfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ezq.jiagoushi.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rdu.nwbrower.top

Ruby: s1 == s2; s1 <=> s2
来源：http://eit.sweek.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://egr.tarul.cn

[A26] 类型转换总览
来源：http://guu.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bcd.vehdjk.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ige.52xcode.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fyp.zhoulong.xyz

TS:   Number() String() Boolean() x as number
来源：http://hbq.gotoacloud.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fjy.guowangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hiy.ehwqpu.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://mjx.havefunace.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qvc.ywan-chungtsiang.top

================================================================================
来源：http://smg.hammf.cn

B. 流程控制
来源：http://ctk.jqgfzy.top

================================================================================
来源：http://jmt.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://ngq.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ocx.hcnkem.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vwp.nwbrower.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://igc.meibo888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://usv.chenzaomai.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://peg.shzxlz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lym.yueranfly.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cma.wangdashe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xxw.tanke756.top

[B02] 多分支 else if / elif
来源：http://wks.hnxiangtu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zjt.yuxming.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uzf.ybcxt.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fio.havefunace.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jbo.hammf.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pov.cdnleiting.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fui.hongshengwenyu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rcw.iojbl.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ipo.52xcode.cn

[B03] switch / match / case
来源：http://nqr.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rux.bjfxy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iew.zhoulong.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fvg.jyoumei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fsn.jqgfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oui.zhixingplan.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://myp.dashuyun.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cch.guannengcc.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://grq.sxryk.cn

[B04] for 计数循环
来源：http://jty.jlsjyb.cn

Py:   for i in range(10): print(i)
来源：http://smt.mhx1999.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://beb.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qyv.sufxvd.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vjy.hcnkem.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qgs.zycfv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wnq.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://acr.daxiang520.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ogz.zdqjudy.top

[B05] 遍历数组 / 列表
来源：http://xfa.guannengcc.top

Py:   for item in arr: print(item)
来源：http://hzw.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dhs.ybcxt.top

JS:   for (const item of arr) { console.log(item); }
来源：http://klo.guowangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fue.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ehq.zhaomingkeji.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://laq.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://fhr.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jtn.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://lhl.kuanghao11.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eqj.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kkr.shuidangran.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jwq.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zxn.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://thv.iojbl.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aku.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kdm.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rlk.zhoulong.xyz

[B07] while 循环
来源：http://iia.daxiang520.top

Py:   while i < 10: i += 1
来源：http://zhj.havefunace.top

PHP:  while ($i < 10) { $i++; }
来源：http://glz.yueranfly.top

JS:   while (i < 10) { i++; }
来源：http://dmf.daxiang520.top

TS:   while (i < 10) { i++; }
来源：http://xmd.jyoumei.cn

Java: while (i < 10) { i++; }
来源：http://vne.ydzc1.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jdb.ppjwa.cn

Ruby: while i < 10; i += 1; end
来源：http://vgz.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://hvm.nanxinkj.top

[B08] do-while（至少执行一次）
来源：http://htd.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://fzb.xuetiantiany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tvw.fktsv.cn

JS:   do { i++; } while (i < 10);
来源：http://gfj.jinyuanbaomall.cn

TS:   do { i++; } while (i < 10);
来源：http://vmz.zhaomingkeji.xyz

Java: do { i++; } while (i < 10);
来源：http://lhh.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://unm.fehbvm.com

Ruby: begin; i += 1; end while i < 10
来源：http://tlm.hywenlv.cn

C#:   do { i++; } while (i < 10);
来源：http://rjg.9152youxi.cn

[B09] break 与 continue
来源：http://jyu.tianlin.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ley.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cay.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dju.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ocx.jqgufenzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ohq.bbcook.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rub.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zze.fehbvm.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wjb.hongshengwenyu.top

[B10] 遍历同时拿索引
来源：http://wcp.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://onm.guowangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://slb.sxryk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sqx.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bfn.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ksm.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://spx.ctjpmb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://edz.52xcode.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://usm.kuanghao11.cn

[B11] 生成数字序列 / 区间
来源：http://hgb.fktsv.cn

Py:   list(range(0, 10, 2))
来源：http://smo.ivvv.top

PHP:  range(0, 10, 2);
来源：http://eaj.yueranfly.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cjd.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://alj.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cwf.yfazqb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wot.ydzc1.top

Ruby: (0...10).step(2).to_a
来源：http://iol.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jfl.havefunace.top

[B12] 跳出多层循环
来源：http://ynu.zhaomingkeji.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://hzh.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://umj.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://knw.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tlm.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tek.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fiw.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fwi.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vcw.cheryme.top

[B13] 判断是否为数字
来源：http://ncb.sweek.top

Py:   isinstance(x, (int, float))
来源：http://xxp.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://awz.hongshengwenyu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wfq.xylfe.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pck.ehwqpu.com

Java: x instanceof Number
来源：http://khx.vehdjk.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kca.snrcjt.cn

Ruby: x.is_a?(Numeric)
来源：http://jgn.aibaodan.cn

C#:   x is int or double or decimal
来源：http://hlf.bjfxy.top

[B14] 判断值是否在集合内
来源：http://woo.fengsongda.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ahx.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jus.ppjwa.cn

JS:   [1, 2, 3].includes(x)
来源：http://bnd.yj20258.top

TS:   [1, 2, 3].includes(x)
来源：http://zwc.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lxj.cdnleiting.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jng.zdqjudy.top

Ruby: [1, 2, 3].include?(x)
来源：http://emn.cashguo.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bqn.sysykeji.top

[B15] 布尔运算与取反
来源：http://klh.fanxiaobao.xyz

Py:   a and b or not c
来源：http://lcp.c1oappe.top

PHP:  $a && $b || !$c
来源：http://nki.nanxuanxn.top

JS:   a && b || !c
来源：http://vwu.fehbvm.com

TS:   a && b || !c
来源：http://lef.snrcjt.cn

Java: a && b || !c
来源：http://hsr.zhiwuduotai.top

Go:   a && b || !c
来源：http://qbc.feifeiyinyue.top

Ruby: a && b || !c
来源：http://auh.ehwqpu.com

C#:   a && b || !c
来源：http://tbc.9152youxi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pbq.fanxiaobao.xyz

Py:   if not data: return
来源：http://hsg.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://ojq.yonumen.top

JS:   if (!data) return;
来源：http://orc.gzhubu.top

TS:   if (!data) return;
来源：http://rrr.shuidangran.top

Java: if (data == null) return;
来源：http://lwg.jqgufenzy.top

Go:   if data == nil { return }
来源：http://kzj.zycfv.cn

Ruby: return if data.nil?
来源：http://jqw.wangdashe.top

C#:   if (data == null) return;
来源：http://ikb.jlsjyb.cn

================================================================================
来源：http://bzx.zhaomingkeji.xyz

C. 函数与作用域
来源：http://rrh.ydzc1.top

================================================================================
来源：http://unc.feifeiyinyue.top

[C01] 定义函数
来源：http://urt.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://pcc.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wiv.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://won.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lax.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tgx.redwolf501.top

Go:   func add(a, b int) int { return a + b }
来源：http://nhr.pycfn.com

Ruby: def add(a, b); a + b; end
来源：http://por.cucudq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fcf.fanxiaobao.xyz

[C02] 默认参数
来源：http://cxq.ybcxt.top

Py:   def greet(name="World"): return name
来源：http://vku.yanxiufei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jyv.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://wbd.shanyushiyangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yzl.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bes.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kso.jlsjyb.cn

Ruby: def greet(name = "World") = name
来源：http://tld.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://ajz.yuanzhike.top

[C03] 可变参数
来源：http://poj.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://vay.fehbvm.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yly.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mkc.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://voa.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vac.fanxiaobao.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hve.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://nuc.chenjidiqi.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xnx.tian-w.cn

[C04] 命名参数 / 关键字参数
来源：http://pbn.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://liy.meibo888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gio.chenlongwang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mxg.shanyushiyangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dju.sufxvd.cn

Java: // 无：用 Builder 模式或 record
来源：http://wjg.xingfuxueyuan.xyz

Go:   // 无：用配置结构体参数
来源：http://mfa.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://ffx.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://tzy.dianchejie.cn

[C05] 返回多个值
来源：http://lrv.9152youxi.cn

Py:   return a, b
来源：http://bwz.316326.xyz

PHP:  return [$a, $b];
来源：http://hbj.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://krd.yj20258.top

TS:   return { a, b };
来源：http://jrc.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nch.ydzc1.top

Go:   return a, b
来源：http://zok.shzxlz.cn

Ruby: return a, b
来源：http://qqz.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://cps.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://kgx.aibaodan.cn

Py:   square = lambda x: x * x
来源：http://lax.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cvn.yvedp.cn

JS:   const square = x => x * x;
来源：http://dtx.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://rtm.vqdsnc.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rgn.zdqjudy.top

Go:   sq := func(x int) int { return x * x }
来源：http://zhv.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://wef.ivvv.top

C#:   Func<int, int> square = x => x * x;
来源：http://dmj.yongpay.top

[C07] 把函数作为参数传入
来源：http://iet.shanyushiyangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bvu.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://xec.jinghuilouyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lha.hongshengwenyu.top

TS:   arr.map(String)
来源：http://hsl.meibo888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wij.yonumen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://myr.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://lbq.jiagoushi.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pyi.ppjwa.cn

[C08] 闭包
来源：http://nzj.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://txy.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uvj.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rhn.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qbo.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yiy.yangfankeji.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uam.xuetiantiany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zsl.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hun.shanyushiyangtech.top

[C09] 递归
来源：http://uoa.jinyuanbaomall.cn


<!-- 参考信息 -->