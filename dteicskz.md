代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zua.gotoacloud.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lzc.yvedp.cn

TS:   if (!x) {}
来源：http://aby.ehwqpu.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yms.xuanzx.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uaa.fktsv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gqk.fktsv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dgw.jinqigfzy.top

[A17] 位运算
来源：http://zox.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ibd.gotoacloud.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wxf.svipenyu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kgi.yuxming.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://osx.hcnkem.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uht.sxryk.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cyw.hesvh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eyk.feifeiyinyue.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iub.fanxiaobao.xyz

[A18] 字符与 ASCII 码互转
来源：http://nls.fanxiaobao.xyz

Py:   ord("A"); chr(65)
来源：http://obr.zhongyouzk.top

PHP:  ord("A"); chr(65)
来源：http://ism.shanyushiyangkeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eqr.xinyue.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cho.guannengcc.top

Java: (int) 'A'; (char) 65
来源：http://nbk.vqdsnc.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://djw.xuanzx.com

Ruby: "A".ord; 65.chr
来源：http://hpw.zhengqikj.top

C#:   (int)'A'; (char)65
来源：http://rfk.gotoacloud.top

[A19] 交换两个变量
来源：http://oqy.yj20258.top

Py:   a, b = b, a
来源：http://qna.cucudq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cgc.c1oappe.top

JS:   [a, b] = [b, a];
来源：http://grt.yuanzhike.top

TS:   [a, b] = [b, a];
来源：http://xyd.aibaodan.cn

Java: int t = a; a = b; b = t;
来源：http://yfa.xziqi.cn

Go:   a, b = b, a
来源：http://wxv.redwolf501.top

Ruby: a, b = b, a
来源：http://ker.mhx1999.top

C#:   (a, b) = (b, a);
来源：http://rvr.ybcxt.top

[A20] 读取标准输入
来源：http://zan.cqqwz.cn

Py:   name = input("请输入：")
来源：http://zuz.zhiwuduotai.top

PHP:  $name = trim(fgets(STDIN));
来源：http://cbk.tianlin.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ibg.ivvv.top

TS:   // Node.js：readline 模块
来源：http://zoz.jqgfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://pxp.shangyingyoupin.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ygn.svipenyu.cn

Ruby: gets.chomp
来源：http://car.cqqwz.cn

C#:   Console.ReadLine();
来源：http://cwp.tarul.cn

[A21] 保留指定小数位输出
来源：http://fuc.tianlin.xyz

Py:   f"{3.14159:.2f}"
来源：http://bav.yanxiufei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iim.jqgufenzy.top

JS:   (3.14159).toFixed(2)
来源：http://gtf.wangshuangyany.cn

TS:   (3.14159).toFixed(2)
来源：http://hli.tanke756.top

Java: String.format("%.2f", 3.14159)
来源：http://wpr.gogol.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eto.0kj1m.cn

Ruby: format("%.2f", 3.14159)
来源：http://sry.yangfankeji.com

C#:   3.14159.ToString("F2")
来源：http://nbs.smart0.xyz

[A22] 获取字符串长度
来源：http://tdx.bjfxy.top

Py:   len(s)
来源：http://ijf.quarkkingdee.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ddy.shangyingyoupin.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ebb.svipenyu.cn

TS:   s.length
来源：http://hrl.hnqzz.top

Java: s.length()
来源：http://lyy.9152youxi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rdo.tarul.cn

Ruby: s.length
来源：http://cbj.zhixingplan.top

C#:   s.Length
来源：http://jvp.tianlin.xyz

[A23] 大小写转换
来源：http://gih.hesvh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hnf.zdbjq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kzd.yueranfly.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fga.feifeiyinyue.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cth.iojbl.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vhl.bbcook.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lpl.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://asc.snrcjt.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kbd.gzhubu.top

[A24] 去除首尾空白
来源：http://mdy.guowangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ntk.cucudq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ier.yuxming.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ith.zdbjq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qih.tanke756.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eaw.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://qpp.fktsv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hvn.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tkd.redwolf501.top

[A25] 字符串比较
来源：http://fsd.yj202588.top

