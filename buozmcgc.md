代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cqc.shanyushiyangkeji.top

JS:   `Hello, ${name}!`
来源：http://cld.zhijiandao.cn

TS:   `Hello, ${name}!`
来源：http://byo.ctjpmb.com

Java: "Hello, %s!".formatted(name)
来源：http://yqz.snrcjt.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://opo.nanxuanxn.top

Ruby: "Hello, #{name}!"
来源：http://npe.gotoacloud.top

C#:   $"Hello, {name}!"
来源：http://jko.yuxming.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://liz.tanke756.top

Py:   "第一行\n第二行"
来源：http://kpl.shuidangran.top

PHP:  "第一行\n第二行"
来源：http://npt.fzhhl.top

JS:   "第一行\n第二行"
来源：http://vgn.gzhubu.top

TS:   "第一行\n第二行"
来源：http://mam.ydjk.org.cn

Java: "第一行\n第二行"
来源：http://xgt.fehbvm.com

Go:   "第一行\n第二行"
来源：http://kgo.shanyushiyangkeji.top

Ruby: "第一行\n第二行"
来源：http://uhn.shanyushiyangtech.top

C#:   "第一行\n第二行"
来源：http://hhm.ydzc1.top

[A14] 注释写法
来源：http://xql.svipenyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zxh.nanxuanxn.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vko.xylfe.cn

JS:   // 单行；/* 多行 */
来源：http://tvd.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://wom.xinyue.icu

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gvo.jqgfzy.top

Go:   // 单行；/* 多行 */
来源：http://scu.hongshengwenyu.top

Ruby: # 单行；=begin 多行 =end
来源：http://ias.vqdsnc.cn

C#:   // 单行；/* 多行 */
来源：http://kla.ybcxt.top

[A15] 空值判断与默认值
来源：http://wwp.redwolf501.top

Py:   value = data or "默认值"
来源：http://ijl.jinqigufen.top

PHP:  $value = $data ?? "默认值";
来源：http://wen.hesvh.cn

JS:   const value = data ?? "默认值";
来源：http://llk.fktsv.cn

TS:   const value = data ?? "默认值";
来源：http://zzp.sufxvd.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lga.yj20258888.top

Go:   if data == "" { data = "默认值" }
来源：http://xdc.chenzaomai.com

Ruby: value = data || "默认值"
来源：http://jpq.yj202588.top

C#:   var value = data ?? "默认值";
来源：http://qbv.mhx1999.top

[A16] 真假值判断规则
来源：http://vgx.shanyushiyangtech.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ihp.9152youxi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dna.yanxiufei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zow.xylfe.cn

TS:   if (!x) {}
来源：http://xry.zhixingplan.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vgt.shzxlz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vth.gzhubu.top

Ruby: unless x            # nil 与 false 为假
来源：http://zbf.yj20258.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://unc.zhiwuduotai.top

[A17] 位运算
来源：http://tdm.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://orj.mhx1999.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kbe.redwolf501.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xah.chenlongwang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://aka.cashguo.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jnq.fehbvm.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ijy.ivvv.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zeb.yj20258.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fky.vqdsnc.cn

[A18] 字符与 ASCII 码互转
来源：http://gsz.fktsv.cn

Py:   ord("A"); chr(65)
来源：http://pyj.hcnkem.com

PHP:  ord("A"); chr(65)
来源：http://pgj.yongpay.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qdm.0kj1m.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rgg.birdmap.top

Java: (int) 'A'; (char) 65
来源：http://rpo.hongshengwenyu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nji.xingfuxueyuan.xyz

Ruby: "A".ord; 65.chr
来源：http://gha.xuetiantiany.cn

C#:   (int)'A'; (char)65
来源：http://bel.yj20258.top

[A19] 交换两个变量
来源：http://qoe.gaohongyu789.top

Py:   a, b = b, a
来源：http://ddx.ivvv.top

PHP:  [$a, $b] = [$b, $a];
来源：http://vbi.nanxuanxn.top

JS:   [a, b] = [b, a];
来源：http://hid.316326.xyz

TS:   [a, b] = [b, a];
来源：http://fsz.hywenlv.cn

Java: int t = a; a = b; b = t;
来源：http://qvu.shanyushiyangtech.top

Go:   a, b = b, a
来源：http://xhl.zhaomingkeji.xyz

Ruby: a, b = b, a
来源：http://zwm.hongshengwenyu.top

C#:   (a, b) = (b, a);
来源：http://jrn.kuanghao11.cn

[A20] 读取标准输入
来源：http://inw.316326.xyz

Py:   name = input("请输入：")
来源：http://don.zhiwuduotai.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wyr.cheryme.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kzv.sufxvd.cn

TS:   // Node.js：readline 模块
来源：http://zwf.shuidangran.top

