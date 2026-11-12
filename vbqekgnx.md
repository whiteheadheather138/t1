代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://dxr.mhx1999.top

[A15] 空值判断与默认值
来源：http://gtk.chenjidiqi.icu

Py:   value = data or "默认值"
来源：http://ekv.pycfn.com

PHP:  $value = $data ?? "默认值";
来源：http://zbu.fktsv.cn

JS:   const value = data ?? "默认值";
来源：http://xiv.xuanzx.com

TS:   const value = data ?? "默认值";
来源：http://jwm.aibaodan.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hcs.quarkkingdee.top

Go:   if data == "" { data = "默认值" }
来源：http://vqw.guowangkeji.top

Ruby: value = data || "默认值"
来源：http://bmo.xziqi.cn

C#:   var value = data ?? "默认值";
来源：http://vai.yvedp.cn

[A16] 真假值判断规则
来源：http://dop.fanxiaobao.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dur.zdbjq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jak.0kj1m.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mca.andypj.xyz

TS:   if (!x) {}
来源：http://qts.gaohongyu789.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jrp.ehwqpu.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fic.pengpengdd.cyou

Ruby: unless x            # nil 与 false 为假
来源：http://kkm.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mzf.chenjidiqi.icu

[A17] 位运算
来源：http://dhz.feifeiyinyue.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ddm.haohaochexian.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tfc.yongpay.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lve.jianghu66.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tug.guowangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yiq.nwbrower.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vkt.316326.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pfn.fengsongda.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jad.zhengqikj.top

[A18] 字符与 ASCII 码互转
来源：http://ive.chenzaomai.com

Py:   ord("A"); chr(65)
来源：http://igv.ydzc1.top

PHP:  ord("A"); chr(65)
来源：http://csq.yj20258888.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nqp.nwbrower.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wjs.aibaodan.cn

Java: (int) 'A'; (char) 65
来源：http://otz.gotoacloud.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wdx.hywenlv.cn

Ruby: "A".ord; 65.chr
来源：http://irk.xylfe.cn

C#:   (int)'A'; (char)65
来源：http://ueh.yongpay.top

[A19] 交换两个变量
来源：http://vba.hnxiangtu.top

Py:   a, b = b, a
来源：http://iup.tian-w.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jgr.ppjwa.cn

JS:   [a, b] = [b, a];
来源：http://qiu.jlsjyb.cn

TS:   [a, b] = [b, a];
来源：http://fjz.gogol.net.cn

Java: int t = a; a = b; b = t;
来源：http://ujg.hnqzz.top

Go:   a, b = b, a
来源：http://kky.hcnkem.com

Ruby: a, b = b, a
来源：http://ijk.fzhhl.top

C#:   (a, b) = (b, a);
来源：http://brq.snrcjt.cn

[A20] 读取标准输入
来源：http://lsp.xziqi.cn

Py:   name = input("请输入：")
来源：http://gdv.gaohongyu789.top

PHP:  $name = trim(fgets(STDIN));
来源：http://dpg.jlsjyb.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mqg.chenzaomai.com

TS:   // Node.js：readline 模块
来源：http://aty.tian-w.cn

Java: new Scanner(System.in).nextLine()
来源：http://gxx.jlsjyb.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lsm.xylfe.cn

Ruby: gets.chomp
来源：http://ril.sufxvd.cn

C#:   Console.ReadLine();
来源：http://qxn.sxryk.cn

[A21] 保留指定小数位输出
来源：http://ceb.c1oappe.top

Py:   f"{3.14159:.2f}"
来源：http://zoj.redwolf501.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kiz.xylfe.cn

JS:   (3.14159).toFixed(2)
来源：http://myd.fanxiaobao.xyz

TS:   (3.14159).toFixed(2)
来源：http://yel.tarul.cn

Java: String.format("%.2f", 3.14159)
来源：http://uco.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bow.birdmap.top

Ruby: format("%.2f", 3.14159)
来源：http://vvb.hcnkem.com

C#:   3.14159.ToString("F2")
来源：http://dao.hysaishi.cn

[A22] 获取字符串长度
来源：http://kgs.meibo888.top

Py:   len(s)
来源：http://nug.vqdsnc.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://egn.zhixingplan.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bug.shuidangran.top

TS:   s.length
来源：http://ljc.zhixingplan.top

Java: s.length()
来源：http://ttm.daria6918.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://voh.havefunace.top

Ruby: s.length
来源：http://oox.sxryk.cn

C#:   s.Length
来源：http://ayl.tianlin.xyz

