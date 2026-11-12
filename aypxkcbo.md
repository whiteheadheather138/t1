代发 wailian999

[A14] 注释写法
来源：http://wls.iojbl.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gkg.ydjk.org.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mky.zhixingplan.top

JS:   // 单行；/* 多行 */
来源：http://amj.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://fgu.jlsjyb.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yie.zdqjudy.top

Go:   // 单行；/* 多行 */
来源：http://vng.tanke756.top

Ruby: # 单行；=begin 多行 =end
来源：http://hqu.zhongyouzk.top

C#:   // 单行；/* 多行 */
来源：http://ico.fktsv.cn

[A15] 空值判断与默认值
来源：http://ejg.meibo888.top

Py:   value = data or "默认值"
来源：http://ucz.jlsjyb.cn

PHP:  $value = $data ?? "默认值";
来源：http://bea.smart0.xyz

JS:   const value = data ?? "默认值";
来源：http://jpr.haohaochexian.top

TS:   const value = data ?? "默认值";
来源：http://zie.cashguo.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uze.tianlin.xyz

Go:   if data == "" { data = "默认值" }
来源：http://mzd.epnwcf.com

Ruby: value = data || "默认值"
来源：http://boo.zhiwuduotai.top

C#:   var value = data ?? "默认值";
来源：http://uds.tarul.cn

[A16] 真假值判断规则
来源：http://meb.ydzc1.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pyt.c1oappe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hro.mhx1999.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fmo.xingfuxueyuan.xyz

TS:   if (!x) {}
来源：http://buz.redwolf501.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gkb.yfazqb.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dfu.hysaishi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bvt.meibo888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://buf.hammf.cn

[A17] 位运算
来源：http://rtw.chenlongwang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kiu.tarul.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wbz.yvedp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oni.zhixingplan.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hzv.zhengqikj.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zcr.c1oappe.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sea.meibo888.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jln.ydjk.org.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nop.nanxinkj.top

[A18] 字符与 ASCII 码互转
来源：http://cgj.hnqzz.top

Py:   ord("A"); chr(65)
来源：http://kih.xinyue.icu

PHP:  ord("A"); chr(65)
来源：http://ona.yongpay.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wrn.0kj1m.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ish.fanxiaobao.xyz

Java: (int) 'A'; (char) 65
来源：http://cis.tianlin.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uln.jinyuanbaomall.cn

Ruby: "A".ord; 65.chr
来源：http://kua.chenzaomai.com

C#:   (int)'A'; (char)65
来源：http://ogt.daria6918.cn

[A19] 交换两个变量
来源：http://tns.sysykeji.top

Py:   a, b = b, a
来源：http://yfn.sysykeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jdj.xinyue.icu

JS:   [a, b] = [b, a];
来源：http://lhz.birdmap.top

TS:   [a, b] = [b, a];
来源：http://onp.zycfv.cn

Java: int t = a; a = b; b = t;
来源：http://nnd.zhiwuduotai.top

Go:   a, b = b, a
来源：http://zuq.daxiang520.top

Ruby: a, b = b, a
来源：http://zsu.ehwqpu.com

C#:   (a, b) = (b, a);
来源：http://dif.cucudq.cn

[A20] 读取标准输入
来源：http://utz.kuanghao11.cn

Py:   name = input("请输入：")
来源：http://hze.52xcode.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xpf.shangyingyoupin.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dvv.wangshuangyany.cn

TS:   // Node.js：readline 模块
来源：http://tyh.fktsv.cn

Java: new Scanner(System.in).nextLine()
来源：http://nvh.kuanghao11.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://iwk.quarkkingdee.top

Ruby: gets.chomp
来源：http://bsu.tian-w.cn

C#:   Console.ReadLine();
来源：http://ruf.hongshengwenyu.top

[A21] 保留指定小数位输出
来源：http://fut.hongshengwenyu.top

Py:   f"{3.14159:.2f}"
来源：http://tfr.c1oappe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jab.uphjek.com

JS:   (3.14159).toFixed(2)
来源：http://wjy.nwbrower.top

TS:   (3.14159).toFixed(2)
来源：http://nyr.yongpay.top

Java: String.format("%.2f", 3.14159)
来源：http://gsh.zhoulong.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eqc.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://hkc.mhx1999.top

C#:   3.14159.ToString("F2")
来源：http://ktr.sjlbkw.cn

