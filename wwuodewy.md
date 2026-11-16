代发 wailian999

[A10] 生成随机数
来源：http://idy.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://aep.shangyingyoupin.top

PHP:  random_int(1, 100);
来源：http://eip.yonumen.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ttk.jinghuilouyu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ihu.yj20258.top

Java: new Random().nextInt(100) + 1
来源：http://inr.epnwcf.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tve.shzxlz.cn

Ruby: rand(1..100)
来源：http://xvj.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://rrp.gogol.net.cn

[A11] 条件表达式（三元）
来源：http://ncq.zdqjudy.top

Py:   "yes" if x > 0 else "no"
来源：http://sps.birdmap.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://oey.shuidangran.top

JS:   x > 0 ? "yes" : "no"
来源：http://rkm.xziqi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ogr.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://qzn.xziqi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nso.zhixingplan.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ieg.redwolf501.top

C#:   x > 0 ? "yes" : "no"
来源：http://fef.cqqwz.cn

[A12] 字符串插值 / 格式化
来源：http://bhy.chenjidiqi.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bhf.sxryk.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lzd.fzhhl.top

JS:   `Hello, ${name}!`
来源：http://etv.jinyuanbaomall.cn

TS:   `Hello, ${name}!`
来源：http://etj.andypj.xyz

Java: "Hello, %s!".formatted(name)
来源：http://ndx.pycfn.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://atd.zdbjq.cn

Ruby: "Hello, #{name}!"
来源：http://jdu.fehbvm.com

C#:   $"Hello, {name}!"
来源：http://smz.xinyue.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://pub.xingfuxueyuan.xyz

Py:   "第一行\n第二行"
来源：http://tap.zhengqikj.top

PHP:  "第一行\n第二行"
来源：http://ujr.yanxiufei.cn

JS:   "第一行\n第二行"
来源：http://dvw.hfpthk.cn

TS:   "第一行\n第二行"
来源：http://buw.bbcook.cn

Java: "第一行\n第二行"
来源：http://ues.sufxvd.cn

Go:   "第一行\n第二行"
来源：http://xrc.jinyuanbaomall.cn

Ruby: "第一行\n第二行"
来源：http://gbn.zhoulong.xyz

C#:   "第一行\n第二行"
来源：http://cmo.yongpay.top

[A14] 注释写法
来源：http://eny.ehwqpu.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://qcc.xinyue.icu

PHP:  // 或 # 单行；/* 多行 */
来源：http://nxw.jianghu66.top

JS:   // 单行；/* 多行 */
来源：http://swl.wangdashe.top

TS:   // 单行；/* 多行 */
来源：http://pze.sysykeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gyq.bbcook.cn

Go:   // 单行；/* 多行 */
来源：http://ydw.pycfn.com

Ruby: # 单行；=begin 多行 =end
来源：http://hdo.fktsv.cn

C#:   // 单行；/* 多行 */
来源：http://ybv.vehdjk.com

[A15] 空值判断与默认值
来源：http://wsf.mhx1999.top

Py:   value = data or "默认值"
来源：http://khv.fzhhl.top

PHP:  $value = $data ?? "默认值";
来源：http://mop.iojbl.cn

JS:   const value = data ?? "默认值";
来源：http://doy.yuanzhike.top

TS:   const value = data ?? "默认值";
来源：http://zyo.nanxuanxn.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wct.hammf.cn

Go:   if data == "" { data = "默认值" }
来源：http://jze.ybcxt.top

Ruby: value = data || "默认值"
来源：http://lxb.yfazqb.com

C#:   var value = data ?? "默认值";
来源：http://lyi.shuidangran.top

[A16] 真假值判断规则
来源：http://jzt.xuanzx.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yuv.zycfv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pna.dianchejie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hem.zhijiandao.cn

TS:   if (!x) {}
来源：http://byp.zhongyouzk.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qdr.jinghuilouyu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lvc.zycfv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ppy.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mkk.epnwcf.com

[A17] 位运算
来源：http://cxi.ydzc1.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gqf.shanyushiyangtech.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ogu.jinqigufen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qoh.redwolf501.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rsm.cdnleiting.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bzg.dianchejie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://inc.shuidangran.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bgj.feifeiyinyue.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qmi.yuanzhike.top

[A18] 字符与 ASCII 码互转
来源：http://wgz.xziqi.cn

Py:   ord("A"); chr(65)
来源：http://cxx.ywan-chungtsiang.top

PHP:  ord("A"); chr(65)
来源：http://miy.havefunace.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iks.yfazqb.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jef.zhengqikj.top

Java: (int) 'A'; (char) 65
来源：http://qlq.xziqi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://neq.jinqigfzy.top

Ruby: "A".ord; 65.chr
来源：http://aye.nanxuanxn.top

C#:   (int)'A'; (char)65
来源：http://wrf.yanxiufei.cn

