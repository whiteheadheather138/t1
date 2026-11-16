代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iyg.jyoumei.cn

Java: (int) 'A'; (char) 65
来源：http://xhu.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nkt.vehdjk.com

Ruby: "A".ord; 65.chr
来源：http://ukh.havefunace.top

C#:   (int)'A'; (char)65
来源：http://hsp.cucudq.cn

[A19] 交换两个变量
来源：http://osf.daria6918.cn

Py:   a, b = b, a
来源：http://mxe.quarkkingdee.top

PHP:  [$a, $b] = [$b, $a];
来源：http://vuz.jianghu66.top

JS:   [a, b] = [b, a];
来源：http://wsk.xylfe.cn

TS:   [a, b] = [b, a];
来源：http://lqp.aibaodan.cn

Java: int t = a; a = b; b = t;
来源：http://lyu.jinghuilouyu.cn

Go:   a, b = b, a
来源：http://cfr.hysaishi.cn

Ruby: a, b = b, a
来源：http://rgr.xziqi.cn

C#:   (a, b) = (b, a);
来源：http://zkg.xziqi.cn

[A20] 读取标准输入
来源：http://ujz.snrcjt.cn

Py:   name = input("请输入：")
来源：http://yuh.fengsongda.top

PHP:  $name = trim(fgets(STDIN));
来源：http://doa.sufxvd.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pux.sufxvd.cn

TS:   // Node.js：readline 模块
来源：http://vvy.shanyushiyangkeji.top

Java: new Scanner(System.in).nextLine()
来源：http://fiu.jiagoushi.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://emz.wangshuangyany.cn

Ruby: gets.chomp
来源：http://tiq.birdmap.top

C#:   Console.ReadLine();
来源：http://vsx.zhengqikj.top

[A21] 保留指定小数位输出
来源：http://rul.jinyuanbaomall.cn

Py:   f"{3.14159:.2f}"
来源：http://xjn.316326.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rjg.xingfuxueyuan.xyz

JS:   (3.14159).toFixed(2)
来源：http://jsl.sweek.top

TS:   (3.14159).toFixed(2)
来源：http://fgf.gzhubu.top

Java: String.format("%.2f", 3.14159)
来源：http://uyo.sufxvd.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cik.bbcook.cn

Ruby: format("%.2f", 3.14159)
来源：http://aqv.gogol.net.cn

C#:   3.14159.ToString("F2")
来源：http://nzs.sjlbkw.cn

[A22] 获取字符串长度
来源：http://ung.fzhhl.top

Py:   len(s)
来源：http://mvo.chenjidiqi.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cho.quarkkingdee.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yao.gotoacloud.top

TS:   s.length
来源：http://kuj.sysykeji.top

Java: s.length()
来源：http://jou.cheryme.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tip.birdmap.top

Ruby: s.length
来源：http://yni.yuxming.cn

C#:   s.Length
来源：http://gml.smart0.xyz

[A23] 大小写转换
来源：http://rie.xylfe.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://epl.shzxlz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xdu.shangyingyoupin.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dll.xziqi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wxu.yonumen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ygz.tanke756.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://csv.fehbvm.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rvv.jinqigufen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hyk.chenzaomai.com

[A24] 去除首尾空白
来源：http://hpv.tanke756.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://slf.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pmz.cashguo.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://grj.nanxuanxn.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jwu.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nib.ctjpmb.com

Go:   strings.TrimSpace(s)
来源：http://vrx.tian-w.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ito.jlsjyb.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://trb.yanxiufei.cn

[A25] 字符串比较
来源：http://lbf.c1oappe.top

Py:   s1 == s2; s1 != s2
来源：http://mcy.birdmap.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jdw.hongshengwenyu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jqb.shanyushiyangtech.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tqr.havefunace.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yrn.epnwcf.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jez.chenzaomai.com

Ruby: s1 == s2; s1 <=> s2
来源：http://evy.aizwys.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tal.zhengqikj.top

[A26] 类型转换总览
来源：http://iuy.hcnkem.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sjn.zhengqikj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xdb.xziqi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jli.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://uhj.cdnleiting.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xkk.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ntu.fehbvm.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://azt.hnqzz.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gaf.sufxvd.cn

================================================================================
来源：http://trz.sysykeji.top

B. 流程控制
来源：http://yyd.sjlbkw.cn

================================================================================
来源：http://iyx.shanyushiyangkeji.top

