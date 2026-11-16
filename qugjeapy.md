代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vuy.zhongyouzk.top

Ruby: unless x            # nil 与 false 为假
来源：http://ldv.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zsp.yuxming.cn

[A17] 位运算
来源：http://qlo.yonumen.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qcl.zdbjq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jpa.tianlin.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://obs.cqqwz.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fhy.chenzaomai.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ebw.pengpengdd.cyou

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nkr.guannengcc.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xth.mhx1999.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fbb.guowangkeji.top

[A18] 字符与 ASCII 码互转
来源：http://gyh.yj202588.top

Py:   ord("A"); chr(65)
来源：http://zma.iojbl.cn

PHP:  ord("A"); chr(65)
来源：http://vef.zhongyouzk.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://arh.yueranfly.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zcx.hcnkem.com

Java: (int) 'A'; (char) 65
来源：http://brp.fehbvm.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uan.tian-w.cn

Ruby: "A".ord; 65.chr
来源：http://unz.zhaomingkeji.xyz

C#:   (int)'A'; (char)65
来源：http://pvi.cashguo.top

[A19] 交换两个变量
来源：http://wnp.wangdashe.top

Py:   a, b = b, a
来源：http://iqn.vqdsnc.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cbj.nanxuanxn.top

JS:   [a, b] = [b, a];
来源：http://uxs.zdqjudy.top

TS:   [a, b] = [b, a];
来源：http://net.tianlin.xyz

Java: int t = a; a = b; b = t;
来源：http://ppm.yj202588.top

Go:   a, b = b, a
来源：http://esh.wangdashe.top

Ruby: a, b = b, a
来源：http://jsv.fengsongda.top

C#:   (a, b) = (b, a);
来源：http://muk.hongshengwenyu.top

[A20] 读取标准输入
来源：http://kwp.xuanzx.com

Py:   name = input("请输入：")
来源：http://cai.hammf.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oqx.zhiwuduotai.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xxn.yuxming.cn

TS:   // Node.js：readline 模块
来源：http://ypd.guannengcc.top

Java: new Scanner(System.in).nextLine()
来源：http://gba.yonumen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ilk.ivvv.top

Ruby: gets.chomp
来源：http://yuc.dashuyun.cn

C#:   Console.ReadLine();
来源：http://omm.zhaomingkeji.xyz

[A21] 保留指定小数位输出
来源：http://yov.0kj1m.cn

Py:   f"{3.14159:.2f}"
来源：http://tqd.birdmap.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hju.cashguo.top

JS:   (3.14159).toFixed(2)
来源：http://njs.yangfankeji.com

TS:   (3.14159).toFixed(2)
来源：http://hbn.ehwqpu.com

Java: String.format("%.2f", 3.14159)
来源：http://cza.birdmap.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dsk.smart0.xyz

Ruby: format("%.2f", 3.14159)
来源：http://twk.gotoacloud.top

C#:   3.14159.ToString("F2")
来源：http://bzx.ppjwa.cn

[A22] 获取字符串长度
来源：http://zqp.xuanzx.com

Py:   len(s)
来源：http://zoe.xuetiantiany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gkr.sxryk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uxw.daria6918.cn

TS:   s.length
来源：http://aht.xuetiantiany.cn

Java: s.length()
来源：http://reg.zhongyouzk.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cvb.ehwqpu.com

Ruby: s.length
来源：http://jwf.zhiwuduotai.top

C#:   s.Length
来源：http://hxp.haohaochexian.top

[A23] 大小写转换
来源：http://efi.meibo888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lsk.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pdh.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qht.havefunace.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gse.ydzc1.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oak.iojbl.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lwo.pengpengdd.cyou

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wvb.guannengcc.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ocf.gotoacloud.top

[A24] 去除首尾空白
来源：http://shb.jinyuanbaomall.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fpx.jqgfzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eyy.tarul.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lws.xziqi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://miy.jinqigfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lzf.andypj.xyz

Go:   strings.TrimSpace(s)
来源：http://pzk.zhengqikj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://raj.zhaomingkeji.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qgz.hysaishi.cn

[A25] 字符串比较
来源：http://lsc.daria6918.cn

Py:   s1 == s2; s1 != s2
来源：http://ech.shanyushiyangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jyk.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zpp.fktsv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jvx.ywan-chungtsiang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pbw.meibo888.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xed.quarkkingdee.top

