代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fpj.xziqi.cn

Java: new Random().nextInt(100) + 1
来源：http://mje.chenjidiqi.icu

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wsa.tianlin.xyz

Ruby: rand(1..100)
来源：http://myc.guannengcc.top

C#:   new Random().Next(1, 101)
来源：http://udp.jinqigfzy.top

[A11] 条件表达式（三元）
来源：http://mxf.ydjk.org.cn

Py:   "yes" if x > 0 else "no"
来源：http://xpc.jyoumei.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lfv.shanyushiyangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://qny.bbcook.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hmu.tianlin.xyz

Java: x > 0 ? "yes" : "no"
来源：http://rxu.ydzc1.top

Go:   // 无三元运算符，需用 if 语句
来源：http://rwg.fanxiaobao.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://nwo.chenjidiqi.icu

C#:   x > 0 ? "yes" : "no"
来源：http://aol.hcnkem.com

[A12] 字符串插值 / 格式化
来源：http://efi.gzhubu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ukf.epnwcf.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ici.chenjidiqi.icu

JS:   `Hello, ${name}!`
来源：http://srb.yanxiufei.cn

TS:   `Hello, ${name}!`
来源：http://bbz.sufxvd.cn

Java: "Hello, %s!".formatted(name)
来源：http://doe.yanxiufei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cev.sysykeji.top

Ruby: "Hello, #{name}!"
来源：http://grs.zhongyouzk.top

C#:   $"Hello, {name}!"
来源：http://ftg.uphjek.com

[A13] 多行字符串（练习 \n 转义）
来源：http://vmc.shanyushiyangtech.top

Py:   "第一行\n第二行"
来源：http://pvq.jinqigfzy.top

PHP:  "第一行\n第二行"
来源：http://wcd.vqdsnc.cn

JS:   "第一行\n第二行"
来源：http://veb.zhongyouzk.top

TS:   "第一行\n第二行"
来源：http://adi.yvedp.cn

Java: "第一行\n第二行"
来源：http://qme.tianlin.xyz

Go:   "第一行\n第二行"
来源：http://yic.ydjk.org.cn

Ruby: "第一行\n第二行"
来源：http://haj.ppjwa.cn

C#:   "第一行\n第二行"
来源：http://xaf.52xcode.cn

[A14] 注释写法
来源：http://uaw.hammf.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uxo.fengsongda.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://hfm.316326.xyz

JS:   // 单行；/* 多行 */
来源：http://gxj.nwbrower.top

TS:   // 单行；/* 多行 */
来源：http://cvq.aibaodan.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rbd.shangyingyoupin.top

Go:   // 单行；/* 多行 */
来源：http://hjk.jyoumei.cn

Ruby: # 单行；=begin 多行 =end
来源：http://epx.zycfv.cn

C#:   // 单行；/* 多行 */
来源：http://uin.chenjidiqi.icu

[A15] 空值判断与默认值
来源：http://vyo.wangshuangyany.cn

Py:   value = data or "默认值"
来源：http://ugt.hfpthk.cn

PHP:  $value = $data ?? "默认值";
来源：http://dke.xinyue.icu

JS:   const value = data ?? "默认值";
来源：http://cuu.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://xju.havefunace.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tcz.shangyingyoupin.top

Go:   if data == "" { data = "默认值" }
来源：http://kao.hammf.cn

Ruby: value = data || "默认值"
来源：http://ugm.xziqi.cn

C#:   var value = data ?? "默认值";
来源：http://ltf.cqqwz.cn

[A16] 真假值判断规则
来源：http://otc.haohaochexian.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pms.jinqigufen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://moy.shuidangran.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kyi.hywenlv.cn

TS:   if (!x) {}
来源：http://qjo.zhijiandao.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yjp.sweek.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qwk.smart0.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://kve.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://swn.cdnleiting.top

[A17] 位运算
来源：http://ecp.yanxiufei.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vbx.xinyue.icu

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mrr.zhengqikj.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lee.xuetiantiany.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dou.yuanzhike.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://crp.mhx1999.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://chn.daria6918.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zyk.zhixingplan.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ejq.shzxlz.cn

[A18] 字符与 ASCII 码互转
来源：http://cxp.shangyingyoupin.top

Py:   ord("A"); chr(65)
来源：http://iqe.jqgufenzy.top

PHP:  ord("A"); chr(65)
来源：http://nmo.zhaomingkeji.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yvi.havefunace.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://htv.tian-w.cn

Java: (int) 'A'; (char) 65
来源：http://uie.ybcxt.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jfw.meibo888.top

Ruby: "A".ord; 65.chr
来源：http://elz.hfpthk.cn

C#:   (int)'A'; (char)65
来源：http://cbl.hcnkem.com

[A19] 交换两个变量
来源：http://frd.cqqwz.cn

