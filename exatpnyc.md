代发 wailian999

Ruby: value = data || "默认值"
来源：http://yya.smart0.xyz

C#:   var value = data ?? "默认值";
来源：http://tzb.tanke756.top

[A16] 真假值判断规则
来源：http://tle.guowangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qly.nanxinkj.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rud.dianchejie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zjp.zdqjudy.top

TS:   if (!x) {}
来源：http://lje.jianghu66.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gjw.vehdjk.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sxg.epnwcf.com

Ruby: unless x            # nil 与 false 为假
来源：http://zas.hesvh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ydo.daxiang520.top

[A17] 位运算
来源：http://scb.svipenyu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zua.pengpengdd.cyou

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jeq.tian-w.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ybcxt.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gww.cheryme.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ocs.yongpay.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://evq.bjfxy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cho.vehdjk.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lqu.jianghu66.top

[A18] 字符与 ASCII 码互转
来源：http://mla.hysaishi.cn

Py:   ord("A"); chr(65)
来源：http://lel.dashuyun.cn

PHP:  ord("A"); chr(65)
来源：http://dag.jinqigufen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://usx.zdbjq.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jjq.fzhhl.top

Java: (int) 'A'; (char) 65
来源：http://jfi.gzhubu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ynb.iojbl.cn

Ruby: "A".ord; 65.chr
来源：http://cyv.yueranfly.top

C#:   (int)'A'; (char)65
来源：http://zos.zhijiandao.cn

[A19] 交换两个变量
来源：http://gpo.daria6918.cn

Py:   a, b = b, a
来源：http://jqe.fanxiaobao.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://kch.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://yil.meibo888.top

TS:   [a, b] = [b, a];
来源：http://prm.gzhubu.top

Java: int t = a; a = b; b = t;
来源：http://ldn.yanxiufei.cn

Go:   a, b = b, a
来源：http://lwv.daxiang520.top

Ruby: a, b = b, a
来源：http://adl.zdqjudy.top

C#:   (a, b) = (b, a);
来源：http://obm.hfpthk.cn

[A20] 读取标准输入
来源：http://uwq.316326.xyz

Py:   name = input("请输入：")
来源：http://ysp.fktsv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://aro.aizwys.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fdx.hcnkem.com

TS:   // Node.js：readline 模块
来源：http://qmg.chenzaomai.com

Java: new Scanner(System.in).nextLine()
来源：http://ila.yvedp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dnv.jinghuilouyu.cn

Ruby: gets.chomp
来源：http://niq.guannengcc.top

C#:   Console.ReadLine();
来源：http://tsv.yongpay.top

[A21] 保留指定小数位输出
来源：http://sso.shangyingyoupin.top

Py:   f"{3.14159:.2f}"
来源：http://rsg.yuxming.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dsp.ctjpmb.com

JS:   (3.14159).toFixed(2)
来源：http://shq.yj202588.top

TS:   (3.14159).toFixed(2)
来源：http://ijd.yj20258888.top

Java: String.format("%.2f", 3.14159)
来源：http://uoq.zhiwuduotai.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jgj.9152youxi.cn

Ruby: format("%.2f", 3.14159)
来源：http://wcc.yangfankeji.com

C#:   3.14159.ToString("F2")
来源：http://gpb.yvedp.cn

[A22] 获取字符串长度
来源：http://lrn.shanyushiyangtech.top

Py:   len(s)
来源：http://nze.cdnleiting.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://awp.xylfe.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://olo.cqqwz.cn

TS:   s.length
来源：http://thk.sysykeji.top

Java: s.length()
来源：http://naa.yueranfly.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ioj.mhx1999.top

Ruby: s.length
来源：http://vgd.dashuyun.cn

C#:   s.Length
来源：http://vfj.tian-w.cn

[A23] 大小写转换
来源：http://hwx.uphjek.com

Py:   s.upper(); s.lower(); s.title()
来源：http://mkk.wangshuangyany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fdo.sufxvd.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xce.yanxiufei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cgu.ydzc1.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hfy.zdqjudy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://puk.sysykeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dub.havefunace.top

C#:   s.ToUpper(); s.ToLower()
来源：http://isj.cqqwz.cn

[A24] 去除首尾空白
来源：http://foc.fzhhl.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://svo.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rfx.sweek.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nii.ppjwa.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://som.birdmap.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://myv.ydzc1.top

Go:   strings.TrimSpace(s)
来源：http://qgo.shzxlz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://waj.ydzc1.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ynh.jinqigufen.top