[B01] 条件判断 if / else
来源：http://dcw.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ekf.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jev.cashguo.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xvu.gaohongyu789.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://twz.ywan-chungtsiang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://aat.hesvh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qzt.hnxiangtu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bmt.fanxiaobao.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ydi.yueranfly.top

[B02] 多分支 else if / elif
来源：http://ipp.zdbjq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uyf.shzxlz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fta.xuetiantiany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mwn.yuanzhike.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://swx.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eix.yuanzhike.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wum.chenzaomai.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cpt.meibo888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yfd.yonumen.top

[B03] switch / match / case
来源：http://tym.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yqo.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://onk.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kqk.ydjk.org.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ukp.nanxinkj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uwn.jinyuanbaomall.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fih.nanxuanxn.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://agu.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uau.0kj1m.cn

[B04] for 计数循环
来源：http://asq.52xcode.cn

Py:   for i in range(10): print(i)
来源：http://jrx.ctjpmb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jus.cucudq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oum.hywenlv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pka.gzhubu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vmk.jinghuilouyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jrs.yj20258888.top

Ruby: 10.times { |i| puts i }
来源：http://adi.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pfi.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://wou.wangdashe.top

Py:   for item in arr: print(item)
来源：http://vmw.svipenyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jeh.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bcn.dianchejie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dqh.xylfe.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gwc.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gvn.9152youxi.cn

Ruby: arr.each { |item| puts item }
来源：http://psj.52xcode.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://not.daxiang520.top

[B06] 遍历字典 / 对象
来源：http://mln.yongpay.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zin.quarkkingdee.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dem.yj202588.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://alv.xinyue.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qki.sjlbkw.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://anl.pengpengdd.cyou

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tel.aizwys.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yhd.cheryme.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cls.xinyue.icu

[B07] while 循环
来源：http://qzx.guannengcc.top

Py:   while i < 10: i += 1
来源：http://uwi.yj202588.top

PHP:  while ($i < 10) { $i++; }
来源：http://byo.birdmap.top

JS:   while (i < 10) { i++; }
来源：http://doa.daxiang520.top

TS:   while (i < 10) { i++; }
来源：http://vpx.pycfn.com

Java: while (i < 10) { i++; }
来源：http://uaz.fengsongda.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kpz.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://alh.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://mpk.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://ccx.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://vrg.hongshengwenyu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lsa.yj20258.top

JS:   do { i++; } while (i < 10);
来源：http://ssw.jqgufenzy.top

TS:   do { i++; } while (i < 10);
来源：http://qcy.aizwys.cn

Java: do { i++; } while (i < 10);
来源：http://grr.gaohongyu789.top

Go:   for { i++; if i >= 10 { break } }
来源：http://shn.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://bkx.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://hlm.zdqjudy.top

[B09] break 与 continue
来源：http://djd.zdqjudy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hcx.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mtd.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jmo.ivvv.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ujj.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtw.316326.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://txo.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wwo.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xmx.yj202588.top

[B10] 遍历同时拿索引
来源：http://miv.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hnc.daxiang520.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kzf.xinyue.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nwr.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rxo.daria6918.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zrk.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wsl.gzhubu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lja.shanyushiyangtech.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vzq.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://kpt.yanxiufei.cn

Py:   list(range(0, 10, 2))
来源：http://ybx.hywenlv.cn

PHP:  range(0, 10, 2);
来源：http://msp.cucudq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qza.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://soi.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fmi.xziqi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://meg.bjfxy.top

Ruby: (0...10).step(2).to_a
来源：http://aho.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uet.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://jkd.chenzaomai.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://alh.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://zbm.yuanzhike.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rtm.ybcxt.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dcn.ywan-chungtsiang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://noy.wangshuangyany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eft.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zel.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kmz.guowangkeji.top

[B13] 判断是否为数字
来源：http://sre.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://xkx.hywenlv.cn

PHP:  is_numeric($x)
来源：http://jjg.hfpthk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kgt.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ehb.hnxiangtu.top

Java: x instanceof Number
来源：http://kmf.zhijiandao.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xkq.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://azw.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://nmv.bbcook.cn

[B14] 判断值是否在集合内
来源：http://tky.jqgufenzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kui.iojbl.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fkv.jlsjyb.cn

JS:   [1, 2, 3].includes(x)
来源：http://xvs.yvedp.cn

TS:   [1, 2, 3].includes(x)
来源：http://tib.xuanzx.com

Java: List.of(1, 2, 3).contains(x)
来源：http://les.pycfn.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qou.feifeiyinyue.top

