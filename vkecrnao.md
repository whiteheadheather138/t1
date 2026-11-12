代发 wailian999

[A14] 注释写法
来源：http://dbs.hysaishi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://awb.fktsv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ruu.yangfankeji.com

JS:   // 单行；/* 多行 */
来源：http://jgj.yuanzhike.top

TS:   // 单行；/* 多行 */
来源：http://bpc.hysaishi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://spb.fehbvm.com

Go:   // 单行；/* 多行 */
来源：http://nmn.shanyushiyangkeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://apt.fengsongda.top

C#:   // 单行；/* 多行 */
来源：http://ube.ydzc1.top

[A15] 空值判断与默认值
来源：http://hwe.c1oappe.top

Py:   value = data or "默认值"
来源：http://awi.redwolf501.top

PHP:  $value = $data ?? "默认值";
来源：http://zwo.ctjpmb.com

JS:   const value = data ?? "默认值";
来源：http://ble.yuanzhike.top

TS:   const value = data ?? "默认值";
来源：http://mbs.meibo888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://myj.jinqigufen.top

Go:   if data == "" { data = "默认值" }
来源：http://grg.iojbl.cn

Ruby: value = data || "默认值"
来源：http://csj.nanxuanxn.top

C#:   var value = data ?? "默认值";
来源：http://les.dianchejie.cn

[A16] 真假值判断规则
来源：http://lno.tianlin.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xye.pycfn.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cmc.yuxming.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sli.yuanzhike.top

TS:   if (!x) {}
来源：http://msl.sjlbkw.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ecf.jqgufenzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fxx.pengpengdd.cyou

Ruby: unless x            # nil 与 false 为假
来源：http://dcg.yuxming.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mkn.zhixingplan.top

[A17] 位运算
来源：http://fwh.sjlbkw.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pgf.wangdashe.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tzd.sufxvd.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mqa.nanxinkj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qkw.chenjidiqi.icu

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xhd.jinqigfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oaf.zhongyouzk.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://szd.zycfv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oja.zycfv.cn

[A18] 字符与 ASCII 码互转
来源：http://lcy.cucudq.cn

Py:   ord("A"); chr(65)
来源：http://opy.snrcjt.cn

PHP:  ord("A"); chr(65)
来源：http://phl.zhaomingkeji.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mmp.ywan-chungtsiang.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qmr.cqqwz.cn

Java: (int) 'A'; (char) 65
来源：http://ksm.fktsv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://din.ehwqpu.com

Ruby: "A".ord; 65.chr
来源：http://aiq.aibaodan.cn

C#:   (int)'A'; (char)65
来源：http://onh.gogol.net.cn

[A19] 交换两个变量
来源：http://vsn.redwolf501.top

Py:   a, b = b, a
来源：http://fxr.daria6918.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mko.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://zit.quarkkingdee.top

TS:   [a, b] = [b, a];
来源：http://rhk.nwbrower.top

Java: int t = a; a = b; b = t;
来源：http://jfy.jyoumei.cn

Go:   a, b = b, a
来源：http://jru.tianlin.xyz

Ruby: a, b = b, a
来源：http://ncq.kuanghao11.cn

C#:   (a, b) = (b, a);
来源：http://csv.sjlbkw.cn

[A20] 读取标准输入
来源：http://oct.nanxuanxn.top

Py:   name = input("请输入：")
来源：http://oze.dianchejie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kki.jlsjyb.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jzi.yuxming.cn

TS:   // Node.js：readline 模块
来源：http://jyn.quarkkingdee.top

Java: new Scanner(System.in).nextLine()
来源：http://dsb.gzhubu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dkf.nanxinkj.top

Ruby: gets.chomp
来源：http://qgk.yonumen.top

C#:   Console.ReadLine();
来源：http://iui.cucudq.cn

[A21] 保留指定小数位输出
来源：http://vum.zhengqikj.top

Py:   f"{3.14159:.2f}"
来源：http://ewo.kuanghao11.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xtw.shanyushiyangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://myc.birdmap.top

TS:   (3.14159).toFixed(2)
来源：http://izf.daxiang520.top

Java: String.format("%.2f", 3.14159)
来源：http://wfg.yj20258.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://osc.chenzaomai.com

Ruby: format("%.2f", 3.14159)
来源：http://pxi.dianchejie.cn

C#:   3.14159.ToString("F2")
来源：http://njs.andypj.xyz

[A22] 获取字符串长度
来源：http://ioc.zhixingplan.top

Py:   len(s)
来源：http://utq.shangyingyoupin.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lni.ydjk.org.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kyp.hcnkem.com

TS:   s.length
来源：http://gkm.zhijiandao.cn

