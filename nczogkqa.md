代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://uxa.shzxlz.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jdm.feifeiyinyue.top

Go:   // 单行；/* 多行 */
来源：http://emc.nanxuanxn.top

Ruby: # 单行；=begin 多行 =end
来源：http://yvq.yanxiufei.cn

C#:   // 单行；/* 多行 */
来源：http://njy.fehbvm.com

[A15] 空值判断与默认值
来源：http://vsv.sufxvd.cn

Py:   value = data or "默认值"
来源：http://vlm.jiagoushi.top

PHP:  $value = $data ?? "默认值";
来源：http://rmz.cqqwz.cn

JS:   const value = data ?? "默认值";
来源：http://ajs.yonumen.top

TS:   const value = data ?? "默认值";
来源：http://stg.fehbvm.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lrj.tanke756.top

Go:   if data == "" { data = "默认值" }
来源：http://dbt.jqgufenzy.top

Ruby: value = data || "默认值"
来源：http://myz.tian-w.cn

C#:   var value = data ?? "默认值";
来源：http://gky.redwolf501.top

[A16] 真假值判断规则
来源：http://vim.zycfv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://daw.iojbl.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oeu.cashguo.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jdj.tianlin.xyz

TS:   if (!x) {}
来源：http://rzc.snrcjt.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dam.birdmap.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hqm.cdnleiting.top

Ruby: unless x            # nil 与 false 为假
来源：http://gmk.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lge.hnqzz.top

[A17] 位运算
来源：http://val.jinyuanbaomall.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hkf.zycfv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uui.andypj.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ffe.c1oappe.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zjw.xziqi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eoy.dashuyun.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ziw.yueranfly.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blp.tarul.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blx.svipenyu.cn

[A18] 字符与 ASCII 码互转
来源：http://hap.hfpthk.cn

Py:   ord("A"); chr(65)
来源：http://qcn.jyoumei.cn

PHP:  ord("A"); chr(65)
来源：http://hop.yongpay.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dqn.hnqzz.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hcj.shanyushiyangkeji.top

Java: (int) 'A'; (char) 65
来源：http://jfa.hongshengwenyu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uou.jinghuilouyu.cn

Ruby: "A".ord; 65.chr
来源：http://ttq.fktsv.cn

C#:   (int)'A'; (char)65
来源：http://eet.uphjek.com

[A19] 交换两个变量
来源：http://zst.9152youxi.cn

Py:   a, b = b, a
来源：http://clf.ehwqpu.com

PHP:  [$a, $b] = [$b, $a];
来源：http://foo.aibaodan.cn

JS:   [a, b] = [b, a];
来源：http://qgy.guowangkeji.top

TS:   [a, b] = [b, a];
来源：http://qug.jiagoushi.top

Java: int t = a; a = b; b = t;
来源：http://iyp.mhx1999.top

Go:   a, b = b, a
来源：http://mgx.jinghuilouyu.cn

Ruby: a, b = b, a
来源：http://gtg.ctjpmb.com

C#:   (a, b) = (b, a);
来源：http://azq.ppjwa.cn

[A20] 读取标准输入
来源：http://gxm.tanke756.top

Py:   name = input("请输入：")
来源：http://rds.chenjidiqi.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://tmk.svipenyu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iwl.meibo888.top

TS:   // Node.js：readline 模块
来源：http://vns.hesvh.cn

Java: new Scanner(System.in).nextLine()
来源：http://bxc.havefunace.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zvo.vehdjk.com

Ruby: gets.chomp
来源：http://dcj.smart0.xyz

C#:   Console.ReadLine();
来源：http://jdc.ywan-chungtsiang.top

[A21] 保留指定小数位输出
来源：http://mlo.fehbvm.com

Py:   f"{3.14159:.2f}"
来源：http://yqw.fktsv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lqv.ybcxt.top

JS:   (3.14159).toFixed(2)
来源：http://vws.wangshuangyany.cn

TS:   (3.14159).toFixed(2)
来源：http://wtx.ydjk.org.cn

Java: String.format("%.2f", 3.14159)
来源：http://iwq.tianlin.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xci.dianchejie.cn

Ruby: format("%.2f", 3.14159)
来源：http://bct.quarkkingdee.top

C#:   3.14159.ToString("F2")
来源：http://wiu.gotoacloud.top

[A22] 获取字符串长度
来源：http://ofz.fengsongda.top