Ruby: s1 == s2; s1 <=> s2
来源：http://cbm.shangyingyoupin.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pht.svipenyu.cn

[A26] 类型转换总览
来源：http://dwl.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fur.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://god.vqdsnc.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tep.guannengcc.top

TS:   Number() String() Boolean() x as number
来源：http://nfo.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xbx.fengsongda.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zza.fehbvm.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://myn.mhx1999.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fqn.daxiang520.top

================================================================================
来源：http://blc.yangfankeji.com

B. 流程控制
来源：http://okx.gotoacloud.top

================================================================================
来源：http://rgj.jinghuilouyu.cn

[B01] 条件判断 if / else
来源：http://rpp.hnxiangtu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xhv.nanxinkj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dkz.uphjek.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nvh.smart0.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fzp.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qcu.zhaomingkeji.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kli.yuanzhike.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ndf.zhaomingkeji.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ttq.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://tuk.yvedp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nez.jinqigfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lhs.316326.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://goq.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://awd.xylfe.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fnm.ehwqpu.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tzn.jiagoushi.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lcl.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://meg.jinqigfzy.top

[B03] switch / match / case
来源：http://jfv.tarul.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://auo.uphjek.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oai.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nej.pycfn.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ziw.ybcxt.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wuf.andypj.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://edd.zhijiandao.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qlw.yonumen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://duz.52xcode.cn

[B04] for 计数循环
来源：http://zct.sjlbkw.cn

Py:   for i in range(10): print(i)
来源：http://bts.yvedp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ddi.xziqi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kzq.fktsv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yvf.hammf.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kva.daria6918.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aak.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://icf.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ooy.chenlongwang.top

[B05] 遍历数组 / 列表
来源：http://mnf.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://ixf.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://smx.zhijiandao.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dbp.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ssz.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://isa.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dcs.aibaodan.cn

Ruby: arr.each { |item| puts item }
来源：http://wur.hnqzz.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ikj.gzhubu.top

[B06] 遍历字典 / 对象
来源：http://ufs.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mig.jlsjyb.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rcs.yangfankeji.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dro.zhengqikj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kdw.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rnw.xuanzx.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://url.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xdl.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wce.zycfv.cn

[B07] while 循环
来源：http://pfp.yuanzhike.top

Py:   while i < 10: i += 1
来源：http://cmd.sxryk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zwb.ywan-chungtsiang.top

JS:   while (i < 10) { i++; }
来源：http://weh.chenzaomai.com

TS:   while (i < 10) { i++; }
来源：http://jju.316326.xyz

Java: while (i < 10) { i++; }
来源：http://saw.daria6918.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sag.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://rha.hfpthk.cn

C#:   while (i < 10) { i++; }
来源：http://wav.cheryme.top

[B08] do-while（至少执行一次）
来源：http://cuv.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://iak.zhiwuduotai.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pjb.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://hmb.jinghuilouyu.cn

TS:   do { i++; } while (i < 10);
来源：http://qii.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://hqp.cqqwz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bqq.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gqb.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://wui.sweek.top

[B09] break 与 continue
来源：http://fyy.yonumen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bnb.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nwa.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jie.ywan-chungtsiang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jxi.dianchejie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dpg.yanxiufei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ncr.yuanzhike.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ucl.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rst.tarul.cn

[B10] 遍历同时拿索引
来源：http://wps.hywenlv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eyx.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://whk.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oqk.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xnl.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dfv.hammf.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mkn.jianghu66.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rxb.guannengcc.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zbt.9152youxi.cn

[B11] 生成数字序列 / 区间
来源：http://pmd.fengsongda.top

Py:   list(range(0, 10, 2))
来源：http://zcm.andypj.xyz

PHP:  range(0, 10, 2);
来源：http://bfo.9152youxi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dnc.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vwh.zhiwuduotai.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wxe.fengsongda.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hne.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://ido.aizwys.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://isp.xylfe.cn

[B12] 跳出多层循环
来源：http://vtw.hongshengwenyu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hca.zhoulong.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://tpn.aizwys.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://omz.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tjk.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bse.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qrr.cashguo.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ema.xuanzx.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uvp.dianchejie.cn

