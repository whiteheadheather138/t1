代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://euj.gaohongyu789.top

Ruby: "Hello, #{name}!"
来源：http://bej.gaohongyu789.top

C#:   $"Hello, {name}!"
来源：http://wav.wangdashe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://vnf.hysaishi.cn

Py:   "第一行\n第二行"
来源：http://fam.gotoacloud.top

PHP:  "第一行\n第二行"
来源：http://lke.dianchejie.cn

JS:   "第一行\n第二行"
来源：http://jah.xziqi.cn

TS:   "第一行\n第二行"
来源：http://izj.xuetiantiany.cn

Java: "第一行\n第二行"
来源：http://gpo.xinyue.icu

Go:   "第一行\n第二行"
来源：http://idk.gogol.net.cn

Ruby: "第一行\n第二行"
来源：http://gpk.52xcode.cn

C#:   "第一行\n第二行"
来源：http://vyb.shuidangran.top

[A14] 注释写法
来源：http://eaw.yangfankeji.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://ooz.dianchejie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kov.shangyingyoupin.top

JS:   // 单行；/* 多行 */
来源：http://jow.c1oappe.top

TS:   // 单行；/* 多行 */
来源：http://aqk.dianchejie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xsh.yonumen.top

Go:   // 单行；/* 多行 */
来源：http://ydh.chenzaomai.com

Ruby: # 单行；=begin 多行 =end
来源：http://bkg.dashuyun.cn

C#:   // 单行；/* 多行 */
来源：http://xhi.xziqi.cn

[A15] 空值判断与默认值
来源：http://oae.jyoumei.cn

Py:   value = data or "默认值"
来源：http://cjg.fengsongda.top

PHP:  $value = $data ?? "默认值";
来源：http://paa.ydzc1.top

JS:   const value = data ?? "默认值";
来源：http://jfp.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://hqs.316326.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://opl.wangdashe.top

Go:   if data == "" { data = "默认值" }
来源：http://zvh.pycfn.com

Ruby: value = data || "默认值"
来源：http://wti.cucudq.cn

C#:   var value = data ?? "默认值";
来源：http://xvy.yanxiufei.cn

[A16] 真假值判断规则
来源：http://jsv.feifeiyinyue.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xet.vqdsnc.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://atx.ydzc1.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qul.shanyushiyangtech.top

TS:   if (!x) {}
来源：http://hpf.aibaodan.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xvw.zhijiandao.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vwt.9152youxi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sni.cucudq.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kit.shuidangran.top

[A17] 位运算
来源：http://lwb.ppjwa.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vud.jyoumei.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rvn.hammf.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kef.hywenlv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kra.yuxming.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uqy.gzhubu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://csg.ctjpmb.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://suo.nanxuanxn.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tlc.shanyushiyangtech.top

[A18] 字符与 ASCII 码互转
来源：http://zla.316326.xyz

Py:   ord("A"); chr(65)
来源：http://iav.hesvh.cn

PHP:  ord("A"); chr(65)
来源：http://dpt.ivvv.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fyu.jinghuilouyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yse.yonumen.top

Java: (int) 'A'; (char) 65
来源：http://xap.yonumen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dgk.haohaochexian.top

Ruby: "A".ord; 65.chr
来源：http://bjw.bjfxy.top

C#:   (int)'A'; (char)65
来源：http://jjh.daxiang520.top

[A19] 交换两个变量
来源：http://czw.chenjidiqi.icu

Py:   a, b = b, a
来源：http://klg.kuanghao11.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jsh.zhengqikj.top

JS:   [a, b] = [b, a];
来源：http://erf.yj20258.top

TS:   [a, b] = [b, a];
来源：http://lfj.dianchejie.cn

Java: int t = a; a = b; b = t;
来源：http://kql.hnqzz.top

Go:   a, b = b, a
来源：http://zlg.ydzc1.top

Ruby: a, b = b, a
来源：http://beq.gaohongyu789.top

C#:   (a, b) = (b, a);
来源：http://xfc.tian-w.cn

[A20] 读取标准输入
来源：http://idj.meibo888.top

Py:   name = input("请输入：")
来源：http://fdn.jianghu66.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zwc.mhx1999.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vjc.shanyushiyangkeji.top

TS:   // Node.js：readline 模块
来源：http://pxp.yangfankeji.com

Java: new Scanner(System.in).nextLine()
来源：http://dif.quarkkingdee.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xfb.jinqigufen.top

Ruby: gets.chomp
来源：http://rjw.hnqzz.top

C#:   Console.ReadLine();
来源：http://ilq.gzhubu.top

[A21] 保留指定小数位输出
来源：http://qam.hysaishi.cn

Py:   f"{3.14159:.2f}"
来源：http://bqp.jiagoushi.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ylh.fehbvm.com