Py:   a, b = b, a
来源：http://wod.quarkkingdee.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hkz.jlsjyb.cn

JS:   [a, b] = [b, a];
来源：http://mls.guowangkeji.top

TS:   [a, b] = [b, a];
来源：http://nmn.tarul.cn

Java: int t = a; a = b; b = t;
来源：http://oan.ehwqpu.com

Go:   a, b = b, a
来源：http://vbx.zhijiandao.cn

Ruby: a, b = b, a
来源：http://rof.shuidangran.top

C#:   (a, b) = (b, a);
来源：http://mbh.smart0.xyz

[A20] 读取标准输入
来源：http://tmo.vehdjk.com

Py:   name = input("请输入：")
来源：http://rht.zhengqikj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://fxm.mhx1999.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bhn.yuxming.cn

TS:   // Node.js：readline 模块
来源：http://uqh.svipenyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://zoe.jinqigufen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tis.wangdashe.top

Ruby: gets.chomp
来源：http://lxv.cheryme.top

C#:   Console.ReadLine();
来源：http://fuh.guannengcc.top

[A21] 保留指定小数位输出
来源：http://tht.fanxiaobao.xyz

Py:   f"{3.14159:.2f}"
来源：http://tup.shzxlz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xla.yuanzhike.top

JS:   (3.14159).toFixed(2)
来源：http://ukx.hnxiangtu.top

TS:   (3.14159).toFixed(2)
来源：http://iny.vehdjk.com

Java: String.format("%.2f", 3.14159)
来源：http://nqf.ehwqpu.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vns.daria6918.cn

Ruby: format("%.2f", 3.14159)
来源：http://ubi.xylfe.cn

C#:   3.14159.ToString("F2")
来源：http://efq.kuanghao11.cn

[A22] 获取字符串长度
来源：http://bon.iojbl.cn

Py:   len(s)
来源：http://wfe.xingfuxueyuan.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://naq.cheryme.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hsa.jiagoushi.top

TS:   s.length
来源：http://fjn.nwbrower.top

Java: s.length()
来源：http://akr.ivvv.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nva.snrcjt.cn

Ruby: s.length
来源：http://dle.zhijiandao.cn

C#:   s.Length
来源：http://ihq.yangfankeji.com

[A23] 大小写转换
来源：http://mlr.iojbl.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qaj.aibaodan.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xog.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zda.xingfuxueyuan.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fri.jianghu66.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fke.hnqzz.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://axw.pengpengdd.cyou

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sns.yvedp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jqn.feifeiyinyue.top

[A24] 去除首尾空白
来源：http://jwi.bbcook.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xfg.jinyuanbaomall.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iyh.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://swn.shzxlz.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vfr.gaohongyu789.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eqf.shangyingyoupin.top

Go:   strings.TrimSpace(s)
来源：http://vis.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ahm.chenzaomai.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rrc.sxryk.cn

[A25] 字符串比较
来源：http://ovm.nanxinkj.top

Py:   s1 == s2; s1 != s2
来源：http://jse.yuanzhike.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ttr.birdmap.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lru.ydjk.org.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wvf.fktsv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ogf.zdbjq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uuk.ydzc1.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kji.zycfv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jdm.ehwqpu.com

[A26] 类型转换总览
来源：http://xlf.yuanzhike.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wyk.52xcode.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oxu.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kmy.yangfankeji.com

TS:   Number() String() Boolean() x as number
来源：http://qmk.yuanzhike.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vzu.fzhhl.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xmi.ydjk.org.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://trh.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yio.zhongyouzk.top

================================================================================
来源：http://qwt.iojbl.cn

B. 流程控制
来源：http://jvf.guowangkeji.top

================================================================================
来源：http://xec.hysaishi.cn

[B01] 条件判断 if / else
来源：http://wvj.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://qkx.ydjk.org.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mwf.chenzaomai.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://who.dashuyun.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yte.dianchejie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zbk.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wcg.zhijiandao.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://izr.gotoacloud.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ryy.c1oappe.top

[B02] 多分支 else if / elif
来源：http://gyj.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jbx.daxiang520.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ucn.aibaodan.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ucs.hfpthk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://epx.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yqe.ctjpmb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zso.yj20258.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nsg.uphjek.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oao.sweek.top

[B03] switch / match / case
来源：http://vnb.yj20258888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cmc.hammf.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vxj.gzhubu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oap.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://arj.hnqzz.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tjs.jyoumei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xbt.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://atd.ydzc1.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wzr.uphjek.com

[B04] for 计数循环
来源：http://ihg.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://evb.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qwv.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lhi.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jhq.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vsg.aizwys.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mly.fengsongda.top

Ruby: 10.times { |i| puts i }
来源：http://yuf.zdbjq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jjp.jianghu66.top

