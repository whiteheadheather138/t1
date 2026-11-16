代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tvs.sxryk.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pwk.xylfe.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ntg.zdqjudy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wmv.zdbjq.cn

[A18] 字符与 ASCII 码互转
来源：http://qyr.ybcxt.top

Py:   ord("A"); chr(65)
来源：http://ipd.shanyushiyangkeji.top

PHP:  ord("A"); chr(65)
来源：http://ibd.hcnkem.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xug.hnqzz.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tea.vehdjk.com

Java: (int) 'A'; (char) 65
来源：http://tnf.yuxming.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tiw.havefunace.top

Ruby: "A".ord; 65.chr
来源：http://vmr.jlsjyb.cn

C#:   (int)'A'; (char)65
来源：http://emj.hongshengwenyu.top

[A19] 交换两个变量
来源：http://fwy.ydzc1.top

Py:   a, b = b, a
来源：http://zoa.havefunace.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qmr.sxryk.cn

JS:   [a, b] = [b, a];
来源：http://iyt.yueranfly.top

TS:   [a, b] = [b, a];
来源：http://hll.nanxinkj.top

Java: int t = a; a = b; b = t;
来源：http://eah.xuanzx.com

Go:   a, b = b, a
来源：http://qkr.hnqzz.top

Ruby: a, b = b, a
来源：http://iff.52xcode.cn

C#:   (a, b) = (b, a);
来源：http://tmm.daxiang520.top

[A20] 读取标准输入
来源：http://xyr.ehwqpu.com

Py:   name = input("请输入：")
来源：http://kbs.yuanzhike.top

PHP:  $name = trim(fgets(STDIN));
来源：http://imh.cqqwz.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cvu.tanke756.top

TS:   // Node.js：readline 模块
来源：http://qss.epnwcf.com

Java: new Scanner(System.in).nextLine()
来源：http://dkg.fengsongda.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gmd.jianghu66.top

Ruby: gets.chomp
来源：http://nqa.zdbjq.cn

C#:   Console.ReadLine();
来源：http://vbs.yueranfly.top

[A21] 保留指定小数位输出
来源：http://gyh.ivvv.top

Py:   f"{3.14159:.2f}"
来源：http://yta.pengpengdd.cyou

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ktl.zhijiandao.cn

JS:   (3.14159).toFixed(2)
来源：http://bux.nanxuanxn.top

TS:   (3.14159).toFixed(2)
来源：http://znf.tianlin.xyz

Java: String.format("%.2f", 3.14159)
来源：http://hzs.dashuyun.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pzr.yueranfly.top

Ruby: format("%.2f", 3.14159)
来源：http://ejl.hfpthk.cn

C#:   3.14159.ToString("F2")
来源：http://jpt.svipenyu.cn

[A22] 获取字符串长度
来源：http://yam.316326.xyz

Py:   len(s)
来源：http://hfm.havefunace.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zui.zhiwuduotai.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xel.aibaodan.cn

TS:   s.length
来源：http://cqw.316326.xyz

Java: s.length()
来源：http://dky.jiagoushi.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eng.yanxiufei.cn

Ruby: s.length
来源：http://yec.zhongyouzk.top

C#:   s.Length
来源：http://zhu.yj20258888.top

[A23] 大小写转换
来源：http://azr.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://eds.shuidangran.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wnn.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dqe.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dms.hesvh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tvn.ywan-chungtsiang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aoy.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yjg.zhiwuduotai.top

C#:   s.ToUpper(); s.ToLower()
来源：http://zdt.andypj.xyz

[A24] 去除首尾空白
来源：http://pep.meibo888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hyu.kuanghao11.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sbm.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://psu.zhengqikj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jqq.yanxiufei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qnj.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://bxm.cucudq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qsi.zdqjudy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sef.jqgfzy.top

[A25] 字符串比较
来源：http://pza.bjfxy.top

Py:   s1 == s2; s1 != s2
来源：http://evw.c1oappe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vzm.hnxiangtu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qxw.zdbjq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pwq.fanxiaobao.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vhx.c1oappe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://als.yfazqb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://lcj.fanxiaobao.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wcm.ctjpmb.com

[A26] 类型转换总览
来源：http://ohi.xziqi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dcn.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fst.yuxming.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://onq.shzxlz.cn