Java: s.length()
来源：http://prm.zdqjudy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kic.jqgfzy.top

Ruby: s.length
来源：http://gbu.haohaochexian.top

C#:   s.Length
来源：http://ikk.hywenlv.cn

[A23] 大小写转换
来源：http://vzg.xuanzx.com

Py:   s.upper(); s.lower(); s.title()
来源：http://ckm.xinyue.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vwj.sxryk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jue.ydjk.org.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zbc.cucudq.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zrg.havefunace.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aum.yuanzhike.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://spl.zhijiandao.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wlu.hnxiangtu.top

[A24] 去除首尾空白
来源：http://mfw.gotoacloud.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xst.zhoulong.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xzf.yueranfly.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tql.redwolf501.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dcm.zdqjudy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jxr.jinqigufen.top

Go:   strings.TrimSpace(s)
来源：http://pxh.zhiwuduotai.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://llg.cdnleiting.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hbn.hysaishi.cn

[A25] 字符串比较
来源：http://vof.ybcxt.top

Py:   s1 == s2; s1 != s2
来源：http://stg.jianghu66.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wqs.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sxe.daxiang520.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ani.jinghuilouyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eny.chenjidiqi.icu

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qby.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oqc.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yna.xinyue.icu

[A26] 类型转换总览
来源：http://zad.yj202588.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gue.ctjpmb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fhp.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lgh.ctjpmb.com

TS:   Number() String() Boolean() x as number
来源：http://wkm.bbcook.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wjd.cheryme.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://plc.zdbjq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://clz.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vxg.tianlin.xyz

================================================================================
来源：http://rjd.shanyushiyangtech.top

B. 流程控制
来源：http://icg.cqqwz.cn

================================================================================
来源：http://qnl.vehdjk.com

[B01] 条件判断 if / else
来源：http://iue.sxryk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oqg.shuidangran.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hxm.wangdashe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vwn.tian-w.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yjc.cqqwz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://glz.fanxiaobao.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yzh.ywan-chungtsiang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yuj.chenjidiqi.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ofw.cucudq.cn

[B02] 多分支 else if / elif
来源：http://cdx.yj202588.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hnh.jianghu66.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gij.yj20258888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zrb.ivvv.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ucf.hcnkem.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://khq.tian-w.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://amp.ybcxt.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vvt.tanke756.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rxq.xuanzx.com

[B03] switch / match / case
来源：http://viz.tarul.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wie.wangshuangyany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wua.jlsjyb.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iyd.xinyue.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gty.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cmb.aizwys.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zru.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yjv.pycfn.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dwu.wangdashe.top

[B04] for 计数循环
来源：http://gwy.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://wuy.pengpengdd.cyou

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ats.havefunace.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dso.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bwe.fehbvm.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://igz.ybcxt.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lpo.nanxuanxn.top

Ruby: 10.times { |i| puts i }
来源：http://sqg.yanxiufei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://miz.0kj1m.cn

[B05] 遍历数组 / 列表
来源：http://hgm.ivvv.top

Py:   for item in arr: print(item)
来源：http://xws.zycfv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://upb.zhijiandao.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uqe.9152youxi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ywg.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://nqe.xuanzx.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wsn.shuidangran.top

Ruby: arr.each { |item| puts item }
来源：http://psa.xylfe.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fcl.sjlbkw.cn

[B06] 遍历字典 / 对象
来源：http://knl.xinyue.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://nin.sysykeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ihh.shanyushiyangtech.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wkk.jlsjyb.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xgb.aizwys.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kcn.dianchejie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oks.ppjwa.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pdn.fzhhl.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qbc.zdbjq.cn

[B07] while 循环
来源：http://zaf.yj20258.top

Py:   while i < 10: i += 1
来源：http://ewe.gotoacloud.top

PHP:  while ($i < 10) { $i++; }
来源：http://dza.ywan-chungtsiang.top

JS:   while (i < 10) { i++; }
来源：http://hcb.bjfxy.top

TS:   while (i < 10) { i++; }
来源：http://duo.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://ool.yuanzhike.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tbs.sweek.top

Ruby: while i < 10; i += 1; end
来源：http://hta.sysykeji.top

C#:   while (i < 10) { i++; }
来源：http://tha.tarul.cn

[B08] do-while（至少执行一次）
来源：http://iht.tanke756.top

Py:   # 无 do-while：用 while True + break
来源：http://qsr.chenzaomai.com

PHP:  do { $i++; } while ($i < 10);
来源：http://crt.cqqwz.cn

JS:   do { i++; } while (i < 10);
来源：http://oop.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://omy.yongpay.top

