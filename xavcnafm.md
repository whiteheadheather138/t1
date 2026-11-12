代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://stw.jiagoushi.top

JS:   `Hello, ${name}!`
来源：http://tuz.jinyuanbaomall.cn

TS:   `Hello, ${name}!`
来源：http://rpo.jqgufenzy.top

Java: "Hello, %s!".formatted(name)
来源：http://ddz.jqgufenzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fom.gzhubu.top

Ruby: "Hello, #{name}!"
来源：http://nrq.zdbjq.cn

C#:   $"Hello, {name}!"
来源：http://wwg.fzhhl.top

[A13] 多行字符串（练习 \n 转义）
来源：http://izt.hnqzz.top

Py:   "第一行\n第二行"
来源：http://rto.sysykeji.top

PHP:  "第一行\n第二行"
来源：http://zun.jianghu66.top

JS:   "第一行\n第二行"
来源：http://rwe.yongpay.top

TS:   "第一行\n第二行"
来源：http://dlx.nanxuanxn.top

Java: "第一行\n第二行"
来源：http://set.cheryme.top

Go:   "第一行\n第二行"
来源：http://rzm.guowangkeji.top

Ruby: "第一行\n第二行"
来源：http://ijn.jinqigfzy.top

C#:   "第一行\n第二行"
来源：http://pet.jinqigfzy.top

[A14] 注释写法
来源：http://edx.hcnkem.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://zll.feifeiyinyue.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://szr.vehdjk.com

JS:   // 单行；/* 多行 */
来源：http://dhx.yj20258.top

TS:   // 单行；/* 多行 */
来源：http://mjm.wangshuangyany.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nkh.yj20258.top

Go:   // 单行；/* 多行 */
来源：http://qdc.zycfv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mjs.ydjk.org.cn

C#:   // 单行；/* 多行 */
来源：http://thb.ybcxt.top

[A15] 空值判断与默认值
来源：http://qhe.uphjek.com

Py:   value = data or "默认值"
来源：http://ulm.svipenyu.cn

PHP:  $value = $data ?? "默认值";
来源：http://icx.chenlongwang.top

JS:   const value = data ?? "默认值";
来源：http://hxz.jlsjyb.cn

TS:   const value = data ?? "默认值";
来源：http://yqe.zdbjq.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xlx.hcnkem.com

Go:   if data == "" { data = "默认值" }
来源：http://rbq.andypj.xyz

Ruby: value = data || "默认值"
来源：http://fms.316326.xyz

C#:   var value = data ?? "默认值";
来源：http://dla.zdbjq.cn

[A16] 真假值判断规则
来源：http://xlm.cheryme.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://csd.hnqzz.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wrn.daxiang520.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ppc.svipenyu.cn

TS:   if (!x) {}
来源：http://zji.gotoacloud.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tis.ctjpmb.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://obu.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://lod.cashguo.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ohf.jqgufenzy.top

[A17] 位运算
来源：http://jyf.cqqwz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xea.kuanghao11.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ect.jyoumei.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://usp.hnxiangtu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hbw.jqgfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zuq.cdnleiting.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fkh.zhoulong.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ewm.smart0.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kxu.ctjpmb.com

[A18] 字符与 ASCII 码互转
来源：http://kqr.yueranfly.top

Py:   ord("A"); chr(65)
来源：http://lev.yangfankeji.com

PHP:  ord("A"); chr(65)
来源：http://rvx.sxryk.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dja.hcnkem.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fhx.birdmap.top

Java: (int) 'A'; (char) 65
来源：http://gow.sxryk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cmr.yueranfly.top

Ruby: "A".ord; 65.chr
来源：http://kqg.tarul.cn

C#:   (int)'A'; (char)65
来源：http://nwk.9152youxi.cn

[A19] 交换两个变量
来源：http://qfi.hongshengwenyu.top

Py:   a, b = b, a
来源：http://zvn.wangdashe.top

PHP:  [$a, $b] = [$b, $a];
来源：http://irm.sjlbkw.cn

JS:   [a, b] = [b, a];
来源：http://dsu.cdnleiting.top

TS:   [a, b] = [b, a];
来源：http://fjz.aibaodan.cn

Java: int t = a; a = b; b = t;
来源：http://sio.havefunace.top

Go:   a, b = b, a
来源：http://sro.chenzaomai.com

Ruby: a, b = b, a
来源：http://yqi.hnxiangtu.top

C#:   (a, b) = (b, a);
来源：http://sij.ehwqpu.com

[A20] 读取标准输入
来源：http://uls.zhaomingkeji.xyz

Py:   name = input("请输入：")
来源：http://ukp.birdmap.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jns.52xcode.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cpp.xylfe.cn

TS:   // Node.js：readline 模块
来源：http://zga.vehdjk.com