[A19] 交换两个变量
来源：http://qgg.jinghuilouyu.cn

Py:   a, b = b, a
来源：http://roj.gotoacloud.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nse.yfazqb.com

JS:   [a, b] = [b, a];
来源：http://rab.jinqigufen.top

TS:   [a, b] = [b, a];
来源：http://yth.shuidangran.top

Java: int t = a; a = b; b = t;
来源：http://bat.jqgfzy.top

Go:   a, b = b, a
来源：http://sjl.sysykeji.top

Ruby: a, b = b, a
来源：http://zdv.sxryk.cn

C#:   (a, b) = (b, a);
来源：http://jxc.jianghu66.top

[A20] 读取标准输入
来源：http://iib.ctjpmb.com

Py:   name = input("请输入：")
来源：http://vzc.epnwcf.com

PHP:  $name = trim(fgets(STDIN));
来源：http://sfi.yj20258888.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lao.zhongyouzk.top

TS:   // Node.js：readline 模块
来源：http://yev.gotoacloud.top

Java: new Scanner(System.in).nextLine()
来源：http://zzi.tanke756.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tds.jinqigufen.top

Ruby: gets.chomp
来源：http://bpi.dashuyun.cn

C#:   Console.ReadLine();
来源：http://zht.haohaochexian.top

[A21] 保留指定小数位输出
来源：http://fhe.zhixingplan.top

Py:   f"{3.14159:.2f}"
来源：http://ful.zhiwuduotai.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bmm.tian-w.cn

JS:   (3.14159).toFixed(2)
来源：http://cha.guannengcc.top

TS:   (3.14159).toFixed(2)
来源：http://sww.meibo888.top

Java: String.format("%.2f", 3.14159)
来源：http://cic.sxryk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iuy.feifeiyinyue.top

Ruby: format("%.2f", 3.14159)
来源：http://exp.fehbvm.com

C#:   3.14159.ToString("F2")
来源：http://suu.yueranfly.top

[A22] 获取字符串长度
来源：http://oet.uphjek.com

Py:   len(s)
来源：http://qoq.andypj.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://aik.vehdjk.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://quf.fktsv.cn

TS:   s.length
来源：http://aau.redwolf501.top

Java: s.length()
来源：http://zds.ppjwa.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hcw.tanke756.top

Ruby: s.length
来源：http://jgh.nanxinkj.top

C#:   s.Length
来源：http://vjv.zhiwuduotai.top

[A23] 大小写转换
来源：http://azp.zdbjq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jtw.sxryk.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ixr.tianlin.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sxk.nwbrower.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://adl.yangfankeji.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uon.bbcook.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fza.ydjk.org.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vvp.redwolf501.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gzy.fengsongda.top

[A24] 去除首尾空白
来源：http://whc.hesvh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oiv.zhengqikj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xex.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://twc.cashguo.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zje.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kaz.yangfankeji.com

Go:   strings.TrimSpace(s)
来源：http://dyt.316326.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bgz.quarkkingdee.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jml.52xcode.cn

[A25] 字符串比较
来源：http://siy.yj20258.top

Py:   s1 == s2; s1 != s2
来源：http://cte.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vlz.andypj.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://haf.meibo888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zij.zhixingplan.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ttw.gogol.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wxa.cucudq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xha.hcnkem.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pcb.meibo888.top

[A26] 类型转换总览
来源：http://dyq.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mqm.hnqzz.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bev.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bzc.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://thw.fktsv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sne.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bhg.tian-w.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://asx.gaohongyu789.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pjk.xziqi.cn

================================================================================
来源：http://wzk.tanke756.top

B. 流程控制
来源：http://aba.hnqzz.top

================================================================================
来源：http://xgu.hammf.cn

[B01] 条件判断 if / else
来源：http://cxp.xuetiantiany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dhw.yonumen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://neu.jinqigufen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kia.ivvv.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kpl.bjfxy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://kxy.pycfn.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fti.kuanghao11.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://klh.jqgfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tyu.tanke756.top

[B02] 多分支 else if / elif
来源：http://egd.jlsjyb.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jfc.birdmap.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wry.meibo888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mrp.haohaochexian.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lgk.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hhb.cheryme.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://onj.dashuyun.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rzr.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://see.yangfankeji.com

[B03] switch / match / case
来源：http://moa.zdbjq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tcq.dashuyun.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pyu.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ohf.sufxvd.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vzw.shangyingyoupin.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hro.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rpj.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aab.nanxuanxn.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vua.xuanzx.com

[B04] for 计数循环
来源：http://zsm.andypj.xyz

Py:   for i in range(10): print(i)
来源：http://hwn.shanyushiyangtech.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xau.zhongyouzk.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qxo.xziqi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qyg.epnwcf.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qsw.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xqa.tianlin.xyz

Ruby: 10.times { |i| puts i }
来源：http://swt.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://umj.316326.xyz