[A22] 获取字符串长度
来源：http://rev.cashguo.top

Py:   len(s)
来源：http://deb.zhoulong.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sru.ybcxt.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kmn.hnqzz.top

TS:   s.length
来源：http://qoz.yonumen.top

Java: s.length()
来源：http://fss.shzxlz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://aar.svipenyu.cn

Ruby: s.length
来源：http://liv.yangfankeji.com

C#:   s.Length
来源：http://jmv.hnxiangtu.top

[A23] 大小写转换
来源：http://mgb.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ucr.sysykeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rbn.zdqjudy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://svn.xuetiantiany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vgb.yvedp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wau.xziqi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mre.jinghuilouyu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://scq.yvedp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tsa.sjlbkw.cn

[A24] 去除首尾空白
来源：http://cqk.gotoacloud.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oij.sufxvd.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://csc.kuanghao11.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dix.pycfn.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bqn.snrcjt.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ixh.guowangkeji.top

Go:   strings.TrimSpace(s)
来源：http://dgk.chenlongwang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iqc.feifeiyinyue.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ofi.gzhubu.top

[A25] 字符串比较
来源：http://okj.mhx1999.top

Py:   s1 == s2; s1 != s2
来源：http://fus.cqqwz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://onx.yanxiufei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nxj.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wqv.guowangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nlx.daria6918.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ppv.andypj.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://cyr.zdqjudy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wec.chenlongwang.top

[A26] 类型转换总览
来源：http://vqn.yj20258888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dze.cheryme.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vvk.aibaodan.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ocq.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://vbn.jqgufenzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://asq.hnqzz.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://git.cucudq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lxn.316326.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fhv.nanxinkj.top

================================================================================
来源：http://rsx.gotoacloud.top

B. 流程控制
来源：http://upe.hnqzz.top

================================================================================
来源：http://imb.yanxiufei.cn

[B01] 条件判断 if / else
来源：http://thv.shzxlz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wen.uphjek.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://her.zycfv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xiy.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ilc.hysaishi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oaq.0kj1m.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xlh.zhijiandao.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bsb.chenzaomai.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hsv.ydzc1.top

[B02] 多分支 else if / elif
来源：http://odv.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xbn.dashuyun.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zee.shuidangran.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ezg.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bxy.pycfn.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iux.hesvh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://txr.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://czc.jyoumei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbn.nanxinkj.top

[B03] switch / match / case
来源：http://nqt.yj20258.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qpc.snrcjt.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pcs.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tod.xylfe.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ykv.pengpengdd.cyou

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://scz.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nlv.zhiwuduotai.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jga.sjlbkw.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tiz.iojbl.cn

[B04] for 计数循环
来源：http://hfb.gaohongyu789.top

Py:   for i in range(10): print(i)
来源：http://iaz.yj20258888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ygr.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://szw.shangyingyoupin.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oyr.zdqjudy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zil.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://asc.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://ais.xinyue.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hmj.yanxiufei.cn

[B05] 遍历数组 / 列表
来源：http://icv.sxryk.cn

Py:   for item in arr: print(item)
来源：http://hrh.dianchejie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aqb.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hvy.xingfuxueyuan.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://jrm.dianchejie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mxk.jiagoushi.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xlq.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://bvh.mhx1999.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://alm.ivvv.top

[B06] 遍历字典 / 对象
来源：http://lpo.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://qry.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uks.xinyue.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dwy.gotoacloud.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oxc.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://krm.chenjidiqi.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bzt.fehbvm.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://utj.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hzp.haohaochexian.top

[B07] while 循环
来源：http://rlc.zycfv.cn

Py:   while i < 10: i += 1
来源：http://nab.xingfuxueyuan.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://gfy.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://rff.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://tds.sufxvd.cn

Java: while (i < 10) { i++; }
来源：http://nvj.hcnkem.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fwq.tanke756.top

Ruby: while i < 10; i += 1; end
来源：http://abm.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://yoz.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://tln.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://kjp.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xll.nanxuanxn.top

JS:   do { i++; } while (i < 10);
来源：http://plz.dashuyun.cn

TS:   do { i++; } while (i < 10);
来源：http://xgc.sufxvd.cn

Java: do { i++; } while (i < 10);
来源：http://gmz.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://jzt.ydzc1.top

Ruby: begin; i += 1; end while i < 10
来源：http://vmq.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://jvh.daxiang520.top