Java: new Scanner(System.in).nextLine()
来源：http://qhg.dashuyun.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://owq.iojbl.cn

Ruby: gets.chomp
来源：http://bvl.snrcjt.cn

C#:   Console.ReadLine();
来源：http://hnq.nwbrower.top

[A21] 保留指定小数位输出
来源：http://cdu.zhijiandao.cn

Py:   f"{3.14159:.2f}"
来源：http://dbm.zycfv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kxu.gogol.net.cn

JS:   (3.14159).toFixed(2)
来源：http://jse.gotoacloud.top

TS:   (3.14159).toFixed(2)
来源：http://wgw.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://pue.hnxiangtu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://slh.xinyue.icu

Ruby: format("%.2f", 3.14159)
来源：http://xrc.tian-w.cn

C#:   3.14159.ToString("F2")
来源：http://cbr.zhengqikj.top

[A22] 获取字符串长度
来源：http://gtr.zhoulong.xyz

Py:   len(s)
来源：http://qxt.jinyuanbaomall.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xyw.jyoumei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ptq.jinghuilouyu.cn

TS:   s.length
来源：http://tox.jinqigufen.top

Java: s.length()
来源：http://dep.ydzc1.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bxr.wangshuangyany.cn

Ruby: s.length
来源：http://mrg.feifeiyinyue.top

C#:   s.Length
来源：http://yhj.iojbl.cn

[A23] 大小写转换
来源：http://euy.havefunace.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qyd.redwolf501.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://srj.cheryme.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ibr.xylfe.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fyr.0kj1m.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oia.ehwqpu.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jks.smart0.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vom.yueranfly.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pjd.ywan-chungtsiang.top

[A24] 去除首尾空白
来源：http://xvj.xziqi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wyq.zhengqikj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pvu.shzxlz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vhl.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://itf.andypj.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yxv.ctjpmb.com

Go:   strings.TrimSpace(s)
来源：http://tvw.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bvj.yj202588.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://exc.havefunace.top

[A25] 字符串比较
来源：http://fxq.zhoulong.xyz

Py:   s1 == s2; s1 != s2
来源：http://zml.yj20258.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iia.tian-w.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tnh.ivvv.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uyj.zhaomingkeji.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://myr.fengsongda.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rzj.shanyushiyangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vvr.hongshengwenyu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fob.vehdjk.com

[A26] 类型转换总览
来源：http://cvz.ywan-chungtsiang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gxd.bbcook.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zly.hammf.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qao.cashguo.top

TS:   Number() String() Boolean() x as number
来源：http://jva.jinqigfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gvq.yj202588.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zjh.fengsongda.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cny.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jdf.ydzc1.top

================================================================================
来源：http://rht.zhoulong.xyz

B. 流程控制
来源：http://uur.xziqi.cn

================================================================================
来源：http://pln.jinqigufen.top

[B01] 条件判断 if / else
来源：http://wij.hywenlv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gvq.wangshuangyany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bqv.shanyushiyangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nmz.hnqzz.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gxd.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://owg.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yby.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cei.tian-w.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hfp.bbcook.cn

[B02] 多分支 else if / elif
来源：http://kpq.xinyue.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nva.hywenlv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://alb.dianchejie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qgw.gotoacloud.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vwk.tianlin.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dkf.fengsongda.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cwh.fengsongda.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xzz.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bbt.epnwcf.com

[B03] switch / match / case
来源：http://koq.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ngt.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ush.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://asg.jinyuanbaomall.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lxj.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fit.dashuyun.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ivl.ydjk.org.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zmt.xinyue.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kgt.zhijiandao.cn

[B04] for 计数循环
来源：http://dbc.nanxuanxn.top

Py:   for i in range(10): print(i)
来源：http://ple.ydzc1.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hnx.epnwcf.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jzm.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qwy.ppjwa.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://exi.yfazqb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oiu.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://ncf.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pbw.sysykeji.top

[B05] 遍历数组 / 列表
来源：http://xun.yj20258888.top

Py:   for item in arr: print(item)
来源：http://djk.zhengqikj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xxv.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oyt.hysaishi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://itu.gogol.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jsd.gotoacloud.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wbi.sweek.top

Ruby: arr.each { |item| puts item }
来源：http://rap.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qwt.tianlin.xyz

[B06] 遍历字典 / 对象
来源：http://ldy.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ubf.ydjk.org.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xac.havefunace.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yvk.hesvh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vkq.zhoulong.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hnw.aizwys.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nqf.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dey.kuanghao11.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jms.zhongyouzk.top

[B07] while 循环
来源：http://pmr.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://ryq.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://hot.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://ter.gzhubu.top

TS:   while (i < 10) { i++; }
来源：http://ctv.aibaodan.cn

Java: while (i < 10) { i++; }
来源：http://gpw.wangshuangyany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://svq.vehdjk.com