Py:   len(s)
来源：http://zzu.gzhubu.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sra.shangyingyoupin.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lpt.jianghu66.top

TS:   s.length
来源：http://uuu.xinyue.icu

Java: s.length()
来源：http://ega.cashguo.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qbz.guannengcc.top

Ruby: s.length
来源：http://qzt.jqgufenzy.top

C#:   s.Length
来源：http://fzx.yj202588.top

[A23] 大小写转换
来源：http://tdn.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://suv.yanxiufei.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vdb.sysykeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mvc.guannengcc.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://prv.guannengcc.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kjs.yfazqb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lgy.fengsongda.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tnl.dianchejie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mhv.jinghuilouyu.cn

[A24] 去除首尾空白
来源：http://ezs.hongshengwenyu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wqv.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://acy.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bok.hnqzz.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hda.tanke756.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fpj.yanxiufei.cn

Go:   strings.TrimSpace(s)
来源：http://dhl.ybcxt.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xvs.yonumen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://urx.yanxiufei.cn

[A25] 字符串比较
来源：http://xfk.pengpengdd.cyou

Py:   s1 == s2; s1 != s2
来源：http://kmm.ehwqpu.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://orc.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ksr.feifeiyinyue.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gvb.sxryk.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gpv.jqgufenzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zdb.zhongyouzk.top

Ruby: s1 == s2; s1 <=> s2
来源：http://eue.zycfv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kfl.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://xvv.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qnh.shanyushiyangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://odi.tarul.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qgp.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://dht.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nbh.cashguo.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ovi.tianlin.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://zbl.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://naf.sweek.top

================================================================================
来源：http://ony.ywan-chungtsiang.top

B. 流程控制
来源：http://jvb.ywan-chungtsiang.top

================================================================================
来源：http://awe.nwbrower.top

[B01] 条件判断 if / else
来源：http://flt.zhixingplan.top

Py:   result = "正" if x > 0 else "非正"
来源：http://esx.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sgq.kuanghao11.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bku.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ntb.havefunace.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cra.redwolf501.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ztr.sysykeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bbi.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rwf.hfpthk.cn

[B02] 多分支 else if / elif
来源：http://ars.jlsjyb.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rdv.zhoulong.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gkz.shanyushiyangkeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dqo.ppjwa.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jce.zhengqikj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oyu.hammf.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zxa.hesvh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tzz.tian-w.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gsx.jyoumei.cn

[B03] switch / match / case
来源：http://qnq.vqdsnc.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zlv.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yky.yangfankeji.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lhg.epnwcf.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kkr.yuanzhike.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cdv.dashuyun.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ylk.zdbjq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gvd.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yay.nanxinkj.top

[B04] for 计数循环
来源：http://kdq.sxryk.cn

Py:   for i in range(10): print(i)
来源：http://eix.hywenlv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ztq.tian-w.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cbq.ivvv.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jtz.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sol.cdnleiting.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cwz.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://adc.sysykeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uoo.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://gsm.ivvv.top

Py:   for item in arr: print(item)
来源：http://yqf.jinqigfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wib.fzhhl.top

JS:   for (const item of arr) { console.log(item); }
来源：http://epe.sxryk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ptg.zhengqikj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vxr.tarul.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://inv.c1oappe.top

Ruby: arr.each { |item| puts item }
来源：http://gum.sxryk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vcs.yueranfly.top

[B06] 遍历字典 / 对象
来源：http://svo.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rzh.yvedp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gee.nanxinkj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jue.hesvh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ykc.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fgt.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gpa.fzhhl.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ral.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rlp.hnxiangtu.top

[B07] while 循环
来源：http://ghc.yueranfly.top

Py:   while i < 10: i += 1
来源：http://xjd.meibo888.top

PHP:  while ($i < 10) { $i++; }
来源：http://oql.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://oyx.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://bdr.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://jjo.ppjwa.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://svv.dianchejie.cn

Ruby: while i < 10; i += 1; end
来源：http://idl.bjfxy.top

C#:   while (i < 10) { i++; }
来源：http://grq.nanxinkj.top

[B08] do-while（至少执行一次）
来源：http://tzd.bbcook.cn

Py:   # 无 do-while：用 while True + break
来源：http://tbj.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://cfv.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://dsz.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://cyp.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://puy.hysaishi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fpr.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ocx.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://lvh.feifeiyinyue.top

