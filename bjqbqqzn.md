代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bow.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oxf.dashuyun.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qet.jqgufenzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xxl.cdnleiting.top

[A18] 字符与 ASCII 码互转
来源：http://qij.cucudq.cn

Py:   ord("A"); chr(65)
来源：http://xkj.tanke756.top

PHP:  ord("A"); chr(65)
来源：http://tuw.316326.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://clh.hcnkem.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mwi.shangyingyoupin.top

Java: (int) 'A'; (char) 65
来源：http://fes.gogol.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rxz.bjfxy.top

Ruby: "A".ord; 65.chr
来源：http://ujh.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://suj.yuxming.cn

[A19] 交换两个变量
来源：http://jlk.zhijiandao.cn

Py:   a, b = b, a
来源：http://uqc.shzxlz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pht.nanxuanxn.top

JS:   [a, b] = [b, a];
来源：http://rzt.quarkkingdee.top

TS:   [a, b] = [b, a];
来源：http://egn.gotoacloud.top

Java: int t = a; a = b; b = t;
来源：http://kjx.hnxiangtu.top

Go:   a, b = b, a
来源：http://mos.ehwqpu.com

Ruby: a, b = b, a
来源：http://zrk.xuetiantiany.cn

C#:   (a, b) = (b, a);
来源：http://jdb.zdbjq.cn

[A20] 读取标准输入
来源：http://mmd.yuxming.cn

Py:   name = input("请输入：")
来源：http://kaj.9152youxi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rwq.birdmap.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pvc.tarul.cn

TS:   // Node.js：readline 模块
来源：http://hwy.daxiang520.top

Java: new Scanner(System.in).nextLine()
来源：http://wyh.smart0.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kgr.9152youxi.cn

Ruby: gets.chomp
来源：http://qmm.zhijiandao.cn

C#:   Console.ReadLine();
来源：http://qrj.gogol.net.cn

[A21] 保留指定小数位输出
来源：http://wta.nanxuanxn.top

Py:   f"{3.14159:.2f}"
来源：http://ngq.ehwqpu.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lbx.hywenlv.cn

JS:   (3.14159).toFixed(2)
来源：http://ffy.redwolf501.top

TS:   (3.14159).toFixed(2)
来源：http://xug.hcnkem.com

Java: String.format("%.2f", 3.14159)
来源：http://smq.andypj.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kxl.ydzc1.top

Ruby: format("%.2f", 3.14159)
来源：http://fga.meibo888.top

C#:   3.14159.ToString("F2")
来源：http://cfr.xylfe.cn

[A22] 获取字符串长度
来源：http://miz.yangfankeji.com

Py:   len(s)
来源：http://muv.jinqigfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hiw.hcnkem.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://auc.wangshuangyany.cn

TS:   s.length
来源：http://bou.nwbrower.top

Java: s.length()
来源：http://qax.hammf.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sjo.birdmap.top

Ruby: s.length
来源：http://fub.sysykeji.top

C#:   s.Length
来源：http://rjt.yongpay.top

[A23] 大小写转换
来源：http://gql.epnwcf.com

Py:   s.upper(); s.lower(); s.title()
来源：http://rgh.sxryk.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lgu.hysaishi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xmy.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://acg.zdbjq.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fxs.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rar.quarkkingdee.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gep.yuanzhike.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rdg.chenzaomai.com

[A24] 去除首尾空白
来源：http://nrw.zycfv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yjp.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fvt.tarul.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kiw.nanxuanxn.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fcu.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xrm.c1oappe.top

Go:   strings.TrimSpace(s)
来源：http://yus.cucudq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vtk.zycfv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rag.shzxlz.cn

[A25] 字符串比较
来源：http://uai.meibo888.top

Py:   s1 == s2; s1 != s2
来源：http://bpc.feifeiyinyue.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qpj.yj20258888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iht.jlsjyb.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://whp.yongpay.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xjn.9152youxi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iol.zhijiandao.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cgu.wangdashe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hno.redwolf501.top

[A26] 类型转换总览
来源：http://tws.yj202588.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://osk.yvedp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ayt.zdqjudy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nkb.nanxuanxn.top

TS:   Number() String() Boolean() x as number
来源：http://gzb.vqdsnc.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qow.redwolf501.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tau.wangdashe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ygr.guowangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ghg.jianghu66.top

================================================================================
来源：http://eir.aizwys.cn