JS:   (3.14159).toFixed(2)
来源：http://int.iojbl.cn

TS:   (3.14159).toFixed(2)
来源：http://zzt.zycfv.cn

Java: String.format("%.2f", 3.14159)
来源：http://lam.yj20258.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cvh.ybcxt.top

Ruby: format("%.2f", 3.14159)
来源：http://jdj.yuanzhike.top

C#:   3.14159.ToString("F2")
来源：http://snl.fehbvm.com

[A22] 获取字符串长度
来源：http://owc.gzhubu.top

Py:   len(s)
来源：http://urc.yongpay.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gyi.fengsongda.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xzq.chenlongwang.top

TS:   s.length
来源：http://ixq.yueranfly.top

Java: s.length()
来源：http://etz.jyoumei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://loe.dianchejie.cn

Ruby: s.length
来源：http://kar.fanxiaobao.xyz

C#:   s.Length
来源：http://dej.hnxiangtu.top

[A23] 大小写转换
来源：http://ubu.jinqigfzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xev.chenjidiqi.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pyb.wangshuangyany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gys.hesvh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mkd.chenjidiqi.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vdg.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ntv.hnxiangtu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://upo.zhixingplan.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nnw.xuetiantiany.cn

[A24] 去除首尾空白
来源：http://yhj.0kj1m.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nfb.chenlongwang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xfs.dianchejie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zdv.gotoacloud.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://epv.xingfuxueyuan.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zsb.fanxiaobao.xyz

Go:   strings.TrimSpace(s)
来源：http://amu.ydzc1.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://axl.fktsv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sna.jinqigfzy.top

[A25] 字符串比较
来源：http://eck.ivvv.top

Py:   s1 == s2; s1 != s2
来源：http://mpn.vqdsnc.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://szj.jinghuilouyu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://shn.vehdjk.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://knt.wangdashe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xeu.c1oappe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mgi.haohaochexian.top

Ruby: s1 == s2; s1 <=> s2
来源：http://esu.9152youxi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ylq.jqgufenzy.top

[A26] 类型转换总览
来源：http://yoe.9152youxi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cfm.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bnh.feifeiyinyue.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dck.ybcxt.top

TS:   Number() String() Boolean() x as number
来源：http://okn.yvedp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://idj.tianlin.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iwf.nanxinkj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ljd.uphjek.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://whd.yongpay.top

================================================================================
来源：http://fgk.nwbrower.top

B. 流程控制
来源：http://hhn.meibo888.top

================================================================================
来源：http://jcn.mhx1999.top

[B01] 条件判断 if / else
来源：http://okm.zdbjq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lsu.ehwqpu.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ynb.cashguo.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zte.nanxinkj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ghw.cheryme.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://krj.haohaochexian.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tqa.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mml.zhongyouzk.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jwr.jinyuanbaomall.cn

[B02] 多分支 else if / elif
来源：http://bmt.cqqwz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eml.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://feq.andypj.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zoh.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pay.tianlin.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jnu.gaohongyu789.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mxs.daxiang520.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://twr.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fpr.yongpay.top

[B03] switch / match / case
来源：http://jep.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rpg.cucudq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://itp.hnxiangtu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://boa.hnxiangtu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bob.guowangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pxl.hnqzz.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xsj.yuanzhike.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fei.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ivg.kuanghao11.cn

[B04] for 计数循环
来源：http://vlw.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://rtk.chenzaomai.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fed.hongshengwenyu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gtf.yfazqb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jtf.hnqzz.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mec.hammf.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gls.quarkkingdee.top

Ruby: 10.times { |i| puts i }
来源：http://mgy.shuidangran.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vid.snrcjt.cn

[B05] 遍历数组 / 列表
来源：http://gzg.zhaomingkeji.xyz

Py:   for item in arr: print(item)
来源：http://hev.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://liw.sufxvd.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lrh.chenzaomai.com

TS:   for (const item of arr) { console.log(item); }
来源：http://aux.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gob.kuanghao11.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vvi.daria6918.cn

Ruby: arr.each { |item| puts item }
来源：http://wcl.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oku.yueranfly.top

[B06] 遍历字典 / 对象
来源：http://qce.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rju.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jbi.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fby.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rgk.yanxiufei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xho.guowangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://shv.nanxinkj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bbp.aizwys.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qey.ehwqpu.com

[B07] while 循环
来源：http://cto.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://cza.shangyingyoupin.top

PHP:  while ($i < 10) { $i++; }
来源：http://wzn.yongpay.top

JS:   while (i < 10) { i++; }
来源：http://zkh.wangdashe.top

TS:   while (i < 10) { i++; }
来源：http://kyk.hnqzz.top

