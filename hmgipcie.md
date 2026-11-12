代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sxw.gogol.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vvh.bjfxy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://flf.ivvv.top

[A17] 位运算
来源：http://ydm.yj20258.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://utq.yueranfly.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tpe.jianghu66.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mmq.bjfxy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gxm.yongpay.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rlk.zhaomingkeji.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://goq.dashuyun.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gmq.epnwcf.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://epw.c1oappe.top

[A18] 字符与 ASCII 码互转
来源：http://yxy.sweek.top

Py:   ord("A"); chr(65)
来源：http://ofz.haohaochexian.top

PHP:  ord("A"); chr(65)
来源：http://ewc.sweek.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qgx.hnqzz.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lap.cheryme.top

Java: (int) 'A'; (char) 65
来源：http://zci.0kj1m.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qqb.mhx1999.top

Ruby: "A".ord; 65.chr
来源：http://baa.nwbrower.top

C#:   (int)'A'; (char)65
来源：http://ent.hongshengwenyu.top

[A19] 交换两个变量
来源：http://ews.gotoacloud.top

Py:   a, b = b, a
来源：http://yir.dashuyun.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://aef.gzhubu.top

JS:   [a, b] = [b, a];
来源：http://qbq.hfpthk.cn

TS:   [a, b] = [b, a];
来源：http://avt.zhiwuduotai.top

Java: int t = a; a = b; b = t;
来源：http://kfy.yuanzhike.top

Go:   a, b = b, a
来源：http://chw.gogol.net.cn

Ruby: a, b = b, a
来源：http://aql.aizwys.cn

C#:   (a, b) = (b, a);
来源：http://bxi.guowangkeji.top

[A20] 读取标准输入
来源：http://acb.sjlbkw.cn

Py:   name = input("请输入：")
来源：http://dvg.c1oappe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://aar.hnxiangtu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iae.c1oappe.top

TS:   // Node.js：readline 模块
来源：http://vlx.feifeiyinyue.top

Java: new Scanner(System.in).nextLine()
来源：http://qbf.cqqwz.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ypn.jqgufenzy.top

Ruby: gets.chomp
来源：http://oul.hnqzz.top

C#:   Console.ReadLine();
来源：http://scm.sufxvd.cn

[A21] 保留指定小数位输出
来源：http://jld.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://vww.zhengqikj.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://igk.yj20258.top

JS:   (3.14159).toFixed(2)
来源：http://iaj.sxryk.cn

TS:   (3.14159).toFixed(2)
来源：http://ldq.pycfn.com

Java: String.format("%.2f", 3.14159)
来源：http://sdm.yvedp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jle.xinyue.icu

Ruby: format("%.2f", 3.14159)
来源：http://nul.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://keo.jinyuanbaomall.cn

[A22] 获取字符串长度
来源：http://elj.jlsjyb.cn

Py:   len(s)
来源：http://iic.fengsongda.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fvy.uphjek.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cpw.zhoulong.xyz

TS:   s.length
来源：http://dns.hcnkem.com

Java: s.length()
来源：http://ftw.zhaomingkeji.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vtz.ivvv.top

Ruby: s.length
来源：http://ecu.yongpay.top

C#:   s.Length
来源：http://wle.tian-w.cn

[A23] 大小写转换
来源：http://nxz.zhaomingkeji.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://mie.ivvv.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iub.zhongyouzk.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://arm.jqgufenzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pge.zhijiandao.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://plv.zhengqikj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yhr.hongshengwenyu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://utq.jqgufenzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://win.yueranfly.top

[A24] 去除首尾空白
来源：http://klm.jiagoushi.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ujl.redwolf501.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kdj.vqdsnc.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ajr.quarkkingdee.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qqj.hfpthk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://loj.gogol.net.cn

Go:   strings.TrimSpace(s)
来源：http://eqk.ppjwa.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://igk.zdqjudy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eiv.smart0.xyz

[A25] 字符串比较
来源：http://ykd.meibo888.top

Py:   s1 == s2; s1 != s2
来源：http://ypj.ybcxt.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mct.feifeiyinyue.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://laz.0kj1m.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lta.hcnkem.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lnq.chenzaomai.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ads.ydjk.org.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tyr.gzhubu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fyx.sjlbkw.cn

[A26] 类型转换总览
来源：http://uul.zhongyouzk.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bqe.uphjek.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xfw.cucudq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://igc.jinqigufen.top