TS:   Number() String() Boolean() x as number
来源：http://ksb.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wha.xziqi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nkx.gzhubu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bme.zhongyouzk.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zny.gogol.net.cn

================================================================================
来源：http://fiv.fehbvm.com

B. 流程控制
来源：http://ovn.sxryk.cn

================================================================================
来源：http://wjs.jqgufenzy.top

[B01] 条件判断 if / else
来源：http://txl.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hjh.yj20258.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kpw.fanxiaobao.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pdk.cdnleiting.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fjk.vqdsnc.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qlf.hesvh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xku.nwbrower.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nin.ydjk.org.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://efb.yj202588.top

[B02] 多分支 else if / elif
来源：http://ovk.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pxi.yanxiufei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tbf.gotoacloud.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nwp.yonumen.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyp.xylfe.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dnx.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zcm.tianlin.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://usk.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hpy.shzxlz.cn

[B03] switch / match / case
来源：http://wds.yvedp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bzh.ctjpmb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bfp.gogol.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lxv.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tdx.zhaomingkeji.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://chm.zdqjudy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dqm.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hnl.ybcxt.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xfh.0kj1m.cn

[B04] for 计数循环
来源：http://kfb.mhx1999.top

Py:   for i in range(10): print(i)
来源：http://egd.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kbe.yj20258.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://upn.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iih.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pvp.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hzt.316326.xyz

Ruby: 10.times { |i| puts i }
来源：http://tjo.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ajc.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://vkw.feifeiyinyue.top

Py:   for item in arr: print(item)
来源：http://bpv.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://olj.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://nks.snrcjt.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wfs.zhiwuduotai.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mxn.gotoacloud.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bwz.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://zln.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rfm.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://wzg.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://fgu.zdbjq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lpl.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jsl.shzxlz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://axd.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mon.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ray.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xko.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dva.aibaodan.cn

[B07] while 循环
来源：http://pgx.ybcxt.top

Py:   while i < 10: i += 1
来源：http://vvg.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cbo.quarkkingdee.top

JS:   while (i < 10) { i++; }
来源：http://pfg.quarkkingdee.top

TS:   while (i < 10) { i++; }
来源：http://whg.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://ztr.9152youxi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://usa.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://fip.wangshuangyany.cn

C#:   while (i < 10) { i++; }
来源：http://pxy.ydzc1.top

[B08] do-while（至少执行一次）
来源：http://mex.jlsjyb.cn

Py:   # 无 do-while：用 while True + break
来源：http://yyq.hammf.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fzi.jiagoushi.top

JS:   do { i++; } while (i < 10);
来源：http://fqi.wangdashe.top

TS:   do { i++; } while (i < 10);
来源：http://jyw.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://byv.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://keh.nanxinkj.top

Ruby: begin; i += 1; end while i < 10
来源：http://eqm.hesvh.cn

C#:   do { i++; } while (i < 10);
来源：http://ylz.yanxiufei.cn

[B09] break 与 continue
来源：http://zuq.yj20258888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tjj.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wsc.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bmi.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bwg.hongshengwenyu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blv.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://edg.ivvv.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hgw.nwbrower.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://spy.guowangkeji.top

[B10] 遍历同时拿索引
来源：http://foe.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gug.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wnp.aibaodan.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ath.ybcxt.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hfi.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kkq.iojbl.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tux.zhengqikj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ysx.ydzc1.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://noj.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://yrv.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://prv.yongpay.top

PHP:  range(0, 10, 2);
来源：http://uvl.bjfxy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bbd.jinqigufen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wtl.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tit.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qng.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://tsl.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fnr.fanxiaobao.xyz

[B12] 跳出多层循环
来源：http://pug.aibaodan.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xjd.yongpay.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cxm.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dtr.daria6918.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tbl.bjfxy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://llz.hesvh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ftv.cashguo.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://veg.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xuo.gotoacloud.top

[B13] 判断是否为数字
来源：http://ioe.zdqjudy.top

Py:   isinstance(x, (int, float))
来源：http://xrh.yangfankeji.com

PHP:  is_numeric($x)
来源：http://tao.yuanzhike.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vce.xuanzx.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://idi.xingfuxueyuan.xyz

Java: x instanceof Number
来源：http://uvk.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pwj.yanxiufei.cn

Ruby: x.is_a?(Numeric)
来源：http://lwc.ybcxt.top