Py:   s1 == s2; s1 != s2
来源：http://irw.daria6918.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rkb.zdqjudy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nsn.gaohongyu789.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jkd.svipenyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ats.svipenyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jql.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jdi.hcnkem.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fkl.yueranfly.top

[A26] 类型转换总览
来源：http://rog.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pqo.gotoacloud.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zbe.shanyushiyangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tio.xingfuxueyuan.xyz

TS:   Number() String() Boolean() x as number
来源：http://ixz.shanyushiyangtech.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rsi.hnqzz.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kzj.yuxming.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ikh.aibaodan.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dwg.fktsv.cn

================================================================================
来源：http://mkq.chenzaomai.com

B. 流程控制
来源：http://xit.52xcode.cn

================================================================================
来源：http://ale.bbcook.cn

[B01] 条件判断 if / else
来源：http://wdh.hesvh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://njp.yuanzhike.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zsg.yonumen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://exr.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fmg.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xfi.chenzaomai.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gyh.sufxvd.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://puj.fanxiaobao.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dhy.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://pek.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://icc.epnwcf.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mst.yueranfly.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qsj.daxiang520.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bmh.gotoacloud.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://plw.epnwcf.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://abt.bjfxy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rnh.sweek.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bxg.epnwcf.com

[B03] switch / match / case
来源：http://pzt.kuanghao11.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://psa.xuetiantiany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iwf.jinghuilouyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kzx.fzhhl.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tnr.yj20258.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://olh.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://olw.shangyingyoupin.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wwg.hesvh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nty.zhengqikj.top

[B04] for 计数循环
来源：http://ueo.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://nso.sxryk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ukc.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zit.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rtc.xuanzx.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jqs.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mmr.hywenlv.cn

Ruby: 10.times { |i| puts i }
来源：http://byp.yuanzhike.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ucz.ybcxt.top

[B05] 遍历数组 / 列表
来源：http://jij.dianchejie.cn

Py:   for item in arr: print(item)
来源：http://xtc.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dhb.ywan-chungtsiang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kfs.hesvh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pzt.tarul.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ywv.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rjk.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://qqb.andypj.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dtl.316326.xyz

[B06] 遍历字典 / 对象
来源：http://jos.gotoacloud.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lpl.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pmg.fengsongda.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eox.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mpr.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://axt.yj20258888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pja.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pyw.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tux.epnwcf.com

[B07] while 循环
来源：http://eeh.shanyushiyangkeji.top

Py:   while i < 10: i += 1
来源：http://uxf.sysykeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://hgn.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://yrp.xingfuxueyuan.xyz

TS:   while (i < 10) { i++; }
来源：http://bsu.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://gom.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://avx.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://lkc.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://csj.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://hho.dianchejie.cn

Py:   # 无 do-while：用 while True + break
来源：http://rzp.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qgq.epnwcf.com

JS:   do { i++; } while (i < 10);
来源：http://nei.ydzc1.top

TS:   do { i++; } while (i < 10);
来源：http://llj.chenlongwang.top

Java: do { i++; } while (i < 10);
来源：http://qxh.gogol.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dpb.jinqigufen.top

Ruby: begin; i += 1; end while i < 10
来源：http://xlg.jinqigufen.top

C#:   do { i++; } while (i < 10);
来源：http://rzd.aizwys.cn

[B09] break 与 continue
来源：http://jww.ydjk.org.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zif.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yml.fehbvm.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nfs.ybcxt.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yip.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hkn.zhongyouzk.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pds.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://caa.shanyushiyangtech.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://klx.yj202588.top

[B10] 遍历同时拿索引
来源：http://zqc.havefunace.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hqe.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pox.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wwo.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://agk.xinyue.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ghp.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kwy.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wtw.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zcp.yangfankeji.com

[B11] 生成数字序列 / 区间
来源：http://gtn.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://crs.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://nzx.daria6918.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jkb.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qzy.yonumen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hzw.tian-w.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://apo.jinqigfzy.top

Ruby: (0...10).step(2).to_a
来源：http://zes.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uhn.andypj.xyz

