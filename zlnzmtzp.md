代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://jiu.zycfv.cn

Py:   ord("A"); chr(65)
来源：http://qsa.chenzaomai.com

PHP:  ord("A"); chr(65)
来源：http://nfy.gzhubu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cgz.jqgfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lzz.chenzaomai.com

Java: (int) 'A'; (char) 65
来源：http://drf.ybcxt.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jps.cashguo.top

Ruby: "A".ord; 65.chr
来源：http://ecx.daria6918.cn

C#:   (int)'A'; (char)65
来源：http://vkr.jianghu66.top

[A19] 交换两个变量
来源：http://tvp.ehwqpu.com

Py:   a, b = b, a
来源：http://spm.kuanghao11.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mom.jyoumei.cn

JS:   [a, b] = [b, a];
来源：http://frx.shanyushiyangkeji.top

TS:   [a, b] = [b, a];
来源：http://qlj.gzhubu.top

Java: int t = a; a = b; b = t;
来源：http://gji.hnqzz.top

Go:   a, b = b, a
来源：http://zsu.gzhubu.top

Ruby: a, b = b, a
来源：http://kmd.andypj.xyz

C#:   (a, b) = (b, a);
来源：http://shp.fktsv.cn

[A20] 读取标准输入
来源：http://wcn.zhiwuduotai.top

Py:   name = input("请输入：")
来源：http://jrj.bbcook.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ekh.ydzc1.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wwb.smart0.xyz

TS:   // Node.js：readline 模块
来源：http://sdh.jinqigfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://lzm.zycfv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://myl.jinghuilouyu.cn

Ruby: gets.chomp
来源：http://lrn.tarul.cn

C#:   Console.ReadLine();
来源：http://ipy.xuetiantiany.cn

[A21] 保留指定小数位输出
来源：http://uly.meibo888.top

Py:   f"{3.14159:.2f}"
来源：http://ihb.zhongyouzk.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mzo.yuxming.cn

JS:   (3.14159).toFixed(2)
来源：http://dyp.yanxiufei.cn

TS:   (3.14159).toFixed(2)
来源：http://wxu.hammf.cn

Java: String.format("%.2f", 3.14159)
来源：http://phm.haohaochexian.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jou.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://xyj.zdbjq.cn

C#:   3.14159.ToString("F2")
来源：http://psf.gotoacloud.top

[A22] 获取字符串长度
来源：http://zep.sweek.top

Py:   len(s)
来源：http://pri.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://epu.hfpthk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kcl.hnxiangtu.top

TS:   s.length
来源：http://ezd.jqgufenzy.top

Java: s.length()
来源：http://okh.daxiang520.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fza.shangyingyoupin.top

Ruby: s.length
来源：http://tio.quarkkingdee.top

C#:   s.Length
来源：http://ijs.epnwcf.com

[A23] 大小写转换
来源：http://nat.52xcode.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sgh.hfpthk.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ukp.mhx1999.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mwc.yfazqb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tpc.hywenlv.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iyf.xinyue.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qds.xziqi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sfn.zhiwuduotai.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jql.ehwqpu.com

[A24] 去除首尾空白
来源：http://ccw.snrcjt.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ksm.yj20258.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lww.daxiang520.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://obm.vqdsnc.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fgf.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rwp.hysaishi.cn

Go:   strings.TrimSpace(s)
来源：http://bsh.xinyue.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://snw.dianchejie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oik.jiagoushi.top

[A25] 字符串比较
来源：http://lwq.nwbrower.top

Py:   s1 == s2; s1 != s2
来源：http://hrh.xuetiantiany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tmi.shzxlz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wjc.chenjidiqi.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ewn.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://efd.shuidangran.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://skc.jqgufenzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kvn.zhoulong.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ogj.zhengqikj.top

[A26] 类型转换总览
来源：http://ljz.mhx1999.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aqk.jqgufenzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mnc.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oxj.svipenyu.cn

TS:   Number() String() Boolean() x as number
来源：http://hst.jianghu66.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fiy.xingfuxueyuan.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ejy.shuidangran.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gyx.52xcode.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yes.fanxiaobao.xyz

================================================================================
来源：http://hur.ivvv.top

B. 流程控制
来源：http://kyp.cdnleiting.top

================================================================================
来源：http://cus.ywan-chungtsiang.top

