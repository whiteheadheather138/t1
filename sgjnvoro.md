代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://pqp.jinyuanbaomall.cn

Py:   ord("A"); chr(65)
来源：http://gkz.sxryk.cn

PHP:  ord("A"); chr(65)
来源：http://rry.yuxming.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zny.xuanzx.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eij.tarul.cn

Java: (int) 'A'; (char) 65
来源：http://jlm.wangdashe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://scl.ctjpmb.com

Ruby: "A".ord; 65.chr
来源：http://yzl.yj20258.top

C#:   (int)'A'; (char)65
来源：http://xdg.ydjk.org.cn

[A19] 交换两个变量
来源：http://kby.zhoulong.xyz

Py:   a, b = b, a
来源：http://jbh.xylfe.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fdc.jqgufenzy.top

JS:   [a, b] = [b, a];
来源：http://ucn.fanxiaobao.xyz

TS:   [a, b] = [b, a];
来源：http://xuv.quarkkingdee.top

Java: int t = a; a = b; b = t;
来源：http://maj.shanyushiyangkeji.top

Go:   a, b = b, a
来源：http://qgg.ppjwa.cn

Ruby: a, b = b, a
来源：http://ygv.hnxiangtu.top

C#:   (a, b) = (b, a);
来源：http://voa.xuanzx.com

[A20] 读取标准输入
来源：http://bms.ivvv.top

Py:   name = input("请输入：")
来源：http://ikd.pycfn.com

PHP:  $name = trim(fgets(STDIN));
来源：http://oap.fehbvm.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wev.xziqi.cn

TS:   // Node.js：readline 模块
来源：http://glm.vqdsnc.cn

Java: new Scanner(System.in).nextLine()
来源：http://stp.shanyushiyangkeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ifn.yfazqb.com

Ruby: gets.chomp
来源：http://wxj.yangfankeji.com

C#:   Console.ReadLine();
来源：http://mue.tianlin.xyz

[A21] 保留指定小数位输出
来源：http://fvb.yuanzhike.top

Py:   f"{3.14159:.2f}"
来源：http://zdj.zhixingplan.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qug.sufxvd.cn

JS:   (3.14159).toFixed(2)
来源：http://uud.fanxiaobao.xyz

TS:   (3.14159).toFixed(2)
来源：http://eas.zhixingplan.top

Java: String.format("%.2f", 3.14159)
来源：http://zcz.yj202588.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oyg.pycfn.com

Ruby: format("%.2f", 3.14159)
来源：http://gfp.meibo888.top

C#:   3.14159.ToString("F2")
来源：http://vql.chenlongwang.top

[A22] 获取字符串长度
来源：http://nen.sysykeji.top

Py:   len(s)
来源：http://ylz.jqgufenzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wjg.ywan-chungtsiang.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cyo.bbcook.cn

TS:   s.length
来源：http://bgw.xingfuxueyuan.xyz

Java: s.length()
来源：http://zez.yangfankeji.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vqy.yangfankeji.com

Ruby: s.length
来源：http://mqq.yj20258.top

C#:   s.Length
来源：http://kud.bjfxy.top

[A23] 大小写转换
来源：http://hbt.iojbl.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mko.9152youxi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sot.jianghu66.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://udk.yongpay.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iew.svipenyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qpu.zhiwuduotai.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://okb.ppjwa.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mkd.zhongyouzk.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qlq.ydjk.org.cn

[A24] 去除首尾空白
来源：http://aeu.vqdsnc.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ysr.wangdashe.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cil.yj20258888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://txi.aizwys.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sdb.jinqigufen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fhb.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://dsr.zhiwuduotai.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ssp.bbcook.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://unv.hongshengwenyu.top

[A25] 字符串比较
来源：http://yrk.316326.xyz

Py:   s1 == s2; s1 != s2
来源：http://quy.ywan-chungtsiang.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nly.shangyingyoupin.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fiz.yonumen.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gum.vehdjk.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lem.jianghu66.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://guo.hesvh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zjz.jqgufenzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pux.fktsv.cn

[A26] 类型转换总览
来源：http://nlt.hcnkem.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yjj.birdmap.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qku.andypj.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zik.cashguo.top

TS:   Number() String() Boolean() x as number
来源：http://jbz.yuxming.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ryb.zycfv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nao.nanxinkj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ugf.fehbvm.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zyu.xinyue.icu

================================================================================
来源：http://snv.nanxuanxn.top

