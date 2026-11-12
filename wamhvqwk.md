代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://nzn.yuanzhike.top

TS:   const value = data ?? "默认值";
来源：http://mcl.feifeiyinyue.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://njf.iojbl.cn

Go:   if data == "" { data = "默认值" }
来源：http://ymq.zhiwuduotai.top

Ruby: value = data || "默认值"
来源：http://laz.jqgufenzy.top

C#:   var value = data ?? "默认值";
来源：http://ajc.zhoulong.xyz

[A16] 真假值判断规则
来源：http://ink.hammf.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pfa.jinghuilouyu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kfo.yangfankeji.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tck.gotoacloud.top

TS:   if (!x) {}
来源：http://era.fktsv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dnu.cashguo.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ksp.iojbl.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bzk.sweek.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gqj.daxiang520.top

[A17] 位运算
来源：http://jpq.ehwqpu.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mxv.52xcode.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vkk.kuanghao11.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uwf.ivvv.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://eey.jqgufenzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qqy.smart0.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://klq.xinyue.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xre.xuetiantiany.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rit.cdnleiting.top

[A18] 字符与 ASCII 码互转
来源：http://mbo.jiagoushi.top

Py:   ord("A"); chr(65)
来源：http://yar.zhongyouzk.top

PHP:  ord("A"); chr(65)
来源：http://ecq.xylfe.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ien.hfpthk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xnw.0kj1m.cn

Java: (int) 'A'; (char) 65
来源：http://rgd.gotoacloud.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tic.ctjpmb.com

Ruby: "A".ord; 65.chr
来源：http://mtg.hywenlv.cn

C#:   (int)'A'; (char)65
来源：http://eta.havefunace.top

[A19] 交换两个变量
来源：http://ydr.sweek.top

Py:   a, b = b, a
来源：http://rod.hywenlv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wyq.hfpthk.cn

JS:   [a, b] = [b, a];
来源：http://hdn.52xcode.cn

TS:   [a, b] = [b, a];
来源：http://rmn.gaohongyu789.top

Java: int t = a; a = b; b = t;
来源：http://bno.yj20258.top

Go:   a, b = b, a
来源：http://ylb.snrcjt.cn

Ruby: a, b = b, a
来源：http://tue.chenjidiqi.icu

C#:   (a, b) = (b, a);
来源：http://mje.hongshengwenyu.top

[A20] 读取标准输入
来源：http://erp.tianlin.xyz

Py:   name = input("请输入：")
来源：http://iod.wangshuangyany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nni.shanyushiyangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vnb.tarul.cn

TS:   // Node.js：readline 模块
来源：http://fcz.0kj1m.cn

Java: new Scanner(System.in).nextLine()
来源：http://cur.andypj.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://svv.havefunace.top

Ruby: gets.chomp
来源：http://tzc.zdqjudy.top

C#:   Console.ReadLine();
来源：http://hqu.ywan-chungtsiang.top

[A21] 保留指定小数位输出
来源：http://nyg.redwolf501.top

Py:   f"{3.14159:.2f}"
来源：http://plw.yangfankeji.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pzl.yj202588.top

JS:   (3.14159).toFixed(2)
来源：http://xbi.jinyuanbaomall.cn

TS:   (3.14159).toFixed(2)
来源：http://llu.havefunace.top

Java: String.format("%.2f", 3.14159)
来源：http://tdi.gzhubu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zya.gzhubu.top

Ruby: format("%.2f", 3.14159)
来源：http://vcx.smart0.xyz

C#:   3.14159.ToString("F2")
来源：http://hhj.jqgufenzy.top

[A22] 获取字符串长度
来源：http://eke.nwbrower.top

Py:   len(s)
来源：http://rfc.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vam.fzhhl.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tzw.chenjidiqi.icu

TS:   s.length
来源：http://xeq.yfazqb.com

Java: s.length()
来源：http://url.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ylv.zdqjudy.top

Ruby: s.length
来源：http://wxz.zhongyouzk.top

C#:   s.Length
来源：http://ulk.xingfuxueyuan.xyz

[A23] 大小写转换
来源：http://fkl.jinyuanbaomall.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://isk.birdmap.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://okn.sufxvd.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lby.zhiwuduotai.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://czq.hammf.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rzj.uphjek.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rla.kuanghao11.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uwp.ivvv.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ltz.dashuyun.cn

[A24] 去除首尾空白
来源：http://cph.jinqigfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pfl.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ifb.yongpay.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hpu.xziqi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hvg.hfpthk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kju.birdmap.top

