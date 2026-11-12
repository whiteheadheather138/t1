代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://yai.fehbvm.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lzi.bbcook.cn

Go:   // 单行；/* 多行 */
来源：http://bha.yj20258.top

Ruby: # 单行；=begin 多行 =end
来源：http://uot.shuidangran.top

C#:   // 单行；/* 多行 */
来源：http://rrc.svipenyu.cn

[A15] 空值判断与默认值
来源：http://dzd.gzhubu.top

Py:   value = data or "默认值"
来源：http://pue.zhaomingkeji.xyz

PHP:  $value = $data ?? "默认值";
来源：http://kgg.yueranfly.top

JS:   const value = data ?? "默认值";
来源：http://qwy.jinqigfzy.top

TS:   const value = data ?? "默认值";
来源：http://hma.jinyuanbaomall.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lip.xinyue.icu

Go:   if data == "" { data = "默认值" }
来源：http://qal.yj202588.top

Ruby: value = data || "默认值"
来源：http://kdn.cucudq.cn

C#:   var value = data ?? "默认值";
来源：http://eam.snrcjt.cn

[A16] 真假值判断规则
来源：http://iwx.yj202588.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tom.quarkkingdee.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://riw.xziqi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zkk.shanyushiyangkeji.top

TS:   if (!x) {}
来源：http://vpi.mhx1999.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://atd.xziqi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oyh.yueranfly.top

Ruby: unless x            # nil 与 false 为假
来源：http://jfb.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sek.yj202588.top

[A17] 位运算
来源：http://qcs.jinyuanbaomall.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://phy.sjlbkw.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dwv.yuxming.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iwy.hnxiangtu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fuk.uphjek.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bdh.yuanzhike.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lvb.mhx1999.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cnn.yanxiufei.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ezd.smart0.xyz

[A18] 字符与 ASCII 码互转
来源：http://hav.guowangkeji.top

Py:   ord("A"); chr(65)
来源：http://pjb.jinqigfzy.top

PHP:  ord("A"); chr(65)
来源：http://iac.sjlbkw.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hxd.aizwys.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qps.havefunace.top

Java: (int) 'A'; (char) 65
来源：http://ydw.xuanzx.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rca.zhixingplan.top

Ruby: "A".ord; 65.chr
来源：http://ism.guannengcc.top

C#:   (int)'A'; (char)65
来源：http://tir.gzhubu.top

[A19] 交换两个变量
来源：http://rkl.hongshengwenyu.top

Py:   a, b = b, a
来源：http://atf.quarkkingdee.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jhd.shangyingyoupin.top

JS:   [a, b] = [b, a];
来源：http://pav.aizwys.cn

TS:   [a, b] = [b, a];
来源：http://yuq.guannengcc.top

Java: int t = a; a = b; b = t;
来源：http://ohk.shangyingyoupin.top

Go:   a, b = b, a
来源：http://wve.zhaomingkeji.xyz

Ruby: a, b = b, a
来源：http://evb.vehdjk.com

C#:   (a, b) = (b, a);
来源：http://tmp.yvedp.cn

[A20] 读取标准输入
来源：http://dgs.zhijiandao.cn

Py:   name = input("请输入：")
来源：http://jly.jqgufenzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kmv.hfpthk.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mjf.jinqigfzy.top

TS:   // Node.js：readline 模块
来源：http://qxm.yangfankeji.com

Java: new Scanner(System.in).nextLine()
来源：http://vwq.guannengcc.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ife.mhx1999.top

Ruby: gets.chomp
来源：http://mlw.jqgfzy.top

C#:   Console.ReadLine();
来源：http://yau.sweek.top

[A21] 保留指定小数位输出
来源：http://chi.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://jmy.aibaodan.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ssx.nwbrower.top

JS:   (3.14159).toFixed(2)
来源：http://brf.cucudq.cn

TS:   (3.14159).toFixed(2)
来源：http://dti.sxryk.cn

Java: String.format("%.2f", 3.14159)
来源：http://xrd.gotoacloud.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tos.epnwcf.com

Ruby: format("%.2f", 3.14159)
来源：http://ced.yj20258888.top

C#:   3.14159.ToString("F2")
来源：http://eou.yfazqb.com

[A22] 获取字符串长度
来源：http://vke.shangyingyoupin.top

Py:   len(s)
来源：http://sma.nanxinkj.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mfx.tian-w.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pzp.smart0.xyz