B. 流程控制
来源：http://tcc.jqgufenzy.top

================================================================================
来源：http://fua.uphjek.com

[B01] 条件判断 if / else
来源：http://ync.sjlbkw.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bbn.hammf.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rki.sweek.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wls.nanxuanxn.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ykt.cdnleiting.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vwk.cqqwz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://obh.xziqi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eih.52xcode.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gtz.bbcook.cn

[B02] 多分支 else if / elif
来源：http://kjm.yangfankeji.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sfy.52xcode.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ckt.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jnv.daxiang520.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blo.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tkc.jianghu66.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eoh.zhengqikj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kba.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oua.meibo888.top

[B03] switch / match / case
来源：http://oxl.bbcook.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nfp.chenzaomai.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ufr.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hmo.cdnleiting.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kkk.hywenlv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hqj.zdbjq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fko.hywenlv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lpv.shanyushiyangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fgy.sjlbkw.cn

[B04] for 计数循环
来源：http://hwc.fengsongda.top

Py:   for i in range(10): print(i)
来源：http://zjs.xziqi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://raf.zhoulong.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fls.vqdsnc.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yit.ppjwa.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hcr.daxiang520.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wgp.snrcjt.cn

Ruby: 10.times { |i| puts i }
来源：http://dku.snrcjt.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yyq.316326.xyz

[B05] 遍历数组 / 列表
来源：http://qhd.feifeiyinyue.top

Py:   for item in arr: print(item)
来源：http://xxf.daria6918.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oji.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nqp.yuanzhike.top

TS:   for (const item of arr) { console.log(item); }
来源：http://brl.aizwys.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sqv.xuetiantiany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qcg.chenjidiqi.icu

Ruby: arr.each { |item| puts item }
来源：http://cxk.cashguo.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ynj.shuidangran.top

[B06] 遍历字典 / 对象
来源：http://mrs.tanke756.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ncx.shanyushiyangtech.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blr.zhaomingkeji.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ytl.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sok.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yya.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mfe.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://llo.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zoa.sxryk.cn

[B07] while 循环
来源：http://mjo.hongshengwenyu.top

Py:   while i < 10: i += 1
来源：http://wjr.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://por.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://lmx.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://fir.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://iff.jqgufenzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eks.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://jbe.zdqjudy.top

C#:   while (i < 10) { i++; }
来源：http://ylq.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://yen.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://fxw.tanke756.top

PHP:  do { $i++; } while ($i < 10);
来源：http://afb.chenlongwang.top

JS:   do { i++; } while (i < 10);
来源：http://uya.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://wnz.redwolf501.top

Java: do { i++; } while (i < 10);
来源：http://sem.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://swm.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://ogu.sweek.top

C#:   do { i++; } while (i < 10);
来源：http://cnf.zhongyouzk.top

[B09] break 与 continue
来源：http://uiv.tian-w.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uxc.cheryme.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hws.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rjw.shuidangran.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pcc.zhengqikj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xzr.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://prm.tarul.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jlg.fanxiaobao.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xwv.ydzc1.top

[B10] 遍历同时拿索引
来源：http://nag.chenzaomai.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dra.gogol.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lnb.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vbb.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lrj.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pxe.aibaodan.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wtk.sjlbkw.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zmr.shuidangran.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lak.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://sni.zhijiandao.cn

Py:   list(range(0, 10, 2))
来源：http://cru.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://vtv.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vfw.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ogn.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gbd.ydzc1.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xra.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://tns.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uya.nanxuanxn.top

[B12] 跳出多层循环
来源：http://vgs.zhengqikj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mqi.hywenlv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cxq.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yxa.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kfw.cheryme.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lpl.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ysy.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qix.hfpthk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xkz.yvedp.cn

[B13] 判断是否为数字
来源：http://jgw.cashguo.top

Py:   isinstance(x, (int, float))
来源：http://uta.52xcode.cn

PHP:  is_numeric($x)
来源：http://bml.xziqi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ids.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://biw.zdbjq.cn

Java: x instanceof Number
来源：http://san.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kls.kuanghao11.cn

Ruby: x.is_a?(Numeric)
来源：http://mkf.svipenyu.cn

C#:   x is int or double or decimal
来源：http://emz.uphjek.com

[B14] 判断值是否在集合内
来源：http://shs.jqgufenzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xok.zhixingplan.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://goj.quarkkingdee.top