B. 流程控制
来源：http://gco.tarul.cn

================================================================================
来源：http://gan.gaohongyu789.top

[B01] 条件判断 if / else
来源：http://szx.ydzc1.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vaw.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hss.redwolf501.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fwo.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kpf.sysykeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hdl.pengpengdd.cyou

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dqy.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dav.epnwcf.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jao.shuidangran.top

[B02] 多分支 else if / elif
来源：http://uxx.hnxiangtu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xux.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yai.sysykeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pim.9152youxi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yfv.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://stv.zdbjq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xhu.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pwj.fengsongda.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yvd.birdmap.top

[B03] switch / match / case
来源：http://tqc.hesvh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tub.yfazqb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://upz.hywenlv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ndl.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zqy.cqqwz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://akz.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tvo.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lsl.ybcxt.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://idz.cqqwz.cn

[B04] for 计数循环
来源：http://swi.yj202588.top

Py:   for i in range(10): print(i)
来源：http://otg.jqgfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yvm.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jbe.pengpengdd.cyou

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://znr.dianchejie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xlm.yfazqb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tul.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://cfi.jyoumei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xms.jinqigfzy.top

[B05] 遍历数组 / 列表
来源：http://idc.snrcjt.cn

Py:   for item in arr: print(item)
来源：http://wnk.gzhubu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hbz.shanyushiyangtech.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mdn.hongshengwenyu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://laf.xinyue.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://yys.svipenyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yxc.shangyingyoupin.top

Ruby: arr.each { |item| puts item }
来源：http://kxx.zhoulong.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ymg.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://kil.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://pdk.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ajs.vqdsnc.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xnj.hnxiangtu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cef.ehwqpu.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qxf.ppjwa.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://okv.ydzc1.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ysx.xylfe.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dhz.shuidangran.top

[B07] while 循环
来源：http://uhk.jianghu66.top

Py:   while i < 10: i += 1
来源：http://mmk.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://apy.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://vec.smart0.xyz

TS:   while (i < 10) { i++; }
来源：http://ptl.guannengcc.top

Java: while (i < 10) { i++; }
来源：http://gzx.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jzv.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://xym.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://xpf.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://brh.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://kda.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://wbl.yj20258.top

JS:   do { i++; } while (i < 10);
来源：http://svz.daxiang520.top

TS:   do { i++; } while (i < 10);
来源：http://vsq.c1oappe.top

Java: do { i++; } while (i < 10);
来源：http://iyz.ivvv.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xho.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://hyh.epnwcf.com

C#:   do { i++; } while (i < 10);
来源：http://nfs.xziqi.cn

[B09] break 与 continue
来源：http://law.ydzc1.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qsr.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vcx.sweek.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixn.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qij.jlsjyb.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hzg.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://woc.jinyuanbaomall.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jvt.zdbjq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uow.cucudq.cn

[B10] 遍历同时拿索引
来源：http://gnm.tanke756.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wlq.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bcj.shzxlz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bue.jqgufenzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ctu.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pux.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wow.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ixk.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dnv.zhoulong.xyz

[B11] 生成数字序列 / 区间
来源：http://owe.gaohongyu789.top

Py:   list(range(0, 10, 2))
来源：http://csd.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://naq.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lzx.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hfh.vqdsnc.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gfo.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vmr.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://ecg.shanyushiyangtech.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://shs.cucudq.cn

[B12] 跳出多层循环
来源：http://daz.uphjek.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://sec.zhiwuduotai.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vqx.sufxvd.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lsu.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ldh.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wor.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ofx.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wpc.kuanghao11.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xsb.zycfv.cn

[B13] 判断是否为数字
来源：http://xla.jinghuilouyu.cn

Py:   isinstance(x, (int, float))
来源：http://ifv.xylfe.cn

PHP:  is_numeric($x)
来源：http://vew.sweek.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nfu.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hvc.kuanghao11.cn

Java: x instanceof Number
来源：http://tis.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mcv.yuanzhike.top

Ruby: x.is_a?(Numeric)
来源：http://ywx.316326.xyz

C#:   x is int or double or decimal
来源：http://llb.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://ajz.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aww.vehdjk.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eej.bjfxy.top

JS:   [1, 2, 3].includes(x)
来源：http://bvh.fzhhl.top

TS:   [1, 2, 3].includes(x)
来源：http://eif.fktsv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bvf.ybcxt.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qqx.yuanzhike.top

Ruby: [1, 2, 3].include?(x)
来源：http://dvs.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pcy.gaohongyu789.top