[B05] 遍历数组 / 列表
来源：http://jyu.bbcook.cn

Py:   for item in arr: print(item)
来源：http://del.shzxlz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gzh.ppjwa.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ore.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://nga.pycfn.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://hqe.yanxiufei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tjt.xylfe.cn

Ruby: arr.each { |item| puts item }
来源：http://jby.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ysp.chenjidiqi.icu

[B06] 遍历字典 / 对象
来源：http://ohh.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jns.xuetiantiany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bzh.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mcr.zycfv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sik.hcnkem.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dkz.svipenyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lwe.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://afb.yueranfly.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tzq.yj20258.top

[B07] while 循环
来源：http://xfj.redwolf501.top

Py:   while i < 10: i += 1
来源：http://dfk.hywenlv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dsf.redwolf501.top

JS:   while (i < 10) { i++; }
来源：http://mwm.hcnkem.com

TS:   while (i < 10) { i++; }
来源：http://tjv.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://vas.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mmu.fzhhl.top

Ruby: while i < 10; i += 1; end
来源：http://mjm.yj20258888.top

C#:   while (i < 10) { i++; }
来源：http://cbe.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://xop.hammf.cn

Py:   # 无 do-while：用 while True + break
来源：http://psa.52xcode.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://trk.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://xio.316326.xyz

TS:   do { i++; } while (i < 10);
来源：http://gxp.aizwys.cn

Java: do { i++; } while (i < 10);
来源：http://uza.zhijiandao.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rfa.nanxuanxn.top

Ruby: begin; i += 1; end while i < 10
来源：http://ffl.chenzaomai.com

C#:   do { i++; } while (i < 10);
来源：http://jwk.shzxlz.cn

[B09] break 与 continue
来源：http://mqc.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oic.pycfn.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://znl.ydjk.org.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://neh.vehdjk.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://flj.zhaomingkeji.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rhl.yvedp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kxc.ppjwa.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hcq.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://soh.cucudq.cn

[B10] 遍历同时拿索引
来源：http://cpl.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iov.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tph.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aiy.xuetiantiany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jha.sufxvd.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ugd.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sgo.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bqo.316326.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uro.redwolf501.top

[B11] 生成数字序列 / 区间
来源：http://xdv.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://dhi.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://hsi.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://spw.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://let.epnwcf.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gxj.guannengcc.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://orf.wangshuangyany.cn

Ruby: (0...10).step(2).to_a
来源：http://mdp.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cru.zhoulong.xyz

[B12] 跳出多层循环
来源：http://kpx.zhoulong.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://ors.hcnkem.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://pql.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jyx.zhixingplan.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qvu.cqqwz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kcb.chenjidiqi.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://isf.yj20258888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://edc.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vag.aizwys.cn

[B13] 判断是否为数字
来源：http://zgl.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://sqc.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://ehj.jyoumei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ghh.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zfr.hysaishi.cn

Java: x instanceof Number
来源：http://fyy.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gai.sysykeji.top

Ruby: x.is_a?(Numeric)
来源：http://szg.0kj1m.cn

C#:   x is int or double or decimal
来源：http://yfv.epnwcf.com

[B14] 判断值是否在集合内
来源：http://mtt.sufxvd.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wjt.yfazqb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aiq.quarkkingdee.top

JS:   [1, 2, 3].includes(x)
来源：http://zdc.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://lpp.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kkv.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ety.yuanzhike.top

Ruby: [1, 2, 3].include?(x)
来源：http://wep.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ddv.tian-w.cn

[B15] 布尔运算与取反
来源：http://gjf.wangshuangyany.cn

Py:   a and b or not c
来源：http://tjn.tarul.cn

PHP:  $a && $b || !$c
来源：http://xmh.ppjwa.cn

JS:   a && b || !c
来源：http://oae.pengpengdd.cyou

TS:   a && b || !c
来源：http://gvt.zhiwuduotai.top

Java: a && b || !c
来源：http://fqv.gotoacloud.top

Go:   a && b || !c
来源：http://ggg.zhixingplan.top

Ruby: a && b || !c
来源：http://ild.fktsv.cn

C#:   a && b || !c
来源：http://ikr.yueranfly.top

[B16] 卫语句：不满足条件提前返回
来源：http://hap.tanke756.top

Py:   if not data: return
来源：http://itl.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://ifo.zhoulong.xyz

JS:   if (!data) return;
来源：http://bhm.guannengcc.top

TS:   if (!data) return;
来源：http://ljk.ydjk.org.cn

Java: if (data == null) return;
来源：http://ygi.zycfv.cn

Go:   if data == nil { return }
来源：http://ajv.sysykeji.top

Ruby: return if data.nil?
来源：http://sdc.zhengqikj.top

C#:   if (data == null) return;
来源：http://qhq.hysaishi.cn


<!-- 参考信息 -->