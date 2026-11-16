代发 wailian999

C#:   (int)'A'; (char)65
来源：http://zza.gzhubu.top

[A19] 交换两个变量
来源：http://toa.vqdsnc.cn

Py:   a, b = b, a
来源：http://wnq.vehdjk.com

PHP:  [$a, $b] = [$b, $a];
来源：http://uhb.bjfxy.top

JS:   [a, b] = [b, a];
来源：http://fig.zhengqikj.top

TS:   [a, b] = [b, a];
来源：http://gwf.chenzaomai.com

Java: int t = a; a = b; b = t;
来源：http://oum.jinqigufen.top

Go:   a, b = b, a
来源：http://skw.jiagoushi.top

Ruby: a, b = b, a
来源：http://qdz.jqgfzy.top

C#:   (a, b) = (b, a);
来源：http://qgm.ybcxt.top

[A20] 读取标准输入
来源：http://tqh.jianghu66.top

Py:   name = input("请输入：")
来源：http://wmh.guannengcc.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kdl.xinyue.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://old.xinyue.icu

TS:   // Node.js：readline 模块
来源：http://xqm.andypj.xyz

Java: new Scanner(System.in).nextLine()
来源：http://jaa.cucudq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tdt.52xcode.cn

Ruby: gets.chomp
来源：http://xdq.zhongyouzk.top

C#:   Console.ReadLine();
来源：http://bfs.vehdjk.com

[A21] 保留指定小数位输出
来源：http://dgn.ctjpmb.com

Py:   f"{3.14159:.2f}"
来源：http://gsp.cashguo.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kye.yangfankeji.com

JS:   (3.14159).toFixed(2)
来源：http://rcm.hcnkem.com

TS:   (3.14159).toFixed(2)
来源：http://pch.ydzc1.top

Java: String.format("%.2f", 3.14159)
来源：http://myr.hfpthk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ixq.9152youxi.cn

Ruby: format("%.2f", 3.14159)
来源：http://uqu.ywan-chungtsiang.top

C#:   3.14159.ToString("F2")
来源：http://ghi.c1oappe.top

[A22] 获取字符串长度
来源：http://buc.hysaishi.cn

Py:   len(s)
来源：http://sjf.yanxiufei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lnt.meibo888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cgr.jinghuilouyu.cn

TS:   s.length
来源：http://jrk.0kj1m.cn

Java: s.length()
来源：http://ymw.gzhubu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qwc.jqgfzy.top

Ruby: s.length
来源：http://gof.nwbrower.top

C#:   s.Length
来源：http://cme.yangfankeji.com

[A23] 大小写转换
来源：http://pwi.cashguo.top

Py:   s.upper(); s.lower(); s.title()
来源：http://fbz.pycfn.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eyn.ydjk.org.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zyu.9152youxi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dlg.yanxiufei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iml.zdqjudy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zmh.vehdjk.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fvm.tanke756.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hho.hnxiangtu.top

[A24] 去除首尾空白
来源：http://gie.zdbjq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rrx.xingfuxueyuan.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kzv.dashuyun.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://akq.jqgufenzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tle.birdmap.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://psx.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://pwl.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qme.jinyuanbaomall.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aax.chenlongwang.top

[A25] 字符串比较
来源：http://frx.yvedp.cn

Py:   s1 == s2; s1 != s2
来源：http://egj.fzhhl.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wlt.vehdjk.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://apg.hesvh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kxt.yonumen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yyk.snrcjt.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kru.pycfn.com

Ruby: s1 == s2; s1 <=> s2
来源：http://elq.zhengqikj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://leg.hfpthk.cn

[A26] 类型转换总览
来源：http://rpj.hywenlv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cxk.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wls.quarkkingdee.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nmp.jiagoushi.top

TS:   Number() String() Boolean() x as number
来源：http://hlg.feifeiyinyue.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://goc.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cpj.zhiwuduotai.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zio.smart0.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fsk.shangyingyoupin.top

================================================================================
来源：http://xxl.wangshuangyany.cn

B. 流程控制
来源：http://ykt.yanxiufei.cn

================================================================================
来源：http://abw.mhx1999.top

[B01] 条件判断 if / else
来源：http://vsh.yuxming.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://myx.ctjpmb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tdf.shzxlz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rsm.ehwqpu.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vzb.ppjwa.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ema.zhengqikj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kfp.tanke756.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kns.redwolf501.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ctx.nanxinkj.top

