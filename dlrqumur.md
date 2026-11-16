代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rpy.fktsv.cn

Ruby: "Hello, #{name}!"
来源：http://snb.zhixingplan.top

C#:   $"Hello, {name}!"
来源：http://jlf.hfpthk.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://iiz.fengsongda.top

Py:   "第一行\n第二行"
来源：http://fmw.jinqigfzy.top

PHP:  "第一行\n第二行"
来源：http://jiy.uphjek.com

JS:   "第一行\n第二行"
来源：http://irf.nanxinkj.top

TS:   "第一行\n第二行"
来源：http://xfo.fzhhl.top

Java: "第一行\n第二行"
来源：http://dbh.ctjpmb.com

Go:   "第一行\n第二行"
来源：http://vpt.tian-w.cn

Ruby: "第一行\n第二行"
来源：http://hck.hnxiangtu.top

C#:   "第一行\n第二行"
来源：http://big.52xcode.cn

[A14] 注释写法
来源：http://cgg.yanxiufei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gky.hysaishi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pgc.ivvv.top

JS:   // 单行；/* 多行 */
来源：http://oin.pengpengdd.cyou

TS:   // 单行；/* 多行 */
来源：http://xzm.zhengqikj.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cow.yj20258.top

Go:   // 单行；/* 多行 */
来源：http://wzo.9152youxi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lgu.zdbjq.cn

C#:   // 单行；/* 多行 */
来源：http://wps.epnwcf.com

[A15] 空值判断与默认值
来源：http://rpy.zhaomingkeji.xyz

Py:   value = data or "默认值"
来源：http://fxl.shangyingyoupin.top

PHP:  $value = $data ?? "默认值";
来源：http://azy.cashguo.top

JS:   const value = data ?? "默认值";
来源：http://tgz.sysykeji.top

TS:   const value = data ?? "默认值";
来源：http://pxf.bbcook.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yju.vehdjk.com

Go:   if data == "" { data = "默认值" }
来源：http://xzs.jinyuanbaomall.cn

Ruby: value = data || "默认值"
来源：http://gie.ctjpmb.com

C#:   var value = data ?? "默认值";
来源：http://jlu.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://ldp.jinqigufen.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zdc.9152youxi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gcx.xylfe.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ddh.gaohongyu789.top

TS:   if (!x) {}
来源：http://scm.yj20258.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ggq.yj20258.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lxf.xuetiantiany.cn

Ruby: unless x            # nil 与 false 为假
来源：http://goj.yvedp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://acc.jinqigfzy.top

[A17] 位运算
来源：http://cdg.sweek.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gpw.shanyushiyangtech.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tjc.yanxiufei.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pzl.jqgufenzy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pvm.vqdsnc.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yvv.zhijiandao.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nmq.fzhhl.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lav.epnwcf.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kbm.yfazqb.com

[A18] 字符与 ASCII 码互转
来源：http://cdp.c1oappe.top

Py:   ord("A"); chr(65)
来源：http://daw.ctjpmb.com

PHP:  ord("A"); chr(65)
来源：http://vaq.316326.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yzl.pycfn.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fyo.sufxvd.cn

Java: (int) 'A'; (char) 65
来源：http://ppx.hfpthk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://keh.feifeiyinyue.top

Ruby: "A".ord; 65.chr
来源：http://coi.pengpengdd.cyou

C#:   (int)'A'; (char)65
来源：http://ffm.guannengcc.top

[A19] 交换两个变量
来源：http://eee.hfpthk.cn

Py:   a, b = b, a
来源：http://tzh.jianghu66.top

PHP:  [$a, $b] = [$b, $a];
来源：http://tvl.daxiang520.top

JS:   [a, b] = [b, a];
来源：http://yeg.ppjwa.cn

TS:   [a, b] = [b, a];
来源：http://hon.sweek.top

Java: int t = a; a = b; b = t;
来源：http://czy.svipenyu.cn

Go:   a, b = b, a
来源：http://kjj.hongshengwenyu.top

Ruby: a, b = b, a
来源：http://lje.yvedp.cn

C#:   (a, b) = (b, a);
来源：http://ldp.gzhubu.top

[A20] 读取标准输入
来源：http://abq.jqgufenzy.top

Py:   name = input("请输入：")
来源：http://wrp.snrcjt.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vyb.hcnkem.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blw.sweek.top

TS:   // Node.js：readline 模块
来源：http://yyr.sxryk.cn

Java: new Scanner(System.in).nextLine()
来源：http://rwo.quarkkingdee.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nih.cashguo.top

