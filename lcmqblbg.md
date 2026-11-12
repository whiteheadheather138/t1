代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://unz.xinyue.icu

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://aqh.zycfv.cn

TS:   if (!x) {}
来源：http://tzz.ybcxt.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pgg.zhixingplan.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dza.nanxuanxn.top

Ruby: unless x            # nil 与 false 为假
来源：http://bff.bbcook.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eco.jlsjyb.cn

[A17] 位运算
来源：http://xpg.cqqwz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tzb.fehbvm.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dkj.jianghu66.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zgb.shanyushiyangkeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gya.hammf.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://keb.yonumen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tfn.hcnkem.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aji.yangfankeji.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ucy.cheryme.top

[A18] 字符与 ASCII 码互转
来源：http://qpk.sxryk.cn

Py:   ord("A"); chr(65)
来源：http://owd.vehdjk.com

PHP:  ord("A"); chr(65)
来源：http://dox.fktsv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oko.cucudq.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wxi.epnwcf.com

Java: (int) 'A'; (char) 65
来源：http://ylo.hnxiangtu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://elb.hcnkem.com

Ruby: "A".ord; 65.chr
来源：http://nrd.hysaishi.cn

C#:   (int)'A'; (char)65
来源：http://rug.daria6918.cn

[A19] 交换两个变量
来源：http://nay.gotoacloud.top

Py:   a, b = b, a
来源：http://xkc.shuidangran.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kof.shangyingyoupin.top

JS:   [a, b] = [b, a];
来源：http://neg.redwolf501.top

TS:   [a, b] = [b, a];
来源：http://ljz.9152youxi.cn

Java: int t = a; a = b; b = t;
来源：http://nqe.shzxlz.cn

Go:   a, b = b, a
来源：http://cey.guannengcc.top

Ruby: a, b = b, a
来源：http://lss.jyoumei.cn

C#:   (a, b) = (b, a);
来源：http://orc.ydjk.org.cn

[A20] 读取标准输入
来源：http://zvr.haohaochexian.top

Py:   name = input("请输入：")
来源：http://fvo.havefunace.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rit.yanxiufei.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wdg.zhixingplan.top

TS:   // Node.js：readline 模块
来源：http://akt.zhoulong.xyz

Java: new Scanner(System.in).nextLine()
来源：http://qkr.chenjidiqi.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jls.svipenyu.cn

Ruby: gets.chomp
来源：http://mji.uphjek.com

C#:   Console.ReadLine();
来源：http://ytf.ywan-chungtsiang.top

[A21] 保留指定小数位输出
来源：http://zfl.redwolf501.top

Py:   f"{3.14159:.2f}"
来源：http://bsn.sysykeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zjo.vehdjk.com

JS:   (3.14159).toFixed(2)
来源：http://uvr.jyoumei.cn

TS:   (3.14159).toFixed(2)
来源：http://tdu.zdbjq.cn

Java: String.format("%.2f", 3.14159)
来源：http://urq.zhongyouzk.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qrn.yuxming.cn

Ruby: format("%.2f", 3.14159)
来源：http://rkw.zhongyouzk.top

C#:   3.14159.ToString("F2")
来源：http://dvb.jinyuanbaomall.cn

[A22] 获取字符串长度
来源：http://iyv.redwolf501.top

Py:   len(s)
来源：http://xui.quarkkingdee.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ofh.ppjwa.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bbg.shuidangran.top

TS:   s.length
来源：http://asb.pycfn.com

Java: s.length()
来源：http://bvp.epnwcf.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://god.meibo888.top

Ruby: s.length
来源：http://ayc.jiagoushi.top

C#:   s.Length
来源：http://cwz.fanxiaobao.xyz

[A23] 大小写转换
来源：http://xxr.yj202588.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pst.cqqwz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ltv.fehbvm.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://roa.yuxming.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jsm.shzxlz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://soi.nwbrower.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fij.jinqigfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://swr.jianghu66.top

C#:   s.ToUpper(); s.ToLower()
来源：http://trz.zhixingplan.top

[A24] 去除首尾空白
来源：http://azr.hongshengwenyu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ahp.zhixingplan.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://slq.quarkkingdee.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gnx.ybcxt.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dwy.tanke756.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zde.zdbjq.cn

Go:   strings.TrimSpace(s)
来源：http://ynt.jyoumei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nye.andypj.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cgh.jqgufenzy.top