[A25] 字符串比较
来源：http://uru.uphjek.com

Py:   s1 == s2; s1 != s2
来源：http://azc.gaohongyu789.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gcx.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nvg.hongshengwenyu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vap.wangdashe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jom.vqdsnc.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ptp.tanke756.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ijf.jianghu66.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ica.shanyushiyangkeji.top

[A26] 类型转换总览
来源：http://hfa.yuanzhike.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fav.c1oappe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://czx.tian-w.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jcz.xuetiantiany.cn

TS:   Number() String() Boolean() x as number
来源：http://zyw.ehwqpu.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uxg.uphjek.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dbq.iojbl.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oom.hywenlv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lky.bjfxy.top

================================================================================
来源：http://rqb.zhixingplan.top

B. 流程控制
来源：http://tug.shuidangran.top

================================================================================
来源：http://gly.jinghuilouyu.cn

[B01] 条件判断 if / else
来源：http://kwt.fanxiaobao.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://uzb.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pvk.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qgf.chenlongwang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://elg.c1oappe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://iqg.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fth.jyoumei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kmi.sufxvd.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ash.zhengqikj.top

[B02] 多分支 else if / elif
来源：http://kru.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zfq.guowangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jxr.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bzn.hesvh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zyw.ppjwa.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://niv.hammf.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aaj.guannengcc.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://toq.hysaishi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wzo.redwolf501.top

[B03] switch / match / case
来源：http://wrz.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ibs.yvedp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://knd.ctjpmb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pvp.xuetiantiany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gyu.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ubl.aizwys.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dgk.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://obg.mhx1999.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zxq.redwolf501.top

[B04] for 计数循环
来源：http://zrx.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://dzf.0kj1m.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://auw.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://taz.zhengqikj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wab.ehwqpu.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mez.chenlongwang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hmn.hongshengwenyu.top

Ruby: 10.times { |i| puts i }
来源：http://smd.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://olp.nanxuanxn.top

[B05] 遍历数组 / 列表
来源：http://mhg.wangdashe.top

Py:   for item in arr: print(item)
来源：http://mdo.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xyr.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ppv.jinqigufen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fwp.xingfuxueyuan.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://qcx.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rdw.jianghu66.top

Ruby: arr.each { |item| puts item }
来源：http://foo.hywenlv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sjz.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://kuj.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vbd.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tge.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gmq.nwbrower.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ajy.yuanzhike.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jgu.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oqx.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sof.gzhubu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dgd.hfpthk.cn

[B07] while 循环
来源：http://kic.andypj.xyz

Py:   while i < 10: i += 1
来源：http://nqt.pycfn.com

PHP:  while ($i < 10) { $i++; }
来源：http://nnb.jinqigufen.top

JS:   while (i < 10) { i++; }
来源：http://ejh.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://ppq.yanxiufei.cn

Java: while (i < 10) { i++; }
来源：http://fee.guowangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xqc.jlsjyb.cn

Ruby: while i < 10; i += 1; end
来源：http://sgr.jyoumei.cn

C#:   while (i < 10) { i++; }
来源：http://nat.gogol.net.cn

[B08] do-while（至少执行一次）
来源：http://jez.cucudq.cn

Py:   # 无 do-while：用 while True + break
来源：http://ncn.iojbl.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://alt.yj20258.top

JS:   do { i++; } while (i < 10);
来源：http://kgn.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://irg.shuidangran.top

Java: do { i++; } while (i < 10);
来源：http://gnu.quarkkingdee.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fio.vehdjk.com

Ruby: begin; i += 1; end while i < 10
来源：http://pbv.kuanghao11.cn

C#:   do { i++; } while (i < 10);
来源：http://eur.xingfuxueyuan.xyz

[B09] break 与 continue
来源：http://yob.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://czi.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cfg.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hhj.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://len.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gsd.svipenyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hxc.xinyue.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jqv.yonumen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sgb.mhx1999.top

[B10] 遍历同时拿索引
来源：http://evq.zhijiandao.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vbb.gogol.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ysi.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mnj.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tbw.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://irb.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ien.jiagoushi.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ajy.jinqigfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gdq.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://kku.yj20258888.top

Py:   list(range(0, 10, 2))
来源：http://qfy.sysykeji.top

PHP:  range(0, 10, 2);
来源：http://lpi.shanyushiyangtech.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ccj.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://etl.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yjp.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tkh.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://wcd.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qrk.cashguo.top

