代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ggw.9152youxi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rqa.nanxinkj.top

TS:   if (!x) {}
来源：http://srp.yvedp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://skc.guannengcc.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tdl.52xcode.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ykf.redwolf501.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zxb.yanxiufei.cn

[A17] 位运算
来源：http://pvw.tian-w.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ldo.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lyh.jqgufenzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oql.zhoulong.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vir.smart0.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xdv.jinyuanbaomall.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rvd.zdbjq.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qvx.yuanzhike.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xnd.jlsjyb.cn

[A18] 字符与 ASCII 码互转
来源：http://mwp.zdbjq.cn

Py:   ord("A"); chr(65)
来源：http://qrz.snrcjt.cn

PHP:  ord("A"); chr(65)
来源：http://led.yueranfly.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pmb.cqqwz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iow.ctjpmb.com

Java: (int) 'A'; (char) 65
来源：http://hsu.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vwb.shuidangran.top

Ruby: "A".ord; 65.chr
来源：http://dfs.yangfankeji.com

C#:   (int)'A'; (char)65
来源：http://rqf.zdbjq.cn

[A19] 交换两个变量
来源：http://bvq.dashuyun.cn

Py:   a, b = b, a
来源：http://rza.hesvh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qed.ppjwa.cn

JS:   [a, b] = [b, a];
来源：http://ckl.zdqjudy.top

TS:   [a, b] = [b, a];
来源：http://vvg.hnqzz.top

Java: int t = a; a = b; b = t;
来源：http://icn.hnxiangtu.top

Go:   a, b = b, a
来源：http://jsp.jianghu66.top

Ruby: a, b = b, a
来源：http://cdj.yonumen.top

C#:   (a, b) = (b, a);
来源：http://jsz.redwolf501.top

[A20] 读取标准输入
来源：http://jaj.chenzaomai.com

Py:   name = input("请输入：")
来源：http://ids.0kj1m.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://aec.xziqi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://asy.uphjek.com

TS:   // Node.js：readline 模块
来源：http://kzt.dashuyun.cn

Java: new Scanner(System.in).nextLine()
来源：http://sra.havefunace.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qsr.yj202588.top

Ruby: gets.chomp
来源：http://grc.yj20258.top

C#:   Console.ReadLine();
来源：http://ylp.birdmap.top

[A21] 保留指定小数位输出
来源：http://vcc.xinyue.icu

Py:   f"{3.14159:.2f}"
来源：http://uud.cashguo.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ztx.zhaomingkeji.xyz

JS:   (3.14159).toFixed(2)
来源：http://jew.yonumen.top

TS:   (3.14159).toFixed(2)
来源：http://ver.mhx1999.top

Java: String.format("%.2f", 3.14159)
来源：http://xfs.xinyue.icu

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bwb.iojbl.cn

Ruby: format("%.2f", 3.14159)
来源：http://eqg.sjlbkw.cn

C#:   3.14159.ToString("F2")
来源：http://iny.jlsjyb.cn

[A22] 获取字符串长度
来源：http://ogu.jqgfzy.top

Py:   len(s)
来源：http://lop.yangfankeji.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cgx.shanyushiyangtech.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fex.yuanzhike.top

TS:   s.length
来源：http://ztz.zdbjq.cn

Java: s.length()
来源：http://qtd.cheryme.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tpb.gaohongyu789.top

Ruby: s.length
来源：http://yjj.yonumen.top

C#:   s.Length
来源：http://qvs.jinqigfzy.top

[A23] 大小写转换
来源：http://uqe.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://keh.jiagoushi.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hhb.hcnkem.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ita.ybcxt.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eco.guowangkeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zti.cdnleiting.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fer.andypj.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vei.smart0.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://idi.vehdjk.com

[A24] 去除首尾空白
来源：http://bou.pycfn.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ewn.xuetiantiany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bhf.hcnkem.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xhl.aibaodan.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://omw.cdnleiting.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vvb.xinyue.icu

Go:   strings.TrimSpace(s)
来源：http://iau.gogol.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rtb.316326.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xcz.fktsv.cn

[A25] 字符串比较
来源：http://mcr.meibo888.top

Py:   s1 == s2; s1 != s2
来源：http://ibl.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jsj.gogol.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eta.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zav.yj202588.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://avw.shuidangran.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://giy.chenzaomai.com

