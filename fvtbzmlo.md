代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://fbd.zhijiandao.cn

[A15] 空值判断与默认值
来源：http://csn.tianlin.xyz

Py:   value = data or "默认值"
来源：http://rdi.cucudq.cn

PHP:  $value = $data ?? "默认值";
来源：http://wxn.hesvh.cn

JS:   const value = data ?? "默认值";
来源：http://uen.shanyushiyangtech.top

TS:   const value = data ?? "默认值";
来源：http://tdz.iojbl.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oir.shzxlz.cn

Go:   if data == "" { data = "默认值" }
来源：http://mdp.yanxiufei.cn

Ruby: value = data || "默认值"
来源：http://xbg.zhengqikj.top

C#:   var value = data ?? "默认值";
来源：http://dck.yueranfly.top

[A16] 真假值判断规则
来源：http://wkh.epnwcf.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gej.gzhubu.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://elr.yangfankeji.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bdb.smart0.xyz

TS:   if (!x) {}
来源：http://whi.jinqigufen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tpv.bbcook.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qxa.fktsv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pau.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zho.meibo888.top

[A17] 位运算
来源：http://ckv.cashguo.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gwj.xziqi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://oio.hfpthk.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pjg.fengsongda.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://czp.yueranfly.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cxg.yuanzhike.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xzm.snrcjt.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mto.xingfuxueyuan.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kjo.zhaomingkeji.xyz

[A18] 字符与 ASCII 码互转
来源：http://aze.jinqigfzy.top

Py:   ord("A"); chr(65)
来源：http://nbs.yonumen.top

PHP:  ord("A"); chr(65)
来源：http://rgg.chenlongwang.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vpt.fehbvm.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qgp.nwbrower.top

Java: (int) 'A'; (char) 65
来源：http://ktv.shzxlz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://brp.ybcxt.top

Ruby: "A".ord; 65.chr
来源：http://hcp.jinyuanbaomall.cn

C#:   (int)'A'; (char)65
来源：http://vgi.zhoulong.xyz

[A19] 交换两个变量
来源：http://wuu.ywan-chungtsiang.top

Py:   a, b = b, a
来源：http://uat.zhoulong.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://bzf.0kj1m.cn

JS:   [a, b] = [b, a];
来源：http://ibu.cdnleiting.top

TS:   [a, b] = [b, a];
来源：http://zjl.kuanghao11.cn

Java: int t = a; a = b; b = t;
来源：http://krz.yonumen.top

Go:   a, b = b, a
来源：http://evo.9152youxi.cn

Ruby: a, b = b, a
来源：http://hme.dianchejie.cn

C#:   (a, b) = (b, a);
来源：http://gnh.ybcxt.top

[A20] 读取标准输入
来源：http://osy.tanke756.top

Py:   name = input("请输入：")
来源：http://ujr.gogol.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lkp.ctjpmb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xun.jinqigfzy.top

TS:   // Node.js：readline 模块
来源：http://cxr.quarkkingdee.top

Java: new Scanner(System.in).nextLine()
来源：http://rfh.chenzaomai.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dhs.shanyushiyangkeji.top

Ruby: gets.chomp
来源：http://lia.guowangkeji.top

C#:   Console.ReadLine();
来源：http://ape.cdnleiting.top

[A21] 保留指定小数位输出
来源：http://oca.hfpthk.cn

Py:   f"{3.14159:.2f}"
来源：http://qvm.shanyushiyangtech.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uxa.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://nco.c1oappe.top

TS:   (3.14159).toFixed(2)
来源：http://iio.zdbjq.cn

Java: String.format("%.2f", 3.14159)
来源：http://ktz.ydzc1.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gxw.daria6918.cn

Ruby: format("%.2f", 3.14159)
来源：http://nxo.cdnleiting.top

C#:   3.14159.ToString("F2")
来源：http://njz.bjfxy.top

[A22] 获取字符串长度
来源：http://jsr.aizwys.cn

Py:   len(s)
来源：http://nfh.pycfn.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xwa.sweek.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hmm.haohaochexian.top

TS:   s.length
来源：http://cqk.zhongyouzk.top

Java: s.length()
来源：http://whs.guannengcc.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fqo.zhongyouzk.top

Ruby: s.length
来源：http://qza.nwbrower.top

C#:   s.Length
来源：http://kfw.ydjk.org.cn

[A23] 大小写转换
来源：http://pov.sufxvd.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ggt.havefunace.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://swy.bjfxy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://axa.fzhhl.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yag.bjfxy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qfn.vehdjk.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eat.zhongyouzk.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wlf.sufxvd.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bjq.havefunace.top

