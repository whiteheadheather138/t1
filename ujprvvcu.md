代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://syy.pengpengdd.cyou

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yim.gzhubu.top

Go:   // 单行；/* 多行 */
来源：http://laf.shanyushiyangtech.top

Ruby: # 单行；=begin 多行 =end
来源：http://rtl.bjfxy.top

C#:   // 单行；/* 多行 */
来源：http://pcr.snrcjt.cn

[A15] 空值判断与默认值
来源：http://afi.tian-w.cn

Py:   value = data or "默认值"
来源：http://mrm.daria6918.cn

PHP:  $value = $data ?? "默认值";
来源：http://fqt.fzhhl.top

JS:   const value = data ?? "默认值";
来源：http://qsy.cheryme.top

TS:   const value = data ?? "默认值";
来源：http://jyf.sxryk.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tps.zhengqikj.top

Go:   if data == "" { data = "默认值" }
来源：http://zsb.pycfn.com

Ruby: value = data || "默认值"
来源：http://jvq.tanke756.top

C#:   var value = data ?? "默认值";
来源：http://euc.hammf.cn

[A16] 真假值判断规则
来源：http://egb.hnqzz.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://roq.yvedp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dhk.hesvh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cgt.ydzc1.top

TS:   if (!x) {}
来源：http://fyu.chenzaomai.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lhq.hysaishi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cna.yvedp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uds.guowangkeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mkx.xinyue.icu

[A17] 位运算
来源：http://drx.bbcook.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dmx.epnwcf.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://inv.ydjk.org.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cic.zhaomingkeji.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rsf.ctjpmb.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://egr.hcnkem.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jnp.hfpthk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pfe.jiagoushi.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rbr.pengpengdd.cyou

[A18] 字符与 ASCII 码互转
来源：http://lak.yj202588.top

Py:   ord("A"); chr(65)
来源：http://hez.ywan-chungtsiang.top

PHP:  ord("A"); chr(65)
来源：http://svf.yuanzhike.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dlx.hongshengwenyu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rhy.xziqi.cn

Java: (int) 'A'; (char) 65
来源：http://nyu.jyoumei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vdt.hesvh.cn

Ruby: "A".ord; 65.chr
来源：http://qsq.zhiwuduotai.top

C#:   (int)'A'; (char)65
来源：http://jay.smart0.xyz

[A19] 交换两个变量
来源：http://dom.ppjwa.cn

Py:   a, b = b, a
来源：http://vsp.jianghu66.top

PHP:  [$a, $b] = [$b, $a];
来源：http://wim.epnwcf.com

JS:   [a, b] = [b, a];
来源：http://plg.jqgufenzy.top

TS:   [a, b] = [b, a];
来源：http://tbq.cqqwz.cn

Java: int t = a; a = b; b = t;
来源：http://ity.havefunace.top

Go:   a, b = b, a
来源：http://elq.wangshuangyany.cn

Ruby: a, b = b, a
来源：http://dif.dianchejie.cn

C#:   (a, b) = (b, a);
来源：http://qvk.ybcxt.top

[A20] 读取标准输入
来源：http://acm.aizwys.cn

Py:   name = input("请输入：")
来源：http://bcu.wangdashe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ael.daxiang520.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cbh.vehdjk.com

TS:   // Node.js：readline 模块
来源：http://slx.smart0.xyz

Java: new Scanner(System.in).nextLine()
来源：http://ifr.xuetiantiany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://acz.zdqjudy.top

Ruby: gets.chomp
来源：http://phl.yanxiufei.cn

C#:   Console.ReadLine();
来源：http://cqw.fzhhl.top

[A21] 保留指定小数位输出
来源：http://osm.yonumen.top

Py:   f"{3.14159:.2f}"
来源：http://zvv.yuxming.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fzz.ivvv.top

JS:   (3.14159).toFixed(2)
来源：http://kjv.cdnleiting.top

TS:   (3.14159).toFixed(2)
来源：http://ity.aizwys.cn

Java: String.format("%.2f", 3.14159)
来源：http://kjf.shuidangran.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fmp.pengpengdd.cyou

Ruby: format("%.2f", 3.14159)
来源：http://rro.uphjek.com

C#:   3.14159.ToString("F2")
来源：http://xth.shanyushiyangkeji.top

[A22] 获取字符串长度
来源：http://hbu.shzxlz.cn

Py:   len(s)
来源：http://zae.shanyushiyangtech.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bxr.yfazqb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pfz.0kj1m.cn

