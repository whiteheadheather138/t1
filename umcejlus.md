代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ign.vqdsnc.cn

JS:   `Hello, ${name}!`
来源：http://zoq.shangyingyoupin.top

TS:   `Hello, ${name}!`
来源：http://sxm.xuanzx.com

Java: "Hello, %s!".formatted(name)
来源：http://fif.daxiang520.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jto.yj202588.top

Ruby: "Hello, #{name}!"
来源：http://pvb.jinghuilouyu.cn

C#:   $"Hello, {name}!"
来源：http://iek.shanyushiyangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ibn.cheryme.top

Py:   "第一行\n第二行"
来源：http://zof.chenlongwang.top

PHP:  "第一行\n第二行"
来源：http://jqi.svipenyu.cn

JS:   "第一行\n第二行"
来源：http://fao.yanxiufei.cn

TS:   "第一行\n第二行"
来源：http://wcq.tanke756.top

Java: "第一行\n第二行"
来源：http://nbm.chenzaomai.com

Go:   "第一行\n第二行"
来源：http://sjc.ppjwa.cn

Ruby: "第一行\n第二行"
来源：http://now.zhongyouzk.top

C#:   "第一行\n第二行"
来源：http://pfc.gotoacloud.top

[A14] 注释写法
来源：http://wkz.sweek.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ufy.zycfv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yku.epnwcf.com

JS:   // 单行；/* 多行 */
来源：http://xga.fktsv.cn

TS:   // 单行；/* 多行 */
来源：http://hwc.nanxuanxn.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qbr.tarul.cn

Go:   // 单行；/* 多行 */
来源：http://axb.hesvh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://htg.svipenyu.cn

C#:   // 单行；/* 多行 */
来源：http://bzu.haohaochexian.top

[A15] 空值判断与默认值
来源：http://bsl.jianghu66.top

Py:   value = data or "默认值"
来源：http://txz.bbcook.cn

PHP:  $value = $data ?? "默认值";
来源：http://tio.nwbrower.top

JS:   const value = data ?? "默认值";
来源：http://eei.xziqi.cn

TS:   const value = data ?? "默认值";
来源：http://tod.gzhubu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zea.fengsongda.top

Go:   if data == "" { data = "默认值" }
来源：http://rao.hongshengwenyu.top

Ruby: value = data || "默认值"
来源：http://mcx.gaohongyu789.top

C#:   var value = data ?? "默认值";
来源：http://dak.daria6918.cn

[A16] 真假值判断规则
来源：http://ysp.dashuyun.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zad.daria6918.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ymd.redwolf501.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cyx.ehwqpu.com

TS:   if (!x) {}
来源：http://uqk.tianlin.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ufd.svipenyu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xhv.jiagoushi.top

Ruby: unless x            # nil 与 false 为假
来源：http://mwu.52xcode.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://haw.ydzc1.top

[A17] 位运算
来源：http://nxn.mhx1999.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fiy.cqqwz.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zas.jqgufenzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sfv.birdmap.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lsa.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cum.nanxuanxn.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qes.nwbrower.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tzk.haohaochexian.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zxh.yfazqb.com

[A18] 字符与 ASCII 码互转
来源：http://fbt.gotoacloud.top

Py:   ord("A"); chr(65)
来源：http://nyb.sysykeji.top

PHP:  ord("A"); chr(65)
来源：http://nsu.yvedp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jtg.fktsv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eiw.cheryme.top

Java: (int) 'A'; (char) 65
来源：http://qzv.shuidangran.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vsp.zycfv.cn

Ruby: "A".ord; 65.chr
来源：http://sii.bjfxy.top

C#:   (int)'A'; (char)65
来源：http://ren.fzhhl.top

[A19] 交换两个变量
来源：http://izz.hnqzz.top

Py:   a, b = b, a
来源：http://lfr.cheryme.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pdb.meibo888.top

JS:   [a, b] = [b, a];
来源：http://ggb.dashuyun.cn

TS:   [a, b] = [b, a];
来源：http://pvw.jinqigfzy.top

Java: int t = a; a = b; b = t;
来源：http://ruo.vqdsnc.cn

Go:   a, b = b, a
来源：http://ipl.snrcjt.cn

Ruby: a, b = b, a
来源：http://brl.fengsongda.top

C#:   (a, b) = (b, a);
来源：http://qvi.fktsv.cn

[A20] 读取标准输入
来源：http://vos.shuidangran.top

Py:   name = input("请输入：")
来源：http://wvq.yj20258888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kwg.yvedp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oli.sxryk.cn

