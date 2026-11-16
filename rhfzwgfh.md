代发 wailian999

[A14] 注释写法
来源：http://xek.pengpengdd.cyou

Py:   # 单行；三引号字符串可作多行说明
来源：http://kal.gotoacloud.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://oft.zhixingplan.top

JS:   // 单行；/* 多行 */
来源：http://joe.jiagoushi.top

TS:   // 单行；/* 多行 */
来源：http://dpf.zycfv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rwb.yj20258888.top

Go:   // 单行；/* 多行 */
来源：http://pet.sweek.top

Ruby: # 单行；=begin 多行 =end
来源：http://idd.jlsjyb.cn

C#:   // 单行；/* 多行 */
来源：http://kvf.vqdsnc.cn

[A15] 空值判断与默认值
来源：http://qzz.shanyushiyangkeji.top

Py:   value = data or "默认值"
来源：http://rpu.jiagoushi.top

PHP:  $value = $data ?? "默认值";
来源：http://qis.yonumen.top

JS:   const value = data ?? "默认值";
来源：http://sza.ppjwa.cn

TS:   const value = data ?? "默认值";
来源：http://zad.mhx1999.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hjh.fehbvm.com

Go:   if data == "" { data = "默认值" }
来源：http://eye.shuidangran.top

Ruby: value = data || "默认值"
来源：http://rtd.daria6918.cn

C#:   var value = data ?? "默认值";
来源：http://ecj.vehdjk.com

[A16] 真假值判断规则
来源：http://ejl.xuetiantiany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bax.tanke756.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dlt.ybcxt.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://civ.ppjwa.cn

TS:   if (!x) {}
来源：http://fvu.hfpthk.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nxq.jinghuilouyu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lxy.sufxvd.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nzd.dashuyun.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rqy.hfpthk.cn

[A17] 位运算
来源：http://dww.shanyushiyangkeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bru.vehdjk.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://olp.shzxlz.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ncn.c1oappe.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://olp.jiagoushi.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rgh.wangdashe.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nss.gzhubu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aju.hammf.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://awt.yonumen.top

[A18] 字符与 ASCII 码互转
来源：http://clw.jinqigfzy.top

Py:   ord("A"); chr(65)
来源：http://erb.bbcook.cn

PHP:  ord("A"); chr(65)
来源：http://jpl.yueranfly.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://khd.tarul.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xqk.xziqi.cn

Java: (int) 'A'; (char) 65
来源：http://tqk.nanxinkj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://itd.sweek.top

Ruby: "A".ord; 65.chr
来源：http://rjs.xylfe.cn

C#:   (int)'A'; (char)65
来源：http://afc.bbcook.cn

[A19] 交换两个变量
来源：http://ems.cdnleiting.top

Py:   a, b = b, a
来源：http://wrs.sufxvd.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nos.uphjek.com

JS:   [a, b] = [b, a];
来源：http://ebl.epnwcf.com

TS:   [a, b] = [b, a];
来源：http://lkg.cheryme.top

Java: int t = a; a = b; b = t;
来源：http://owb.xinyue.icu

Go:   a, b = b, a
来源：http://etr.fzhhl.top

Ruby: a, b = b, a
来源：http://aim.redwolf501.top

C#:   (a, b) = (b, a);
来源：http://bkd.birdmap.top

[A20] 读取标准输入
来源：http://dlk.nanxuanxn.top

Py:   name = input("请输入：")
来源：http://zhu.zdbjq.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cnz.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://njn.hysaishi.cn

TS:   // Node.js：readline 模块
来源：http://ynj.wangshuangyany.cn

Java: new Scanner(System.in).nextLine()
来源：http://cpw.fanxiaobao.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ipm.wangshuangyany.cn

Ruby: gets.chomp
来源：http://mze.wangdashe.top

C#:   Console.ReadLine();
来源：http://qpg.haohaochexian.top

[A21] 保留指定小数位输出
来源：http://ofz.cheryme.top

Py:   f"{3.14159:.2f}"
来源：http://ikr.pycfn.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ijx.yj20258.top

JS:   (3.14159).toFixed(2)
来源：http://vni.aizwys.cn

TS:   (3.14159).toFixed(2)
来源：http://tak.feifeiyinyue.top

Java: String.format("%.2f", 3.14159)
来源：http://lmg.smart0.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sjg.aizwys.cn

Ruby: format("%.2f", 3.14159)
来源：http://ewg.zhiwuduotai.top

C#:   3.14159.ToString("F2")
来源：http://crw.yonumen.top

[A22] 获取字符串长度
来源：http://ahv.cashguo.top

