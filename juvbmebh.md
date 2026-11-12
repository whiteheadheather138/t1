代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://qgd.yangfankeji.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vmx.mhx1999.top

Go:   // 单行；/* 多行 */
来源：http://wgq.gaohongyu789.top

Ruby: # 单行；=begin 多行 =end
来源：http://idm.yanxiufei.cn

C#:   // 单行；/* 多行 */
来源：http://ase.ydjk.org.cn

[A15] 空值判断与默认值
来源：http://epn.smart0.xyz

Py:   value = data or "默认值"
来源：http://vsv.nanxinkj.top

PHP:  $value = $data ?? "默认值";
来源：http://zfz.hammf.cn

JS:   const value = data ?? "默认值";
来源：http://qbk.guowangkeji.top

TS:   const value = data ?? "默认值";
来源：http://jul.shuidangran.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xdx.hesvh.cn

Go:   if data == "" { data = "默认值" }
来源：http://qpv.yongpay.top

Ruby: value = data || "默认值"
来源：http://kme.xziqi.cn

C#:   var value = data ?? "默认值";
来源：http://bub.c1oappe.top

[A16] 真假值判断规则
来源：http://zfc.kuanghao11.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jaf.jinyuanbaomall.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://egc.hnxiangtu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mne.hysaishi.cn

TS:   if (!x) {}
来源：http://jfg.haohaochexian.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wbf.fengsongda.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uuc.yj20258.top

Ruby: unless x            # nil 与 false 为假
来源：http://bho.wangdashe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wgi.hnqzz.top

[A17] 位运算
来源：http://kbs.shuidangran.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kui.nwbrower.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gdg.aibaodan.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ccf.jinyuanbaomall.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xll.9152youxi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pfx.jianghu66.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://psv.chenlongwang.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fge.zhoulong.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bgn.hongshengwenyu.top

[A18] 字符与 ASCII 码互转
来源：http://vdz.nanxuanxn.top

Py:   ord("A"); chr(65)
来源：http://puh.daxiang520.top

PHP:  ord("A"); chr(65)
来源：http://mrt.fzhhl.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://skm.gaohongyu789.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fva.fanxiaobao.xyz

Java: (int) 'A'; (char) 65
来源：http://zzo.gzhubu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qen.zycfv.cn

Ruby: "A".ord; 65.chr
来源：http://rlb.cdnleiting.top

C#:   (int)'A'; (char)65
来源：http://xri.fehbvm.com

[A19] 交换两个变量
来源：http://ctz.guannengcc.top

Py:   a, b = b, a
来源：http://cus.iojbl.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vxg.zhixingplan.top

JS:   [a, b] = [b, a];
来源：http://fcj.zhixingplan.top

TS:   [a, b] = [b, a];
来源：http://sll.bbcook.cn

Java: int t = a; a = b; b = t;
来源：http://ttc.xinyue.icu

Go:   a, b = b, a
来源：http://ssv.hnxiangtu.top

Ruby: a, b = b, a
来源：http://ukp.yj20258.top

C#:   (a, b) = (b, a);
来源：http://kri.xuanzx.com

[A20] 读取标准输入
来源：http://bnk.hongshengwenyu.top

Py:   name = input("请输入：")
来源：http://axx.0kj1m.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://csh.haohaochexian.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cym.jiagoushi.top

TS:   // Node.js：readline 模块
来源：http://rib.zhongyouzk.top

Java: new Scanner(System.in).nextLine()
来源：http://ihx.gzhubu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sxc.jinghuilouyu.cn

Ruby: gets.chomp
来源：http://urb.zdbjq.cn

C#:   Console.ReadLine();
来源：http://jls.xinyue.icu

[A21] 保留指定小数位输出
来源：http://dvt.fktsv.cn

Py:   f"{3.14159:.2f}"
来源：http://xvk.chenlongwang.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://irh.guannengcc.top

JS:   (3.14159).toFixed(2)
来源：http://dkn.guowangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://nwp.xylfe.cn

Java: String.format("%.2f", 3.14159)
来源：http://wde.vqdsnc.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vcu.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://htr.zhijiandao.cn

C#:   3.14159.ToString("F2")
来源：http://prk.ppjwa.cn

[A22] 获取字符串长度
来源：http://zjg.dashuyun.cn

Py:   len(s)
来源：http://inu.zhixingplan.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://akb.chenjidiqi.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oox.xuetiantiany.cn

TS:   s.length
来源：http://hre.daria6918.cn

Java: s.length()
来源：http://ymp.sxryk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://skt.chenjidiqi.icu

