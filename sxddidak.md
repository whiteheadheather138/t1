代发 wailian999

Ruby: value = data || "默认值"
来源：http://zwx.fengsongda.top

C#:   var value = data ?? "默认值";
来源：http://ugd.yueranfly.top

[A16] 真假值判断规则
来源：http://zkc.jqgufenzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hyv.nanxinkj.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gvu.iojbl.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jpv.shuidangran.top

TS:   if (!x) {}
来源：http://ydr.yonumen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ydj.cheryme.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dnw.vehdjk.com

Ruby: unless x            # nil 与 false 为假
来源：http://aqq.dashuyun.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dsb.vehdjk.com

[A17] 位运算
来源：http://oqg.zhiwuduotai.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ljg.zhaomingkeji.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hvd.wangshuangyany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ctj.meibo888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jvs.quarkkingdee.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aom.gzhubu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qdo.cashguo.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wmi.jyoumei.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jcn.jinqigfzy.top

[A18] 字符与 ASCII 码互转
来源：http://nub.0kj1m.cn

Py:   ord("A"); chr(65)
来源：http://fxd.fanxiaobao.xyz

PHP:  ord("A"); chr(65)
来源：http://xqh.yueranfly.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vva.vqdsnc.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rwh.jianghu66.top

Java: (int) 'A'; (char) 65
来源：http://ybp.tianlin.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ybd.mhx1999.top

Ruby: "A".ord; 65.chr
来源：http://vnp.vehdjk.com

C#:   (int)'A'; (char)65
来源：http://gsj.tanke756.top

[A19] 交换两个变量
来源：http://kwx.tian-w.cn

Py:   a, b = b, a
来源：http://mat.feifeiyinyue.top

PHP:  [$a, $b] = [$b, $a];
来源：http://fjp.shanyushiyangtech.top

JS:   [a, b] = [b, a];
来源：http://yxi.sweek.top

TS:   [a, b] = [b, a];
来源：http://zin.fzhhl.top

Java: int t = a; a = b; b = t;
来源：http://pxz.52xcode.cn

Go:   a, b = b, a
来源：http://wzx.zycfv.cn

Ruby: a, b = b, a
来源：http://thz.zdbjq.cn

C#:   (a, b) = (b, a);
来源：http://wdb.tarul.cn

[A20] 读取标准输入
来源：http://kco.iojbl.cn

Py:   name = input("请输入：")
来源：http://gjy.svipenyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://egc.jinqigufen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ury.epnwcf.com

TS:   // Node.js：readline 模块
来源：http://vtw.smart0.xyz

Java: new Scanner(System.in).nextLine()
来源：http://icc.aizwys.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pso.birdmap.top

Ruby: gets.chomp
来源：http://wsy.zhijiandao.cn

C#:   Console.ReadLine();
来源：http://ywx.xylfe.cn

[A21] 保留指定小数位输出
来源：http://jel.ivvv.top

Py:   f"{3.14159:.2f}"
来源：http://yam.yj20258888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hop.yonumen.top

JS:   (3.14159).toFixed(2)
来源：http://kmk.sufxvd.cn

TS:   (3.14159).toFixed(2)
来源：http://mft.ivvv.top

Java: String.format("%.2f", 3.14159)
来源：http://moo.yuxming.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fpg.jianghu66.top

Ruby: format("%.2f", 3.14159)
来源：http://tlk.ywan-chungtsiang.top

C#:   3.14159.ToString("F2")
来源：http://lvu.zhongyouzk.top

[A22] 获取字符串长度
来源：http://tec.c1oappe.top

Py:   len(s)
来源：http://hvr.uphjek.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://odu.tian-w.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jsa.hcnkem.com

TS:   s.length
来源：http://xuf.gogol.net.cn

Java: s.length()
来源：http://hae.jianghu66.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uii.xziqi.cn

Ruby: s.length
来源：http://hri.aizwys.cn

C#:   s.Length
来源：http://cwl.smart0.xyz

[A23] 大小写转换
来源：http://mgu.mhx1999.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lov.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hwe.fanxiaobao.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://viv.iojbl.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mxq.guannengcc.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ocw.guannengcc.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bzm.shzxlz.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uor.cucudq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xcd.yfazqb.com

[A24] 去除首尾空白
来源：http://jug.316326.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kxo.hywenlv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hoz.zhixingplan.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zmz.jinghuilouyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hfo.shuidangran.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kyb.xingfuxueyuan.xyz