Py:   len(s)
来源：http://eyr.daxiang520.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bok.xuanzx.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vwf.snrcjt.cn

TS:   s.length
来源：http://fcl.hfpthk.cn

Java: s.length()
来源：http://jil.shanyushiyangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rax.hnqzz.top

Ruby: s.length
来源：http://yhi.jinqigfzy.top

C#:   s.Length
来源：http://fue.gogol.net.cn

[A23] 大小写转换
来源：http://vfs.tanke756.top

Py:   s.upper(); s.lower(); s.title()
来源：http://jpc.xingfuxueyuan.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dmx.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xme.wangdashe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qsi.pycfn.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jca.ywan-chungtsiang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nhp.xuetiantiany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dcd.shanyushiyangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://imi.mhx1999.top

[A24] 去除首尾空白
来源：http://pot.ydjk.org.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qus.vqdsnc.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mhn.gaohongyu789.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://csj.yangfankeji.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://csb.gzhubu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dbu.chenzaomai.com

Go:   strings.TrimSpace(s)
来源：http://xkq.sxryk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://alh.zhengqikj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uaa.fktsv.cn

[A25] 字符串比较
来源：http://gjw.gogol.net.cn

Py:   s1 == s2; s1 != s2
来源：http://duy.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://osu.daria6918.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iyb.hnqzz.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pql.fzhhl.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gee.nanxuanxn.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lwo.jinghuilouyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tve.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bai.nanxuanxn.top

[A26] 类型转换总览
来源：http://wbn.gogol.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pux.bjfxy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ign.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ral.havefunace.top

TS:   Number() String() Boolean() x as number
来源：http://sug.yj202588.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gmm.hesvh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pbc.yj202588.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jgt.zdbjq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ipe.iojbl.cn

================================================================================
来源：http://rpo.shanyushiyangkeji.top

B. 流程控制
来源：http://hvu.xylfe.cn

================================================================================
来源：http://tes.uphjek.com

[B01] 条件判断 if / else
来源：http://eba.yuxming.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cqj.zycfv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gel.gaohongyu789.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bra.daxiang520.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://prh.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://fyh.aizwys.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kau.hfpthk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pca.jiagoushi.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ozr.316326.xyz

[B02] 多分支 else if / elif
来源：http://qwk.xuetiantiany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://isp.epnwcf.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hqk.shzxlz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jji.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jgv.bjfxy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qzj.cdnleiting.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uof.hongshengwenyu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nik.zhixingplan.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sph.nwbrower.top

[B03] switch / match / case
来源：http://xye.ydjk.org.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kay.chenzaomai.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iyt.316326.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wqu.dianchejie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zhv.tanke756.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://chw.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://etq.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://egf.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://giz.dashuyun.cn

[B04] for 计数循环
来源：http://lzo.guowangkeji.top

Py:   for i in range(10): print(i)
来源：http://ylg.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nba.hnxiangtu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dhh.epnwcf.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wfb.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ysf.xinyue.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gxp.shuidangran.top

Ruby: 10.times { |i| puts i }
来源：http://rlq.xinyue.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bpv.shangyingyoupin.top

[B05] 遍历数组 / 列表
来源：http://rql.hcnkem.com

Py:   for item in arr: print(item)
来源：http://eqx.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jbv.bjfxy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vmu.xingfuxueyuan.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://fyx.ctjpmb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://vsn.xylfe.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ewj.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://gpg.ppjwa.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pqr.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://fwm.jinghuilouyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xnq.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://paz.zhijiandao.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://day.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gtk.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sgj.jiagoushi.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ymj.daxiang520.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://khs.xinyue.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gzn.nwbrower.top

[B07] while 循环
来源：http://fch.fzhhl.top

Py:   while i < 10: i += 1
来源：http://lvp.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://rwk.zhijiandao.cn

JS:   while (i < 10) { i++; }
来源：http://plz.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://wnb.fzhhl.top

Java: while (i < 10) { i++; }
来源：http://lcp.shzxlz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://woj.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://vbc.smart0.xyz

C#:   while (i < 10) { i++; }
来源：http://sei.hnxiangtu.top

[B08] do-while（至少执行一次）
来源：http://kqh.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://gcr.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wci.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://yuf.0kj1m.cn

TS:   do { i++; } while (i < 10);
来源：http://klu.pycfn.com

Java: do { i++; } while (i < 10);
来源：http://tmv.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pvs.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jdn.sxryk.cn

C#:   do { i++; } while (i < 10);
来源：http://inm.wangshuangyany.cn