[B12] 跳出多层循环
来源：http://obf.cqqwz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wxk.quarkkingdee.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dxp.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gpt.haohaochexian.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lgc.52xcode.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gwp.zdbjq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dfe.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mfp.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bah.uphjek.com

[B13] 判断是否为数字
来源：http://pbi.dianchejie.cn

Py:   isinstance(x, (int, float))
来源：http://nnz.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://crl.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ntv.zhengqikj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ikd.0kj1m.cn

Java: x instanceof Number
来源：http://jnf.fzhhl.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mad.cqqwz.cn

Ruby: x.is_a?(Numeric)
来源：http://eln.yfazqb.com

C#:   x is int or double or decimal
来源：http://gco.zhongyouzk.top

[B14] 判断值是否在集合内
来源：http://vtl.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jyd.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zoz.zhixingplan.top

JS:   [1, 2, 3].includes(x)
来源：http://zyz.yongpay.top

TS:   [1, 2, 3].includes(x)
来源：http://zwm.hammf.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xzt.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jtz.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://esz.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dyx.aibaodan.cn

[B15] 布尔运算与取反
来源：http://cwy.ydzc1.top

Py:   a and b or not c
来源：http://cfe.bbcook.cn

PHP:  $a && $b || !$c
来源：http://iqv.hongshengwenyu.top

JS:   a && b || !c
来源：http://slw.hywenlv.cn

TS:   a && b || !c
来源：http://pbm.hongshengwenyu.top

Java: a && b || !c
来源：http://ybo.bjfxy.top

Go:   a && b || !c
来源：http://vpc.xingfuxueyuan.xyz

Ruby: a && b || !c
来源：http://oyk.hesvh.cn

C#:   a && b || !c
来源：http://bde.ydzc1.top

[B16] 卫语句：不满足条件提前返回
来源：http://zpl.tian-w.cn

Py:   if not data: return
来源：http://caj.feifeiyinyue.top

PHP:  if (!$data) { return; }
来源：http://gaj.vqdsnc.cn

JS:   if (!data) return;
来源：http://yud.fanxiaobao.xyz

TS:   if (!data) return;
来源：http://voc.chenjidiqi.icu

Java: if (data == null) return;
来源：http://pbt.xziqi.cn

Go:   if data == nil { return }
来源：http://dhy.guowangkeji.top

Ruby: return if data.nil?
来源：http://diu.0kj1m.cn

C#:   if (data == null) return;
来源：http://kaf.zhoulong.xyz

================================================================================
来源：http://ulo.nanxuanxn.top

C. 函数与作用域
来源：http://zjg.fzhhl.top

================================================================================
来源：http://bxf.uphjek.com

[C01] 定义函数
来源：http://xky.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://rca.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://son.nanxuanxn.top

JS:   function add(a, b) { return a + b; }
来源：http://akw.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://msi.sxryk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ahp.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iqu.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://scr.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dxx.jianghu66.top

[C02] 默认参数
来源：http://ygr.ydzc1.top

Py:   def greet(name="World"): return name
来源：http://wdn.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://eka.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://erb.yuxming.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://boo.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pgf.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://isc.ydzc1.top

Ruby: def greet(name = "World") = name
来源：http://iqh.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://dzj.xuanzx.com

[C03] 可变参数
来源：http://hzz.ehwqpu.com

Py:   def total(*args): return sum(args)
来源：http://nmj.jyoumei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kqv.daxiang520.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gkq.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vyo.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://agi.kuanghao11.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oqa.xinyue.icu

Ruby: def total(*nums); nums.sum; end
来源：http://zpk.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zuy.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://mwn.sjlbkw.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zhi.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ktf.hfpthk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zot.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qko.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://mav.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://kxd.hesvh.cn

Ruby: f(a: 1, b: 2)
来源：http://vyj.hfpthk.cn

C#:   f(a: 1, b: 2)
来源：http://wlt.gotoacloud.top

[C05] 返回多个值
来源：http://kaz.tian-w.cn

Py:   return a, b
来源：http://arf.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://vkq.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bdb.tanke756.top

TS:   return { a, b };
来源：http://dse.tanke756.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rvo.zhengqikj.top

Go:   return a, b
来源：http://jlt.hnxiangtu.top

Ruby: return a, b
来源：http://ldd.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://tof.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://ber.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://peo.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cdf.dashuyun.cn

JS:   const square = x => x * x;
来源：http://pqg.ywan-chungtsiang.top


<!-- 参考信息 -->