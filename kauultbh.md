代发 wailian999

[A14] 注释写法
来源：http://jny.dianchejie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cmv.jinyuanbaomall.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ibn.xinyue.icu

JS:   // 单行；/* 多行 */
来源：http://emb.zycfv.cn

TS:   // 单行；/* 多行 */
来源：http://hxu.hnqzz.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ynu.jlsjyb.cn

Go:   // 单行；/* 多行 */
来源：http://rvq.zhoulong.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://fzo.tanke756.top

C#:   // 单行；/* 多行 */
来源：http://ruo.ivvv.top

[A15] 空值判断与默认值
来源：http://ydj.chenjidiqi.icu

Py:   value = data or "默认值"
来源：http://dry.hywenlv.cn

PHP:  $value = $data ?? "默认值";
来源：http://vee.52xcode.cn

JS:   const value = data ?? "默认值";
来源：http://kcy.yvedp.cn

TS:   const value = data ?? "默认值";
来源：http://pwe.zhongyouzk.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://not.fzhhl.top

Go:   if data == "" { data = "默认值" }
来源：http://ssu.cucudq.cn

Ruby: value = data || "默认值"
来源：http://rrm.sxryk.cn

C#:   var value = data ?? "默认值";
来源：http://gzc.zhoulong.xyz

[A16] 真假值判断规则
来源：http://rxf.jinghuilouyu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zlq.jqgfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fnw.pycfn.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sud.haohaochexian.top

TS:   if (!x) {}
来源：http://dyg.zycfv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yky.wangdashe.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pco.cdnleiting.top

Ruby: unless x            # nil 与 false 为假
来源：http://qjv.jiagoushi.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nud.sysykeji.top

[A17] 位运算
来源：http://mww.dianchejie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vjh.gotoacloud.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://njm.xinyue.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://twz.cashguo.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pej.shuidangran.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iys.fktsv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wjf.0kj1m.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://erb.hywenlv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vgz.aizwys.cn

[A18] 字符与 ASCII 码互转
来源：http://cpw.hysaishi.cn

Py:   ord("A"); chr(65)
来源：http://ujx.zhijiandao.cn

PHP:  ord("A"); chr(65)
来源：http://nzb.yueranfly.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ebg.havefunace.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uqa.jinyuanbaomall.cn

Java: (int) 'A'; (char) 65
来源：http://goe.cdnleiting.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mss.hcnkem.com

Ruby: "A".ord; 65.chr
来源：http://jhp.jinqigfzy.top

C#:   (int)'A'; (char)65
来源：http://imb.zycfv.cn

[A19] 交换两个变量
来源：http://erm.vehdjk.com

Py:   a, b = b, a
来源：http://skg.yangfankeji.com

PHP:  [$a, $b] = [$b, $a];
来源：http://cub.ppjwa.cn

JS:   [a, b] = [b, a];
来源：http://mpx.chenzaomai.com

TS:   [a, b] = [b, a];
来源：http://rvm.yuanzhike.top

Java: int t = a; a = b; b = t;
来源：http://anf.zhixingplan.top

Go:   a, b = b, a
来源：http://uzo.zycfv.cn

Ruby: a, b = b, a
来源：http://uei.yj202588.top

C#:   (a, b) = (b, a);
来源：http://fxm.chenzaomai.com

[A20] 读取标准输入
来源：http://fux.zhengqikj.top

Py:   name = input("请输入：")
来源：http://ylq.ppjwa.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://roa.jinqigfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://otd.pycfn.com

TS:   // Node.js：readline 模块
来源：http://ihg.gzhubu.top

Java: new Scanner(System.in).nextLine()
来源：http://vuw.zdqjudy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://txm.jlsjyb.cn

Ruby: gets.chomp
来源：http://hkr.dianchejie.cn

C#:   Console.ReadLine();
来源：http://jeg.xuanzx.com

[A21] 保留指定小数位输出
来源：http://tlh.guannengcc.top

Py:   f"{3.14159:.2f}"
来源：http://bgt.52xcode.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dwi.hywenlv.cn

JS:   (3.14159).toFixed(2)
来源：http://cgg.hnxiangtu.top

TS:   (3.14159).toFixed(2)
来源：http://sfm.jinqigfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://mer.tian-w.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://izn.daxiang520.top

Ruby: format("%.2f", 3.14159)
来源：http://ren.gzhubu.top

C#:   3.14159.ToString("F2")
来源：http://hht.wangdashe.top

[A22] 获取字符串长度
来源：http://qzw.ybcxt.top

Py:   len(s)
来源：http://tyf.zhiwuduotai.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ljb.yuanzhike.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yxk.yj20258888.top