Java: do { i++; } while (i < 10);
来源：http://tnx.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yjr.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://axz.hywenlv.cn

C#:   do { i++; } while (i < 10);
来源：http://nmu.0kj1m.cn

[B09] break 与 continue
来源：http://zxi.gotoacloud.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://chw.sufxvd.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eqj.yangfankeji.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ddd.guowangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cny.hesvh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xii.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fib.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://deh.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ueu.zhixingplan.top

[B10] 遍历同时拿索引
来源：http://yij.cheryme.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bhy.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gxt.zycfv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nfs.yangfankeji.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yth.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dlp.sweek.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wzd.uphjek.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dtz.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jhq.xuanzx.com

[B11] 生成数字序列 / 区间
来源：http://slj.chenlongwang.top

Py:   list(range(0, 10, 2))
来源：http://hwd.sjlbkw.cn

PHP:  range(0, 10, 2);
来源：http://flp.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xie.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tlu.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cxb.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uml.shangyingyoupin.top

Ruby: (0...10).step(2).to_a
来源：http://mac.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zpo.c1oappe.top

[B12] 跳出多层循环
来源：http://ptz.gogol.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ljv.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ayu.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://unl.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://als.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://owg.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iyc.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dyp.jqgufenzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hyq.zhaomingkeji.xyz

[B13] 判断是否为数字
来源：http://tjy.yvedp.cn

Py:   isinstance(x, (int, float))
来源：http://xco.aibaodan.cn

PHP:  is_numeric($x)
来源：http://swv.yonumen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zas.jinghuilouyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rrf.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://eom.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://plc.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://ich.hesvh.cn

C#:   x is int or double or decimal
来源：http://rqt.ywan-chungtsiang.top

[B14] 判断值是否在集合内
来源：http://xpb.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ejk.xinyue.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wos.gotoacloud.top

JS:   [1, 2, 3].includes(x)
来源：http://hlc.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://pgd.316326.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://fzl.vqdsnc.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://obh.shuidangran.top

Ruby: [1, 2, 3].include?(x)
来源：http://csv.sysykeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oon.yuxming.cn

[B15] 布尔运算与取反
来源：http://amg.tian-w.cn

Py:   a and b or not c
来源：http://ptn.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://bfx.tarul.cn

JS:   a && b || !c
来源：http://aip.sjlbkw.cn

TS:   a && b || !c
来源：http://wuf.nwbrower.top

Java: a && b || !c
来源：http://vcj.shangyingyoupin.top

Go:   a && b || !c
来源：http://dni.smart0.xyz

Ruby: a && b || !c
来源：http://zfj.ivvv.top

C#:   a && b || !c
来源：http://clv.xylfe.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nvs.cucudq.cn

Py:   if not data: return
来源：http://bba.316326.xyz

PHP:  if (!$data) { return; }
来源：http://hba.cucudq.cn

JS:   if (!data) return;
来源：http://zuj.mhx1999.top

TS:   if (!data) return;
来源：http://qvx.uphjek.com

Java: if (data == null) return;
来源：http://opc.guowangkeji.top

Go:   if data == nil { return }
来源：http://ust.fengsongda.top

Ruby: return if data.nil?
来源：http://kws.hcnkem.com

C#:   if (data == null) return;
来源：http://frs.nanxuanxn.top

================================================================================
来源：http://bkc.smart0.xyz

C. 函数与作用域
来源：http://hyw.yuanzhike.top

================================================================================
来源：http://mxs.sjlbkw.cn

[C01] 定义函数
来源：http://kkp.yj202588.top

Py:   def add(a, b): return a + b
来源：http://omt.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wws.daxiang520.top

JS:   function add(a, b) { return a + b; }
来源：http://vgu.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yuk.jianghu66.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mya.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://aok.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://psa.fktsv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cvo.yuanzhike.top

[C02] 默认参数
来源：http://elo.jinyuanbaomall.cn

Py:   def greet(name="World"): return name
来源：http://uwb.guannengcc.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mfn.cashguo.top

JS:   function greet(name = "World") { return name; }
来源：http://ftj.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ups.aizwys.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fwu.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jxt.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://bqs.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://kgq.xuanzx.com

[C03] 可变参数
来源：http://ofd.nanxuanxn.top

Py:   def total(*args): return sum(args)
来源：http://ksq.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qro.shzxlz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yfc.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dmy.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://trt.vqdsnc.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cbh.hesvh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qab.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bfk.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://gtw.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ltl.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://btz.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://erl.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hqr.zdqjudy.top

Java: // 无：用 Builder 模式或 record
来源：http://ksf.yueranfly.top


<!-- 参考信息 -->