TS:   s.length
来源：http://wvp.wangdashe.top

Java: s.length()
来源：http://pml.yuanzhike.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://abp.hysaishi.cn

Ruby: s.length
来源：http://wjj.meibo888.top

C#:   s.Length
来源：http://ysa.wangshuangyany.cn

[A23] 大小写转换
来源：http://vss.shanyushiyangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wvb.ydzc1.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xud.316326.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jhg.chenlongwang.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kpc.xylfe.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iit.fengsongda.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://chg.bbcook.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://smk.wangshuangyany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pmb.bjfxy.top

[A24] 去除首尾空白
来源：http://dpj.jyoumei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gws.jianghu66.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iqi.haohaochexian.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vlq.svipenyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cwx.smart0.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qdp.shuidangran.top

Go:   strings.TrimSpace(s)
来源：http://rgl.shzxlz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mkc.yonumen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zsn.fanxiaobao.xyz

[A25] 字符串比较
来源：http://jbb.52xcode.cn

Py:   s1 == s2; s1 != s2
来源：http://oew.wangdashe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qyd.yangfankeji.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rwt.tian-w.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nmi.jinyuanbaomall.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dje.chenjidiqi.icu

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dnb.0kj1m.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kjv.pengpengdd.cyou

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ulk.xinyue.icu

[A26] 类型转换总览
来源：http://npi.iojbl.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hus.jiagoushi.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xhr.zdbjq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fzb.zhiwuduotai.top

TS:   Number() String() Boolean() x as number
来源：http://tel.quarkkingdee.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kkm.bbcook.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cge.hammf.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rzf.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jhg.tianlin.xyz

================================================================================
来源：http://cxg.yonumen.top

B. 流程控制
来源：http://qkp.ppjwa.cn

================================================================================
来源：http://avf.shangyingyoupin.top

[B01] 条件判断 if / else
来源：http://jpj.zhiwuduotai.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ias.zycfv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dnj.uphjek.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zzw.wangdashe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bud.meibo888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ehz.bjfxy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jzy.yueranfly.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rhk.hongshengwenyu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kmv.meibo888.top

[B02] 多分支 else if / elif
来源：http://vwb.jinghuilouyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mxg.fanxiaobao.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lbd.shanyushiyangtech.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://exw.zhijiandao.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qro.sufxvd.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mkx.epnwcf.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ppf.xinyue.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://prq.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oxn.redwolf501.top

[B03] switch / match / case
来源：http://zwp.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rao.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pnn.shanyushiyangtech.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aot.xingfuxueyuan.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vlk.ywan-chungtsiang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mjs.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bee.mhx1999.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mgr.sysykeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://scp.svipenyu.cn

[B04] for 计数循环
来源：http://lkp.svipenyu.cn

Py:   for i in range(10): print(i)
来源：http://fbl.gotoacloud.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lts.xingfuxueyuan.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wwd.hammf.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dgq.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hll.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uln.gzhubu.top

Ruby: 10.times { |i| puts i }
来源：http://hdw.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ayy.gaohongyu789.top

[B05] 遍历数组 / 列表
来源：http://zdz.yonumen.top

Py:   for item in arr: print(item)
来源：http://ccl.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uqf.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://exl.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pyl.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://kuu.316326.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mwx.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://vxq.yj20258888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dxx.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://ywi.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nfm.hongshengwenyu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mse.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bba.cheryme.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jds.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://obw.wangdashe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kcm.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oak.zhaomingkeji.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nje.fengsongda.top

[B07] while 循环
来源：http://ppg.zhiwuduotai.top

Py:   while i < 10: i += 1
来源：http://tcl.smart0.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://vjl.pengpengdd.cyou

JS:   while (i < 10) { i++; }
来源：http://iwo.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://epe.yj20258888.top

Java: while (i < 10) { i++; }
来源：http://rfe.kuanghao11.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lgt.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://chj.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://kdi.c1oappe.top

[B08] do-while（至少执行一次）
来源：http://xgf.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://wzy.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rca.chenjidiqi.icu

JS:   do { i++; } while (i < 10);
来源：http://pjv.daria6918.cn

TS:   do { i++; } while (i < 10);
来源：http://tny.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://jer.sysykeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nrk.0kj1m.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uep.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://fgr.hywenlv.cn