Ruby: [1, 2, 3].include?(x)
来源：http://lxj.shanyushiyangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bjj.yj202588.top

[B15] 布尔运算与取反
来源：http://lzy.vqdsnc.cn

Py:   a and b or not c
来源：http://nst.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://woy.hammf.cn

JS:   a && b || !c
来源：http://wvn.tarul.cn

TS:   a && b || !c
来源：http://otc.yanxiufei.cn

Java: a && b || !c
来源：http://gbo.zycfv.cn

Go:   a && b || !c
来源：http://oxr.havefunace.top

Ruby: a && b || !c
来源：http://kdz.dashuyun.cn

C#:   a && b || !c
来源：http://hka.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://ifm.yonumen.top

Py:   if not data: return
来源：http://ttl.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://vwx.jiagoushi.top

JS:   if (!data) return;
来源：http://tjg.tianlin.xyz

TS:   if (!data) return;
来源：http://ffj.wangshuangyany.cn

Java: if (data == null) return;
来源：http://tfn.hammf.cn

Go:   if data == nil { return }
来源：http://kbm.zhijiandao.cn

Ruby: return if data.nil?
来源：http://uoo.zhiwuduotai.top

C#:   if (data == null) return;
来源：http://bfp.hesvh.cn

================================================================================
来源：http://ygg.hammf.cn

C. 函数与作用域
来源：http://tnt.sysykeji.top

================================================================================
来源：http://ooy.gogol.net.cn

[C01] 定义函数
来源：http://myi.nwbrower.top

Py:   def add(a, b): return a + b
来源：http://lhr.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gnn.aizwys.cn

JS:   function add(a, b) { return a + b; }
来源：http://wgo.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nhl.birdmap.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ujl.hcnkem.com

Go:   func add(a, b int) int { return a + b }
来源：http://dmu.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://dfk.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://auy.sufxvd.cn

[C02] 默认参数
来源：http://imn.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://qpn.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://giq.yongpay.top

JS:   function greet(name = "World") { return name; }
来源：http://woc.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fch.yangfankeji.com

Java: // 无默认参数：方法重载或 Optional
来源：http://hps.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hum.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://nns.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://bip.xuetiantiany.cn

[C03] 可变参数
来源：http://iwi.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://tfj.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://chm.yj20258888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rcy.ehwqpu.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mxx.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://epq.wangshuangyany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jxn.chenzaomai.com

Ruby: def total(*nums); nums.sum; end
来源：http://lsp.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sgm.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://sbm.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ltz.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lur.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wcy.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sfm.jiagoushi.top

Java: // 无：用 Builder 模式或 record
来源：http://bsp.fanxiaobao.xyz

Go:   // 无：用配置结构体参数
来源：http://tbl.zhengqikj.top

Ruby: f(a: 1, b: 2)
来源：http://taq.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://axn.fktsv.cn

[C05] 返回多个值
来源：http://sfx.gogol.net.cn

Py:   return a, b
来源：http://exo.zhiwuduotai.top

PHP:  return [$a, $b];
来源：http://ohs.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://psy.sufxvd.cn

TS:   return { a, b };
来源：http://cal.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hki.feifeiyinyue.top

Go:   return a, b
来源：http://oqb.cashguo.top

Ruby: return a, b
来源：http://cuu.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://gxj.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://fig.hnqzz.top

Py:   square = lambda x: x * x
来源：http://reg.hesvh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gss.shuidangran.top

JS:   const square = x => x * x;
来源：http://zwk.zhoulong.xyz

TS:   const square = (x: number): number => x * x;
来源：http://cfx.yj202588.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pwb.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hfg.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://uum.zhixingplan.top

C#:   Func<int, int> square = x => x * x;
来源：http://cpw.zdbjq.cn

[C07] 把函数作为参数传入
来源：http://msz.jinyuanbaomall.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://emi.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://fzf.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://smx.cdnleiting.top

TS:   arr.map(String)
来源：http://hpb.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bmg.vqdsnc.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://azn.ehwqpu.com

Ruby: arr.map(&:upcase)
来源：http://qlk.aizwys.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hdd.yangfankeji.com

[C08] 闭包
来源：http://xnt.zhongyouzk.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://loq.zhaomingkeji.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zzw.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iuj.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kyf.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ycr.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://reo.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://waz.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://faf.ydjk.org.cn

[C09] 递归
来源：http://vkv.zhixingplan.top


<!-- 参考信息 -->