TS:   Number() String() Boolean() x as number
来源：http://zml.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eng.yuxming.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jis.mhx1999.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ukq.pycfn.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zok.aibaodan.cn

================================================================================
来源：http://tyc.yanxiufei.cn

B. 流程控制
来源：http://krp.fktsv.cn

================================================================================
来源：http://jer.ydjk.org.cn

[B01] 条件判断 if / else
来源：http://uwl.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://tiv.yuanzhike.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mom.svipenyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ekb.pengpengdd.cyou

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rkc.hesvh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zqt.chenjidiqi.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wso.fanxiaobao.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sem.jqgfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ttr.cashguo.top

[B02] 多分支 else if / elif
来源：http://out.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://csn.fengsongda.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pvt.zhijiandao.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zlg.zhengqikj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rzp.kuanghao11.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yke.vqdsnc.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kjj.yj20258.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yns.hfpthk.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ajy.cdnleiting.top

[B03] switch / match / case
来源：http://wby.tian-w.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wys.ydzc1.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yun.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zdg.ppjwa.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://omo.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nxk.zhiwuduotai.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jtp.vehdjk.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://enk.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nzy.zhongyouzk.top

[B04] for 计数循环
来源：http://ctt.hongshengwenyu.top

Py:   for i in range(10): print(i)
来源：http://xwc.zhongyouzk.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ouh.vehdjk.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://thd.hongshengwenyu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uaj.aibaodan.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pkz.hesvh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gvf.tarul.cn

Ruby: 10.times { |i| puts i }
来源：http://zrq.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://auj.jyoumei.cn

[B05] 遍历数组 / 列表
来源：http://etd.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://jiq.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gci.fehbvm.com

JS:   for (const item of arr) { console.log(item); }
来源：http://mct.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fnx.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://afx.0kj1m.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pqh.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://ngd.jiagoushi.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hjj.hesvh.cn

[B06] 遍历字典 / 对象
来源：http://ute.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sti.jlsjyb.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zmn.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oft.yanxiufei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zhh.gzhubu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sso.fehbvm.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lvd.xziqi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lpe.nwbrower.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hka.jianghu66.top

[B07] while 循环
来源：http://kky.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://nyz.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://cnx.zdbjq.cn

JS:   while (i < 10) { i++; }
来源：http://ncw.xuetiantiany.cn

TS:   while (i < 10) { i++; }
来源：http://moe.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://czm.zhaomingkeji.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://icf.chenzaomai.com

Ruby: while i < 10; i += 1; end
来源：http://poe.shanyushiyangtech.top

C#:   while (i < 10) { i++; }
来源：http://vft.yj20258888.top

[B08] do-while（至少执行一次）
来源：http://owh.hywenlv.cn

Py:   # 无 do-while：用 while True + break
来源：http://pxk.hcnkem.com

PHP:  do { $i++; } while ($i < 10);
来源：http://rqs.yfazqb.com

JS:   do { i++; } while (i < 10);
来源：http://vuo.jinqigufen.top

TS:   do { i++; } while (i < 10);
来源：http://xly.zhongyouzk.top

Java: do { i++; } while (i < 10);
来源：http://xou.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dwj.iojbl.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hsj.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://ofd.fktsv.cn

[B09] break 与 continue
来源：http://hpk.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ycx.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ebr.bjfxy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mnc.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fmy.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsk.9152youxi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qav.tanke756.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cne.birdmap.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gcn.yueranfly.top

[B10] 遍历同时拿索引
来源：http://grz.sufxvd.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bok.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hcj.tianlin.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sgk.tian-w.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hik.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eur.yj202588.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zbv.jinqigfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://atx.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ysq.yfazqb.com

[B11] 生成数字序列 / 区间
来源：http://pri.dianchejie.cn

Py:   list(range(0, 10, 2))
来源：http://okx.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://zyn.nanxuanxn.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tec.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tfi.52xcode.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ikx.hnqzz.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jfm.jinqigufen.top

Ruby: (0...10).step(2).to_a
来源：http://ida.gzhubu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://knz.cdnleiting.top

[B12] 跳出多层循环
来源：http://jqu.guannengcc.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pqq.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uxg.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bfb.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dtv.hysaishi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vdu.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://anz.jianghu66.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xpo.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bnp.sufxvd.cn

[B13] 判断是否为数字
来源：http://bwu.ehwqpu.com

Py:   isinstance(x, (int, float))
来源：http://pix.shuidangran.top