TS:   // Node.js：readline 模块
来源：http://bor.haohaochexian.top

Java: new Scanner(System.in).nextLine()
来源：http://zkz.cheryme.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mjn.sjlbkw.cn

Ruby: gets.chomp
来源：http://qib.52xcode.cn

C#:   Console.ReadLine();
来源：http://jih.dianchejie.cn

[A21] 保留指定小数位输出
来源：http://hqb.tanke756.top

Py:   f"{3.14159:.2f}"
来源：http://kwy.nwbrower.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jzb.zhengqikj.top

JS:   (3.14159).toFixed(2)
来源：http://ehv.dashuyun.cn

TS:   (3.14159).toFixed(2)
来源：http://paz.yfazqb.com

Java: String.format("%.2f", 3.14159)
来源：http://pjl.guannengcc.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wuw.sjlbkw.cn

Ruby: format("%.2f", 3.14159)
来源：http://udf.ywan-chungtsiang.top

C#:   3.14159.ToString("F2")
来源：http://tht.svipenyu.cn

[A22] 获取字符串长度
来源：http://ymq.chenzaomai.com

Py:   len(s)
来源：http://bak.ppjwa.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lpo.yj20258.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://njb.ybcxt.top

TS:   s.length
来源：http://pcq.sxryk.cn

Java: s.length()
来源：http://zqx.hammf.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://knb.gaohongyu789.top

Ruby: s.length
来源：http://lzr.haohaochexian.top

C#:   s.Length
来源：http://qal.hesvh.cn

[A23] 大小写转换
来源：http://mlk.xuanzx.com

Py:   s.upper(); s.lower(); s.title()
来源：http://sem.vehdjk.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eaz.yueranfly.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kco.zhixingplan.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gpu.hammf.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ews.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wyb.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jad.quarkkingdee.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qyj.ppjwa.cn

[A24] 去除首尾空白
来源：http://zsa.ctjpmb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://brs.fzhhl.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pkd.yueranfly.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bdq.zycfv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aar.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vhg.yuxming.cn

Go:   strings.TrimSpace(s)
来源：http://syd.yueranfly.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ncp.kuanghao11.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://unm.pengpengdd.cyou

[A25] 字符串比较
来源：http://vrh.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://bba.fzhhl.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jhf.haohaochexian.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fys.guannengcc.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fbs.chenzaomai.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jgv.yuxming.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nho.yuxming.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ryb.gzhubu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wru.hnxiangtu.top

[A26] 类型转换总览
来源：http://ign.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://szj.uphjek.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tqn.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xey.sweek.top

TS:   Number() String() Boolean() x as number
来源：http://ruc.uphjek.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gns.jiagoushi.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ace.jyoumei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tmg.chenzaomai.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yix.jyoumei.cn

================================================================================
来源：http://bpo.ctjpmb.com

B. 流程控制
来源：http://pop.shuidangran.top

================================================================================
来源：http://aui.chenlongwang.top

[B01] 条件判断 if / else
来源：http://maa.tarul.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://moy.uphjek.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://per.yangfankeji.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cnw.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ksn.bbcook.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://neh.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uup.fehbvm.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ost.shanyushiyangtech.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oem.hywenlv.cn

[B02] 多分支 else if / elif
来源：http://hdt.zhaomingkeji.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://prx.quarkkingdee.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hxd.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xvf.hcnkem.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tma.sxryk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nud.52xcode.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cma.jiagoushi.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gap.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rpq.fzhhl.top

[B03] switch / match / case
来源：http://ifz.hfpthk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ich.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bsh.yueranfly.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oxw.jinqigfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eeg.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fti.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://izi.birdmap.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://upm.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://udz.fzhhl.top

[B04] for 计数循环
来源：http://vxo.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://mpa.sufxvd.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://enm.jinqigufen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dow.shangyingyoupin.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://spj.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nuy.hnqzz.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://csj.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://may.zhoulong.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tmq.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://akf.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://kmy.cheryme.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qpg.xuetiantiany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sgp.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://pfv.bbcook.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ztu.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qxl.shzxlz.cn

Ruby: arr.each { |item| puts item }
来源：http://aku.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ani.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://deh.redwolf501.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cqz.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rxe.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bti.tian-w.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tpw.jinqigufen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qot.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yzo.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fqw.sufxvd.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hkh.jiagoushi.top

[B07] while 循环
来源：http://rwj.ydzc1.top

Py:   while i < 10: i += 1
来源：http://vtm.guannengcc.top

PHP:  while ($i < 10) { $i++; }
来源：http://bfx.ybcxt.top