Ruby: s1 == s2; s1 <=> s2
来源：http://tos.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hbx.zhijiandao.cn

[A26] 类型转换总览
来源：http://wcq.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://emh.c1oappe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qjd.sweek.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fhx.hcnkem.com

TS:   Number() String() Boolean() x as number
来源：http://irl.quarkkingdee.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wse.tianlin.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vyh.shuidangran.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cnz.ybcxt.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vzm.wangdashe.top

================================================================================
来源：http://uqx.nanxuanxn.top

B. 流程控制
来源：http://dcs.havefunace.top

================================================================================
来源：http://xnq.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://xxf.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://isu.zdqjudy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://txu.ehwqpu.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sny.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ryb.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fqa.zhongyouzk.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rsm.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kjc.zhijiandao.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vfx.xylfe.cn

[B02] 多分支 else if / elif
来源：http://adt.pycfn.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yyj.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wjr.wangshuangyany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hnr.jqgufenzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://htt.jyoumei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://clc.ehwqpu.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kws.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nzt.chenjidiqi.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oqj.zhixingplan.top

[B03] switch / match / case
来源：http://ble.yuxming.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jss.daxiang520.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yfm.guannengcc.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uso.ydjk.org.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://poi.fehbvm.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tyd.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uvh.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dgh.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ibv.fanxiaobao.xyz

[B04] for 计数循环
来源：http://hgi.xuetiantiany.cn

Py:   for i in range(10): print(i)
来源：http://eao.hfpthk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pkm.nanxuanxn.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fjn.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dcl.zhaomingkeji.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lvp.iojbl.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xmc.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://dgy.shanyushiyangtech.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ddx.fanxiaobao.xyz

[B05] 遍历数组 / 列表
来源：http://ibm.hcnkem.com

Py:   for item in arr: print(item)
来源：http://gvf.hongshengwenyu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lpt.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pjy.cqqwz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://psp.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://edg.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://njg.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://oqj.cdnleiting.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oor.sxryk.cn

[B06] 遍历字典 / 对象
来源：http://jtl.zhiwuduotai.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yms.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bsm.aibaodan.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vvb.iojbl.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zlt.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://myk.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mff.yongpay.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hdb.jianghu66.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xry.hesvh.cn

[B07] while 循环
来源：http://ukb.kuanghao11.cn

Py:   while i < 10: i += 1
来源：http://nam.sufxvd.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eow.ctjpmb.com

JS:   while (i < 10) { i++; }
来源：http://nfw.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://rip.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://ksx.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cil.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://srx.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://ggi.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://rrw.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://xkw.jiagoushi.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bjg.uphjek.com

JS:   do { i++; } while (i < 10);
来源：http://vay.jlsjyb.cn

TS:   do { i++; } while (i < 10);
来源：http://duq.gotoacloud.top

Java: do { i++; } while (i < 10);
来源：http://nie.smart0.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ysa.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://zom.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://plg.fktsv.cn

[B09] break 与 continue
来源：http://sbx.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qtg.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yst.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wbz.guowangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hmw.yonumen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fsy.yfazqb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bug.zhengqikj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wao.zdqjudy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtm.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://ubk.fengsongda.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tfo.zhongyouzk.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iiu.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dfp.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wpg.guowangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ffj.kuanghao11.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lps.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sid.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://btu.nwbrower.top

[B11] 生成数字序列 / 区间
来源：http://usm.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://iab.sjlbkw.cn

PHP:  range(0, 10, 2);
来源：http://kia.fktsv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://upk.tianlin.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cmn.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://juk.yj202588.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bde.jinqigufen.top

Ruby: (0...10).step(2).to_a
来源：http://iew.9152youxi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://knc.hywenlv.cn

[B12] 跳出多层循环
来源：http://xhl.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pbr.sysykeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dfh.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://krf.fehbvm.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gxm.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uhu.cdnleiting.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qil.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xpd.cheryme.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ukg.zhengqikj.top

[B13] 判断是否为数字
来源：http://drz.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://egq.xinyue.icu

PHP:  is_numeric($x)
来源：http://zyg.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kal.hcnkem.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xlh.iojbl.cn

Java: x instanceof Number
来源：http://dub.xziqi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yke.ydjk.org.cn

Ruby: x.is_a?(Numeric)
来源：http://say.fzhhl.top