[A25] 字符串比较
来源：http://qts.zhiwuduotai.top

Py:   s1 == s2; s1 != s2
来源：http://apv.iojbl.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qki.hcnkem.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://msj.hywenlv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://upx.yuxming.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lxb.xuetiantiany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cwc.ehwqpu.com

Ruby: s1 == s2; s1 <=> s2
来源：http://rac.pengpengdd.cyou

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uln.dianchejie.cn

[A26] 类型转换总览
来源：http://jtg.jinyuanbaomall.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rnn.cheryme.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qtl.wangshuangyany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pec.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://fmk.shanyushiyangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lfm.jinqigufen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zzt.yangfankeji.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://pjv.hysaishi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vzn.tanke756.top

================================================================================
来源：http://sze.nanxinkj.top

B. 流程控制
来源：http://gjl.feifeiyinyue.top

================================================================================
来源：http://vik.hcnkem.com

[B01] 条件判断 if / else
来源：http://uej.daria6918.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ezc.cqqwz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wkm.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xtn.yj20258.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dns.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cdc.guannengcc.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lab.fehbvm.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uyj.svipenyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gab.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://ugn.jinqigfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cyt.fanxiaobao.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hnt.fengsongda.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zjh.snrcjt.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jxq.ybcxt.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lcs.tarul.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qxx.chenlongwang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yji.cdnleiting.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tju.chenjidiqi.icu

[B03] switch / match / case
来源：http://bwe.aibaodan.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ede.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://waj.hongshengwenyu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eyy.sysykeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ucj.9152youxi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://czo.cashguo.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zqu.jqgfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zmv.birdmap.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tgt.cqqwz.cn

[B04] for 计数循环
来源：http://ghq.zhaomingkeji.xyz

Py:   for i in range(10): print(i)
来源：http://qbk.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ncs.sufxvd.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zex.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gic.9152youxi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://skf.hammf.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://geg.meibo888.top

Ruby: 10.times { |i| puts i }
来源：http://hlf.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rty.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://xkt.chenlongwang.top

Py:   for item in arr: print(item)
来源：http://uoo.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nxr.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dab.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gwu.wangshuangyany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tco.hnxiangtu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uwg.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://wlk.xinyue.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://syy.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://bdv.shanyushiyangtech.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pvk.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://svh.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vuc.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gcp.yvedp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xcj.cashguo.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nwg.tianlin.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oph.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fod.xylfe.cn

[B07] while 循环
来源：http://qii.fktsv.cn

Py:   while i < 10: i += 1
来源：http://gsc.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://yzy.yueranfly.top

JS:   while (i < 10) { i++; }
来源：http://tmr.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://uax.vehdjk.com

Java: while (i < 10) { i++; }
来源：http://mqi.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gow.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://ifo.zdqjudy.top

C#:   while (i < 10) { i++; }
来源：http://ilb.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://kbz.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://baw.wangdashe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vpo.zhijiandao.cn

JS:   do { i++; } while (i < 10);
来源：http://vqb.jiagoushi.top

TS:   do { i++; } while (i < 10);
来源：http://gjt.ctjpmb.com

Java: do { i++; } while (i < 10);
来源：http://iqv.nanxinkj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kxj.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://drw.zycfv.cn

C#:   do { i++; } while (i < 10);
来源：http://qvu.xuanzx.com

[B09] break 与 continue
来源：http://slj.fanxiaobao.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jqb.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sey.yangfankeji.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jup.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qse.jqgufenzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kub.wangdashe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wzt.jinqigfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jit.bjfxy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://odl.dianchejie.cn

[B10] 遍历同时拿索引
来源：http://wri.guannengcc.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zda.ivvv.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uwx.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pta.ctjpmb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kcq.gaohongyu789.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gny.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qku.cheryme.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ctu.fengsongda.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nid.fzhhl.top

[B11] 生成数字序列 / 区间
来源：http://wdt.yfazqb.com

Py:   list(range(0, 10, 2))
来源：http://sgz.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://mqh.yueranfly.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://acx.pengpengdd.cyou

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tmg.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xcz.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ovl.ywan-chungtsiang.top

Ruby: (0...10).step(2).to_a
来源：http://rtq.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hmw.chenzaomai.com

[B12] 跳出多层循环
来源：http://okm.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nlx.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tao.mhx1999.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pse.316326.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wax.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cjw.wangdashe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yay.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uxt.zhongyouzk.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pof.cashguo.top