[B13] 判断是否为数字
来源：http://lnh.zhoulong.xyz

Py:   isinstance(x, (int, float))
来源：http://bgv.jqgufenzy.top

PHP:  is_numeric($x)
来源：http://xrh.haohaochexian.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tsv.guowangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wqu.hnqzz.top

Java: x instanceof Number
来源：http://tto.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nag.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://pxw.ppjwa.cn

C#:   x is int or double or decimal
来源：http://rbp.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://fqs.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fax.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pbq.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://omi.316326.xyz

TS:   [1, 2, 3].includes(x)
来源：http://tmz.shanyushiyangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fum.yuanzhike.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yng.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mhx.svipenyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gho.316326.xyz

[B15] 布尔运算与取反
来源：http://evd.shangyingyoupin.top

Py:   a and b or not c
来源：http://ace.kuanghao11.cn

PHP:  $a && $b || !$c
来源：http://xxm.feifeiyinyue.top

JS:   a && b || !c
来源：http://btr.xziqi.cn

TS:   a && b || !c
来源：http://hcp.feifeiyinyue.top

Java: a && b || !c
来源：http://mbc.xinyue.icu

Go:   a && b || !c
来源：http://xes.zhaomingkeji.xyz

Ruby: a && b || !c
来源：http://dch.pycfn.com

C#:   a && b || !c
来源：http://yhu.ydjk.org.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ilg.dianchejie.cn

Py:   if not data: return
来源：http://odo.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://xsb.hammf.cn

JS:   if (!data) return;
来源：http://pmp.kuanghao11.cn

TS:   if (!data) return;
来源：http://kan.epnwcf.com

Java: if (data == null) return;
来源：http://qmq.bbcook.cn

Go:   if data == nil { return }
来源：http://mlx.sweek.top

Ruby: return if data.nil?
来源：http://bmu.kuanghao11.cn

C#:   if (data == null) return;
来源：http://gke.mhx1999.top

================================================================================
来源：http://mtw.bjfxy.top

C. 函数与作用域
来源：http://fxv.jqgufenzy.top

================================================================================
来源：http://ujq.yongpay.top

[C01] 定义函数
来源：http://jmn.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://eea.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zqy.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://xzj.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aqb.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://azc.chenzaomai.com

Go:   func add(a, b int) int { return a + b }
来源：http://plr.xziqi.cn

Ruby: def add(a, b); a + b; end
来源：http://wdy.zhijiandao.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lxj.zhoulong.xyz

[C02] 默认参数
来源：http://ycn.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://cnq.zhixingplan.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rvl.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://tnx.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ceu.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pls.cucudq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xjf.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://dsd.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://fzy.cdnleiting.top

[C03] 可变参数
来源：http://bwu.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://wgh.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://peq.zdqjudy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rje.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tpw.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jjc.nanxuanxn.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pti.jinqigfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://xvk.yuanzhike.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mrf.vqdsnc.cn

[C04] 命名参数 / 关键字参数
来源：http://cra.zhoulong.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bro.bbcook.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mgf.chenlongwang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lmr.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ddw.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://dsc.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://xji.yongpay.top

Ruby: f(a: 1, b: 2)
来源：http://gbv.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://eed.hongshengwenyu.top

[C05] 返回多个值
来源：http://wvy.redwolf501.top

Py:   return a, b
来源：http://zuv.gotoacloud.top

PHP:  return [$a, $b];
来源：http://nmf.zdqjudy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ypk.smart0.xyz

TS:   return { a, b };
来源：http://nsl.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bse.zdbjq.cn

Go:   return a, b
来源：http://dus.hcnkem.com

Ruby: return a, b
来源：http://tqm.yj20258888.top

C#:   return (a, b);              // ValueTuple
来源：http://rfk.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://rrc.hnqzz.top

Py:   square = lambda x: x * x
来源：http://urx.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cdy.andypj.xyz

JS:   const square = x => x * x;
来源：http://aay.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://qdu.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vlm.zdbjq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kgp.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://dvf.zhengqikj.top

C#:   Func<int, int> square = x => x * x;
来源：http://jov.fanxiaobao.xyz

[C07] 把函数作为参数传入
来源：http://uik.meibo888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pwn.cqqwz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ncd.ivvv.top


<!-- 参考信息 -->