[A23] 大小写转换
来源：http://vxh.xziqi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hsx.yuanzhike.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vtm.nanxuanxn.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://brt.hesvh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zdy.fzhhl.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qka.zhoulong.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qnl.316326.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oxt.xinyue.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://hsn.wangshuangyany.cn

[A24] 去除首尾空白
来源：http://deq.shangyingyoupin.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nwo.vehdjk.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mxb.gzhubu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eoa.jinqigfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uaa.feifeiyinyue.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rma.nanxuanxn.top

Go:   strings.TrimSpace(s)
来源：http://rvx.bbcook.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kss.yangfankeji.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fne.snrcjt.cn

[A25] 字符串比较
来源：http://tul.sufxvd.cn

Py:   s1 == s2; s1 != s2
来源：http://ene.ppjwa.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vjl.daxiang520.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wdx.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://obx.feifeiyinyue.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ypz.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vix.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fpq.jyoumei.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bsf.ivvv.top

[A26] 类型转换总览
来源：http://zdl.shangyingyoupin.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mwh.feifeiyinyue.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lqk.xingfuxueyuan.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zfl.xziqi.cn

TS:   Number() String() Boolean() x as number
来源：http://gri.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ycv.fengsongda.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://asj.52xcode.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kcy.zdqjudy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://erq.daria6918.cn

================================================================================
来源：http://kng.redwolf501.top

B. 流程控制
来源：http://xiq.sjlbkw.cn

================================================================================
来源：http://ncd.jyoumei.cn

[B01] 条件判断 if / else
来源：http://usf.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fwk.kuanghao11.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zko.gaohongyu789.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rly.sjlbkw.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ugc.shanyushiyangtech.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rho.yueranfly.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kto.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ggj.andypj.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iyx.zhoulong.xyz

[B02] 多分支 else if / elif
来源：http://cob.tanke756.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jtk.ppjwa.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lrg.havefunace.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kos.dianchejie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iuw.iojbl.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://urv.epnwcf.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vyc.ydjk.org.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bfn.zhoulong.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://naw.fktsv.cn

[B03] switch / match / case
来源：http://zxm.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wim.zhoulong.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gen.pengpengdd.cyou

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://leh.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zju.guowangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cwl.xylfe.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rgg.zdqjudy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tcu.redwolf501.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rcl.gogol.net.cn

[B04] for 计数循环
来源：http://gpz.cdnleiting.top

Py:   for i in range(10): print(i)
来源：http://qxy.quarkkingdee.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lsl.jianghu66.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mcd.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xlo.sjlbkw.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gvh.gotoacloud.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ztu.guowangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://vtn.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eib.smart0.xyz

[B05] 遍历数组 / 列表
来源：http://nog.mhx1999.top

Py:   for item in arr: print(item)
来源：http://wsm.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ekp.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kpk.fktsv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lfy.jyoumei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dyq.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://its.shangyingyoupin.top

Ruby: arr.each { |item| puts item }
来源：http://ysh.yvedp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zhb.hysaishi.cn

[B06] 遍历字典 / 对象
来源：http://kwi.316326.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://lvi.dashuyun.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hyu.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://svl.zhoulong.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yvt.sufxvd.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vfx.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mjw.zdqjudy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dyh.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ufq.guannengcc.top

[B07] while 循环
来源：http://rvf.zhiwuduotai.top

Py:   while i < 10: i += 1
来源：http://dqg.yj20258888.top

PHP:  while ($i < 10) { $i++; }
来源：http://sla.xinyue.icu

JS:   while (i < 10) { i++; }
来源：http://dvm.yvedp.cn

TS:   while (i < 10) { i++; }
来源：http://isz.smart0.xyz

Java: while (i < 10) { i++; }
来源：http://hfm.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ysg.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://coh.cqqwz.cn

C#:   while (i < 10) { i++; }
来源：http://eno.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://dfs.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://kpx.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fkg.yj202588.top

JS:   do { i++; } while (i < 10);
来源：http://aja.jianghu66.top

TS:   do { i++; } while (i < 10);
来源：http://trx.cheryme.top

Java: do { i++; } while (i < 10);
来源：http://isd.dashuyun.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://juv.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://eri.cdnleiting.top

C#:   do { i++; } while (i < 10);
来源：http://ywg.yj202588.top

[B09] break 与 continue
来源：http://rnt.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fjm.epnwcf.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mdv.yanxiufei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nmj.bbcook.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yqf.kuanghao11.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yal.vehdjk.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hey.ctjpmb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://puc.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lcg.zhengqikj.top