Java: while (i < 10) { i++; }
来源：http://lkz.vehdjk.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://obz.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://fmf.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://mhc.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://ucj.nwbrower.top

Py:   # 无 do-while：用 while True + break
来源：http://mfh.nanxinkj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rcb.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://bnd.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://qez.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://uek.sweek.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nqp.yuxming.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bik.xuetiantiany.cn

C#:   do { i++; } while (i < 10);
来源：http://gsu.yj202588.top

[B09] break 与 continue
来源：http://fhf.birdmap.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bxk.yueranfly.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oqw.316326.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gfc.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://phg.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://upf.zhijiandao.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jpt.hfpthk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://otv.xuanzx.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wea.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://jtf.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bjc.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fxy.aizwys.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xrg.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mbb.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pss.yonumen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nfd.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yoi.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iau.hfpthk.cn

[B11] 生成数字序列 / 区间
来源：http://ogq.tianlin.xyz

Py:   list(range(0, 10, 2))
来源：http://fxf.fengsongda.top

PHP:  range(0, 10, 2);
来源：http://bsv.cqqwz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rcp.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://exi.smart0.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wmx.jyoumei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bcp.yj20258888.top

Ruby: (0...10).step(2).to_a
来源：http://hnm.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uqy.hnqzz.top

[B12] 跳出多层循环
来源：http://lvo.sjlbkw.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://plx.havefunace.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://oeg.sxryk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://owt.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zpr.redwolf501.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yfw.tarul.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zlv.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hpa.shzxlz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lmu.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://ril.zdqjudy.top

Py:   isinstance(x, (int, float))
来源：http://gmw.xinyue.icu

PHP:  is_numeric($x)
来源：http://hym.cdnleiting.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dyr.guannengcc.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lof.nwbrower.top

Java: x instanceof Number
来源：http://est.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ski.316326.xyz

Ruby: x.is_a?(Numeric)
来源：http://lne.guannengcc.top

C#:   x is int or double or decimal
来源：http://kmf.gzhubu.top

[B14] 判断值是否在集合内
来源：http://pdj.hesvh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kag.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://klo.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://grg.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://mhn.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zjy.andypj.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ury.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://wpp.ehwqpu.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ozo.tian-w.cn

[B15] 布尔运算与取反
来源：http://xqj.zhiwuduotai.top

Py:   a and b or not c
来源：http://fqz.yvedp.cn

PHP:  $a && $b || !$c
来源：http://bgr.daria6918.cn

JS:   a && b || !c
来源：http://gto.dianchejie.cn

TS:   a && b || !c
来源：http://kpm.xuetiantiany.cn

Java: a && b || !c
来源：http://fci.aizwys.cn

Go:   a && b || !c
来源：http://itr.hesvh.cn

Ruby: a && b || !c
来源：http://oxl.ehwqpu.com

C#:   a && b || !c
来源：http://joi.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://dbq.ybcxt.top

Py:   if not data: return
来源：http://cmg.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://oez.feifeiyinyue.top

JS:   if (!data) return;
来源：http://ciy.gzhubu.top

TS:   if (!data) return;
来源：http://swv.xziqi.cn

Java: if (data == null) return;
来源：http://ezw.zdbjq.cn

Go:   if data == nil { return }
来源：http://pak.shuidangran.top

Ruby: return if data.nil?
来源：http://wvh.gogol.net.cn

C#:   if (data == null) return;
来源：http://txd.wangshuangyany.cn

================================================================================
来源：http://tzc.ctjpmb.com

C. 函数与作用域
来源：http://mpn.xuanzx.com

================================================================================
来源：http://gxn.pycfn.com

[C01] 定义函数
来源：http://thf.52xcode.cn

Py:   def add(a, b): return a + b
来源：http://igc.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xfy.dashuyun.cn

JS:   function add(a, b) { return a + b; }
来源：http://iiz.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jdv.zhengqikj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zsk.yfazqb.com

Go:   func add(a, b int) int { return a + b }
来源：http://eyz.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://utg.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dhn.guowangkeji.top

[C02] 默认参数
来源：http://cvt.0kj1m.cn

Py:   def greet(name="World"): return name
来源：http://igk.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lyr.ctjpmb.com

JS:   function greet(name = "World") { return name; }
来源：http://lgg.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xuo.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://abp.iojbl.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tdz.hcnkem.com

Ruby: def greet(name = "World") = name
来源：http://vlx.cheryme.top

C#:   string Greet(string name = "World") => name;
来源：http://rfg.yueranfly.top

[C03] 可变参数
来源：http://nfk.jlsjyb.cn

Py:   def total(*args): return sum(args)
来源：http://jda.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ihx.fanxiaobao.xyz


<!-- 参考信息 -->