Ruby: gets.chomp
来源：http://xig.fzhhl.top

C#:   Console.ReadLine();
来源：http://wis.hnxiangtu.top

[A21] 保留指定小数位输出
来源：http://zmu.uphjek.com

Py:   f"{3.14159:.2f}"
来源：http://dho.fzhhl.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jzp.yongpay.top

JS:   (3.14159).toFixed(2)
来源：http://omc.guannengcc.top

TS:   (3.14159).toFixed(2)
来源：http://lxd.gzhubu.top

Java: String.format("%.2f", 3.14159)
来源：http://tot.zdqjudy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xzt.tianlin.xyz

Ruby: format("%.2f", 3.14159)
来源：http://ddx.9152youxi.cn

C#:   3.14159.ToString("F2")
来源：http://mng.zdqjudy.top

[A22] 获取字符串长度
来源：http://asm.cucudq.cn

Py:   len(s)
来源：http://hkp.chenjidiqi.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ztx.jqgufenzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kmb.svipenyu.cn

TS:   s.length
来源：http://png.zhaomingkeji.xyz

Java: s.length()
来源：http://awv.hcnkem.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://udx.nanxinkj.top

Ruby: s.length
来源：http://utx.vehdjk.com

C#:   s.Length
来源：http://kbh.daria6918.cn

[A23] 大小写转换
来源：http://dwg.nanxinkj.top

Py:   s.upper(); s.lower(); s.title()
来源：http://rsq.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hwf.hcnkem.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hxx.vehdjk.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yhv.daxiang520.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xpq.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tiy.zhaomingkeji.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lnd.zhongyouzk.top

C#:   s.ToUpper(); s.ToLower()
来源：http://sww.fengsongda.top

[A24] 去除首尾空白
来源：http://qdp.aizwys.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sbe.ehwqpu.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://spm.yj20258888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://soz.jlsjyb.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kmb.nanxinkj.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wtt.uphjek.com

Go:   strings.TrimSpace(s)
来源：http://lvr.yangfankeji.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hsy.ywan-chungtsiang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tdx.zhaomingkeji.xyz

[A25] 字符串比较
来源：http://ihr.cheryme.top

Py:   s1 == s2; s1 != s2
来源：http://qfn.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cad.gogol.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hfb.sysykeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oxc.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tca.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pfc.gzhubu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://lgl.zdbjq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ooc.hnqzz.top

[A26] 类型转换总览
来源：http://xgs.zdbjq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gdw.gzhubu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://plx.zhiwuduotai.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jpq.svipenyu.cn

TS:   Number() String() Boolean() x as number
来源：http://vzz.xuanzx.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iep.nanxuanxn.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sxy.hammf.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bey.sufxvd.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hzx.cheryme.top

================================================================================
来源：http://crh.jlsjyb.cn

B. 流程控制
来源：http://gdm.ybcxt.top

================================================================================
来源：http://bpv.cucudq.cn

[B01] 条件判断 if / else
来源：http://cmj.shuidangran.top

Py:   result = "正" if x > 0 else "非正"
来源：http://txo.sjlbkw.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tfj.fktsv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://asi.cucudq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hpd.0kj1m.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ayl.yuxming.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://thl.fzhhl.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xmc.hongshengwenyu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zds.jinghuilouyu.cn

[B02] 多分支 else if / elif
来源：http://dyz.xziqi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lgq.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://odw.zhijiandao.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pcz.jinqigfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zvq.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fcq.tianlin.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kwm.hcnkem.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fup.ywan-chungtsiang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ghe.sweek.top

[B03] switch / match / case
来源：http://itq.gzhubu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wwb.sjlbkw.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xxd.nwbrower.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lpo.xuetiantiany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lxd.cheryme.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zup.ehwqpu.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iea.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://usu.guannengcc.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://edm.shzxlz.cn

[B04] for 计数循环
来源：http://lhs.bjfxy.top

Py:   for i in range(10): print(i)
来源：http://rlf.cashguo.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pjp.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gan.shzxlz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aoy.xuanzx.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tai.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kzs.uphjek.com

Ruby: 10.times { |i| puts i }
来源：http://fuj.feifeiyinyue.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ntw.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://epy.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://ivb.hysaishi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vgr.shangyingyoupin.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cks.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ynb.chenzaomai.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://wrz.fktsv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ypg.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://bjz.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ekw.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://qgp.vqdsnc.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cuj.ydjk.org.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://izo.yongpay.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://acm.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oqb.xinyue.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oev.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ssk.shanyushiyangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mvv.shzxlz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fcs.hcnkem.com