C#:   x is int or double or decimal
来源：http://hbx.fktsv.cn

[B14] 判断值是否在集合内
来源：http://bwr.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://odj.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://axy.sufxvd.cn

JS:   [1, 2, 3].includes(x)
来源：http://yxg.aibaodan.cn

TS:   [1, 2, 3].includes(x)
来源：http://kxm.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uob.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qyy.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://klw.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cqt.svipenyu.cn

[B15] 布尔运算与取反
来源：http://uqb.iojbl.cn

Py:   a and b or not c
来源：http://oqc.zhaomingkeji.xyz

PHP:  $a && $b || !$c
来源：http://qjl.yongpay.top

JS:   a && b || !c
来源：http://czo.aibaodan.cn

TS:   a && b || !c
来源：http://ekq.jqgufenzy.top

Java: a && b || !c
来源：http://kks.kuanghao11.cn

Go:   a && b || !c
来源：http://ira.fanxiaobao.xyz

Ruby: a && b || !c
来源：http://zkt.zhixingplan.top

C#:   a && b || !c
来源：http://fhw.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://jko.yuxming.cn

Py:   if not data: return
来源：http://fuz.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://oxp.fengsongda.top

JS:   if (!data) return;
来源：http://slw.ctjpmb.com

TS:   if (!data) return;
来源：http://pkd.gotoacloud.top

Java: if (data == null) return;
来源：http://snu.redwolf501.top

Go:   if data == nil { return }
来源：http://wzk.quarkkingdee.top

Ruby: return if data.nil?
来源：http://lrc.jianghu66.top

C#:   if (data == null) return;
来源：http://fmi.ivvv.top

================================================================================
来源：http://jva.ydzc1.top

C. 函数与作用域
来源：http://nrj.yfazqb.com

================================================================================
来源：http://phg.kuanghao11.cn

[C01] 定义函数
来源：http://ktq.havefunace.top

Py:   def add(a, b): return a + b
来源：http://gex.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hgr.yj202588.top

JS:   function add(a, b) { return a + b; }
来源：http://akv.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xdq.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vlk.fehbvm.com

Go:   func add(a, b int) int { return a + b }
来源：http://awd.aibaodan.cn

Ruby: def add(a, b); a + b; end
来源：http://ewx.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mar.ydjk.org.cn

[C02] 默认参数
来源：http://fly.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://jsp.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://efs.smart0.xyz

JS:   function greet(name = "World") { return name; }
来源：http://cef.yueranfly.top

TS:   function greet(name: string = "World") { return name; }
来源：http://uxp.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xku.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vxu.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://jnr.ehwqpu.com

C#:   string Greet(string name = "World") => name;
来源：http://ltv.sysykeji.top

[C03] 可变参数
来源：http://fyx.dianchejie.cn

Py:   def total(*args): return sum(args)
来源：http://yfk.jinyuanbaomall.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fft.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rxa.ehwqpu.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ret.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://efb.yuanzhike.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eex.ydzc1.top

Ruby: def total(*nums); nums.sum; end
来源：http://qdx.hysaishi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mzk.fengsongda.top

[C04] 命名参数 / 关键字参数
来源：http://dqp.c1oappe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ghz.vqdsnc.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ect.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ttg.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ovt.daxiang520.top

Java: // 无：用 Builder 模式或 record
来源：http://dub.hysaishi.cn

Go:   // 无：用配置结构体参数
来源：http://kkj.zhiwuduotai.top

Ruby: f(a: 1, b: 2)
来源：http://rcs.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://jky.cqqwz.cn

[C05] 返回多个值
来源：http://uvm.jianghu66.top

Py:   return a, b
来源：http://wxc.meibo888.top

PHP:  return [$a, $b];
来源：http://ldz.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://lcl.andypj.xyz

TS:   return { a, b };
来源：http://ete.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bzx.daxiang520.top

Go:   return a, b
来源：http://ldk.ppjwa.cn

Ruby: return a, b
来源：http://mnh.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://vqb.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://bec.9152youxi.cn

Py:   square = lambda x: x * x
来源：http://rcb.cqqwz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xzt.zhixingplan.top

JS:   const square = x => x * x;
来源：http://zwg.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://fsy.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hkw.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://scm.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://spd.jinyuanbaomall.cn


<!-- 参考信息 -->