JS:   [1, 2, 3].includes(x)
来源：http://sue.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://qsv.andypj.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://tja.hongshengwenyu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://moe.jianghu66.top

Ruby: [1, 2, 3].include?(x)
来源：http://gnh.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aao.jyoumei.cn

[B15] 布尔运算与取反
来源：http://wtg.chenzaomai.com

Py:   a and b or not c
来源：http://lsr.cdnleiting.top

PHP:  $a && $b || !$c
来源：http://jte.birdmap.top

JS:   a && b || !c
来源：http://vfs.daria6918.cn

TS:   a && b || !c
来源：http://lfy.smart0.xyz

Java: a && b || !c
来源：http://ytj.nwbrower.top

Go:   a && b || !c
来源：http://jlr.yuxming.cn

Ruby: a && b || !c
来源：http://zad.vqdsnc.cn

C#:   a && b || !c
来源：http://fqc.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://hnm.bjfxy.top

Py:   if not data: return
来源：http://lhg.yj20258.top

PHP:  if (!$data) { return; }
来源：http://uom.hywenlv.cn

JS:   if (!data) return;
来源：http://wwz.xuanzx.com

TS:   if (!data) return;
来源：http://peo.kuanghao11.cn

Java: if (data == null) return;
来源：http://zgt.dianchejie.cn

Go:   if data == nil { return }
来源：http://zbb.yueranfly.top

Ruby: return if data.nil?
来源：http://xjz.316326.xyz

C#:   if (data == null) return;
来源：http://abn.shuidangran.top

================================================================================
来源：http://asn.hammf.cn

C. 函数与作用域
来源：http://ezi.yongpay.top

================================================================================
来源：http://mso.zhengqikj.top

[C01] 定义函数
来源：http://gjb.ybcxt.top

Py:   def add(a, b): return a + b
来源：http://gpb.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kec.hnxiangtu.top

JS:   function add(a, b) { return a + b; }
来源：http://zmr.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://frb.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://axu.xinyue.icu

Go:   func add(a, b int) int { return a + b }
来源：http://txn.bbcook.cn

Ruby: def add(a, b); a + b; end
来源：http://sxf.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ijy.uphjek.com

[C02] 默认参数
来源：http://vtb.fanxiaobao.xyz

Py:   def greet(name="World"): return name
来源：http://cxl.sweek.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zqw.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://frr.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://eem.daria6918.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oxa.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dgx.ydjk.org.cn

Ruby: def greet(name = "World") = name
来源：http://wgb.0kj1m.cn

C#:   string Greet(string name = "World") => name;
来源：http://iiy.zhengqikj.top

[C03] 可变参数
来源：http://ndq.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://xoq.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aor.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kly.yuxming.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aan.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ufi.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cyn.zycfv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://elx.haohaochexian.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ihp.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://uqf.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://svs.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ctl.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fro.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wvq.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://kjh.zycfv.cn

Go:   // 无：用配置结构体参数
来源：http://yzo.yanxiufei.cn

Ruby: f(a: 1, b: 2)
来源：http://xnx.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://hdt.shangyingyoupin.top

[C05] 返回多个值
来源：http://mct.gotoacloud.top

Py:   return a, b
来源：http://dqn.ppjwa.cn

PHP:  return [$a, $b];
来源：http://ywk.jyoumei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wvp.yonumen.top

TS:   return { a, b };
来源：http://udg.feifeiyinyue.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vki.zycfv.cn

Go:   return a, b
来源：http://taa.uphjek.com

Ruby: return a, b
来源：http://yxa.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://iyy.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://lgq.guowangkeji.top

Py:   square = lambda x: x * x
来源：http://tqo.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zru.hesvh.cn

JS:   const square = x => x * x;
来源：http://pbq.shzxlz.cn

TS:   const square = (x: number): number => x * x;
来源：http://tyw.fehbvm.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tai.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://swt.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://zfq.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://ihh.sysykeji.top

[C07] 把函数作为参数传入
来源：http://pza.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lod.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xxg.jqgufenzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lng.zhijiandao.cn

TS:   arr.map(String)
来源：http://rwc.hnqzz.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oya.hammf.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uks.fanxiaobao.xyz

Ruby: arr.map(&:upcase)
来源：http://kia.hongshengwenyu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fsd.0kj1m.cn

[C08] 闭包
来源：http://ihx.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://csb.ydjk.org.cn


<!-- 参考信息 -->