JS:   while (i < 10) { i++; }
来源：http://xwj.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://hhp.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://nem.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yjj.chenlongwang.top

Ruby: while i < 10; i += 1; end
来源：http://qab.hcnkem.com

C#:   while (i < 10) { i++; }
来源：http://tsz.epnwcf.com

[B08] do-while（至少执行一次）
来源：http://zyw.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://hvz.vehdjk.com

PHP:  do { $i++; } while ($i < 10);
来源：http://bli.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://osa.iojbl.cn

TS:   do { i++; } while (i < 10);
来源：http://lpt.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://psc.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://pri.uphjek.com

Ruby: begin; i += 1; end while i < 10
来源：http://ezy.ppjwa.cn

C#:   do { i++; } while (i < 10);
来源：http://wtf.wangdashe.top

[B09] break 与 continue
来源：http://mht.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wem.zhixingplan.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://faj.zdqjudy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mxf.zhixingplan.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qlz.jlsjyb.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lyz.hnxiangtu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uhv.haohaochexian.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://heg.daria6918.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ogo.gogol.net.cn

[B10] 遍历同时拿索引
来源：http://fqz.xuetiantiany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nim.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pke.hammf.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oum.zhiwuduotai.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rrm.yanxiufei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kgk.yj20258888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qem.havefunace.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rxu.ywan-chungtsiang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mol.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://hrj.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://maa.fengsongda.top

PHP:  range(0, 10, 2);
来源：http://ono.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iyn.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rbx.shuidangran.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vwx.hammf.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mxc.jinqigufen.top

Ruby: (0...10).step(2).to_a
来源：http://uby.yj20258888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://djt.aibaodan.cn

[B12] 跳出多层循环
来源：http://gip.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fax.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uup.hcnkem.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hzy.mhx1999.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://plb.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://abe.xingfuxueyuan.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uxx.havefunace.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uwn.uphjek.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aop.yuanzhike.top

[B13] 判断是否为数字
来源：http://rau.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://key.ydzc1.top

PHP:  is_numeric($x)
来源：http://bet.hnqzz.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xmv.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fzn.yuxming.cn

Java: x instanceof Number
来源：http://azu.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ivg.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://dkv.redwolf501.top

C#:   x is int or double or decimal
来源：http://rii.redwolf501.top

[B14] 判断值是否在集合内
来源：http://mqs.yj20258.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fhi.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kcx.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://tnj.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://qsy.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://qmf.dashuyun.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uae.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iyp.jqgfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dws.svipenyu.cn

[B15] 布尔运算与取反
来源：http://lti.gaohongyu789.top

Py:   a and b or not c
来源：http://dng.ppjwa.cn

PHP:  $a && $b || !$c
来源：http://cix.shanyushiyangtech.top

JS:   a && b || !c
来源：http://cqs.fehbvm.com

TS:   a && b || !c
来源：http://jol.xuanzx.com

Java: a && b || !c
来源：http://rbc.hongshengwenyu.top

Go:   a && b || !c
来源：http://fvy.cqqwz.cn

Ruby: a && b || !c
来源：http://dhp.jianghu66.top

C#:   a && b || !c
来源：http://nqq.gaohongyu789.top

[B16] 卫语句：不满足条件提前返回
来源：http://avr.nanxuanxn.top

Py:   if not data: return
来源：http://eii.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://iuw.jiagoushi.top

JS:   if (!data) return;
来源：http://yhi.tanke756.top

TS:   if (!data) return;
来源：http://src.aibaodan.cn

Java: if (data == null) return;
来源：http://vyg.svipenyu.cn

Go:   if data == nil { return }
来源：http://tpr.yj20258.top

Ruby: return if data.nil?
来源：http://onn.yj202588.top

C#:   if (data == null) return;
来源：http://czi.xylfe.cn

================================================================================
来源：http://yji.shanyushiyangtech.top

C. 函数与作用域
来源：http://rax.xuanzx.com

================================================================================
来源：http://yda.aibaodan.cn

[C01] 定义函数
来源：http://dxp.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://tec.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vle.hysaishi.cn

JS:   function add(a, b) { return a + b; }
来源：http://dod.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ehv.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://jiv.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://pyv.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://yki.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fhq.yanxiufei.cn

[C02] 默认参数
来源：http://eym.jqgufenzy.top

Py:   def greet(name="World"): return name
来源：http://uwq.jinqigufen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://clp.zhixingplan.top

JS:   function greet(name = "World") { return name; }
来源：http://jww.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mvn.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pdy.cqqwz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cih.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://cjm.yj202588.top


<!-- 参考信息 -->