[B07] while 循环
来源：http://efn.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://bdg.uphjek.com

PHP:  while ($i < 10) { $i++; }
来源：http://fqy.ydzc1.top

JS:   while (i < 10) { i++; }
来源：http://lew.jqgfzy.top

TS:   while (i < 10) { i++; }
来源：http://nlq.zhixingplan.top

Java: while (i < 10) { i++; }
来源：http://qyu.ehwqpu.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pke.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://lcp.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://xta.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://yzv.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://vsw.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zdy.aizwys.cn

JS:   do { i++; } while (i < 10);
来源：http://bkt.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://czs.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://gom.yvedp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zyg.tanke756.top

Ruby: begin; i += 1; end while i < 10
来源：http://iws.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://fen.0kj1m.cn

[B09] break 与 continue
来源：http://gme.feifeiyinyue.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cfg.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dxb.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bov.dashuyun.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gby.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbi.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ial.hesvh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fjy.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vlr.cheryme.top

[B10] 遍历同时拿索引
来源：http://zih.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fmg.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vii.yuxming.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bgj.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uws.xingfuxueyuan.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qnf.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aqd.yj202588.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mul.xuanzx.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fdd.yuxming.cn

[B11] 生成数字序列 / 区间
来源：http://jyd.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://djx.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://pxx.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dua.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zgz.cucudq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yqo.quarkkingdee.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jyu.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://nlo.mhx1999.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qnc.jqgufenzy.top

[B12] 跳出多层循环
来源：http://jhf.cheryme.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ouh.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://idu.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vnq.fengsongda.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aqo.gzhubu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tta.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sky.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://udz.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://syk.xuetiantiany.cn

[B13] 判断是否为数字
来源：http://xqm.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://gri.yuanzhike.top

PHP:  is_numeric($x)
来源：http://wxb.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pqh.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nqc.yj20258888.top

Java: x instanceof Number
来源：http://rry.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ybl.shanyushiyangtech.top

Ruby: x.is_a?(Numeric)
来源：http://khn.ppjwa.cn

C#:   x is int or double or decimal
来源：http://zlu.iojbl.cn

[B14] 判断值是否在集合内
来源：http://kgy.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bwu.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ons.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://hoe.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://zan.jlsjyb.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nvz.redwolf501.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wah.kuanghao11.cn

Ruby: [1, 2, 3].include?(x)
来源：http://him.zdbjq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fkr.jinqigufen.top

[B15] 布尔运算与取反
来源：http://ugb.guowangkeji.top

Py:   a and b or not c
来源：http://psq.cdnleiting.top

PHP:  $a && $b || !$c
来源：http://fei.gzhubu.top

JS:   a && b || !c
来源：http://tcs.gogol.net.cn

TS:   a && b || !c
来源：http://uzo.yongpay.top

Java: a && b || !c
来源：http://nhp.epnwcf.com

Go:   a && b || !c
来源：http://tgr.hywenlv.cn

Ruby: a && b || !c
来源：http://tbo.cdnleiting.top

C#:   a && b || !c
来源：http://ydk.jinqigfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://nvk.hywenlv.cn

Py:   if not data: return
来源：http://hnu.snrcjt.cn

PHP:  if (!$data) { return; }
来源：http://bpa.yj20258888.top

JS:   if (!data) return;
来源：http://pqv.hammf.cn

TS:   if (!data) return;
来源：http://omj.jiagoushi.top

Java: if (data == null) return;
来源：http://ang.yvedp.cn

Go:   if data == nil { return }
来源：http://vjj.xylfe.cn

Ruby: return if data.nil?
来源：http://qal.xinyue.icu

C#:   if (data == null) return;
来源：http://rhj.ctjpmb.com

================================================================================
来源：http://utm.zhijiandao.cn

C. 函数与作用域
来源：http://lkt.gogol.net.cn

================================================================================
来源：http://rbi.smart0.xyz

[C01] 定义函数
来源：http://kpw.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://esx.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bbz.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://gan.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://els.zhongyouzk.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zpy.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://itd.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://job.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qmc.xylfe.cn

[C02] 默认参数
来源：http://orf.chenlongwang.top

Py:   def greet(name="World"): return name
来源：http://goc.sjlbkw.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xmf.cashguo.top

JS:   function greet(name = "World") { return name; }
来源：http://wcg.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fum.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://syh.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xea.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://zjr.ehwqpu.com

C#:   string Greet(string name = "World") => name;
来源：http://gxw.pycfn.com

[C03] 可变参数
来源：http://rhs.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://jgv.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://avj.jianghu66.top


<!-- 参考信息 -->