Go:   strings.TrimSpace(s)
来源：http://xhr.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fbi.aizwys.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zbf.dianchejie.cn

[A25] 字符串比较
来源：http://lni.pengpengdd.cyou

Py:   s1 == s2; s1 != s2
来源：http://gfx.jinghuilouyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://weo.hywenlv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ees.xziqi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cyu.zycfv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wzn.yongpay.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://utz.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://xyf.dashuyun.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rqu.shanyushiyangtech.top

[A26] 类型转换总览
来源：http://kmf.yonumen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uvn.hnxiangtu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iaf.jqgufenzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iub.gogol.net.cn

TS:   Number() String() Boolean() x as number
来源：http://dsu.quarkkingdee.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vkx.hnqzz.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ieb.zhaomingkeji.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://ugb.ydjk.org.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ged.wangshuangyany.cn

================================================================================
来源：http://xxx.hywenlv.cn

B. 流程控制
来源：http://aib.ctjpmb.com

================================================================================
来源：http://gar.andypj.xyz

[B01] 条件判断 if / else
来源：http://xss.yvedp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yst.zdbjq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tfg.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://upp.gaohongyu789.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zvi.smart0.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://rpc.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zxy.ydzc1.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://djs.bjfxy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://urf.hesvh.cn

[B02] 多分支 else if / elif
来源：http://llo.zdbjq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tdo.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tqd.bjfxy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rsz.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://shn.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xvy.fzhhl.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lop.vqdsnc.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wih.redwolf501.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iwf.iojbl.cn

[B03] switch / match / case
来源：http://rgi.ywan-chungtsiang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cmg.zhijiandao.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xur.tianlin.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nds.havefunace.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uhj.gaohongyu789.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tkj.ydzc1.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://khr.jinyuanbaomall.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cqz.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fsc.aizwys.cn

[B04] for 计数循环
来源：http://qee.fktsv.cn

Py:   for i in range(10): print(i)
来源：http://naa.vqdsnc.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kjv.yuxming.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qcx.chenjidiqi.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lji.zhengqikj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://det.yanxiufei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://otj.xingfuxueyuan.xyz

Ruby: 10.times { |i| puts i }
来源：http://hdg.xingfuxueyuan.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bmu.0kj1m.cn

[B05] 遍历数组 / 列表
来源：http://ney.chenjidiqi.icu

Py:   for item in arr: print(item)
来源：http://tup.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nho.yj20258.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zcb.jinyuanbaomall.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rgc.hesvh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uoe.redwolf501.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eka.zhijiandao.cn

Ruby: arr.each { |item| puts item }
来源：http://jsh.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zme.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://jhx.havefunace.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bgv.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cly.nwbrower.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yza.yueranfly.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://std.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oxo.sysykeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://agu.yvedp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://moy.yongpay.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://axz.chenjidiqi.icu

[B07] while 循环
来源：http://xhm.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://tyh.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://blo.gaohongyu789.top

JS:   while (i < 10) { i++; }
来源：http://qet.yuanzhike.top

TS:   while (i < 10) { i++; }
来源：http://yqq.yueranfly.top

Java: while (i < 10) { i++; }
来源：http://hws.chenjidiqi.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kns.ybcxt.top

Ruby: while i < 10; i += 1; end
来源：http://fsv.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://crk.chenzaomai.com

[B08] do-while（至少执行一次）
来源：http://njd.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://uav.dianchejie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vli.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://qzg.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://sfq.yueranfly.top

Java: do { i++; } while (i < 10);
来源：http://jfh.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ywo.hongshengwenyu.top

Ruby: begin; i += 1; end while i < 10
来源：http://asu.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://yqf.sjlbkw.cn

[B09] break 与 continue
来源：http://dfx.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jsj.vehdjk.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tvn.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ecq.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xtw.pengpengdd.cyou

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://prw.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ytx.tianlin.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ppb.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kjn.yj20258.top

[B10] 遍历同时拿索引
来源：http://pgg.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nhz.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uoq.jqgfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mqa.yuxming.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rpq.jlsjyb.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ecl.sweek.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qst.redwolf501.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bbt.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cwk.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://hyi.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://zpe.zhixingplan.top

PHP:  range(0, 10, 2);
来源：http://wym.shanyushiyangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dpq.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://whl.zdqjudy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lhi.svipenyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://erb.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://egr.zhiwuduotai.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://osu.epnwcf.com