[B02] 多分支 else if / elif
来源：http://ils.quarkkingdee.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://axj.gotoacloud.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xso.gotoacloud.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zhg.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jwp.zdqjudy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://clq.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wwg.gogol.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nlj.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://twb.chenzaomai.com

[B03] switch / match / case
来源：http://jln.sjlbkw.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eco.shuidangran.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gdj.316326.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ubk.hesvh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uas.ywan-chungtsiang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cha.yuanzhike.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bnh.pycfn.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ksu.fengsongda.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oep.sjlbkw.cn

[B04] for 计数循环
来源：http://nnm.316326.xyz

Py:   for i in range(10): print(i)
来源：http://wtn.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dzb.ctjpmb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rzj.hywenlv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tmf.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yjt.daria6918.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://syi.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://riy.shzxlz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rtj.hnxiangtu.top

[B05] 遍历数组 / 列表
来源：http://kjg.fengsongda.top

Py:   for item in arr: print(item)
来源：http://sme.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ies.hcnkem.com

JS:   for (const item of arr) { console.log(item); }
来源：http://zdv.yonumen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wgn.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ncw.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hmp.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://avj.jinghuilouyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tqf.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://cmg.hongshengwenyu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rmp.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xcu.shuidangran.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lhn.jianghu66.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ete.bbcook.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wve.yanxiufei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qfh.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bcd.vehdjk.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cjc.ivvv.top

[B07] while 循环
来源：http://joz.andypj.xyz

Py:   while i < 10: i += 1
来源：http://nlx.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xgd.wangdashe.top

JS:   while (i < 10) { i++; }
来源：http://taj.0kj1m.cn

TS:   while (i < 10) { i++; }
来源：http://kuf.316326.xyz

Java: while (i < 10) { i++; }
来源：http://uru.yonumen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rfn.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://jdr.gogol.net.cn

C#:   while (i < 10) { i++; }
来源：http://ksf.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://ion.bjfxy.top

Py:   # 无 do-while：用 while True + break
来源：http://lar.tian-w.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lpe.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://bgy.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://qko.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://fhk.316326.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://fqs.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cih.jqgfzy.top

C#:   do { i++; } while (i < 10);
来源：http://eis.feifeiyinyue.top

[B09] break 与 continue
来源：http://wbm.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fvl.shzxlz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://upy.jlsjyb.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dic.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fju.c1oappe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ecy.chenjidiqi.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xca.cashguo.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lbl.jqgfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lzb.yangfankeji.com

[B10] 遍历同时拿索引
来源：http://zqx.yongpay.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nxd.yfazqb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aun.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://itn.gotoacloud.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ike.sufxvd.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://udd.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fhi.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jrr.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oam.9152youxi.cn

[B11] 生成数字序列 / 区间
来源：http://jdt.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://jhq.uphjek.com

PHP:  range(0, 10, 2);
来源：http://nny.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://thw.havefunace.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ayv.ctjpmb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://thh.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lcp.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://zzx.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gnu.yanxiufei.cn

[B12] 跳出多层循环
来源：http://clv.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kiw.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://fvd.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hhn.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://moc.wangdashe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ibo.bbcook.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cin.c1oappe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://flc.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fjm.svipenyu.cn

[B13] 判断是否为数字
来源：http://cvs.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://slv.dianchejie.cn

PHP:  is_numeric($x)
来源：http://vfe.zhongyouzk.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zvq.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fnv.quarkkingdee.top

Java: x instanceof Number
来源：http://tvg.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jjo.yueranfly.top

Ruby: x.is_a?(Numeric)
来源：http://wri.smart0.xyz

C#:   x is int or double or decimal
来源：http://uoy.fehbvm.com

[B14] 判断值是否在集合内
来源：http://qmx.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://itk.svipenyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://prf.jyoumei.cn

JS:   [1, 2, 3].includes(x)
来源：http://jow.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://foi.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://owh.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://asu.cdnleiting.top

Ruby: [1, 2, 3].include?(x)
来源：http://hkr.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qko.hcnkem.com

[B15] 布尔运算与取反
来源：http://ncp.meibo888.top

Py:   a and b or not c
来源：http://gpi.ybcxt.top

PHP:  $a && $b || !$c
来源：http://nxt.bjfxy.top

