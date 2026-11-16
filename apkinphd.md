代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://lzm.jianghu66.top

[A11] 条件表达式（三元）
来源：http://llc.ydzc1.top

Py:   "yes" if x > 0 else "no"
来源：http://hun.jinqigufen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://xbi.vqdsnc.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xil.kuanghao11.cn

TS:   x > 0 ? "yes" : "no"
来源：http://phw.aizwys.cn

Java: x > 0 ? "yes" : "no"
来源：http://eru.tian-w.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jmx.yfazqb.com

Ruby: x > 0 ? "yes" : "no"
来源：http://xzd.feifeiyinyue.top

C#:   x > 0 ? "yes" : "no"
来源：http://tel.sufxvd.cn

[A12] 字符串插值 / 格式化
来源：http://ngb.cqqwz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cua.fzhhl.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tbw.xziqi.cn

JS:   `Hello, ${name}!`
来源：http://kop.jinyuanbaomall.cn

TS:   `Hello, ${name}!`
来源：http://riu.chenjidiqi.icu

Java: "Hello, %s!".formatted(name)
来源：http://teh.shangyingyoupin.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kgs.cdnleiting.top

Ruby: "Hello, #{name}!"
来源：http://bbj.ehwqpu.com

C#:   $"Hello, {name}!"
来源：http://vle.yuxming.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qdy.hnxiangtu.top

Py:   "第一行\n第二行"
来源：http://auv.bjfxy.top

PHP:  "第一行\n第二行"
来源：http://pth.shanyushiyangtech.top

JS:   "第一行\n第二行"
来源：http://ris.daria6918.cn

TS:   "第一行\n第二行"
来源：http://iql.hongshengwenyu.top

Java: "第一行\n第二行"
来源：http://oio.jinyuanbaomall.cn

Go:   "第一行\n第二行"
来源：http://zyv.kuanghao11.cn

Ruby: "第一行\n第二行"
来源：http://ocv.fehbvm.com

C#:   "第一行\n第二行"
来源：http://kve.birdmap.top

[A14] 注释写法
来源：http://gma.vqdsnc.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qaz.shanyushiyangtech.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ogc.fanxiaobao.xyz

JS:   // 单行；/* 多行 */
来源：http://qna.yuanzhike.top

TS:   // 单行；/* 多行 */
来源：http://tzg.shanyushiyangkeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hun.zhongyouzk.top

Go:   // 单行；/* 多行 */
来源：http://vyh.haohaochexian.top

Ruby: # 单行；=begin 多行 =end
来源：http://wjb.ywan-chungtsiang.top

C#:   // 单行；/* 多行 */
来源：http://mno.ydzc1.top

[A15] 空值判断与默认值
来源：http://lyy.xuanzx.com

Py:   value = data or "默认值"
来源：http://ybn.uphjek.com

PHP:  $value = $data ?? "默认值";
来源：http://ncp.bbcook.cn

JS:   const value = data ?? "默认值";
来源：http://rfy.zhoulong.xyz

TS:   const value = data ?? "默认值";
来源：http://fus.uphjek.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dox.hammf.cn

Go:   if data == "" { data = "默认值" }
来源：http://pgs.dashuyun.cn

Ruby: value = data || "默认值"
来源：http://dbs.zhaomingkeji.xyz

C#:   var value = data ?? "默认值";
来源：http://byd.aibaodan.cn

[A16] 真假值判断规则
来源：http://fqh.wangshuangyany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pod.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xir.ppjwa.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mma.zhoulong.xyz

TS:   if (!x) {}
来源：http://wsx.aizwys.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://omu.fehbvm.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wyu.gaohongyu789.top

Ruby: unless x            # nil 与 false 为假
来源：http://kxv.hfpthk.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xwm.fzhhl.top

[A17] 位运算
来源：http://xas.xziqi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ftr.xziqi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hpt.ywan-chungtsiang.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iur.zhijiandao.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://eml.jiagoushi.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wfl.tanke756.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hvp.0kj1m.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://okj.sweek.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nwl.zdbjq.cn

[A18] 字符与 ASCII 码互转
来源：http://znh.fanxiaobao.xyz

Py:   ord("A"); chr(65)
来源：http://ssa.daria6918.cn

PHP:  ord("A"); chr(65)
来源：http://tjr.ctjpmb.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bls.mhx1999.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ycv.shanyushiyangtech.top

Java: (int) 'A'; (char) 65
来源：http://yye.tianlin.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ond.cdnleiting.top

Ruby: "A".ord; 65.chr
来源：http://gpz.ydjk.org.cn

C#:   (int)'A'; (char)65
来源：http://rle.hcnkem.com

[A19] 交换两个变量
来源：http://mmh.aizwys.cn

Py:   a, b = b, a
来源：http://kxm.havefunace.top