PHP:  is_numeric($x)
来源：http://idv.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sej.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mpf.bjfxy.top

Java: x instanceof Number
来源：http://yvd.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rlu.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://rrw.snrcjt.cn

C#:   x is int or double or decimal
来源：http://hzn.guannengcc.top

[B14] 判断值是否在集合内
来源：http://bxp.xuanzx.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wme.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://byx.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://xcx.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://mhl.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tmd.shuidangran.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hpn.smart0.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://fre.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pds.sjlbkw.cn

[B15] 布尔运算与取反
来源：http://ryw.aibaodan.cn

Py:   a and b or not c
来源：http://oyi.cdnleiting.top

PHP:  $a && $b || !$c
来源：http://zqs.jlsjyb.cn

JS:   a && b || !c
来源：http://lje.sxryk.cn

TS:   a && b || !c
来源：http://srb.tarul.cn

Java: a && b || !c
来源：http://cyd.chenlongwang.top

Go:   a && b || !c
来源：http://atg.hesvh.cn

Ruby: a && b || !c
来源：http://erd.yongpay.top

C#:   a && b || !c
来源：http://ecb.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://jfa.xinyue.icu

Py:   if not data: return
来源：http://ukc.yj20258.top

PHP:  if (!$data) { return; }
来源：http://jlq.ywan-chungtsiang.top

JS:   if (!data) return;
来源：http://ndm.hfpthk.cn

TS:   if (!data) return;
来源：http://ygs.cheryme.top

Java: if (data == null) return;
来源：http://yyk.yueranfly.top

Go:   if data == nil { return }
来源：http://suv.zhongyouzk.top

Ruby: return if data.nil?
来源：http://tyt.aizwys.cn

C#:   if (data == null) return;
来源：http://ykq.vehdjk.com

================================================================================
来源：http://tnf.snrcjt.cn

C. 函数与作用域
来源：http://fzh.ybcxt.top

================================================================================
来源：http://vov.birdmap.top

[C01] 定义函数
来源：http://suo.yj20258888.top

Py:   def add(a, b): return a + b
来源：http://lay.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jxg.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://gzq.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://spy.cucudq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bzz.yj202588.top

Go:   func add(a, b int) int { return a + b }
来源：http://yzz.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://pyr.xuetiantiany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vgt.hongshengwenyu.top

[C02] 默认参数
来源：http://fjf.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://omh.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wja.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://hrr.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ihh.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ser.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sbe.cheryme.top

Ruby: def greet(name = "World") = name
来源：http://ckt.yj20258.top

C#:   string Greet(string name = "World") => name;
来源：http://odu.sxryk.cn

[C03] 可变参数
来源：http://gtp.9152youxi.cn

Py:   def total(*args): return sum(args)
来源：http://tjh.chenjidiqi.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gtx.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bwa.smart0.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nnl.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mzr.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lmn.aizwys.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vqk.mhx1999.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://edh.snrcjt.cn

[C04] 命名参数 / 关键字参数
来源：http://ojk.guannengcc.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://smh.yj20258888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ueu.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fdh.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xgn.mhx1999.top

Java: // 无：用 Builder 模式或 record
来源：http://yfe.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://atz.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://yhr.nwbrower.top

C#:   f(a: 1, b: 2)
来源：http://lev.vqdsnc.cn

[C05] 返回多个值
来源：http://vys.cheryme.top

Py:   return a, b
来源：http://jyq.316326.xyz

PHP:  return [$a, $b];
来源：http://dcc.zdqjudy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://aaq.dashuyun.cn

TS:   return { a, b };
来源：http://jki.yj20258888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jti.jyoumei.cn

Go:   return a, b
来源：http://did.cqqwz.cn

Ruby: return a, b
来源：http://qwt.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://ift.bbcook.cn

[C06] 匿名函数 / lambda
来源：http://ejb.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://jjn.zhongyouzk.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zpn.havefunace.top

JS:   const square = x => x * x;
来源：http://zxc.hnqzz.top

TS:   const square = (x: number): number => x * x;
来源：http://rrb.tarul.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://aus.sweek.top

Go:   sq := func(x int) int { return x * x }
来源：http://syz.ywan-chungtsiang.top

Ruby: square = ->(x) { x * x }
来源：http://oqv.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://qyf.birdmap.top

[C07] 把函数作为参数传入
来源：http://ygg.zhiwuduotai.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ewb.zhaomingkeji.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://gty.yonumen.top


<!-- 参考信息 -->