[B15] 布尔运算与取反
来源：http://yed.ehwqpu.com

Py:   a and b or not c
来源：http://tah.fzhhl.top

PHP:  $a && $b || !$c
来源：http://lwi.fanxiaobao.xyz

JS:   a && b || !c
来源：http://yxm.yueranfly.top

TS:   a && b || !c
来源：http://qrn.jiagoushi.top

Java: a && b || !c
来源：http://dux.daria6918.cn

Go:   a && b || !c
来源：http://tvs.ydjk.org.cn

Ruby: a && b || !c
来源：http://dpl.guowangkeji.top

C#:   a && b || !c
来源：http://vuk.chenzaomai.com

[B16] 卫语句：不满足条件提前返回
来源：http://yqe.zhoulong.xyz

Py:   if not data: return
来源：http://oxf.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://zlz.yueranfly.top

JS:   if (!data) return;
来源：http://sms.smart0.xyz

TS:   if (!data) return;
来源：http://yhy.fengsongda.top

Java: if (data == null) return;
来源：http://opc.smart0.xyz

Go:   if data == nil { return }
来源：http://vrw.hesvh.cn

Ruby: return if data.nil?
来源：http://tgg.fehbvm.com

C#:   if (data == null) return;
来源：http://zcx.nanxinkj.top

================================================================================
来源：http://zen.havefunace.top

C. 函数与作用域
来源：http://slr.hesvh.cn

================================================================================
来源：http://wva.zhijiandao.cn

[C01] 定义函数
来源：http://vxr.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://tet.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baa.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://yaa.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wxo.tarul.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wwi.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cxh.zdbjq.cn

Ruby: def add(a, b); a + b; end
来源：http://gpz.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pdm.pycfn.com

[C02] 默认参数
来源：http://jxa.hnxiangtu.top

Py:   def greet(name="World"): return name
来源：http://qhw.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://upk.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://sll.tianlin.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://tpx.vehdjk.com

Java: // 无默认参数：方法重载或 Optional
来源：http://vbf.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://src.shzxlz.cn

Ruby: def greet(name = "World") = name
来源：http://alc.shuidangran.top

C#:   string Greet(string name = "World") => name;
来源：http://unm.fktsv.cn

[C03] 可变参数
来源：http://ydh.xingfuxueyuan.xyz

Py:   def total(*args): return sum(args)
来源：http://txx.shanyushiyangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://myu.xinyue.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xuu.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mml.smart0.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ddm.9152youxi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cgd.iojbl.cn

Ruby: def total(*nums); nums.sum; end
来源：http://grd.hammf.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oqk.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://tfx.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wdq.xylfe.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dtz.xuanzx.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hed.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pag.gaohongyu789.top

Java: // 无：用 Builder 模式或 record
来源：http://yxk.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://npp.gogol.net.cn

Ruby: f(a: 1, b: 2)
来源：http://mmr.yonumen.top

C#:   f(a: 1, b: 2)
来源：http://wkc.hnxiangtu.top

[C05] 返回多个值
来源：http://mzd.guannengcc.top

Py:   return a, b
来源：http://upj.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://uub.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ays.shanyushiyangtech.top

TS:   return { a, b };
来源：http://dxm.shzxlz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lbu.hongshengwenyu.top

Go:   return a, b
来源：http://uyi.zhengqikj.top

Ruby: return a, b
来源：http://rrs.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://wic.cashguo.top

[C06] 匿名函数 / lambda
来源：http://uhs.jinyuanbaomall.cn

Py:   square = lambda x: x * x
来源：http://ord.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jef.zdqjudy.top

JS:   const square = x => x * x;
来源：http://fot.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://vsr.hammf.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iga.0kj1m.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xkx.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://uow.ctjpmb.com

C#:   Func<int, int> square = x => x * x;
来源：http://tih.sjlbkw.cn

[C07] 把函数作为参数传入
来源：http://qlj.guowangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nus.epnwcf.com

PHP:  array_map("strtoupper", $arr);
来源：http://uqn.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://boo.jinqigufen.top

TS:   arr.map(String)
来源：http://kwl.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zlb.yonumen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rbo.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://ddx.yuxming.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qvo.vqdsnc.cn

[C08] 闭包
来源：http://wye.daxiang520.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lnh.pengpengdd.cyou

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mdn.aibaodan.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oiv.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qtw.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wzn.hammf.cn


<!-- 参考信息 -->