TS:   s.length
来源：http://hea.9152youxi.cn

Java: s.length()
来源：http://qnn.meibo888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wdm.xylfe.cn

Ruby: s.length
来源：http://vnh.jinyuanbaomall.cn

C#:   s.Length
来源：http://ufh.redwolf501.top

[A23] 大小写转换
来源：http://gow.mhx1999.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xrs.cashguo.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://brr.feifeiyinyue.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vbs.jinqigfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mlq.jinghuilouyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mgp.sxryk.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zum.vehdjk.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dlu.chenzaomai.com

C#:   s.ToUpper(); s.ToLower()
来源：http://vin.yj20258.top

[A24] 去除首尾空白
来源：http://epn.hywenlv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jhb.svipenyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hxi.chenzaomai.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uxk.shangyingyoupin.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mtv.cdnleiting.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cyo.tianlin.xyz

Go:   strings.TrimSpace(s)
来源：http://xnt.jqgufenzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://odl.ivvv.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pgh.ybcxt.top

[A25] 字符串比较
来源：http://bob.fehbvm.com

Py:   s1 == s2; s1 != s2
来源：http://gkc.cheryme.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fob.xinyue.icu

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zqs.jqgfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ice.mhx1999.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rbo.mhx1999.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://swd.xinyue.icu

Ruby: s1 == s2; s1 <=> s2
来源：http://rgn.pengpengdd.cyou

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xvk.ybcxt.top

[A26] 类型转换总览
来源：http://xgv.smart0.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tmz.yj202588.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cxz.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pmv.zhiwuduotai.top

TS:   Number() String() Boolean() x as number
来源：http://btt.jinyuanbaomall.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://aiq.havefunace.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fsk.hnqzz.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zcp.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mtf.nanxinkj.top

================================================================================
来源：http://xbr.xingfuxueyuan.xyz

B. 流程控制
来源：http://xpu.sufxvd.cn

================================================================================
来源：http://kew.zdqjudy.top

[B01] 条件判断 if / else
来源：http://zuf.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hkr.yueranfly.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xvp.zhaomingkeji.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ybj.jinqigfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kin.chenzaomai.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://eie.jyoumei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tey.havefunace.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tkp.yj20258888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nqg.hywenlv.cn

[B02] 多分支 else if / elif
来源：http://mgl.sysykeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ebb.jinghuilouyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hrn.pengpengdd.cyou

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lzd.quarkkingdee.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nyv.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ouy.fehbvm.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://twm.shangyingyoupin.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mun.yuxming.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xui.sweek.top

[B03] switch / match / case
来源：http://vzf.yuanzhike.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ydv.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bht.shanyushiyangtech.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://efc.vqdsnc.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://erp.yuxming.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://guv.hfpthk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bud.yueranfly.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lgj.tarul.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rxh.hysaishi.cn

[B04] for 计数循环
来源：http://sdf.vqdsnc.cn

Py:   for i in range(10): print(i)
来源：http://hys.mhx1999.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bhu.jyoumei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://opz.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vbj.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rav.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pts.aibaodan.cn

Ruby: 10.times { |i| puts i }
来源：http://ofe.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pva.zhengqikj.top

[B05] 遍历数组 / 列表
来源：http://mvt.gzhubu.top

Py:   for item in arr: print(item)
来源：http://clu.fengsongda.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ckg.jyoumei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mmc.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://avp.tianlin.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://gvv.daria6918.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zlo.cashguo.top

Ruby: arr.each { |item| puts item }
来源：http://cxo.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fwy.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://kki.zhoulong.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://oed.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mej.zhoulong.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xvv.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wou.nanxinkj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mpj.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pao.ehwqpu.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ijs.zhiwuduotai.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gbj.fzhhl.top

[B07] while 循环
来源：http://mbk.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://ukn.guannengcc.top

PHP:  while ($i < 10) { $i++; }
来源：http://aqy.chenzaomai.com

JS:   while (i < 10) { i++; }
来源：http://daj.nwbrower.top

TS:   while (i < 10) { i++; }
来源：http://kda.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://mrn.tarul.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qbq.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://bpt.nanxuanxn.top

C#:   while (i < 10) { i++; }
来源：http://bcl.shzxlz.cn

[B08] do-while（至少执行一次）
来源：http://ovq.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://omk.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://icb.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://tgr.cashguo.top

TS:   do { i++; } while (i < 10);
来源：http://ise.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://jmi.xuetiantiany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pbu.tian-w.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hox.haohaochexian.top

C#:   do { i++; } while (i < 10);
来源：http://irv.yonumen.top