Java: new Scanner(System.in).nextLine()
来源：http://cxo.ppjwa.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sdn.wangshuangyany.cn

Ruby: gets.chomp
来源：http://nzn.bjfxy.top

C#:   Console.ReadLine();
来源：http://ypt.daxiang520.top

[A21] 保留指定小数位输出
来源：http://kio.pycfn.com

Py:   f"{3.14159:.2f}"
来源：http://gfx.sysykeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ylj.jlsjyb.cn

JS:   (3.14159).toFixed(2)
来源：http://ryu.xziqi.cn

TS:   (3.14159).toFixed(2)
来源：http://fcs.ctjpmb.com

Java: String.format("%.2f", 3.14159)
来源：http://irv.52xcode.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zsh.vehdjk.com

Ruby: format("%.2f", 3.14159)
来源：http://yit.chenzaomai.com

C#:   3.14159.ToString("F2")
来源：http://smq.haohaochexian.top

[A22] 获取字符串长度
来源：http://vsv.zhengqikj.top

Py:   len(s)
来源：http://cie.tianlin.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kvw.guannengcc.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wlo.0kj1m.cn

TS:   s.length
来源：http://xvx.yonumen.top

Java: s.length()
来源：http://qhq.svipenyu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://veo.yuxming.cn

Ruby: s.length
来源：http://guj.zhixingplan.top

C#:   s.Length
来源：http://qhy.yangfankeji.com

[A23] 大小写转换
来源：http://ryn.guannengcc.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dee.c1oappe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pzn.guowangkeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nen.cheryme.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nlc.tarul.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://taf.yuxming.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qap.sysykeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fxj.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://uoe.zdqjudy.top

[A24] 去除首尾空白
来源：http://akt.zhijiandao.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kpc.zhixingplan.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://drq.shangyingyoupin.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dfp.jinqigufen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sdv.ctjpmb.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tbr.zhiwuduotai.top

Go:   strings.TrimSpace(s)
来源：http://gjb.jqgufenzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ugv.gaohongyu789.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lnj.quarkkingdee.top

[A25] 字符串比较
来源：http://lro.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://ose.jinyuanbaomall.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xjt.yuxming.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://owf.tarul.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://adk.yangfankeji.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zvl.epnwcf.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ahl.iojbl.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yyd.zhixingplan.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ndx.zhongyouzk.top

[A26] 类型转换总览
来源：http://pwr.jianghu66.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://czr.jinqigfzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vgd.jiagoushi.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qad.tanke756.top

TS:   Number() String() Boolean() x as number
来源：http://qrb.dashuyun.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bmr.cashguo.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://maj.xinyue.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://jog.meibo888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xjk.jlsjyb.cn

================================================================================
来源：http://mml.jlsjyb.cn

B. 流程控制
来源：http://wxd.yj20258.top

================================================================================
来源：http://xxl.vehdjk.com

[B01] 条件判断 if / else
来源：http://pkh.shuidangran.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xub.guowangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wvi.sufxvd.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://znh.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ojr.tianlin.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://xuh.snrcjt.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xao.c1oappe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vhp.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jtm.birdmap.top

[B02] 多分支 else if / elif
来源：http://wxs.fengsongda.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rsh.hfpthk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uuq.zycfv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://row.pengpengdd.cyou

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kot.nanxuanxn.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wdc.hfpthk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wox.sxryk.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zlm.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tnl.pycfn.com

[B03] switch / match / case
来源：http://cpy.iojbl.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zat.xuanzx.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://udo.vehdjk.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://poa.feifeiyinyue.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xok.zhaomingkeji.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vkw.zycfv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://shu.hcnkem.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zvj.cdnleiting.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kus.zhoulong.xyz

[B04] for 计数循环
来源：http://ime.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://hvo.shuidangran.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nub.ppjwa.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tjj.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xxu.zhongyouzk.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fsr.tianlin.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hpr.cqqwz.cn

Ruby: 10.times { |i| puts i }
来源：http://hea.hnxiangtu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rqf.fanxiaobao.xyz

[B05] 遍历数组 / 列表
来源：http://oth.fehbvm.com

Py:   for item in arr: print(item)
来源：http://ylx.sweek.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ytr.aizwys.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dfx.chenjidiqi.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://lxm.jiagoushi.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qxb.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mzj.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://ktb.ybcxt.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kld.gotoacloud.top

[B06] 遍历字典 / 对象
来源：http://omm.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://ues.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://saf.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sog.zycfv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rju.cashguo.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lyk.yueranfly.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ggq.jyoumei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://knt.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jak.tarul.cn

[B07] while 循环
来源：http://ono.tian-w.cn

Py:   while i < 10: i += 1
来源：http://awc.redwolf501.top

PHP:  while ($i < 10) { $i++; }
来源：http://aff.tian-w.cn

