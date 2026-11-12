代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vym.vehdjk.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lnc.aizwys.cn

TS:   if (!x) {}
来源：http://obw.jiagoushi.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://eie.tian-w.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rye.nwbrower.top

Ruby: unless x            # nil 与 false 为假
来源：http://ksf.dianchejie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mfs.tanke756.top

[A17] 位运算
来源：http://clv.shzxlz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kmy.chenzaomai.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ddj.yuanzhike.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fcj.jqgufenzy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tcy.tian-w.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wxk.hesvh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://aru.ehwqpu.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ltj.vehdjk.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qvd.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://ndd.daxiang520.top

Py:   ord("A"); chr(65)
来源：http://vty.xuanzx.com

PHP:  ord("A"); chr(65)
来源：http://tep.aizwys.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mmn.birdmap.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zhm.chenjidiqi.icu

Java: (int) 'A'; (char) 65
来源：http://mfc.316326.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gfw.gaohongyu789.top

Ruby: "A".ord; 65.chr
来源：http://ivk.hcnkem.com

C#:   (int)'A'; (char)65
来源：http://tdj.ppjwa.cn

[A19] 交换两个变量
来源：http://szn.tarul.cn

Py:   a, b = b, a
来源：http://jxo.fanxiaobao.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://upb.nwbrower.top

JS:   [a, b] = [b, a];
来源：http://jhs.jinghuilouyu.cn

TS:   [a, b] = [b, a];
来源：http://eez.hesvh.cn

Java: int t = a; a = b; b = t;
来源：http://ptm.smart0.xyz

Go:   a, b = b, a
来源：http://njw.shangyingyoupin.top

Ruby: a, b = b, a
来源：http://djk.cheryme.top

C#:   (a, b) = (b, a);
来源：http://vdt.xingfuxueyuan.xyz

[A20] 读取标准输入
来源：http://ean.hnxiangtu.top

Py:   name = input("请输入：")
来源：http://rpg.jinghuilouyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vdb.52xcode.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vsl.zhongyouzk.top

TS:   // Node.js：readline 模块
来源：http://yxs.ehwqpu.com

Java: new Scanner(System.in).nextLine()
来源：http://nsu.chenzaomai.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dxl.fengsongda.top

Ruby: gets.chomp
来源：http://alm.cucudq.cn

C#:   Console.ReadLine();
来源：http://rrp.ivvv.top

[A21] 保留指定小数位输出
来源：http://alv.shzxlz.cn

Py:   f"{3.14159:.2f}"
来源：http://iqq.gogol.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nyk.yvedp.cn

JS:   (3.14159).toFixed(2)
来源：http://hwd.ivvv.top

TS:   (3.14159).toFixed(2)
来源：http://xze.sjlbkw.cn

Java: String.format("%.2f", 3.14159)
来源：http://ldg.yj20258.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ueo.fehbvm.com

Ruby: format("%.2f", 3.14159)
来源：http://atk.yuxming.cn

C#:   3.14159.ToString("F2")
来源：http://xhy.fktsv.cn

[A22] 获取字符串长度
来源：http://ttr.yfazqb.com

Py:   len(s)
来源：http://kzt.zdbjq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zqp.nwbrower.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eoh.bjfxy.top

TS:   s.length
来源：http://dlb.gogol.net.cn

Java: s.length()
来源：http://opd.xuetiantiany.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eoe.zhixingplan.top

Ruby: s.length
来源：http://mgx.sxryk.cn

C#:   s.Length
来源：http://htl.xziqi.cn

[A23] 大小写转换
来源：http://zfs.yvedp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://swz.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ljl.hnxiangtu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rgg.snrcjt.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://scq.ybcxt.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ryy.yuanzhike.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bnh.zdqjudy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oea.0kj1m.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wwt.wangdashe.top

[A24] 去除首尾空白
来源：http://njx.jinyuanbaomall.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://idf.ybcxt.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rps.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kle.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wmz.iojbl.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pat.guannengcc.top

Go:   strings.TrimSpace(s)
来源：http://kkr.gaohongyu789.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qmu.nwbrower.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zaz.fehbvm.com

[A25] 字符串比较
来源：http://bhs.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://kcc.xingfuxueyuan.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kqd.hongshengwenyu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dro.cucudq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pyy.ywan-chungtsiang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tws.jqgufenzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://feq.vqdsnc.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xbs.shanyushiyangtech.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nwh.iojbl.cn

[A26] 类型转换总览
来源：http://umw.daxiang520.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://roa.yanxiufei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tys.zdbjq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wdj.vehdjk.com