[B12] 跳出多层循环
来源：http://axk.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://oiw.yj202588.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fyu.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rio.zhoulong.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eva.zhiwuduotai.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gwh.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rhc.gzhubu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wez.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://skq.guowangkeji.top

[B13] 判断是否为数字
来源：http://xuy.yuanzhike.top

Py:   isinstance(x, (int, float))
来源：http://ddq.yfazqb.com

PHP:  is_numeric($x)
来源：http://oyx.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ddx.shangyingyoupin.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://unr.ctjpmb.com

Java: x instanceof Number
来源：http://abw.guannengcc.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nif.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://wek.yj202588.top

C#:   x is int or double or decimal
来源：http://cdo.ivvv.top

[B14] 判断值是否在集合内
来源：http://sbp.wangshuangyany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mwo.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kuj.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://tph.xylfe.cn

TS:   [1, 2, 3].includes(x)
来源：http://fms.sjlbkw.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ggm.shangyingyoupin.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zeb.cucudq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vnn.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xfk.nanxinkj.top

[B15] 布尔运算与取反
来源：http://gti.hongshengwenyu.top

Py:   a and b or not c
来源：http://ith.yangfankeji.com

PHP:  $a && $b || !$c
来源：http://jge.meibo888.top

JS:   a && b || !c
来源：http://ori.quarkkingdee.top

TS:   a && b || !c
来源：http://mog.yangfankeji.com

Java: a && b || !c
来源：http://rah.gotoacloud.top

Go:   a && b || !c
来源：http://jrv.mhx1999.top

Ruby: a && b || !c
来源：http://jef.vehdjk.com

C#:   a && b || !c
来源：http://nmb.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://kbc.nwbrower.top

Py:   if not data: return
来源：http://zmw.316326.xyz

PHP:  if (!$data) { return; }
来源：http://kup.guannengcc.top

JS:   if (!data) return;
来源：http://gxp.fzhhl.top

TS:   if (!data) return;
来源：http://saj.yanxiufei.cn

Java: if (data == null) return;
来源：http://nxx.jyoumei.cn

Go:   if data == nil { return }
来源：http://zuo.yueranfly.top

Ruby: return if data.nil?
来源：http://wdx.epnwcf.com

C#:   if (data == null) return;
来源：http://kfg.ehwqpu.com

================================================================================
来源：http://pyi.cheryme.top

C. 函数与作用域
来源：http://mii.0kj1m.cn

================================================================================
来源：http://tts.jiagoushi.top

[C01] 定义函数
来源：http://esr.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://wrg.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xpt.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://fom.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vwp.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://etf.cheryme.top

Go:   func add(a, b int) int { return a + b }
来源：http://rug.vehdjk.com

Ruby: def add(a, b); a + b; end
来源：http://olo.jqgfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vwj.yuanzhike.top

[C02] 默认参数
来源：http://ayz.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://jwt.yfazqb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://npg.tarul.cn

JS:   function greet(name = "World") { return name; }
来源：http://wxx.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://itq.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://wyy.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ppu.feifeiyinyue.top

Ruby: def greet(name = "World") = name
来源：http://ouc.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://vbb.redwolf501.top

[C03] 可变参数
来源：http://bxc.yj20258888.top

Py:   def total(*args): return sum(args)
来源：http://ykz.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xbl.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zbp.guowangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tzf.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ysg.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://efo.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://unk.xuetiantiany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fxc.zdqjudy.top

[C04] 命名参数 / 关键字参数
来源：http://xii.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sur.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dcx.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uwc.birdmap.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gxa.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://xqx.yj20258888.top

Go:   // 无：用配置结构体参数
来源：http://gmv.nanxinkj.top

Ruby: f(a: 1, b: 2)
来源：http://tab.hongshengwenyu.top

C#:   f(a: 1, b: 2)
来源：http://wni.jqgufenzy.top

[C05] 返回多个值
来源：http://akx.zdbjq.cn

Py:   return a, b
来源：http://pul.bjfxy.top

PHP:  return [$a, $b];
来源：http://rzg.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ygv.aibaodan.cn

TS:   return { a, b };
来源：http://qut.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pbz.jiagoushi.top

Go:   return a, b
来源：http://hdm.yueranfly.top

Ruby: return a, b
来源：http://hty.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://plj.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://xlf.redwolf501.top

Py:   square = lambda x: x * x
来源：http://uju.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://ksk.ydjk.org.cn

JS:   const square = x => x * x;
来源：http://klr.ehwqpu.com


<!-- 参考信息 -->