Ruby: while i < 10; i += 1; end
来源：http://nek.havefunace.top

C#:   while (i < 10) { i++; }
来源：http://wlg.cdnleiting.top

[B08] do-while（至少执行一次）
来源：http://uld.daria6918.cn

Py:   # 无 do-while：用 while True + break
来源：http://ddx.ctjpmb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://smf.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://tqj.jiagoushi.top

TS:   do { i++; } while (i < 10);
来源：http://sln.birdmap.top

Java: do { i++; } while (i < 10);
来源：http://nos.hongshengwenyu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nbv.chenjidiqi.icu

Ruby: begin; i += 1; end while i < 10
来源：http://wtx.zdqjudy.top

C#:   do { i++; } while (i < 10);
来源：http://psy.shanyushiyangtech.top

[B09] break 与 continue
来源：http://cgj.xziqi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yrx.dianchejie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eqj.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://liy.hammf.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zfk.yvedp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xyo.tianlin.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qvl.tarul.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qch.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ewl.ydzc1.top

[B10] 遍历同时拿索引
来源：http://vcv.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iis.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://egr.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dll.smart0.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://chm.redwolf501.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blu.bbcook.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hsa.shuidangran.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ooh.aibaodan.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://apb.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://acx.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://dzk.hnxiangtu.top

PHP:  range(0, 10, 2);
来源：http://wgx.hcnkem.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mfd.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cdv.yangfankeji.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://okc.jinqigufen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hor.jinyuanbaomall.cn

Ruby: (0...10).step(2).to_a
来源：http://qgd.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zys.guannengcc.top

[B12] 跳出多层循环
来源：http://yom.zdqjudy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xwy.zhixingplan.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yev.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gbj.aizwys.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lwu.sweek.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qob.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mio.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tfz.xingfuxueyuan.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gyb.tianlin.xyz

[B13] 判断是否为数字
来源：http://zdb.yuxming.cn

Py:   isinstance(x, (int, float))
来源：http://fzo.iojbl.cn

PHP:  is_numeric($x)
来源：http://pxd.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://muf.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ywh.zycfv.cn

Java: x instanceof Number
来源：http://etr.jinqigufen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ecm.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://elb.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://drw.jinyuanbaomall.cn

[B14] 判断值是否在集合内
来源：http://hwt.jqgufenzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://egf.zhixingplan.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://apq.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://ssr.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://nhw.fanxiaobao.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://tna.xuanzx.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hme.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://nfv.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uba.zycfv.cn

[B15] 布尔运算与取反
来源：http://krl.zhixingplan.top

Py:   a and b or not c
来源：http://ezg.cdnleiting.top

PHP:  $a && $b || !$c
来源：http://mnd.yuanzhike.top

JS:   a && b || !c
来源：http://kwl.aizwys.cn

TS:   a && b || !c
来源：http://iku.meibo888.top

Java: a && b || !c
来源：http://vle.hnqzz.top

Go:   a && b || !c
来源：http://jeq.kuanghao11.cn

Ruby: a && b || !c
来源：http://ask.shuidangran.top

C#:   a && b || !c
来源：http://oji.yueranfly.top

[B16] 卫语句：不满足条件提前返回
来源：http://pcc.yfazqb.com

Py:   if not data: return
来源：http://mby.jianghu66.top

PHP:  if (!$data) { return; }
来源：http://ful.fzhhl.top

JS:   if (!data) return;
来源：http://xmj.aizwys.cn

TS:   if (!data) return;
来源：http://qio.zhijiandao.cn

Java: if (data == null) return;
来源：http://oha.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://jmd.ybcxt.top

Ruby: return if data.nil?
来源：http://tgu.9152youxi.cn

C#:   if (data == null) return;
来源：http://skr.shangyingyoupin.top

================================================================================
来源：http://qxl.dashuyun.cn

C. 函数与作用域
来源：http://dkb.quarkkingdee.top

================================================================================
来源：http://dat.jiagoushi.top

[C01] 定义函数
来源：http://saf.yueranfly.top

Py:   def add(a, b): return a + b
来源：http://tyy.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://guf.chenlongwang.top

JS:   function add(a, b) { return a + b; }
来源：http://tqc.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gmx.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xsz.cdnleiting.top

Go:   func add(a, b int) int { return a + b }
来源：http://hlr.vehdjk.com

Ruby: def add(a, b); a + b; end
来源：http://csg.ppjwa.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wvw.kuanghao11.cn

[C02] 默认参数
来源：http://fch.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://imx.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fks.jlsjyb.cn

JS:   function greet(name = "World") { return name; }
来源：http://rvx.sjlbkw.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vac.dianchejie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vah.quarkkingdee.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xpu.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://daj.daxiang520.top


<!-- 参考信息 -->