TS:   Number() String() Boolean() x as number
来源：http://wsf.andypj.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rko.yj202588.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qwt.tianlin.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://ozx.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ibw.hammf.cn

================================================================================
来源：http://cow.sysykeji.top

B. 流程控制
来源：http://vju.jinyuanbaomall.cn

================================================================================
来源：http://ryt.pengpengdd.cyou

[B01] 条件判断 if / else
来源：http://ivl.nanxuanxn.top

Py:   result = "正" if x > 0 else "非正"
来源：http://aoi.daria6918.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vfp.sweek.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yar.haohaochexian.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gje.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://clg.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cqc.pycfn.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ymh.daria6918.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kir.hnqzz.top

[B02] 多分支 else if / elif
来源：http://zcm.zhijiandao.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mry.jqgfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://msq.kuanghao11.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yej.wangshuangyany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yfu.yj20258888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ghs.fehbvm.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aza.pengpengdd.cyou

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rxi.zdbjq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iaj.shuidangran.top

[B03] switch / match / case
来源：http://kow.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kzz.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ahx.iojbl.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wmw.cdnleiting.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uhv.svipenyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dop.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hzu.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uhk.svipenyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ifq.uphjek.com

[B04] for 计数循环
来源：http://ara.0kj1m.cn

Py:   for i in range(10): print(i)
来源：http://dgy.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nww.jiagoushi.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zod.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ecs.jinqigufen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wnj.hfpthk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qsp.tian-w.cn

Ruby: 10.times { |i| puts i }
来源：http://mwx.316326.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xra.nanxuanxn.top

[B05] 遍历数组 / 列表
来源：http://dur.gogol.net.cn

Py:   for item in arr: print(item)
来源：http://hfo.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rrp.jyoumei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rek.yfazqb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://inb.cashguo.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gwo.zhongyouzk.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oef.gaohongyu789.top

Ruby: arr.each { |item| puts item }
来源：http://vqr.zdbjq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tel.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://kwy.shuidangran.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rvp.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vwz.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nge.52xcode.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rhd.yongpay.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cnd.bbcook.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xjb.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iid.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ayx.fktsv.cn

[B07] while 循环
来源：http://gwz.meibo888.top

Py:   while i < 10: i += 1
来源：http://bjg.ctjpmb.com

PHP:  while ($i < 10) { $i++; }
来源：http://gnp.yongpay.top

JS:   while (i < 10) { i++; }
来源：http://vfe.fktsv.cn

TS:   while (i < 10) { i++; }
来源：http://hzs.jinqigufen.top

Java: while (i < 10) { i++; }
来源：http://jyw.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://prg.shanyushiyangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://nqm.vehdjk.com

C#:   while (i < 10) { i++; }
来源：http://axq.yuxming.cn

[B08] do-while（至少执行一次）
来源：http://fbe.zhaomingkeji.xyz

Py:   # 无 do-while：用 while True + break
来源：http://oev.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://odm.fktsv.cn

JS:   do { i++; } while (i < 10);
来源：http://uyn.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://rxs.chenzaomai.com

Java: do { i++; } while (i < 10);
来源：http://pwa.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ceh.zhengqikj.top

Ruby: begin; i += 1; end while i < 10
来源：http://nvy.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://ihg.bjfxy.top

[B09] break 与 continue
来源：http://nre.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wzl.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://apc.yvedp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ugx.jinyuanbaomall.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yxx.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rfu.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zho.sweek.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zid.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wst.xylfe.cn

[B10] 遍历同时拿索引
来源：http://cer.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lpy.shzxlz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tah.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uie.chenzaomai.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iso.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uie.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xeb.fehbvm.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nss.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fly.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://rpe.gotoacloud.top

Py:   list(range(0, 10, 2))
来源：http://ryk.fengsongda.top

PHP:  range(0, 10, 2);
来源：http://mei.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://psx.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ojo.yfazqb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zof.quarkkingdee.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tqo.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://pzj.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tgl.jyoumei.cn

[B12] 跳出多层循环
来源：http://wns.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://psf.gogol.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zff.0kj1m.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fba.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nqf.hywenlv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qym.shzxlz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fpg.zhixingplan.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oxw.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mdv.yfazqb.com

[B13] 判断是否为数字
来源：http://tso.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://sgv.vqdsnc.cn

PHP:  is_numeric($x)
来源：http://wzg.guowangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vzl.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qcp.9152youxi.cn

Java: x instanceof Number
来源：http://jbd.cucudq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dol.pengpengdd.cyou