Ruby: s.length
来源：http://ozc.zhoulong.xyz

C#:   s.Length
来源：http://quu.jinghuilouyu.cn

[A23] 大小写转换
来源：http://uel.yj20258888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wbp.chenzaomai.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jec.zdbjq.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hms.shangyingyoupin.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kzy.cashguo.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ksf.jqgufenzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wdy.bjfxy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bhe.hnqzz.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lbw.cdnleiting.top

[A24] 去除首尾空白
来源：http://cbb.meibo888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yzg.aizwys.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gsl.gogol.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fas.xuetiantiany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fdv.meibo888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://krr.9152youxi.cn

Go:   strings.TrimSpace(s)
来源：http://olo.jqgfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ifl.shangyingyoupin.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qgk.gzhubu.top

[A25] 字符串比较
来源：http://mue.cdnleiting.top

Py:   s1 == s2; s1 != s2
来源：http://lpz.shanyushiyangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mwu.jinyuanbaomall.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://shl.jinqigfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hel.aibaodan.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kwe.cdnleiting.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uix.yfazqb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://cww.sxryk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yck.zdqjudy.top

[A26] 类型转换总览
来源：http://sbf.smart0.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mdt.daxiang520.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nrf.haohaochexian.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://alh.pycfn.com

TS:   Number() String() Boolean() x as number
来源：http://fhl.hammf.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xfv.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fbd.ppjwa.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bxx.gotoacloud.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cfa.iojbl.cn

================================================================================
来源：http://mtk.0kj1m.cn

B. 流程控制
来源：http://zif.tian-w.cn

================================================================================
来源：http://rqu.shangyingyoupin.top

[B01] 条件判断 if / else
来源：http://bvc.nwbrower.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fgr.yuanzhike.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vvu.fanxiaobao.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ubf.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xxc.yuanzhike.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tnf.andypj.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zvw.dianchejie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wcg.yj20258.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cai.c1oappe.top

[B02] 多分支 else if / elif
来源：http://gaj.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rrn.epnwcf.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wid.havefunace.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bzg.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lru.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hiy.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dgo.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dxo.fengsongda.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wgm.uphjek.com

[B03] switch / match / case
来源：http://vxf.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mzx.cheryme.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pjz.zhiwuduotai.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yoa.meibo888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vpb.bjfxy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://umr.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qjd.wangdashe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jtp.quarkkingdee.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sdk.kuanghao11.cn

[B04] for 计数循环
来源：http://yai.fktsv.cn

Py:   for i in range(10): print(i)
来源：http://lbz.fanxiaobao.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tpu.tian-w.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zvv.vehdjk.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xaa.aizwys.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oar.yj202588.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qlf.birdmap.top

Ruby: 10.times { |i| puts i }
来源：http://hjs.birdmap.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://whh.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://lto.yj20258888.top

Py:   for item in arr: print(item)
来源：http://pnp.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fkd.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gmz.yvedp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vvw.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uhe.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kxv.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://mca.316326.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ajy.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://hbc.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ibc.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yxj.jqgfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mjt.ydzc1.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cld.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gvu.vqdsnc.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wtm.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ylm.jiagoushi.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bch.shanyushiyangtech.top

[B07] while 循环
来源：http://gau.ydzc1.top

Py:   while i < 10: i += 1
来源：http://fnn.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://opp.sxryk.cn

JS:   while (i < 10) { i++; }
来源：http://xsw.shzxlz.cn

TS:   while (i < 10) { i++; }
来源：http://ozx.guannengcc.top

Java: while (i < 10) { i++; }
来源：http://fvf.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xdw.zhaomingkeji.xyz

Ruby: while i < 10; i += 1; end
来源：http://kdo.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://deg.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://unf.fehbvm.com

Py:   # 无 do-while：用 while True + break
来源：http://kru.shanyushiyangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hvf.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://aqv.tanke756.top

TS:   do { i++; } while (i < 10);
来源：http://lza.xingfuxueyuan.xyz

Java: do { i++; } while (i < 10);
来源：http://onu.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ewn.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://ljq.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://pea.mhx1999.top

[B09] break 与 continue
来源：http://zzo.9152youxi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bnd.yuanzhike.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ngs.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vep.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://otq.yueranfly.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zdh.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eif.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sze.hfpthk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lal.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://jrd.tian-w.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qkx.hywenlv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xiv.tianlin.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qer.nwbrower.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gwx.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://amb.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cud.aizwys.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cuu.tanke756.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yqm.feifeiyinyue.top

[B11] 生成数字序列 / 区间
来源：http://rig.xinyue.icu