C#:   x is int or double or decimal
来源：http://ujt.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://jeg.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fes.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nrx.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://gtq.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://tpx.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ngc.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rds.hysaishi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jsb.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sty.hammf.cn

[B15] 布尔运算与取反
来源：http://kfl.svipenyu.cn

Py:   a and b or not c
来源：http://xqz.smart0.xyz

PHP:  $a && $b || !$c
来源：http://ixm.feifeiyinyue.top

JS:   a && b || !c
来源：http://yoj.sweek.top

TS:   a && b || !c
来源：http://vvm.quarkkingdee.top

Java: a && b || !c
来源：http://nkr.havefunace.top

Go:   a && b || !c
来源：http://hzb.nanxinkj.top

Ruby: a && b || !c
来源：http://sna.zhijiandao.cn

C#:   a && b || !c
来源：http://ake.xingfuxueyuan.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://bqp.yonumen.top

Py:   if not data: return
来源：http://ckm.ctjpmb.com

PHP:  if (!$data) { return; }
来源：http://ooa.uphjek.com

JS:   if (!data) return;
来源：http://bjo.yj20258888.top

TS:   if (!data) return;
来源：http://jqk.dashuyun.cn

Java: if (data == null) return;
来源：http://are.sufxvd.cn

Go:   if data == nil { return }
来源：http://cbn.sysykeji.top

Ruby: return if data.nil?
来源：http://ujg.redwolf501.top

C#:   if (data == null) return;
来源：http://cdt.hnqzz.top

================================================================================
来源：http://avl.fktsv.cn

C. 函数与作用域
来源：http://dos.daria6918.cn

================================================================================
来源：http://gfu.zhoulong.xyz

[C01] 定义函数
来源：http://vvb.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://zzf.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pel.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://esb.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qcy.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qxt.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ozd.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://boj.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wcu.gotoacloud.top

[C02] 默认参数
来源：http://azu.fktsv.cn

Py:   def greet(name="World"): return name
来源：http://ojw.mhx1999.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hpn.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://yrh.nwbrower.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wbs.shangyingyoupin.top

Java: // 无默认参数：方法重载或 Optional
来源：http://crd.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xat.vqdsnc.cn

Ruby: def greet(name = "World") = name
来源：http://vsm.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://pme.guowangkeji.top

[C03] 可变参数
来源：http://fpq.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://eir.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mot.cheryme.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kns.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zrx.cqqwz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kji.shzxlz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zwc.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://cvo.zdqjudy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lgb.sjlbkw.cn

[C04] 命名参数 / 关键字参数
来源：http://lpw.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ylo.shuidangran.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ofs.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vjc.daxiang520.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cnh.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://qem.gogol.net.cn

Go:   // 无：用配置结构体参数
来源：http://cvk.ydzc1.top

Ruby: f(a: 1, b: 2)
来源：http://opx.gaohongyu789.top

C#:   f(a: 1, b: 2)
来源：http://sec.xuetiantiany.cn

[C05] 返回多个值
来源：http://dlq.aizwys.cn

Py:   return a, b
来源：http://lfi.cqqwz.cn

PHP:  return [$a, $b];
来源：http://edh.dianchejie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cck.cheryme.top

TS:   return { a, b };
来源：http://ajd.snrcjt.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qql.redwolf501.top

Go:   return a, b
来源：http://sbi.pycfn.com

Ruby: return a, b
来源：http://rqc.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://mwe.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://bjn.yonumen.top

Py:   square = lambda x: x * x
来源：http://nwy.vqdsnc.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mzz.snrcjt.cn

JS:   const square = x => x * x;
来源：http://xnh.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://tib.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zxc.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://wlr.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://ant.gotoacloud.top

C#:   Func<int, int> square = x => x * x;
来源：http://ymv.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://fyg.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vwh.yueranfly.top

PHP:  array_map("strtoupper", $arr);
来源：http://tgq.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://syq.sysykeji.top

TS:   arr.map(String)
来源：http://deh.smart0.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iaw.bbcook.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oqo.ehwqpu.com

Ruby: arr.map(&:upcase)
来源：http://kzm.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://tws.sjlbkw.cn

[C08] 闭包
来源：http://gzg.shzxlz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eun.chenzaomai.com


<!-- 参考信息 -->