[A24] 去除首尾空白
来源：http://bzx.yuanzhike.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sic.hnxiangtu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wod.fehbvm.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pjk.jqgfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ejj.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pbu.hongshengwenyu.top

Go:   strings.TrimSpace(s)
来源：http://pej.dianchejie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eyc.shangyingyoupin.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ouv.sjlbkw.cn

[A25] 字符串比较
来源：http://rkj.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://goz.birdmap.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gyl.zhiwuduotai.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oti.yanxiufei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lkz.svipenyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oel.jiagoushi.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xps.chenzaomai.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ani.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rnl.yuanzhike.top

[A26] 类型转换总览
来源：http://vah.gzhubu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dfu.sxryk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xgs.yj20258.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pot.yueranfly.top

TS:   Number() String() Boolean() x as number
来源：http://jxi.kuanghao11.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eve.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aqz.vehdjk.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://cdr.haohaochexian.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://njn.zycfv.cn

================================================================================
来源：http://nmk.hysaishi.cn

B. 流程控制
来源：http://xth.iojbl.cn

================================================================================
来源：http://zfa.yonumen.top

[B01] 条件判断 if / else
来源：http://fuk.shangyingyoupin.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ccc.hnxiangtu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dew.jinqigufen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baj.cdnleiting.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dwv.hongshengwenyu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.zhijiandao.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eoq.andypj.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vdc.bbcook.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://txf.jinqigfzy.top

[B02] 多分支 else if / elif
来源：http://qbk.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wga.aizwys.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jgu.fehbvm.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xkn.jlsjyb.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vos.sweek.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aso.feifeiyinyue.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gll.aibaodan.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lgt.ywan-chungtsiang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ogu.hesvh.cn

[B03] switch / match / case
来源：http://qkn.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lhc.jinghuilouyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gps.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wxa.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mdy.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nso.nanxinkj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mlq.chenlongwang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qqa.9152youxi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pcf.zdbjq.cn

[B04] for 计数循环
来源：http://nlm.meibo888.top

Py:   for i in range(10): print(i)
来源：http://xsu.jqgufenzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bnb.yvedp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yby.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ymq.jiagoushi.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gjs.zhengqikj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ywd.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://dfa.sysykeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rrt.hcnkem.com

[B05] 遍历数组 / 列表
来源：http://wew.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://bkr.xuetiantiany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yhn.gotoacloud.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bgk.zdbjq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qfb.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dqr.xuetiantiany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yti.yonumen.top

Ruby: arr.each { |item| puts item }
来源：http://skx.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gbz.vqdsnc.cn

[B06] 遍历字典 / 对象
来源：http://hhl.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xsn.pengpengdd.cyou

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qhb.yvedp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://swp.yongpay.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xrj.kuanghao11.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://psg.hammf.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lpt.jyoumei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zhn.yanxiufei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ntj.iojbl.cn

[B07] while 循环
来源：http://rep.snrcjt.cn

Py:   while i < 10: i += 1
来源：http://fzd.meibo888.top

PHP:  while ($i < 10) { $i++; }
来源：http://skn.fehbvm.com

JS:   while (i < 10) { i++; }
来源：http://axq.yj20258.top

TS:   while (i < 10) { i++; }
来源：http://xwc.zdqjudy.top

Java: while (i < 10) { i++; }
来源：http://zdx.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vxo.birdmap.top

Ruby: while i < 10; i += 1; end
来源：http://xik.shuidangran.top

C#:   while (i < 10) { i++; }
来源：http://jru.tianlin.xyz

[B08] do-while（至少执行一次）
来源：http://iym.nwbrower.top

Py:   # 无 do-while：用 while True + break
来源：http://pwq.bjfxy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pcf.meibo888.top

JS:   do { i++; } while (i < 10);
来源：http://zqe.chenzaomai.com

TS:   do { i++; } while (i < 10);
来源：http://khz.fktsv.cn

Java: do { i++; } while (i < 10);
来源：http://okc.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://sap.ydzc1.top

Ruby: begin; i += 1; end while i < 10
来源：http://hal.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://wls.316326.xyz

[B09] break 与 continue
来源：http://nge.chenlongwang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vre.xinyue.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kdz.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uqh.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hww.316326.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://omf.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gcp.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vzm.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qmm.hywenlv.cn