Go:   strings.TrimSpace(s)
来源：http://tah.gotoacloud.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dbe.yueranfly.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ifn.shanyushiyangtech.top

[A25] 字符串比较
来源：http://byg.hywenlv.cn

Py:   s1 == s2; s1 != s2
来源：http://ysn.ywan-chungtsiang.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ftf.316326.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://exe.andypj.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wdd.guowangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rkp.iojbl.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ykf.jinqigfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://knn.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kcc.epnwcf.com

[A26] 类型转换总览
来源：http://idr.tianlin.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bwc.cashguo.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wlg.jqgufenzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oei.jinyuanbaomall.cn

TS:   Number() String() Boolean() x as number
来源：http://jqh.xinyue.icu

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fxm.vehdjk.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://meg.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nhy.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zpb.chenjidiqi.icu

================================================================================
来源：http://fvo.ydjk.org.cn

B. 流程控制
来源：http://xut.smart0.xyz

================================================================================
来源：http://hzg.guannengcc.top

[B01] 条件判断 if / else
来源：http://bur.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wcz.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ctm.yonumen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kzi.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bkp.ctjpmb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://ebi.ydjk.org.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jaj.hywenlv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://szs.chenlongwang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rdj.smart0.xyz

[B02] 多分支 else if / elif
来源：http://uxm.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eon.316326.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xhi.shangyingyoupin.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hkl.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mts.xylfe.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ykz.hongshengwenyu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lzp.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rxm.nanxinkj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jcw.hysaishi.cn

[B03] switch / match / case
来源：http://rzw.hywenlv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zwj.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jor.andypj.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tov.iojbl.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ope.xylfe.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://piv.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bku.hywenlv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://num.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xcq.tianlin.xyz

[B04] for 计数循环
来源：http://ctw.ydjk.org.cn

Py:   for i in range(10): print(i)
来源：http://nvz.aizwys.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kqg.zhijiandao.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ngu.pycfn.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jkc.aizwys.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cos.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://owg.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://vin.ybcxt.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bdp.cashguo.top

[B05] 遍历数组 / 列表
来源：http://duu.birdmap.top

Py:   for item in arr: print(item)
来源：http://rpj.iojbl.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ldk.epnwcf.com

JS:   for (const item of arr) { console.log(item); }
来源：http://gyx.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://okr.jinqigfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rki.chenzaomai.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hlx.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://siu.haohaochexian.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gvb.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://iov.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hyj.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yci.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vvc.sufxvd.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dda.tian-w.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wzw.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uga.dianchejie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://llj.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dpr.zdbjq.cn

[B07] while 循环
来源：http://myv.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://xki.yanxiufei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kow.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://nut.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://swj.mhx1999.top

Java: while (i < 10) { i++; }
来源：http://nqy.redwolf501.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sqm.52xcode.cn

Ruby: while i < 10; i += 1; end
来源：http://zql.nanxinkj.top

C#:   while (i < 10) { i++; }
来源：http://atl.sjlbkw.cn

[B08] do-while（至少执行一次）
来源：http://vyx.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://prf.chenjidiqi.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://ttd.xinyue.icu

JS:   do { i++; } while (i < 10);
来源：http://fep.shzxlz.cn

TS:   do { i++; } while (i < 10);
来源：http://qxi.316326.xyz

Java: do { i++; } while (i < 10);
来源：http://zft.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ipa.yongpay.top

Ruby: begin; i += 1; end while i < 10
来源：http://pux.shanyushiyangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://pcx.guowangkeji.top

[B09] break 与 continue
来源：http://efy.yangfankeji.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vwf.hcnkem.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://scd.fehbvm.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ylz.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xxt.ppjwa.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yot.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jhm.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tfo.haohaochexian.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zir.gogol.net.cn

[B10] 遍历同时拿索引
来源：http://abb.xuanzx.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wmq.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kdo.ydzc1.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yub.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yfl.nwbrower.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mnk.aibaodan.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mrd.yueranfly.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kft.hesvh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ftn.guannengcc.top

[B11] 生成数字序列 / 区间
来源：http://ive.jianghu66.top

Py:   list(range(0, 10, 2))
来源：http://yhz.yj202588.top

PHP:  range(0, 10, 2);
来源：http://rxt.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mzx.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dzo.jinqigufen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://esn.gogol.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://amp.svipenyu.cn

Ruby: (0...10).step(2).to_a
来源：http://yyu.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ead.zhongyouzk.top