[B09] break 与 continue
来源：http://hea.zhengqikj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tga.meibo888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mdu.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://asq.jqgufenzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fti.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aao.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fdv.tianlin.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://adh.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ahl.ydjk.org.cn

[B10] 遍历同时拿索引
来源：http://hdm.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hoh.gogol.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://czf.snrcjt.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zpj.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fgl.316326.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xto.wangdashe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aui.yangfankeji.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cak.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qra.xingfuxueyuan.xyz

[B11] 生成数字序列 / 区间
来源：http://svm.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://tae.vehdjk.com

PHP:  range(0, 10, 2);
来源：http://ffg.hongshengwenyu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qep.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ame.feifeiyinyue.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hvf.zhongyouzk.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fqe.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://bdu.quarkkingdee.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wwj.chenzaomai.com

[B12] 跳出多层循环
来源：http://fki.yonumen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xxv.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://qnr.yuanzhike.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cxk.pengpengdd.cyou

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tcb.feifeiyinyue.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wmc.yj20258888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vqr.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lsh.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oxg.jinyuanbaomall.cn

[B13] 判断是否为数字
来源：http://rev.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://vnh.hammf.cn

PHP:  is_numeric($x)
来源：http://esu.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://esk.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ipz.andypj.xyz

Java: x instanceof Number
来源：http://myr.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://khq.ppjwa.cn

Ruby: x.is_a?(Numeric)
来源：http://zlh.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://olm.fengsongda.top

[B14] 判断值是否在集合内
来源：http://ycc.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uor.cdnleiting.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ybr.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://jrn.fzhhl.top

TS:   [1, 2, 3].includes(x)
来源：http://hob.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cww.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fci.cdnleiting.top

Ruby: [1, 2, 3].include?(x)
来源：http://ivc.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bmj.iojbl.cn

[B15] 布尔运算与取反
来源：http://scu.shanyushiyangtech.top

Py:   a and b or not c
来源：http://uqu.xuetiantiany.cn

PHP:  $a && $b || !$c
来源：http://kfu.shzxlz.cn

JS:   a && b || !c
来源：http://kll.birdmap.top

TS:   a && b || !c
来源：http://zeq.jlsjyb.cn

Java: a && b || !c
来源：http://bob.chenlongwang.top

Go:   a && b || !c
来源：http://hcw.ydzc1.top

Ruby: a && b || !c
来源：http://tda.fanxiaobao.xyz

C#:   a && b || !c
来源：http://rtn.yonumen.top

[B16] 卫语句：不满足条件提前返回
来源：http://jxy.jinyuanbaomall.cn

Py:   if not data: return
来源：http://xic.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://two.guowangkeji.top

JS:   if (!data) return;
来源：http://qou.cdnleiting.top

TS:   if (!data) return;
来源：http://vws.sjlbkw.cn

Java: if (data == null) return;
来源：http://nbm.pengpengdd.cyou

Go:   if data == nil { return }
来源：http://xxu.hesvh.cn

Ruby: return if data.nil?
来源：http://jlg.meibo888.top

C#:   if (data == null) return;
来源：http://jsh.svipenyu.cn

================================================================================
来源：http://tjx.wangshuangyany.cn

C. 函数与作用域
来源：http://ocg.hammf.cn

================================================================================
来源：http://seu.hnxiangtu.top

[C01] 定义函数
来源：http://ngz.jinqigfzy.top

Py:   def add(a, b): return a + b
来源：http://lqb.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://exs.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://dtt.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://scl.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://krr.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kys.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://bdr.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://huy.52xcode.cn

[C02] 默认参数
来源：http://jkj.ehwqpu.com

Py:   def greet(name="World"): return name
来源：http://ijw.sjlbkw.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cla.ybcxt.top

JS:   function greet(name = "World") { return name; }
来源：http://utp.jinqigfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://swk.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://tnq.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://had.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://qdk.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://npp.bjfxy.top

[C03] 可变参数
来源：http://rpu.xuanzx.com

Py:   def total(*args): return sum(args)
来源：http://gon.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ufa.jianghu66.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oyu.vehdjk.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ngb.smart0.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blp.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qld.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wfo.ydzc1.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://epd.wangdashe.top

[C04] 命名参数 / 关键字参数
来源：http://wnr.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zwa.c1oappe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dsf.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jpa.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fzj.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://slv.yj20258.top


<!-- 参考信息 -->