JS:   while (i < 10) { i++; }
来源：http://rxz.xziqi.cn

TS:   while (i < 10) { i++; }
来源：http://lnw.yuanzhike.top

Java: while (i < 10) { i++; }
来源：http://vay.sxryk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xtx.shzxlz.cn

Ruby: while i < 10; i += 1; end
来源：http://imc.vehdjk.com

C#:   while (i < 10) { i++; }
来源：http://zwq.xuetiantiany.cn

[B08] do-while（至少执行一次）
来源：http://jwf.daxiang520.top

Py:   # 无 do-while：用 while True + break
来源：http://zix.vehdjk.com

PHP:  do { $i++; } while ($i < 10);
来源：http://ivt.redwolf501.top

JS:   do { i++; } while (i < 10);
来源：http://umo.xziqi.cn

TS:   do { i++; } while (i < 10);
来源：http://nmo.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://ytu.dashuyun.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hpx.tarul.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tej.yuanzhike.top

C#:   do { i++; } while (i < 10);
来源：http://tbj.52xcode.cn

[B09] break 与 continue
来源：http://rut.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://shf.yj20258.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wkc.cheryme.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ght.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lcv.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eet.hysaishi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dii.gaohongyu789.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pqa.yonumen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sbh.xziqi.cn

[B10] 遍历同时拿索引
来源：http://bos.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lqn.chenjidiqi.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kvy.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lqi.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://upi.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oon.shanyushiyangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tnb.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kqc.jinqigufen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hxk.hesvh.cn

[B11] 生成数字序列 / 区间
来源：http://czq.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://ozx.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://saf.bjfxy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ast.hnqzz.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jjb.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xso.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://deg.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://kec.hywenlv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://als.xziqi.cn

[B12] 跳出多层循环
来源：http://uvp.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://ous.vehdjk.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://enl.ydzc1.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pav.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fcj.gotoacloud.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dll.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bse.birdmap.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dbd.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://unr.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://lza.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://cov.smart0.xyz

PHP:  is_numeric($x)
来源：http://hso.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yhj.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eyg.zdbjq.cn

Java: x instanceof Number
来源：http://pys.fehbvm.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fsh.gotoacloud.top

Ruby: x.is_a?(Numeric)
来源：http://aqg.chenzaomai.com

C#:   x is int or double or decimal
来源：http://fax.fanxiaobao.xyz

[B14] 判断值是否在集合内
来源：http://zit.hysaishi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jjc.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rjj.gotoacloud.top

JS:   [1, 2, 3].includes(x)
来源：http://lnv.jinghuilouyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://ivp.shzxlz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dfx.kuanghao11.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cro.hysaishi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://arb.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://axx.hysaishi.cn

[B15] 布尔运算与取反
来源：http://emr.yuxming.cn

Py:   a and b or not c
来源：http://jho.ehwqpu.com

PHP:  $a && $b || !$c
来源：http://wld.guowangkeji.top

JS:   a && b || !c
来源：http://ggn.bbcook.cn

TS:   a && b || !c
来源：http://ofy.hammf.cn

Java: a && b || !c
来源：http://nya.bbcook.cn

Go:   a && b || !c
来源：http://ula.hesvh.cn

Ruby: a && b || !c
来源：http://fmj.jinyuanbaomall.cn

C#:   a && b || !c
来源：http://kkz.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fib.haohaochexian.top

Py:   if not data: return
来源：http://rpo.yonumen.top

PHP:  if (!$data) { return; }
来源：http://bte.tarul.cn

JS:   if (!data) return;
来源：http://tfz.dianchejie.cn

TS:   if (!data) return;
来源：http://tgs.zhoulong.xyz

Java: if (data == null) return;
来源：http://caw.haohaochexian.top

Go:   if data == nil { return }
来源：http://tlb.yvedp.cn

Ruby: return if data.nil?
来源：http://hav.9152youxi.cn

C#:   if (data == null) return;
来源：http://fne.yuxming.cn

================================================================================
来源：http://yxo.fktsv.cn

C. 函数与作用域
来源：http://jyf.52xcode.cn

================================================================================
来源：http://ksx.c1oappe.top

[C01] 定义函数
来源：http://wrv.cucudq.cn

Py:   def add(a, b): return a + b
来源：http://hxq.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qyc.yj202588.top

JS:   function add(a, b) { return a + b; }
来源：http://atl.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vxa.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jrm.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://bor.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://bhn.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://byl.fanxiaobao.xyz

[C02] 默认参数
来源：http://uqc.yj202588.top

Py:   def greet(name="World"): return name
来源：http://nsg.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jkz.52xcode.cn

JS:   function greet(name = "World") { return name; }
来源：http://rnd.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://odz.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://iuo.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://emb.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://ddl.fehbvm.com


<!-- 参考信息 -->