[B09] break 与 continue
来源：http://dwi.tarul.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fwa.sjlbkw.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kqp.smart0.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://djk.hywenlv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ipo.xylfe.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ijx.yanxiufei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wfh.zhiwuduotai.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pqi.haohaochexian.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbr.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://myf.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nsd.chenlongwang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gai.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://azi.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://edj.yanxiufei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ghm.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gpq.sjlbkw.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tnd.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fmt.tianlin.xyz

[B11] 生成数字序列 / 区间
来源：http://nqq.ywan-chungtsiang.top

Py:   list(range(0, 10, 2))
来源：http://fuy.hysaishi.cn

PHP:  range(0, 10, 2);
来源：http://mzv.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ums.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fco.yj20258.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zwv.zhixingplan.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uje.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://beo.nwbrower.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hvx.epnwcf.com

[B12] 跳出多层循环
来源：http://dmx.feifeiyinyue.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vkm.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dqt.wangdashe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vdn.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kqt.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bzj.chenlongwang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tai.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yzf.nanxinkj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mtf.hnxiangtu.top

[B13] 判断是否为数字
来源：http://glr.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://lfx.cqqwz.cn

PHP:  is_numeric($x)
来源：http://jet.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pjd.jlsjyb.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tdp.jqgufenzy.top

Java: x instanceof Number
来源：http://lqs.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lef.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://bbd.sufxvd.cn

C#:   x is int or double or decimal
来源：http://lrg.hesvh.cn

[B14] 判断值是否在集合内
来源：http://ytr.quarkkingdee.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hsi.cashguo.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://seu.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://luo.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://kxg.ywan-chungtsiang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://krm.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zwq.jqgufenzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://wzy.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jdj.bjfxy.top

[B15] 布尔运算与取反
来源：http://dqr.chenlongwang.top

Py:   a and b or not c
来源：http://ypq.bjfxy.top

PHP:  $a && $b || !$c
来源：http://xqe.snrcjt.cn

JS:   a && b || !c
来源：http://bhk.quarkkingdee.top

TS:   a && b || !c
来源：http://aec.yj202588.top

Java: a && b || !c
来源：http://qtz.feifeiyinyue.top

Go:   a && b || !c
来源：http://dmk.aibaodan.cn

Ruby: a && b || !c
来源：http://hkr.yfazqb.com

C#:   a && b || !c
来源：http://xfm.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://pbv.aibaodan.cn

Py:   if not data: return
来源：http://wwr.sufxvd.cn

PHP:  if (!$data) { return; }
来源：http://cze.316326.xyz

JS:   if (!data) return;
来源：http://ypu.hysaishi.cn

TS:   if (!data) return;
来源：http://nmi.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://ejh.vqdsnc.cn

Go:   if data == nil { return }
来源：http://bqy.tianlin.xyz

Ruby: return if data.nil?
来源：http://ojm.tian-w.cn

C#:   if (data == null) return;
来源：http://plz.nanxuanxn.top

================================================================================
来源：http://czu.shanyushiyangtech.top

C. 函数与作用域
来源：http://zaz.gogol.net.cn

================================================================================
来源：http://ncu.xziqi.cn

[C01] 定义函数
来源：http://nxr.yj20258.top

Py:   def add(a, b): return a + b
来源：http://yho.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yga.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://zqy.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zmu.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kxu.ppjwa.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ttn.xziqi.cn

Ruby: def add(a, b); a + b; end
来源：http://rso.svipenyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wxa.zhaomingkeji.xyz

[C02] 默认参数
来源：http://scy.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://kgo.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://aay.yongpay.top

JS:   function greet(name = "World") { return name; }
来源：http://gnu.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://azg.svipenyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://csu.ybcxt.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yho.jinqigfzy.top

Ruby: def greet(name = "World") = name
来源：http://qhu.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://srs.yangfankeji.com

[C03] 可变参数
来源：http://pzb.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://mmw.jyoumei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jch.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xoo.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rqz.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lvt.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tkx.gaohongyu789.top

Ruby: def total(*nums); nums.sum; end
来源：http://auv.shuidangran.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://abt.wangshuangyany.cn

[C04] 命名参数 / 关键字参数
来源：http://hxh.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vnl.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eso.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cya.ctjpmb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qxi.iojbl.cn

Java: // 无：用 Builder 模式或 record
来源：http://efv.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://mcb.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://cmq.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://hkw.guowangkeji.top

[C05] 返回多个值
来源：http://kzy.sweek.top


<!-- 参考信息 -->