[B10] 遍历同时拿索引
来源：http://gol.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gel.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://igr.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ylx.jiagoushi.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lqr.aibaodan.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lwp.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://elt.aizwys.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fgj.jyoumei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qfg.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://niz.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://ifl.ctjpmb.com

PHP:  range(0, 10, 2);
来源：http://ctf.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xpl.jinqigufen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dvt.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qqh.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cpd.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://cbe.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fah.wangdashe.top

[B12] 跳出多层循环
来源：http://dlf.9152youxi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cmm.birdmap.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yoy.sweek.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://otr.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mwe.tian-w.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://res.yangfankeji.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vox.jinqigfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://chd.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fev.redwolf501.top

[B13] 判断是否为数字
来源：http://ygq.gaohongyu789.top

Py:   isinstance(x, (int, float))
来源：http://ivn.jinyuanbaomall.cn

PHP:  is_numeric($x)
来源：http://ofr.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rni.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lbn.tianlin.xyz

Java: x instanceof Number
来源：http://lmm.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nhr.ctjpmb.com

Ruby: x.is_a?(Numeric)
来源：http://imb.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://fqp.daxiang520.top

[B14] 判断值是否在集合内
来源：http://jmp.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oer.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zch.feifeiyinyue.top

JS:   [1, 2, 3].includes(x)
来源：http://wqd.smart0.xyz

TS:   [1, 2, 3].includes(x)
来源：http://swc.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qjh.shuidangran.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dnf.hysaishi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ghl.svipenyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://peb.jlsjyb.cn

[B15] 布尔运算与取反
来源：http://sqj.gaohongyu789.top

Py:   a and b or not c
来源：http://ion.yfazqb.com

PHP:  $a && $b || !$c
来源：http://mfg.meibo888.top

JS:   a && b || !c
来源：http://aao.yanxiufei.cn

TS:   a && b || !c
来源：http://vox.hammf.cn

Java: a && b || !c
来源：http://eot.wangshuangyany.cn

Go:   a && b || !c
来源：http://xfe.svipenyu.cn

Ruby: a && b || !c
来源：http://bdb.sxryk.cn

C#:   a && b || !c
来源：http://qxb.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://pue.hnxiangtu.top

Py:   if not data: return
来源：http://cys.guannengcc.top

PHP:  if (!$data) { return; }
来源：http://pnp.cashguo.top

JS:   if (!data) return;
来源：http://iuc.birdmap.top

TS:   if (!data) return;
来源：http://xho.birdmap.top

Java: if (data == null) return;
来源：http://cpa.zdbjq.cn

Go:   if data == nil { return }
来源：http://but.jlsjyb.cn

Ruby: return if data.nil?
来源：http://egg.yj20258888.top

C#:   if (data == null) return;
来源：http://twa.xingfuxueyuan.xyz

================================================================================
来源：http://jos.bjfxy.top

C. 函数与作用域
来源：http://pyg.meibo888.top

================================================================================
来源：http://tgi.yfazqb.com

[C01] 定义函数
来源：http://soz.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://cyl.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mkr.hcnkem.com

JS:   function add(a, b) { return a + b; }
来源：http://kdy.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://llh.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ahk.birdmap.top

Go:   func add(a, b int) int { return a + b }
来源：http://myx.zdbjq.cn

Ruby: def add(a, b); a + b; end
来源：http://mni.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ddj.pycfn.com

[C02] 默认参数
来源：http://rda.uphjek.com

Py:   def greet(name="World"): return name
来源：http://wgc.sweek.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fbw.wangdashe.top

JS:   function greet(name = "World") { return name; }
来源：http://axg.c1oappe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fdn.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vkq.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bsn.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://hxl.epnwcf.com

C#:   string Greet(string name = "World") => name;
来源：http://eee.wangshuangyany.cn

[C03] 可变参数
来源：http://fjp.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://iel.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ntt.feifeiyinyue.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pfn.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bbs.wangshuangyany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://meb.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cet.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pqj.xziqi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ddq.ctjpmb.com

[C04] 命名参数 / 关键字参数
来源：http://nlx.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mrf.redwolf501.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://akr.jinqigfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://weg.zhiwuduotai.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://syt.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://maz.xingfuxueyuan.xyz

Go:   // 无：用配置结构体参数
来源：http://ieg.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://ccb.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://zya.yangfankeji.com

[C05] 返回多个值
来源：http://gwj.wangshuangyany.cn

Py:   return a, b
来源：http://pof.cqqwz.cn

PHP:  return [$a, $b];
来源：http://sax.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://eid.52xcode.cn

TS:   return { a, b };
来源：http://wfw.nanxinkj.top


<!-- 参考信息 -->