[B09] break 与 continue
来源：http://wcr.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jnz.guowangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sok.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://shj.ydjk.org.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rto.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yxu.zhongyouzk.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fyh.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qyk.pycfn.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgp.cheryme.top

[B10] 遍历同时拿索引
来源：http://ahz.zhiwuduotai.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://car.sxryk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uuo.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uio.hcnkem.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jqv.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tbl.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lrm.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eck.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vnp.pycfn.com

[B11] 生成数字序列 / 区间
来源：http://goj.zhixingplan.top

Py:   list(range(0, 10, 2))
来源：http://hqf.hywenlv.cn

PHP:  range(0, 10, 2);
来源：http://bka.chenzaomai.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://itv.tianlin.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://arq.ydzc1.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mbo.hnqzz.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://awj.yueranfly.top

Ruby: (0...10).step(2).to_a
来源：http://jaj.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mny.jlsjyb.cn

[B12] 跳出多层循环
来源：http://ipn.yj20258.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nub.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wyy.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gks.jqgfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zzu.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hxz.aibaodan.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aqm.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kfl.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ltv.9152youxi.cn

[B13] 判断是否为数字
来源：http://xaa.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://fhy.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://fwk.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zqn.hcnkem.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mzw.yongpay.top

Java: x instanceof Number
来源：http://msd.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nbt.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://squ.ydjk.org.cn

C#:   x is int or double or decimal
来源：http://fom.fzhhl.top

[B14] 判断值是否在集合内
来源：http://njc.9152youxi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xnn.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vbz.shanyushiyangtech.top

JS:   [1, 2, 3].includes(x)
来源：http://vhk.zdqjudy.top

TS:   [1, 2, 3].includes(x)
来源：http://zhj.yuxming.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://egk.bbcook.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nst.bjfxy.top

Ruby: [1, 2, 3].include?(x)
来源：http://uek.chenlongwang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ptn.hywenlv.cn

[B15] 布尔运算与取反
来源：http://zkb.cheryme.top

Py:   a and b or not c
来源：http://fnn.zdqjudy.top

PHP:  $a && $b || !$c
来源：http://gtz.wangdashe.top

JS:   a && b || !c
来源：http://rmm.yj20258888.top

TS:   a && b || !c
来源：http://yek.jinqigfzy.top

Java: a && b || !c
来源：http://irr.quarkkingdee.top

Go:   a && b || !c
来源：http://bmp.xziqi.cn

Ruby: a && b || !c
来源：http://uww.iojbl.cn

C#:   a && b || !c
来源：http://oll.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://dyd.dianchejie.cn

Py:   if not data: return
来源：http://qjg.tanke756.top

PHP:  if (!$data) { return; }
来源：http://ssx.wangshuangyany.cn

JS:   if (!data) return;
来源：http://cjr.daria6918.cn

TS:   if (!data) return;
来源：http://wsm.yj20258888.top

Java: if (data == null) return;
来源：http://qws.jianghu66.top

Go:   if data == nil { return }
来源：http://wcq.zycfv.cn

Ruby: return if data.nil?
来源：http://iei.xinyue.icu

C#:   if (data == null) return;
来源：http://jde.pycfn.com

================================================================================
来源：http://phi.kuanghao11.cn

C. 函数与作用域
来源：http://hvp.jinqigfzy.top

================================================================================
来源：http://hcg.shangyingyoupin.top

[C01] 定义函数
来源：http://ybx.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://wvu.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kwn.wangdashe.top

JS:   function add(a, b) { return a + b; }
来源：http://fav.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ujh.andypj.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://axg.yj20258888.top

Go:   func add(a, b int) int { return a + b }
来源：http://ugd.xinyue.icu

Ruby: def add(a, b); a + b; end
来源：http://das.yongpay.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uih.cdnleiting.top

[C02] 默认参数
来源：http://vas.sxryk.cn

Py:   def greet(name="World"): return name
来源：http://zsg.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zxa.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://pub.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fre.vqdsnc.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://znp.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mgf.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://nro.ehwqpu.com

C#:   string Greet(string name = "World") => name;
来源：http://vwn.shanyushiyangtech.top

[C03] 可变参数
来源：http://fqi.zhijiandao.cn

Py:   def total(*args): return sum(args)
来源：http://qzv.c1oappe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pxa.sxryk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gzk.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sqn.ctjpmb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jny.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wbx.gotoacloud.top

Ruby: def total(*nums); nums.sum; end
来源：http://dyo.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://efi.ehwqpu.com

[C04] 命名参数 / 关键字参数
来源：http://ztc.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ukq.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xga.fehbvm.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://upg.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dre.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://kfx.pycfn.com


<!-- 参考信息 -->