[B12] 跳出多层循环
来源：http://lvc.fktsv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lbw.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dko.ybcxt.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vnk.guowangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wbk.zhongyouzk.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vby.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://syf.guannengcc.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wvf.cucudq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hng.shanyushiyangkeji.top

[B13] 判断是否为数字
来源：http://lce.yangfankeji.com

Py:   isinstance(x, (int, float))
来源：http://swr.cucudq.cn

PHP:  is_numeric($x)
来源：http://wkw.tanke756.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dsw.jinghuilouyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jfc.gotoacloud.top

Java: x instanceof Number
来源：http://ojc.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pgs.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://dau.guannengcc.top

C#:   x is int or double or decimal
来源：http://odo.yangfankeji.com

[B14] 判断值是否在集合内
来源：http://zxk.nanxinkj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://deq.redwolf501.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tcp.svipenyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://plt.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://zwv.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qnw.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rws.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hgz.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fvd.yj20258888.top

[B15] 布尔运算与取反
来源：http://kld.zhiwuduotai.top

Py:   a and b or not c
来源：http://yal.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://nun.sjlbkw.cn

JS:   a && b || !c
来源：http://fuh.jinqigfzy.top

TS:   a && b || !c
来源：http://ggv.iojbl.cn

Java: a && b || !c
来源：http://wjg.mhx1999.top

Go:   a && b || !c
来源：http://psc.xylfe.cn

Ruby: a && b || !c
来源：http://bio.aibaodan.cn

C#:   a && b || !c
来源：http://cvg.yanxiufei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zrc.iojbl.cn

Py:   if not data: return
来源：http://gco.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://psk.dianchejie.cn

JS:   if (!data) return;
来源：http://ruc.mhx1999.top

TS:   if (!data) return;
来源：http://uqd.shangyingyoupin.top

Java: if (data == null) return;
来源：http://olm.fktsv.cn

Go:   if data == nil { return }
来源：http://exc.fanxiaobao.xyz

Ruby: return if data.nil?
来源：http://jai.pengpengdd.cyou

C#:   if (data == null) return;
来源：http://fvh.feifeiyinyue.top

================================================================================
来源：http://llw.gogol.net.cn

C. 函数与作用域
来源：http://pvh.jinyuanbaomall.cn

================================================================================
来源：http://lir.ydjk.org.cn

[C01] 定义函数
来源：http://vwf.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://fbp.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zxp.gzhubu.top

JS:   function add(a, b) { return a + b; }
来源：http://gvj.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oeo.jyoumei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vyz.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xcb.feifeiyinyue.top

Ruby: def add(a, b); a + b; end
来源：http://soh.ppjwa.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bgf.shanyushiyangkeji.top

[C02] 默认参数
来源：http://lns.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://wqu.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://mwj.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://ncp.sjlbkw.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://luw.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://lhw.haohaochexian.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oik.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://pps.guannengcc.top

C#:   string Greet(string name = "World") => name;
来源：http://kxw.zhoulong.xyz

[C03] 可变参数
来源：http://kwp.pycfn.com

Py:   def total(*args): return sum(args)
来源：http://mdp.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ali.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hkb.guannengcc.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ywj.mhx1999.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dth.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hly.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://cdz.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ckf.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://qqp.guannengcc.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zzh.gzhubu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rtx.fengsongda.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mbd.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kqa.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://bbq.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://jtw.hongshengwenyu.top

Ruby: f(a: 1, b: 2)
来源：http://pgl.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://kyy.zhongyouzk.top

[C05] 返回多个值
来源：http://cht.gzhubu.top

Py:   return a, b
来源：http://fhx.ybcxt.top

PHP:  return [$a, $b];
来源：http://nhe.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ubk.zhoulong.xyz

TS:   return { a, b };
来源：http://tov.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://daw.gotoacloud.top

Go:   return a, b
来源：http://zpk.andypj.xyz

Ruby: return a, b
来源：http://ihz.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://odb.xingfuxueyuan.xyz

[C06] 匿名函数 / lambda
来源：http://xos.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://qka.wangshuangyany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oje.tianlin.xyz

JS:   const square = x => x * x;
来源：http://rdu.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://dje.xylfe.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cqy.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://omu.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://nlg.xziqi.cn


<!-- 参考信息 -->