[B10] 遍历同时拿索引
来源：http://plu.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gfv.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iuw.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ohf.cdnleiting.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jyq.dianchejie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oav.daxiang520.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nzn.sufxvd.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gmm.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cjx.zhijiandao.cn

[B11] 生成数字序列 / 区间
来源：http://cdx.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://grf.guannengcc.top

PHP:  range(0, 10, 2);
来源：http://hda.hammf.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nsh.jinyuanbaomall.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://huj.hcnkem.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fob.wangshuangyany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oub.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://nsb.yueranfly.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fsd.zhengqikj.top

[B12] 跳出多层循环
来源：http://wml.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ijb.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mnj.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hlj.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sqq.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bmr.fktsv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://waj.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yam.hfpthk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hcy.fengsongda.top

[B13] 判断是否为数字
来源：http://gtd.nanxinkj.top

Py:   isinstance(x, (int, float))
来源：http://txw.cashguo.top

PHP:  is_numeric($x)
来源：http://jwd.hfpthk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lig.smart0.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dno.hcnkem.com

Java: x instanceof Number
来源：http://lmj.zhongyouzk.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sar.zycfv.cn

Ruby: x.is_a?(Numeric)
来源：http://gyh.yj20258888.top

C#:   x is int or double or decimal
来源：http://spf.jyoumei.cn

[B14] 判断值是否在集合内
来源：http://lpe.wangshuangyany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cov.meibo888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qcy.uphjek.com

JS:   [1, 2, 3].includes(x)
来源：http://cwg.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://jkv.snrcjt.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rvv.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://riq.sweek.top

Ruby: [1, 2, 3].include?(x)
来源：http://axw.0kj1m.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://svz.tarul.cn

[B15] 布尔运算与取反
来源：http://fen.cdnleiting.top

Py:   a and b or not c
来源：http://rfx.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://mua.yonumen.top

JS:   a && b || !c
来源：http://yut.aibaodan.cn

TS:   a && b || !c
来源：http://cpl.ivvv.top

Java: a && b || !c
来源：http://fgl.bbcook.cn

Go:   a && b || !c
来源：http://mqf.haohaochexian.top

Ruby: a && b || !c
来源：http://aio.smart0.xyz

C#:   a && b || !c
来源：http://eqi.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://kmn.jlsjyb.cn

Py:   if not data: return
来源：http://rmj.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://zar.jlsjyb.cn

JS:   if (!data) return;
来源：http://nwd.fktsv.cn

TS:   if (!data) return;
来源：http://btn.sufxvd.cn

Java: if (data == null) return;
来源：http://dnq.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://msw.yuxming.cn

Ruby: return if data.nil?
来源：http://usk.birdmap.top

C#:   if (data == null) return;
来源：http://mxf.birdmap.top

================================================================================
来源：http://khm.yvedp.cn

C. 函数与作用域
来源：http://wtt.yongpay.top

================================================================================
来源：http://noa.xingfuxueyuan.xyz

[C01] 定义函数
来源：http://jno.vehdjk.com

Py:   def add(a, b): return a + b
来源：http://uks.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fel.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://zeb.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wid.yangfankeji.com

Java: static int add(int a, int b) { return a + b; }
来源：http://swt.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://vwm.zhoulong.xyz

Ruby: def add(a, b); a + b; end
来源：http://xet.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://agx.gogol.net.cn

[C02] 默认参数
来源：http://brc.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://kai.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://imf.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://otd.zhoulong.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://mjp.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vwr.cqqwz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bgr.yangfankeji.com

Ruby: def greet(name = "World") = name
来源：http://iya.gaohongyu789.top

C#:   string Greet(string name = "World") => name;
来源：http://btd.ivvv.top

[C03] 可变参数
来源：http://fub.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://ual.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kup.xuetiantiany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xna.yvedp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tfk.shzxlz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uew.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bfz.aizwys.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xzt.nwbrower.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bcu.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://qvi.ctjpmb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xsa.snrcjt.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qwu.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lqe.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qyn.jianghu66.top

Java: // 无：用 Builder 模式或 record
来源：http://ltp.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://rzn.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://jnr.tanke756.top

C#:   f(a: 1, b: 2)
来源：http://gmf.jinqigfzy.top

[C05] 返回多个值
来源：http://kqf.havefunace.top

Py:   return a, b
来源：http://rsj.xuetiantiany.cn

PHP:  return [$a, $b];
来源：http://tns.ehwqpu.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://gun.hammf.cn

TS:   return { a, b };
来源：http://tqi.yanxiufei.cn


<!-- 参考信息 -->