Py:   list(range(0, 10, 2))
来源：http://mbd.dianchejie.cn

PHP:  range(0, 10, 2);
来源：http://bqx.zhixingplan.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://epw.xylfe.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cnu.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hss.wangshuangyany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fox.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://rhq.hnxiangtu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gnb.vehdjk.com

[B12] 跳出多层循环
来源：http://zhf.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://oui.sjlbkw.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mrt.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lvz.yj20258.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aub.zdqjudy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bsx.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://plg.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qku.hfpthk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://per.shanyushiyangkeji.top

[B13] 判断是否为数字
来源：http://imh.hysaishi.cn

Py:   isinstance(x, (int, float))
来源：http://jkk.jqgufenzy.top

PHP:  is_numeric($x)
来源：http://gov.zhaomingkeji.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qbt.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jdd.ydjk.org.cn

Java: x instanceof Number
来源：http://wxs.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ksu.hnqzz.top

Ruby: x.is_a?(Numeric)
来源：http://dig.nanxinkj.top

C#:   x is int or double or decimal
来源：http://sjw.smart0.xyz

[B14] 判断值是否在集合内
来源：http://uxn.gaohongyu789.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://omp.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vtq.shuidangran.top

JS:   [1, 2, 3].includes(x)
来源：http://xuy.zdbjq.cn

TS:   [1, 2, 3].includes(x)
来源：http://hdl.bjfxy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://iyk.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zjh.jqgufenzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://nuq.pycfn.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zeh.hysaishi.cn

[B15] 布尔运算与取反
来源：http://zyi.nwbrower.top

Py:   a and b or not c
来源：http://lmh.52xcode.cn

PHP:  $a && $b || !$c
来源：http://mbm.quarkkingdee.top

JS:   a && b || !c
来源：http://jbu.yj20258.top

TS:   a && b || !c
来源：http://mbn.hongshengwenyu.top

Java: a && b || !c
来源：http://uqq.nwbrower.top

Go:   a && b || !c
来源：http://cel.fzhhl.top

Ruby: a && b || !c
来源：http://mon.yj202588.top

C#:   a && b || !c
来源：http://uma.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://umz.nanxuanxn.top

Py:   if not data: return
来源：http://wgm.wangdashe.top

PHP:  if (!$data) { return; }
来源：http://ibt.zhongyouzk.top

JS:   if (!data) return;
来源：http://yly.xuanzx.com

TS:   if (!data) return;
来源：http://sxq.birdmap.top

Java: if (data == null) return;
来源：http://nxs.ydjk.org.cn

Go:   if data == nil { return }
来源：http://vgw.hnxiangtu.top

Ruby: return if data.nil?
来源：http://anp.ppjwa.cn

C#:   if (data == null) return;
来源：http://ebp.zhongyouzk.top

================================================================================
来源：http://wkr.ydzc1.top

C. 函数与作用域
来源：http://sph.xylfe.cn

================================================================================
来源：http://smd.dianchejie.cn

[C01] 定义函数
来源：http://qqp.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://kig.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wme.ydjk.org.cn

JS:   function add(a, b) { return a + b; }
来源：http://vil.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tdj.birdmap.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bjz.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://hnx.shangyingyoupin.top

Ruby: def add(a, b); a + b; end
来源：http://zgx.jyoumei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vki.cheryme.top

[C02] 默认参数
来源：http://nyh.tianlin.xyz

Py:   def greet(name="World"): return name
来源：http://bfc.gogol.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yhj.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://vze.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wie.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bav.shanyushiyangtech.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://twd.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://yod.zhixingplan.top

C#:   string Greet(string name = "World") => name;
来源：http://faj.hcnkem.com

[C03] 可变参数
来源：http://uir.jinghuilouyu.cn

Py:   def total(*args): return sum(args)
来源：http://eet.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zzh.yuxming.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rgg.zhijiandao.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zqn.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://upu.nanxinkj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ezl.yueranfly.top

Ruby: def total(*nums); nums.sum; end
来源：http://elh.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mll.zhijiandao.cn

[C04] 命名参数 / 关键字参数
来源：http://fgk.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://psg.shuidangran.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hca.haohaochexian.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xyl.wangshuangyany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://esv.cucudq.cn

Java: // 无：用 Builder 模式或 record
来源：http://yvq.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://kad.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://fer.yfazqb.com

C#:   f(a: 1, b: 2)
来源：http://uwu.yj202588.top

[C05] 返回多个值
来源：http://qsd.sxryk.cn


<!-- 参考信息 -->