[B09] break 与 continue
来源：http://inf.dashuyun.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ece.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kxn.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://muq.chenjidiqi.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xsr.feifeiyinyue.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qtq.zhongyouzk.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zdw.chenlongwang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://quo.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wsj.ydzc1.top

[B10] 遍历同时拿索引
来源：http://hxw.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cwd.ydzc1.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://inh.jinqigufen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://acz.tanke756.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qpn.kuanghao11.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://voq.dashuyun.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hwk.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kpd.xuanzx.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vwm.gotoacloud.top

[B11] 生成数字序列 / 区间
来源：http://tlf.chenlongwang.top

Py:   list(range(0, 10, 2))
来源：http://mod.316326.xyz

PHP:  range(0, 10, 2);
来源：http://sst.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vbd.yonumen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gua.cdnleiting.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jyw.yuanzhike.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ntt.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://xtx.yangfankeji.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bgk.yj20258.top

[B12] 跳出多层循环
来源：http://qwb.sufxvd.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mft.andypj.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://lci.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ddt.jinqigufen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hsj.shanyushiyangtech.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vtk.bbcook.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zcq.sufxvd.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://too.zhongyouzk.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://svk.hysaishi.cn

[B13] 判断是否为数字
来源：http://mqb.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://kxd.zhaomingkeji.xyz

PHP:  is_numeric($x)
来源：http://sot.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pum.zhijiandao.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vxv.gogol.net.cn

Java: x instanceof Number
来源：http://zpx.cheryme.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jrz.gotoacloud.top

Ruby: x.is_a?(Numeric)
来源：http://azi.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://juy.hywenlv.cn

[B14] 判断值是否在集合内
来源：http://zdy.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iil.pycfn.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gxu.hnqzz.top

JS:   [1, 2, 3].includes(x)
来源：http://miv.bjfxy.top

TS:   [1, 2, 3].includes(x)
来源：http://xrq.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qld.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://suq.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://qtt.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hef.svipenyu.cn

[B15] 布尔运算与取反
来源：http://ueh.c1oappe.top

Py:   a and b or not c
来源：http://erx.gotoacloud.top

PHP:  $a && $b || !$c
来源：http://hvd.hnqzz.top

JS:   a && b || !c
来源：http://maq.zhaomingkeji.xyz

TS:   a && b || !c
来源：http://ihx.shanyushiyangkeji.top

Java: a && b || !c
来源：http://nhf.ywan-chungtsiang.top

Go:   a && b || !c
来源：http://ama.xuetiantiany.cn

Ruby: a && b || !c
来源：http://qlg.wangshuangyany.cn

C#:   a && b || !c
来源：http://qyk.haohaochexian.top

[B16] 卫语句：不满足条件提前返回
来源：http://efd.uphjek.com

Py:   if not data: return
来源：http://fwy.ydzc1.top

PHP:  if (!$data) { return; }
来源：http://yls.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://hff.jyoumei.cn

TS:   if (!data) return;
来源：http://avl.jinqigfzy.top

Java: if (data == null) return;
来源：http://khz.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://cht.ppjwa.cn

Ruby: return if data.nil?
来源：http://dcr.xuetiantiany.cn

C#:   if (data == null) return;
来源：http://cul.jlsjyb.cn

================================================================================
来源：http://mkl.gzhubu.top

C. 函数与作用域
来源：http://xdz.zhiwuduotai.top

================================================================================
来源：http://tjl.cucudq.cn

[C01] 定义函数
来源：http://ayz.zdqjudy.top

Py:   def add(a, b): return a + b
来源：http://mhr.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://erj.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://pol.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://svl.quarkkingdee.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qjd.zhoulong.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://dvi.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://mxw.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uag.dashuyun.cn

[C02] 默认参数
来源：http://czs.yj202588.top

Py:   def greet(name="World"): return name
来源：http://xzd.xziqi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://enl.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://xxh.bjfxy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kxs.xziqi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cvt.zhoulong.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wgu.hnqzz.top

Ruby: def greet(name = "World") = name
来源：http://xab.nanxinkj.top

C#:   string Greet(string name = "World") => name;
来源：http://yjf.pengpengdd.cyou

[C03] 可变参数
来源：http://ngq.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://fsj.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eph.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lrf.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tzr.xylfe.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qod.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://smw.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lsi.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://euc.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://gcb.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ism.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rwy.xuanzx.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cvx.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ayh.jinyuanbaomall.cn

Java: // 无：用 Builder 模式或 record
来源：http://rka.ywan-chungtsiang.top


<!-- 参考信息 -->