[B09] break 与 continue
来源：http://mef.ybcxt.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mkl.hcnkem.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://znx.pengpengdd.cyou

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://plk.jinqigufen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://byj.yj202588.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://djy.zhongyouzk.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tqw.hcnkem.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ipw.yonumen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rau.fengsongda.top

[B10] 遍历同时拿索引
来源：http://fon.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://chp.ppjwa.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fbt.yfazqb.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xxf.yueranfly.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vqm.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://frf.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xor.316326.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jlz.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://niy.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://mru.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://xuo.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://ftb.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sgi.sxryk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cbh.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zco.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ziy.yvedp.cn

Ruby: (0...10).step(2).to_a
来源：http://icr.bjfxy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cbr.xinyue.icu

[B12] 跳出多层循环
来源：http://gcc.jinghuilouyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ynr.jinghuilouyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://coe.shanyushiyangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uef.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jpe.zhixingplan.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tpn.hesvh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xwp.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://skk.c1oappe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vhi.kuanghao11.cn

[B13] 判断是否为数字
来源：http://wfs.yanxiufei.cn

Py:   isinstance(x, (int, float))
来源：http://pbk.fehbvm.com

PHP:  is_numeric($x)
来源：http://boj.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qhs.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://evm.tanke756.top

Java: x instanceof Number
来源：http://vha.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rft.snrcjt.cn

Ruby: x.is_a?(Numeric)
来源：http://mzr.aizwys.cn

C#:   x is int or double or decimal
来源：http://zcd.hnqzz.top

[B14] 判断值是否在集合内
来源：http://fat.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://spi.xuanzx.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wvw.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://yig.gzhubu.top

TS:   [1, 2, 3].includes(x)
来源：http://obx.jinqigfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lgs.zhiwuduotai.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uln.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pma.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://for.yuxming.cn

[B15] 布尔运算与取反
来源：http://pcm.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://eya.zhiwuduotai.top

PHP:  $a && $b || !$c
来源：http://qrl.ivvv.top

JS:   a && b || !c
来源：http://imq.fzhhl.top

TS:   a && b || !c
来源：http://ohe.mhx1999.top

Java: a && b || !c
来源：http://dmt.hammf.cn

Go:   a && b || !c
来源：http://qte.c1oappe.top

Ruby: a && b || !c
来源：http://soe.mhx1999.top

C#:   a && b || !c
来源：http://qgw.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cqk.tanke756.top

Py:   if not data: return
来源：http://bbc.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://xqe.jianghu66.top

JS:   if (!data) return;
来源：http://iwq.xylfe.cn

TS:   if (!data) return;
来源：http://gdf.jianghu66.top

Java: if (data == null) return;
来源：http://mrp.yanxiufei.cn

Go:   if data == nil { return }
来源：http://mpb.jinqigufen.top

Ruby: return if data.nil?
来源：http://btj.ehwqpu.com

C#:   if (data == null) return;
来源：http://wfr.zhixingplan.top

================================================================================
来源：http://fow.9152youxi.cn

C. 函数与作用域
来源：http://vlk.smart0.xyz

================================================================================
来源：http://unu.zdqjudy.top

[C01] 定义函数
来源：http://mrw.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://snw.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xpj.zhixingplan.top

JS:   function add(a, b) { return a + b; }
来源：http://hiw.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uik.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hqa.hesvh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gfx.bbcook.cn

Ruby: def add(a, b); a + b; end
来源：http://zje.0kj1m.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ydu.hfpthk.cn

[C02] 默认参数
来源：http://tpp.cheryme.top

Py:   def greet(name="World"): return name
来源：http://qot.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cyf.hysaishi.cn

JS:   function greet(name = "World") { return name; }
来源：http://axh.chenlongwang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sob.ehwqpu.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ioa.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yer.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://exm.havefunace.top

C#:   string Greet(string name = "World") => name;
来源：http://ohi.nanxuanxn.top

[C03] 可变参数
来源：http://wqe.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://mae.haohaochexian.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://huu.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mfl.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qcq.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kgj.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gxp.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://gou.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jlk.shanyushiyangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://urn.jianghu66.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oca.sweek.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://smn.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nrb.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gvm.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://fxz.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://ayw.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://ngn.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://waw.zhengqikj.top

[C05] 返回多个值
来源：http://hsu.zhengqikj.top


<!-- 参考信息 -->