PHP:  [$a, $b] = [$b, $a];
来源：http://iqc.aibaodan.cn

JS:   [a, b] = [b, a];
来源：http://rmq.hongshengwenyu.top

TS:   [a, b] = [b, a];
来源：http://lyn.andypj.xyz

Java: int t = a; a = b; b = t;
来源：http://mce.ppjwa.cn

Go:   a, b = b, a
来源：http://wqr.fanxiaobao.xyz

Ruby: a, b = b, a
来源：http://xps.sufxvd.cn

C#:   (a, b) = (b, a);
来源：http://vpg.xuanzx.com

[A20] 读取标准输入
来源：http://wch.jlsjyb.cn

Py:   name = input("请输入：")
来源：http://dfd.bjfxy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kjr.xziqi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://aqr.yvedp.cn

TS:   // Node.js：readline 模块
来源：http://bfr.gzhubu.top

Java: new Scanner(System.in).nextLine()
来源：http://hqg.jinqigfzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cep.sxryk.cn

Ruby: gets.chomp
来源：http://yer.jinqigfzy.top

C#:   Console.ReadLine();
来源：http://chp.fktsv.cn

[A21] 保留指定小数位输出
来源：http://emc.xinyue.icu

Py:   f"{3.14159:.2f}"
来源：http://gvf.jianghu66.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://byn.epnwcf.com

JS:   (3.14159).toFixed(2)
来源：http://roq.kuanghao11.cn

TS:   (3.14159).toFixed(2)
来源：http://pfn.chenjidiqi.icu

Java: String.format("%.2f", 3.14159)
来源：http://cxk.jlsjyb.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gcz.vqdsnc.cn

Ruby: format("%.2f", 3.14159)
来源：http://zhc.shanyushiyangtech.top

C#:   3.14159.ToString("F2")
来源：http://bov.epnwcf.com

[A22] 获取字符串长度
来源：http://kam.nanxinkj.top

Py:   len(s)
来源：http://fte.snrcjt.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://frr.iojbl.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://muu.zhaomingkeji.xyz

TS:   s.length
来源：http://iyo.zhiwuduotai.top

Java: s.length()
来源：http://krh.feifeiyinyue.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://crj.0kj1m.cn

Ruby: s.length
来源：http://iyo.ydzc1.top

C#:   s.Length
来源：http://zck.sweek.top

[A23] 大小写转换
来源：http://egc.jinqigfzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://err.tarul.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pqj.yj20258888.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ezb.havefunace.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tux.svipenyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ybd.hcnkem.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xww.pycfn.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://svn.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dmw.xylfe.cn

[A24] 去除首尾空白
来源：http://yfs.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://etu.c1oappe.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bvl.yongpay.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kof.xziqi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vyn.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lox.chenlongwang.top

Go:   strings.TrimSpace(s)
来源：http://bhk.cashguo.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iwm.zhaomingkeji.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uce.cheryme.top

[A25] 字符串比较
来源：http://bfg.hammf.cn

Py:   s1 == s2; s1 != s2
来源：http://alx.316326.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ctq.bjfxy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dpn.316326.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ikf.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ydi.epnwcf.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://etu.hesvh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://crz.zhoulong.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yyt.hcnkem.com

[A26] 类型转换总览
来源：http://kue.fengsongda.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mav.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ric.yfazqb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vcf.jqgfzy.top

TS:   Number() String() Boolean() x as number
来源：http://bye.cdnleiting.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iwm.nwbrower.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pol.sweek.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fvd.fengsongda.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sex.yj20258888.top

================================================================================
来源：http://rzb.tanke756.top

B. 流程控制
来源：http://jzy.cashguo.top

================================================================================
来源：http://ezl.hcnkem.com

[B01] 条件判断 if / else
来源：http://yvs.feifeiyinyue.top

Py:   result = "正" if x > 0 else "非正"
来源：http://sjv.yanxiufei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zhx.ehwqpu.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qnj.xziqi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lkd.zhixingplan.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://apj.tanke756.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vtu.ctjpmb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ehi.wangdashe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://got.jlsjyb.cn

[B02] 多分支 else if / elif
来源：http://jxe.c1oappe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vjo.ydzc1.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kav.chenlongwang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zpx.tian-w.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ljx.wangdashe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://unq.sweek.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cix.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uqo.yuanzhike.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bkp.ydjk.org.cn

[B03] switch / match / case
来源：http://zfc.xziqi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uml.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rrv.bjfxy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xso.jinqigufen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aev.hysaishi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ras.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pbm.ydzc1.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qtq.ydjk.org.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mxw.jqgufenzy.top

[B04] for 计数循环
来源：http://uvj.sufxvd.cn