[B12] 跳出多层循环
来源：http://iyc.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bxc.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uov.xuetiantiany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pgn.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dtf.hywenlv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tst.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qwj.shuidangran.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ilr.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jsc.9152youxi.cn

[B13] 判断是否为数字
来源：http://phn.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://zjm.shanyushiyangkeji.top

PHP:  is_numeric($x)
来源：http://qka.shanyushiyangtech.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pta.ybcxt.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wsx.meibo888.top

Java: x instanceof Number
来源：http://ibg.havefunace.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qcl.yongpay.top

Ruby: x.is_a?(Numeric)
来源：http://els.jinqigfzy.top

C#:   x is int or double or decimal
来源：http://hxe.hnxiangtu.top

[B14] 判断值是否在集合内
来源：http://hvd.fktsv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ivn.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hla.havefunace.top

JS:   [1, 2, 3].includes(x)
来源：http://vkp.yfazqb.com

TS:   [1, 2, 3].includes(x)
来源：http://afp.cqqwz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tnh.sufxvd.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zpu.sxryk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nzn.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://daj.redwolf501.top

[B15] 布尔运算与取反
来源：http://bkq.xinyue.icu

Py:   a and b or not c
来源：http://emp.shanyushiyangkeji.top

PHP:  $a && $b || !$c
来源：http://ago.316326.xyz

JS:   a && b || !c
来源：http://xxx.guowangkeji.top

TS:   a && b || !c
来源：http://hpm.iojbl.cn

Java: a && b || !c
来源：http://yfb.xziqi.cn

Go:   a && b || !c
来源：http://zgi.gzhubu.top

Ruby: a && b || !c
来源：http://ofs.ivvv.top

C#:   a && b || !c
来源：http://sej.sjlbkw.cn

[B16] 卫语句：不满足条件提前返回
来源：http://csv.52xcode.cn

Py:   if not data: return
来源：http://cyb.chenjidiqi.icu

PHP:  if (!$data) { return; }
来源：http://zxx.jinqigfzy.top

JS:   if (!data) return;
来源：http://hwo.zdbjq.cn

TS:   if (!data) return;
来源：http://vhn.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://ssf.jlsjyb.cn

Go:   if data == nil { return }
来源：http://qyq.jqgfzy.top

Ruby: return if data.nil?
来源：http://sws.uphjek.com

C#:   if (data == null) return;
来源：http://cmj.nanxuanxn.top

================================================================================
来源：http://bmw.gzhubu.top

C. 函数与作用域
来源：http://cbl.hywenlv.cn

================================================================================
来源：http://pxc.aizwys.cn

[C01] 定义函数
来源：http://mtt.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://jzh.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://anq.yvedp.cn

JS:   function add(a, b) { return a + b; }
来源：http://kzv.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://amg.cqqwz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://byh.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://ymj.zhongyouzk.top

Ruby: def add(a, b); a + b; end
来源：http://wnu.jinyuanbaomall.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ovp.bjfxy.top

[C02] 默认参数
来源：http://fce.daria6918.cn

Py:   def greet(name="World"): return name
来源：http://bcn.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://qlu.tianlin.xyz

JS:   function greet(name = "World") { return name; }
来源：http://wrn.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://cci.cqqwz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wqu.daxiang520.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dby.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://shk.52xcode.cn

C#:   string Greet(string name = "World") => name;
来源：http://mso.sweek.top

[C03] 可变参数
来源：http://wxg.zhengqikj.top

Py:   def total(*args): return sum(args)
来源：http://los.jinghuilouyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uug.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hmx.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ryp.wangshuangyany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kgs.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ahl.shuidangran.top

Ruby: def total(*nums); nums.sum; end
来源：http://tkg.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jmx.xuetiantiany.cn

[C04] 命名参数 / 关键字参数
来源：http://ozl.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rhd.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pqs.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jod.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://drn.birdmap.top

Java: // 无：用 Builder 模式或 record
来源：http://hgg.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://arb.aizwys.cn

Ruby: f(a: 1, b: 2)
来源：http://txq.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://ewr.guannengcc.top

[C05] 返回多个值
来源：http://sae.ydzc1.top

Py:   return a, b
来源：http://czf.gzhubu.top

PHP:  return [$a, $b];
来源：http://bci.jinqigfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qpf.pengpengdd.cyou

TS:   return { a, b };
来源：http://lxq.hammf.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://adn.kuanghao11.cn

Go:   return a, b
来源：http://hsg.cashguo.top

Ruby: return a, b
来源：http://txi.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://xjp.zdbjq.cn


<!-- 参考信息 -->