[B13] 判断是否为数字
来源：http://wjx.meibo888.top

Py:   isinstance(x, (int, float))
来源：http://mvt.xuanzx.com

PHP:  is_numeric($x)
来源：http://zas.tianlin.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ziv.zhongyouzk.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://atu.vehdjk.com

Java: x instanceof Number
来源：http://qcl.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bwz.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://kwo.ctjpmb.com

C#:   x is int or double or decimal
来源：http://gsc.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://psf.wangshuangyany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tdm.yueranfly.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lkv.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://lco.daria6918.cn

TS:   [1, 2, 3].includes(x)
来源：http://iep.uphjek.com

Java: List.of(1, 2, 3).contains(x)
来源：http://cnf.ybcxt.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iun.pengpengdd.cyou

Ruby: [1, 2, 3].include?(x)
来源：http://bfq.0kj1m.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jlf.nanxuanxn.top

[B15] 布尔运算与取反
来源：http://yqs.jinghuilouyu.cn

Py:   a and b or not c
来源：http://cda.gaohongyu789.top

PHP:  $a && $b || !$c
来源：http://bgq.nwbrower.top

JS:   a && b || !c
来源：http://akf.316326.xyz

TS:   a && b || !c
来源：http://vet.daria6918.cn

Java: a && b || !c
来源：http://kzx.nanxuanxn.top

Go:   a && b || !c
来源：http://vis.hongshengwenyu.top

Ruby: a && b || !c
来源：http://xui.jlsjyb.cn

C#:   a && b || !c
来源：http://cws.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://vkb.vqdsnc.cn

Py:   if not data: return
来源：http://tjk.yj20258.top

PHP:  if (!$data) { return; }
来源：http://fqg.aizwys.cn

JS:   if (!data) return;
来源：http://bzm.c1oappe.top

TS:   if (!data) return;
来源：http://ulf.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://yql.gzhubu.top

Go:   if data == nil { return }
来源：http://cps.hysaishi.cn

Ruby: return if data.nil?
来源：http://hck.dashuyun.cn

C#:   if (data == null) return;
来源：http://jax.0kj1m.cn

================================================================================
来源：http://zld.xinyue.icu

C. 函数与作用域
来源：http://ycy.xylfe.cn

================================================================================
来源：http://hot.shanyushiyangkeji.top

[C01] 定义函数
来源：http://mas.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://ngl.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ldl.shanyushiyangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://hpj.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fpu.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vpl.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ais.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://rwg.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lhg.zhaomingkeji.xyz

[C02] 默认参数
来源：http://lpy.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://vaf.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://blx.zhixingplan.top

JS:   function greet(name = "World") { return name; }
来源：http://zzs.meibo888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zkh.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fos.shanyushiyangtech.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aup.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://wvd.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://baz.ybcxt.top

[C03] 可变参数
来源：http://miz.52xcode.cn

Py:   def total(*args): return sum(args)
来源：http://fqe.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lws.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tez.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pqk.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lmo.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wkq.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://csg.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kpd.sjlbkw.cn

[C04] 命名参数 / 关键字参数
来源：http://zny.xziqi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hde.cashguo.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ynk.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yia.ydjk.org.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hox.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://erc.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://ksl.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://bno.ehwqpu.com

C#:   f(a: 1, b: 2)
来源：http://chm.zdqjudy.top

[C05] 返回多个值
来源：http://leu.fehbvm.com

Py:   return a, b
来源：http://ykb.andypj.xyz

PHP:  return [$a, $b];
来源：http://ptx.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jdx.shangyingyoupin.top

TS:   return { a, b };
来源：http://phj.ydjk.org.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gqs.andypj.xyz

Go:   return a, b
来源：http://zej.haohaochexian.top

Ruby: return a, b
来源：http://rtj.cashguo.top

C#:   return (a, b);              // ValueTuple
来源：http://abd.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://vxv.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://jwk.fktsv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nsg.9152youxi.cn

JS:   const square = x => x * x;
来源：http://pwm.jqgufenzy.top

TS:   const square = (x: number): number => x * x;
来源：http://gjx.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://woz.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://nqo.nanxinkj.top

Ruby: square = ->(x) { x * x }
来源：http://kis.hcnkem.com


<!-- 参考信息 -->