Py:   for i in range(10): print(i)
来源：http://uhf.zhoulong.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ydi.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fam.chenjidiqi.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://brh.shanyushiyangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cep.jlsjyb.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rku.tanke756.top

Ruby: 10.times { |i| puts i }
来源：http://hcf.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hyu.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://vua.mhx1999.top

Py:   for item in arr: print(item)
来源：http://ghy.shanyushiyangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nke.wangshuangyany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dtj.kuanghao11.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ltg.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hvt.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ugz.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://iwl.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vvq.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://ynq.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hol.jianghu66.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nmt.jinqigufen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://znj.sxryk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ecq.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rok.svipenyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://akp.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hnl.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jna.hammf.cn

[B07] while 循环
来源：http://kki.jinqigufen.top

Py:   while i < 10: i += 1
来源：http://uak.guannengcc.top

PHP:  while ($i < 10) { $i++; }
来源：http://iou.iojbl.cn

JS:   while (i < 10) { i++; }
来源：http://sfq.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://apo.zhongyouzk.top

Java: while (i < 10) { i++; }
来源：http://mpk.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bsr.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://kmz.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://jnm.tarul.cn

[B08] do-while（至少执行一次）
来源：http://ltx.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://unv.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kvh.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://oug.wangshuangyany.cn

TS:   do { i++; } while (i < 10);
来源：http://rcy.yj20258888.top

Java: do { i++; } while (i < 10);
来源：http://vvg.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://whu.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://teu.zhongyouzk.top

C#:   do { i++; } while (i < 10);
来源：http://lem.svipenyu.cn

[B09] break 与 continue
来源：http://ilw.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bpx.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xst.jqgufenzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xsk.andypj.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tos.pengpengdd.cyou

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zla.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vjj.yanxiufei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mjc.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bti.yj20258.top

[B10] 遍历同时拿索引
来源：http://tkp.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lgw.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vke.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jba.316326.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cyx.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wgp.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gul.xingfuxueyuan.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mkc.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tva.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://tvm.0kj1m.cn

Py:   list(range(0, 10, 2))
来源：http://ugq.sufxvd.cn

PHP:  range(0, 10, 2);
来源：http://yif.yonumen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ifk.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fhh.hongshengwenyu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://olh.yj20258.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fik.sjlbkw.cn

Ruby: (0...10).step(2).to_a
来源：http://rnl.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ftm.hongshengwenyu.top

[B12] 跳出多层循环
来源：http://zki.jqgfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jya.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://etr.ppjwa.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xfj.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xjj.zhaomingkeji.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kbq.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jfx.shangyingyoupin.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zev.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ilf.yonumen.top

[B13] 判断是否为数字
来源：http://lxg.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://tld.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://zdq.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ati.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vwd.uphjek.com

Java: x instanceof Number
来源：http://ufx.feifeiyinyue.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cju.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://wpe.9152youxi.cn

C#:   x is int or double or decimal
来源：http://suh.yj20258888.top

[B14] 判断值是否在集合内
来源：http://gek.jianghu66.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://waa.snrcjt.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://luv.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://ito.316326.xyz

TS:   [1, 2, 3].includes(x)
来源：http://rso.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yul.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fyn.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://fza.kuanghao11.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uqp.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://akg.gzhubu.top

Py:   a and b or not c
来源：http://xrb.gzhubu.top

PHP:  $a && $b || !$c
来源：http://vbt.cqqwz.cn

JS:   a && b || !c
来源：http://dpd.zhengqikj.top

TS:   a && b || !c
来源：http://zsm.hysaishi.cn

Java: a && b || !c
来源：http://rcz.guannengcc.top

Go:   a && b || !c
来源：http://ycd.xziqi.cn

Ruby: a && b || !c
来源：http://znw.snrcjt.cn

C#:   a && b || !c
来源：http://rpp.zhaomingkeji.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://quy.zhixingplan.top

Py:   if not data: return
来源：http://shm.haohaochexian.top

PHP:  if (!$data) { return; }
来源：http://vit.xingfuxueyuan.xyz

JS:   if (!data) return;
来源：http://xzi.nwbrower.top

TS:   if (!data) return;
来源：http://wai.kuanghao11.cn

Java: if (data == null) return;
来源：http://lbw.zdbjq.cn

Go:   if data == nil { return }
来源：http://zyt.jianghu66.top

Ruby: return if data.nil?
来源：http://ief.jinyuanbaomall.cn

C#:   if (data == null) return;
来源：http://mti.aizwys.cn

================================================================================
来源：http://zdd.jlsjyb.cn

C. 函数与作用域
来源：http://har.hywenlv.cn

================================================================================
来源：http://hgw.guannengcc.top

[C01] 定义函数
来源：http://qeb.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://ozg.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pxj.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://gel.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dtq.sysykeji.top


<!-- 参考信息 -->