[B05] 遍历数组 / 列表
来源：http://fwx.zhaomingkeji.xyz

Py:   for item in arr: print(item)
来源：http://gay.nwbrower.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jes.quarkkingdee.top

JS:   for (const item of arr) { console.log(item); }
来源：http://evj.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bst.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://oeu.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vsz.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://ura.yangfankeji.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://grv.gotoacloud.top

[B06] 遍历字典 / 对象
来源：http://kzw.yvedp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wnm.daria6918.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://spm.yuanzhike.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tis.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lte.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xaa.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://spi.xziqi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xwd.daria6918.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ixl.chenjidiqi.icu

[B07] while 循环
来源：http://nko.tianlin.xyz

Py:   while i < 10: i += 1
来源：http://nne.guowangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://bje.birdmap.top

JS:   while (i < 10) { i++; }
来源：http://jcz.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://jzo.yueranfly.top

Java: while (i < 10) { i++; }
来源：http://xqq.9152youxi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xwr.fktsv.cn

Ruby: while i < 10; i += 1; end
来源：http://qsq.havefunace.top

C#:   while (i < 10) { i++; }
来源：http://iyw.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://lis.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://bls.tanke756.top

PHP:  do { $i++; } while ($i < 10);
来源：http://imu.tanke756.top

JS:   do { i++; } while (i < 10);
来源：http://xko.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://wqp.chenlongwang.top

Java: do { i++; } while (i < 10);
来源：http://xek.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uuu.hfpthk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qce.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://ydg.shuidangran.top

[B09] break 与 continue
来源：http://iaq.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zcd.xuanzx.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ivk.bjfxy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ehz.sxryk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nzm.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yeo.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://swv.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fnb.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qkh.shanyushiyangkeji.top

[B10] 遍历同时拿索引
来源：http://bem.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://djt.wangshuangyany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ziy.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wab.dianchejie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hvm.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wve.redwolf501.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wib.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://waj.xziqi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mhh.hywenlv.cn

[B11] 生成数字序列 / 区间
来源：http://ytr.jlsjyb.cn

Py:   list(range(0, 10, 2))
来源：http://dbz.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://ezp.jqgufenzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rsm.gogol.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://umu.hfpthk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nyj.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vup.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://cdr.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://awo.tian-w.cn

[B12] 跳出多层循环
来源：http://wbj.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pjo.shangyingyoupin.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://afw.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cwp.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://reh.yj20258888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hmp.uphjek.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mhf.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ymg.sweek.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://arp.0kj1m.cn

[B13] 判断是否为数字
来源：http://gzc.fehbvm.com

Py:   isinstance(x, (int, float))
来源：http://tie.xinyue.icu

PHP:  is_numeric($x)
来源：http://tiz.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zgx.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://usd.jqgufenzy.top

Java: x instanceof Number
来源：http://oas.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bwu.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://uwk.shuidangran.top

C#:   x is int or double or decimal
来源：http://wtm.daria6918.cn

[B14] 判断值是否在集合内
来源：http://dgb.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kul.cheryme.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mab.yj202588.top

JS:   [1, 2, 3].includes(x)
来源：http://nli.sxryk.cn

TS:   [1, 2, 3].includes(x)
来源：http://zgj.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yvw.jqgfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jsd.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://eai.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ibt.cucudq.cn

[B15] 布尔运算与取反
来源：http://ulb.ywan-chungtsiang.top

Py:   a and b or not c
来源：http://yiz.ydzc1.top

PHP:  $a && $b || !$c
来源：http://rwa.quarkkingdee.top

JS:   a && b || !c
来源：http://yux.shangyingyoupin.top

TS:   a && b || !c
来源：http://obr.zhengqikj.top

Java: a && b || !c
来源：http://tae.shangyingyoupin.top

Go:   a && b || !c
来源：http://wag.daxiang520.top

Ruby: a && b || !c
来源：http://qcg.jinyuanbaomall.cn

C#:   a && b || !c
来源：http://jeu.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://wdh.daxiang520.top

Py:   if not data: return
来源：http://tbp.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://mke.sweek.top

JS:   if (!data) return;
来源：http://ymf.yvedp.cn

TS:   if (!data) return;
来源：http://pbi.shangyingyoupin.top

Java: if (data == null) return;
来源：http://ylj.ydjk.org.cn

Go:   if data == nil { return }
来源：http://ioo.daria6918.cn

Ruby: return if data.nil?
来源：http://plb.ppjwa.cn

C#:   if (data == null) return;
来源：http://dhs.yj20258888.top

================================================================================
来源：http://gsu.epnwcf.com

C. 函数与作用域
来源：http://muv.zhixingplan.top

================================================================================
来源：http://peu.yj20258888.top

[C01] 定义函数
来源：http://yov.epnwcf.com


<!-- 参考信息 -->