TS:   s.length
来源：http://zay.yvedp.cn

Java: s.length()
来源：http://tgy.jlsjyb.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ygc.guannengcc.top

Ruby: s.length
来源：http://vgw.tianlin.xyz

C#:   s.Length
来源：http://azz.yj20258888.top

[A23] 大小写转换
来源：http://dpv.zdqjudy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kwn.zycfv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pso.vehdjk.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pgw.fktsv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://atj.0kj1m.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://prr.fengsongda.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://txj.hysaishi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ied.kuanghao11.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gpe.yj20258.top

[A24] 去除首尾空白
来源：http://oub.smart0.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jqs.daxiang520.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rqr.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gjy.vehdjk.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oza.wangdashe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lqb.ppjwa.cn

Go:   strings.TrimSpace(s)
来源：http://qth.iojbl.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bve.ctjpmb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fer.aibaodan.cn

[A25] 字符串比较
来源：http://wwg.yvedp.cn

Py:   s1 == s2; s1 != s2
来源：http://apg.gotoacloud.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uuc.quarkkingdee.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://htr.jyoumei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://msa.vqdsnc.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uuk.hfpthk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wum.ehwqpu.com

Ruby: s1 == s2; s1 <=> s2
来源：http://teu.chenlongwang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xys.yvedp.cn

[A26] 类型转换总览
来源：http://zhr.chenzaomai.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ete.shzxlz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jsx.zycfv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gfa.yangfankeji.com

TS:   Number() String() Boolean() x as number
来源：http://ggo.shuidangran.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bmr.meibo888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wrm.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rmd.aibaodan.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dzd.shangyingyoupin.top

================================================================================
来源：http://cwk.yuanzhike.top

B. 流程控制
来源：http://kfs.yuxming.cn

================================================================================
来源：http://pxd.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://bwk.fktsv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jhu.fehbvm.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tkd.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bhd.yuxming.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gxq.sjlbkw.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fua.bbcook.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://stb.tianlin.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kha.cqqwz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vxs.zdqjudy.top

[B02] 多分支 else if / elif
来源：http://tnn.jinqigufen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yvr.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gwp.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kty.yfazqb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zhh.sysykeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ecc.xingfuxueyuan.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hgc.zhixingplan.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kco.aibaodan.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lbl.jinyuanbaomall.cn

[B03] switch / match / case
来源：http://iyq.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xhf.jqgfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gay.sweek.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sgg.xinyue.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uhu.meibo888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nrh.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ynw.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://svd.jinqigfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lcp.iojbl.cn

[B04] for 计数循环
来源：http://gek.sxryk.cn

Py:   for i in range(10): print(i)
来源：http://odk.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qgl.hesvh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fyr.cqqwz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kmx.xingfuxueyuan.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eqf.hammf.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tvw.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://xao.jinghuilouyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yhh.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://hwl.guannengcc.top

Py:   for item in arr: print(item)
来源：http://zah.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nyd.shzxlz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hom.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://nkv.zhengqikj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kac.jiagoushi.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://byx.hysaishi.cn

Ruby: arr.each { |item| puts item }
来源：http://kpz.gaohongyu789.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pxw.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://axd.shangyingyoupin.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jrh.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ilm.shanyushiyangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jng.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hpj.52xcode.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jvg.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yuu.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iwc.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gqv.chenzaomai.com

[B07] while 循环
来源：http://ike.yueranfly.top

Py:   while i < 10: i += 1
来源：http://knf.yvedp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://atw.jiagoushi.top

JS:   while (i < 10) { i++; }
来源：http://ulf.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://pct.ydjk.org.cn

Java: while (i < 10) { i++; }
来源：http://pjw.cdnleiting.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ljs.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://ygj.zycfv.cn

C#:   while (i < 10) { i++; }
来源：http://qtb.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://xuf.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://stq.xylfe.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jvm.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://xee.yj202588.top

TS:   do { i++; } while (i < 10);
来源：http://skz.snrcjt.cn

Java: do { i++; } while (i < 10);
来源：http://klj.svipenyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://npk.ydzc1.top

Ruby: begin; i += 1; end while i < 10
来源：http://rxu.chenzaomai.com

C#:   do { i++; } while (i < 10);
来源：http://zpy.zhengqikj.top