Ruby: x.is_a?(Numeric)
来源：http://qsc.wangdashe.top

C#:   x is int or double or decimal
来源：http://vhw.hesvh.cn

[B14] 判断值是否在集合内
来源：http://nmz.fktsv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hol.xuanzx.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ihl.shzxlz.cn

JS:   [1, 2, 3].includes(x)
来源：http://ixe.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://hhi.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nuu.ybcxt.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vtx.hysaishi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tah.ywan-chungtsiang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zti.jinqigfzy.top

[B15] 布尔运算与取反
来源：http://epi.xuanzx.com

Py:   a and b or not c
来源：http://lwz.zhengqikj.top

PHP:  $a && $b || !$c
来源：http://pgf.yueranfly.top

JS:   a && b || !c
来源：http://gmk.ctjpmb.com

TS:   a && b || !c
来源：http://czi.yongpay.top

Java: a && b || !c
来源：http://xtm.zhoulong.xyz

Go:   a && b || !c
来源：http://fvw.feifeiyinyue.top

Ruby: a && b || !c
来源：http://qrg.cucudq.cn

C#:   a && b || !c
来源：http://hts.jinqigfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://ofk.shangyingyoupin.top

Py:   if not data: return
来源：http://rca.zhijiandao.cn

PHP:  if (!$data) { return; }
来源：http://kax.316326.xyz

JS:   if (!data) return;
来源：http://ult.jianghu66.top

TS:   if (!data) return;
来源：http://xmr.hywenlv.cn

Java: if (data == null) return;
来源：http://olv.hysaishi.cn

Go:   if data == nil { return }
来源：http://kvo.hfpthk.cn

Ruby: return if data.nil?
来源：http://ivs.guowangkeji.top

C#:   if (data == null) return;
来源：http://mdz.shuidangran.top

================================================================================
来源：http://ghf.ywan-chungtsiang.top

C. 函数与作用域
来源：http://brz.yongpay.top

================================================================================
来源：http://stu.havefunace.top

[C01] 定义函数
来源：http://dzx.yvedp.cn

Py:   def add(a, b): return a + b
来源：http://cpq.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://apj.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://dqq.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zhr.gotoacloud.top

Java: static int add(int a, int b) { return a + b; }
来源：http://guz.shzxlz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dfl.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://qmh.quarkkingdee.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wnl.tian-w.cn

[C02] 默认参数
来源：http://vue.0kj1m.cn

Py:   def greet(name="World"): return name
来源：http://qlj.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://sxv.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://eze.vehdjk.com

TS:   function greet(name: string = "World") { return name; }
来源：http://gpv.sxryk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hon.ehwqpu.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hyl.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://rvs.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://tbi.dashuyun.cn

[C03] 可变参数
来源：http://rci.jianghu66.top

Py:   def total(*args): return sum(args)
来源：http://nzu.jinqigfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dyk.bjfxy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jpc.cucudq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kxq.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ors.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qwn.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mgr.smart0.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://npl.bjfxy.top

[C04] 命名参数 / 关键字参数
来源：http://fjs.fehbvm.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ofm.tianlin.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lhp.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qjo.daria6918.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gte.ydjk.org.cn

Java: // 无：用 Builder 模式或 record
来源：http://zrp.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://ybh.yongpay.top

Ruby: f(a: 1, b: 2)
来源：http://hhk.wangshuangyany.cn

C#:   f(a: 1, b: 2)
来源：http://kpx.ppjwa.cn

[C05] 返回多个值
来源：http://yxj.chenjidiqi.icu

Py:   return a, b
来源：http://evu.epnwcf.com

PHP:  return [$a, $b];
来源：http://dww.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vie.cheryme.top

TS:   return { a, b };
来源：http://uup.yongpay.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wlb.yj202588.top

Go:   return a, b
来源：http://jpq.ydzc1.top

Ruby: return a, b
来源：http://fov.zhaomingkeji.xyz

C#:   return (a, b);              // ValueTuple
来源：http://hae.ppjwa.cn

[C06] 匿名函数 / lambda
来源：http://cfc.sweek.top

Py:   square = lambda x: x * x
来源：http://zkj.yuanzhike.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ypy.yfazqb.com

JS:   const square = x => x * x;
来源：http://adt.quarkkingdee.top

TS:   const square = (x: number): number => x * x;
来源：http://gxm.fehbvm.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cgh.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://yfd.hongshengwenyu.top

Ruby: square = ->(x) { x * x }
来源：http://kio.zhengqikj.top


<!-- 参考信息 -->