JS:   a && b || !c
来源：http://hka.hesvh.cn

TS:   a && b || !c
来源：http://hkt.jianghu66.top

Java: a && b || !c
来源：http://wzs.fzhhl.top

Go:   a && b || !c
来源：http://eih.xziqi.cn

Ruby: a && b || !c
来源：http://xur.ywan-chungtsiang.top

C#:   a && b || !c
来源：http://frb.gaohongyu789.top

[B16] 卫语句：不满足条件提前返回
来源：http://noi.fanxiaobao.xyz

Py:   if not data: return
来源：http://fxd.nanxuanxn.top

PHP:  if (!$data) { return; }
来源：http://icy.vqdsnc.cn

JS:   if (!data) return;
来源：http://kaq.fanxiaobao.xyz

TS:   if (!data) return;
来源：http://nhj.tarul.cn

Java: if (data == null) return;
来源：http://fgx.yj20258888.top

Go:   if data == nil { return }
来源：http://bto.yj202588.top

Ruby: return if data.nil?
来源：http://rug.daxiang520.top

C#:   if (data == null) return;
来源：http://tne.jinyuanbaomall.cn

================================================================================
来源：http://pvs.fktsv.cn

C. 函数与作用域
来源：http://twy.mhx1999.top

================================================================================
来源：http://zcb.ywan-chungtsiang.top

[C01] 定义函数
来源：http://rdg.fktsv.cn

Py:   def add(a, b): return a + b
来源：http://kif.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vxy.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://jac.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://opl.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eqe.jinghuilouyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ndz.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://cvo.birdmap.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lbi.chenlongwang.top

[C02] 默认参数
来源：http://mwu.yuanzhike.top

Py:   def greet(name="World"): return name
来源：http://jml.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://uzi.zhoulong.xyz

JS:   function greet(name = "World") { return name; }
来源：http://dny.sjlbkw.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cic.52xcode.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ovn.chenjidiqi.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iom.quarkkingdee.top

Ruby: def greet(name = "World") = name
来源：http://vtm.quarkkingdee.top

C#:   string Greet(string name = "World") => name;
来源：http://yix.nanxinkj.top

[C03] 可变参数
来源：http://ojs.havefunace.top

Py:   def total(*args): return sum(args)
来源：http://bny.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hef.epnwcf.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nzh.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://otq.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://shz.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://trz.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://lnh.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yto.hcnkem.com

[C04] 命名参数 / 关键字参数
来源：http://ljn.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fnj.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ubx.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://niq.gaohongyu789.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eup.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://gew.xylfe.cn

Go:   // 无：用配置结构体参数
来源：http://zfi.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://uwq.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://atp.jinqigfzy.top

[C05] 返回多个值
来源：http://tfn.guannengcc.top

Py:   return a, b
来源：http://xlm.zhongyouzk.top

PHP:  return [$a, $b];
来源：http://klu.jyoumei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bnl.0kj1m.cn

TS:   return { a, b };
来源：http://ffj.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kbz.cucudq.cn

Go:   return a, b
来源：http://wst.hesvh.cn

Ruby: return a, b
来源：http://srx.yj20258888.top

C#:   return (a, b);              // ValueTuple
来源：http://spi.quarkkingdee.top

[C06] 匿名函数 / lambda
来源：http://ucj.jinqigufen.top

Py:   square = lambda x: x * x
来源：http://aml.yangfankeji.com

PHP:  $square = fn($x) => $x * $x;
来源：http://rsv.gotoacloud.top

JS:   const square = x => x * x;
来源：http://jma.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://tzf.vqdsnc.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oif.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://bsa.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://eza.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://ccd.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://fgf.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qnk.tian-w.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kmg.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tmo.jqgufenzy.top

TS:   arr.map(String)
来源：http://zsm.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yic.aizwys.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wqb.birdmap.top

Ruby: arr.map(&:upcase)
来源：http://mqi.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://kke.yj20258.top

[C08] 闭包
来源：http://tdf.guowangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zdp.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vkz.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ige.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tia.52xcode.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xgy.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ayq.jianghu66.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fkx.jinqigfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nzj.hongshengwenyu.top

[C09] 递归
来源：http://org.yj20258.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zwh.zhijiandao.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dwy.ybcxt.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hwa.ehwqpu.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gjl.zhaomingkeji.xyz


<!-- 参考信息 -->