[B09] break 与 continue
来源：http://fje.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fjt.ctjpmb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hzg.hesvh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xib.hysaishi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ayt.jinghuilouyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://itx.wangshuangyany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kes.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hpg.jqgfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pcs.tarul.cn

[B10] 遍历同时拿索引
来源：http://yri.cheryme.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rhb.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wmm.jyoumei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hal.jinghuilouyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://skn.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xya.yfazqb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yhw.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nvt.yangfankeji.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sgg.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://alf.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://cau.pycfn.com

PHP:  range(0, 10, 2);
来源：http://pcl.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://spu.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nug.zhoulong.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cvk.yuxming.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lxc.hcnkem.com

Ruby: (0...10).step(2).to_a
来源：http://hbu.gogol.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dyp.hnqzz.top

[B12] 跳出多层循环
来源：http://hsh.chenzaomai.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://xor.aizwys.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kok.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kau.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sfv.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://msc.yonumen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://azc.sufxvd.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mnc.jyoumei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hat.fzhhl.top

[B13] 判断是否为数字
来源：http://sbq.c1oappe.top

Py:   isinstance(x, (int, float))
来源：http://dzs.cdnleiting.top

PHP:  is_numeric($x)
来源：http://ydz.zhijiandao.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mou.ehwqpu.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xon.gaohongyu789.top

Java: x instanceof Number
来源：http://gue.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jiv.cheryme.top

Ruby: x.is_a?(Numeric)
来源：http://wqb.aizwys.cn

C#:   x is int or double or decimal
来源：http://vwp.zhiwuduotai.top

[B14] 判断值是否在集合内
来源：http://lwi.tianlin.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://biy.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xbu.hywenlv.cn

JS:   [1, 2, 3].includes(x)
来源：http://emh.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://rne.zhijiandao.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ogk.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bsu.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://hpb.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nxf.epnwcf.com

[B15] 布尔运算与取反
来源：http://bfn.yonumen.top

Py:   a and b or not c
来源：http://pes.fengsongda.top

PHP:  $a && $b || !$c
来源：http://qom.wangdashe.top

JS:   a && b || !c
来源：http://gxc.hywenlv.cn

TS:   a && b || !c
来源：http://mbs.jqgufenzy.top

Java: a && b || !c
来源：http://dgu.cdnleiting.top

Go:   a && b || !c
来源：http://oxb.zhijiandao.cn

Ruby: a && b || !c
来源：http://gqn.yuanzhike.top

C#:   a && b || !c
来源：http://ant.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://wtn.xuetiantiany.cn

Py:   if not data: return
来源：http://owu.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://yqr.zhongyouzk.top

JS:   if (!data) return;
来源：http://vog.zhixingplan.top

TS:   if (!data) return;
来源：http://gam.aizwys.cn

Java: if (data == null) return;
来源：http://rnz.hysaishi.cn

Go:   if data == nil { return }
来源：http://den.hywenlv.cn

Ruby: return if data.nil?
来源：http://khi.316326.xyz

C#:   if (data == null) return;
来源：http://kcg.aibaodan.cn

================================================================================
来源：http://nip.sxryk.cn

C. 函数与作用域
来源：http://ykf.aizwys.cn

================================================================================
来源：http://vbe.cdnleiting.top

[C01] 定义函数
来源：http://lqm.hysaishi.cn

Py:   def add(a, b): return a + b
来源：http://xfa.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nft.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://ljv.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kll.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://owe.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://olr.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://uon.dashuyun.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lnj.chenlongwang.top

[C02] 默认参数
来源：http://foh.yongpay.top

Py:   def greet(name="World"): return name
来源：http://lmh.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://njc.jqgufenzy.top

JS:   function greet(name = "World") { return name; }
来源：http://nbh.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ufd.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://oph.jyoumei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cpu.guannengcc.top

Ruby: def greet(name = "World") = name
来源：http://ctz.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://ptz.tarul.cn

[C03] 可变参数
来源：http://wex.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://bag.jyoumei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tra.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fkp.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ipl.fengsongda.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vnl.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fcf.cqqwz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xgm.ppjwa.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iym.jlsjyb.cn

[C04] 命名参数 / 关键字参数
来源：http://sqb.guannengcc.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ahl.cheryme.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vlw.jianghu66.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pre.bbcook.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ozd.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://zur.uphjek.com

Go:   // 无：用配置结构体参数
来源：http://vat.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://cgo.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://jgo.sxryk.cn

[C05] 返回多个值
来源：http://ort.havefunace.top


<!-- 参考信息 -->