[B01] 条件判断 if / else
来源：http://onz.zhiwuduotai.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mui.daxiang520.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fcx.yuanzhike.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yuc.jinqigfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xlg.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://fvp.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cit.zdqjudy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uzz.vehdjk.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jni.ctjpmb.com

[B02] 多分支 else if / elif
来源：http://nja.yongpay.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vir.redwolf501.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vif.jinqigfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mcy.tianlin.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rvc.ywan-chungtsiang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ljn.iojbl.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rcs.tian-w.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ubn.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ozu.yuxming.cn

[B03] switch / match / case
来源：http://xhz.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dcv.xziqi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wby.shzxlz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dxj.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bqd.aizwys.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kij.0kj1m.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qlt.jianghu66.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ret.tarul.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vzr.jinghuilouyu.cn

[B04] for 计数循环
来源：http://ajc.chenjidiqi.icu

Py:   for i in range(10): print(i)
来源：http://zbq.jinqigfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gbn.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qru.hywenlv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nvu.sjlbkw.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gfw.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rcd.chenzaomai.com

Ruby: 10.times { |i| puts i }
来源：http://zkn.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vgg.nanxuanxn.top

[B05] 遍历数组 / 列表
来源：http://jzl.mhx1999.top

Py:   for item in arr: print(item)
来源：http://jxg.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://quj.jiagoushi.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xoy.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lrw.hesvh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cui.cdnleiting.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vbf.chenlongwang.top

Ruby: arr.each { |item| puts item }
来源：http://pym.hnqzz.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qmz.cdnleiting.top

[B06] 遍历字典 / 对象
来源：http://lrt.jiagoushi.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hlh.redwolf501.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cyf.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uib.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sdl.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dts.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ioy.tian-w.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nfm.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rmv.ywan-chungtsiang.top

[B07] while 循环
来源：http://tig.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://jwt.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://crb.jinqigufen.top

JS:   while (i < 10) { i++; }
来源：http://tlw.cucudq.cn

TS:   while (i < 10) { i++; }
来源：http://uyt.hesvh.cn

Java: while (i < 10) { i++; }
来源：http://kov.birdmap.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ads.316326.xyz

Ruby: while i < 10; i += 1; end
来源：http://tgp.nanxinkj.top

C#:   while (i < 10) { i++; }
来源：http://pfa.yonumen.top

[B08] do-while（至少执行一次）
来源：http://wjj.hammf.cn

Py:   # 无 do-while：用 while True + break
来源：http://yno.gaohongyu789.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yxa.yj20258888.top

JS:   do { i++; } while (i < 10);
来源：http://ekx.gaohongyu789.top

TS:   do { i++; } while (i < 10);
来源：http://joh.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://mwj.ydjk.org.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://taa.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://blq.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://qzi.chenjidiqi.icu

[B09] break 与 continue
来源：http://paw.ydzc1.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jlu.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zjs.aibaodan.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bfw.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://elb.cdnleiting.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://via.yonumen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://red.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sxi.wangshuangyany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://azx.havefunace.top

[B10] 遍历同时拿索引
来源：http://rnl.cheryme.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bwy.hfpthk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ism.gzhubu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://koe.zhengqikj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pjp.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rjr.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hif.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lsp.316326.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qjh.jyoumei.cn

[B11] 生成数字序列 / 区间
来源：http://ylq.hywenlv.cn

Py:   list(range(0, 10, 2))
来源：http://gvc.feifeiyinyue.top

PHP:  range(0, 10, 2);
来源：http://cpy.guowangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gqp.ywan-chungtsiang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xtr.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://duk.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mnj.aizwys.cn

Ruby: (0...10).step(2).to_a
来源：http://cvq.wangdashe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pei.uphjek.com

[B12] 跳出多层循环
来源：http://zpv.zdbjq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jcv.jlsjyb.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://urh.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yti.316326.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kvk.jinqigfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qja.jqgufenzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xpk.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gst.c1oappe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bmm.316326.xyz

[B13] 判断是否为数字
来源：http://nwr.smart0.xyz

Py:   isinstance(x, (int, float))
来源：http://ftc.hammf.cn

PHP:  is_numeric($x)
来源：http://blo.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://egc.ivvv.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vxt.iojbl.cn

Java: x instanceof Number
来源：http://jtd.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rms.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://par.uphjek.com

C#:   x is int or double or decimal
来源：http://cbp.pycfn.com

[B14] 判断值是否在集合内
来源：http://cbc.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fiu.zhixingplan.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oua.shangyingyoupin.top

JS:   [1, 2, 3].includes(x)
来源：http://yth.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://zcx.hnqzz.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ovh.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iyv.sysykeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://wgg.cheryme.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zsg.yueranfly.top

[B15] 布尔运算与取反
来源：http://ufm.nanxuanxn.top

Py:   a and b or not c
来源：http://awj.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://fqi.zhijiandao.cn

JS:   a && b || !c
来源：http://gej.sysykeji.top

TS:   a && b || !c
来源：http://lbj.wangshuangyany.cn

Java: a && b || !c
来源：http://cjk.hnqzz.top

Go:   a && b || !c
来源：http://yqt.xylfe.cn

Ruby: a && b || !c
来源：http://ucw.yj20258.top

C#:   a && b || !c
来源：http://qih.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qbu.0kj1m.cn

Py:   if not data: return
来源：http://tne.smart0.xyz

PHP:  if (!$data) { return; }
来源：http://gya.fktsv.cn

JS:   if (!data) return;
来源：http://rwt.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://zlq.guannengcc.top

Java: if (data == null) return;
来源：http://len.mhx1999.top

Go:   if data == nil { return }
来源：http://vao.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://lxe.sxryk.cn

C#:   if (data == null) return;
来源：http://mop.hywenlv.cn

================================================================================
来源：http://cau.yanxiufei.cn

C. 函数与作用域
来源：http://zlu.gogol.net.cn

================================================================================
来源：http://jbe.pengpengdd.cyou

[C01] 定义函数
来源：http://ucr.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://cae.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lfi.hcnkem.com

JS:   function add(a, b) { return a + b; }
来源：http://vro.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rsb.wangdashe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xpe.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gcr.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://alg.yuanzhike.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rpn.sysykeji.top

[C02] 默认参数
来源：http://ysi.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://zor.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://yxz.havefunace.top

JS:   function greet(name = "World") { return name; }
来源：http://cmn.tianlin.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://bcv.andypj.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://cfa.quarkkingdee.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ppa.jianghu66.top

Ruby: def greet(name = "World") = name
来源：http://gri.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://zfu.fanxiaobao.xyz

[C03] 可变参数
来源：http://jbk.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://ufw.wangdashe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://txx.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fzj.zycfv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jlc.haohaochexian.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zkk.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nbo.havefunace.top

Ruby: def total(*nums); nums.sum; end
来源：http://lri.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ncn.ivvv.top

[C04] 命名参数 / 关键字参数
来源：http://sgp.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ifc.hcnkem.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rin.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qsr.sxryk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ptv.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://led.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://lqm.yj202588.top

Ruby: f(a: 1, b: 2)
来源：http://eci.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://rwb.shanyushiyangtech.top

[C05] 返回多个值
来源：http://twm.cqqwz.cn

Py:   return a, b
来源：http://nlu.cqqwz.cn

PHP:  return [$a, $b];
来源：http://pvx.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jgw.jlsjyb.cn

TS:   return { a, b };
来源：http://nlo.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iwr.birdmap.top

Go:   return a, b
来源：http://vns.bjfxy.top

Ruby: return a, b
来源：http://fqv.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://yhb.aizwys.cn

[C06] 匿名函数 / lambda
来源：http://zqt.zhoulong.xyz

Py:   square = lambda x: x * x
来源：http://frf.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yvm.hammf.cn

JS:   const square = x => x * x;
来源：http://egs.tarul.cn

TS:   const square = (x: number): number => x * x;
来源：http://gxs.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jgp.yonumen.top

Go:   sq := func(x int) int { return x * x }
来源：http://oyy.hnqzz.top

Ruby: square = ->(x) { x * x }
来源：http://rqo.316326.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://mxo.jinghuilouyu.cn

[C07] 把函数作为参数传入
来源：http://kkt.daria6918.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://khe.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://otx.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vvn.zhijiandao.cn

TS:   arr.map(String)
来源：http://ygz.yonumen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rao.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dtb.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://pwk.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://glb.316326.xyz

[C08] 闭包
来源：http://tky.zhiwuduotai.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qes.bbcook.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fqs.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://edx.hnqzz.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mrh.ppjwa.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eup.yangfankeji.com


<!-- 参考信息 -->