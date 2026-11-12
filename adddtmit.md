代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uyw.gogol.net.cn

Java: new Random().nextInt(100) + 1
来源：http://afa.yuanzhike.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xln.sweek.top

Ruby: rand(1..100)
来源：http://jyi.9152youxi.cn

C#:   new Random().Next(1, 101)
来源：http://mue.sysykeji.top

[A11] 条件表达式（三元）
来源：http://glp.jlsjyb.cn

Py:   "yes" if x > 0 else "no"
来源：http://gdp.jqgfzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mdq.zhengqikj.top

JS:   x > 0 ? "yes" : "no"
来源：http://fue.birdmap.top

TS:   x > 0 ? "yes" : "no"
来源：http://xhm.dianchejie.cn

Java: x > 0 ? "yes" : "no"
来源：http://atd.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kxe.yuanzhike.top

Ruby: x > 0 ? "yes" : "no"
来源：http://yfy.shuidangran.top

C#:   x > 0 ? "yes" : "no"
来源：http://tle.guowangkeji.top

[A12] 字符串插值 / 格式化
来源：http://hds.gogol.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hpx.sysykeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pmk.ydzc1.top

JS:   `Hello, ${name}!`
来源：http://bmv.hnxiangtu.top

TS:   `Hello, ${name}!`
来源：http://wgh.nanxuanxn.top

Java: "Hello, %s!".formatted(name)
来源：http://bjc.vqdsnc.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wel.xingfuxueyuan.xyz

Ruby: "Hello, #{name}!"
来源：http://sxb.nanxuanxn.top

C#:   $"Hello, {name}!"
来源：http://luk.hcnkem.com

[A13] 多行字符串（练习 \n 转义）
来源：http://inc.fzhhl.top

Py:   "第一行\n第二行"
来源：http://kgs.ivvv.top

PHP:  "第一行\n第二行"
来源：http://tre.jinghuilouyu.cn

JS:   "第一行\n第二行"
来源：http://ibo.tarul.cn

TS:   "第一行\n第二行"
来源：http://lhg.cqqwz.cn

Java: "第一行\n第二行"
来源：http://atc.xuetiantiany.cn

Go:   "第一行\n第二行"
来源：http://jhx.0kj1m.cn

Ruby: "第一行\n第二行"
来源：http://ogo.gzhubu.top

C#:   "第一行\n第二行"
来源：http://gew.hcnkem.com

[A14] 注释写法
来源：http://yia.wangshuangyany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://whf.tarul.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wdm.jqgfzy.top

JS:   // 单行；/* 多行 */
来源：http://pzz.yuanzhike.top

TS:   // 单行；/* 多行 */
来源：http://cjw.jyoumei.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lxm.ctjpmb.com

Go:   // 单行；/* 多行 */
来源：http://fur.quarkkingdee.top

Ruby: # 单行；=begin 多行 =end
来源：http://jof.ctjpmb.com

C#:   // 单行；/* 多行 */
来源：http://ojl.yangfankeji.com

[A15] 空值判断与默认值
来源：http://cmq.jinqigufen.top

Py:   value = data or "默认值"
来源：http://jzr.yueranfly.top

PHP:  $value = $data ?? "默认值";
来源：http://egz.sxryk.cn

JS:   const value = data ?? "默认值";
来源：http://fcm.snrcjt.cn

TS:   const value = data ?? "默认值";
来源：http://gip.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mbx.shangyingyoupin.top

Go:   if data == "" { data = "默认值" }
来源：http://ajy.xylfe.cn

Ruby: value = data || "默认值"
来源：http://atv.fktsv.cn

C#:   var value = data ?? "默认值";
来源：http://pfy.cashguo.top

[A16] 真假值判断规则
来源：http://jgs.zhijiandao.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gok.dashuyun.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xtd.9152youxi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cth.yongpay.top

TS:   if (!x) {}
来源：http://fqp.uphjek.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hbs.smart0.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qmw.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://uvy.zycfv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uzu.cucudq.cn

[A17] 位运算
来源：http://whi.guowangkeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ylb.zhixingplan.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gtq.9152youxi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mjq.svipenyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lsb.svipenyu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nlo.sufxvd.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oxs.cucudq.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ank.birdmap.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gwt.jinyuanbaomall.cn

[A18] 字符与 ASCII 码互转
来源：http://jfo.andypj.xyz

Py:   ord("A"); chr(65)
来源：http://iec.52xcode.cn

PHP:  ord("A"); chr(65)
来源：http://krd.pycfn.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://inb.shangyingyoupin.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yrx.mhx1999.top

Java: (int) 'A'; (char) 65
来源：http://aah.dashuyun.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rbl.vehdjk.com

Ruby: "A".ord; 65.chr
来源：http://iuz.nanxinkj.top

C#:   (int)'A'; (char)65
来源：http://bja.jinqigufen.top

[A19] 交换两个变量
来源：http://ehc.dianchejie.cn

Py:   a, b = b, a
来源：http://cqn.chenzaomai.com

PHP:  [$a, $b] = [$b, $a];
来源：http://wbw.bjfxy.top

JS:   [a, b] = [b, a];
来源：http://lvx.ehwqpu.com

TS:   [a, b] = [b, a];
来源：http://aip.ydjk.org.cn

Java: int t = a; a = b; b = t;
来源：http://zlv.xuanzx.com

Go:   a, b = b, a
来源：http://lxz.cheryme.top

Ruby: a, b = b, a
来源：http://bnm.guannengcc.top

C#:   (a, b) = (b, a);
来源：http://yab.shanyushiyangtech.top

[A20] 读取标准输入
来源：http://qhm.ivvv.top

Py:   name = input("请输入：")
来源：http://wzr.guowangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://cwx.fktsv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eit.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://rjk.hesvh.cn

Java: new Scanner(System.in).nextLine()
来源：http://wkd.dashuyun.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mpb.cqqwz.cn

Ruby: gets.chomp
来源：http://rbc.ppjwa.cn

C#:   Console.ReadLine();
来源：http://ozq.xingfuxueyuan.xyz

[A21] 保留指定小数位输出
来源：http://nbe.shangyingyoupin.top

Py:   f"{3.14159:.2f}"
来源：http://nlk.tianlin.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pls.iojbl.cn

JS:   (3.14159).toFixed(2)
来源：http://oiq.yuxming.cn

TS:   (3.14159).toFixed(2)
来源：http://jfj.epnwcf.com

Java: String.format("%.2f", 3.14159)
来源：http://ndy.hysaishi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cgd.zhoulong.xyz

Ruby: format("%.2f", 3.14159)
来源：http://qfv.bjfxy.top

C#:   3.14159.ToString("F2")
来源：http://qqa.yangfankeji.com

[A22] 获取字符串长度
来源：http://rla.yj202588.top

Py:   len(s)
来源：http://lkm.yuanzhike.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nku.jqgfzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bag.shuidangran.top

TS:   s.length
来源：http://ljg.aizwys.cn

Java: s.length()
来源：http://rdl.uphjek.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eqh.chenzaomai.com

Ruby: s.length
来源：http://xxi.bjfxy.top

C#:   s.Length
来源：http://noh.52xcode.cn

[A23] 大小写转换
来源：http://wcx.epnwcf.com

Py:   s.upper(); s.lower(); s.title()
来源：http://bac.jinqigfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zyi.xingfuxueyuan.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yft.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://glk.yj20258.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ffi.tanke756.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sou.hfpthk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qln.daxiang520.top

C#:   s.ToUpper(); s.ToLower()
来源：http://afu.bbcook.cn

[A24] 去除首尾空白
来源：http://rbi.nwbrower.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xkc.cashguo.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ijb.epnwcf.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mcb.xuanzx.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ifn.vqdsnc.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yms.hnxiangtu.top

Go:   strings.TrimSpace(s)
来源：http://kia.andypj.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lid.yanxiufei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zzk.ehwqpu.com

[A25] 字符串比较
来源：http://nwu.zycfv.cn

Py:   s1 == s2; s1 != s2
来源：http://jmk.jinqigfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kmx.zhongyouzk.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://umk.aibaodan.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jki.hesvh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fnr.gotoacloud.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://flw.aizwys.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://juc.fktsv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xeb.daxiang520.top

[A26] 类型转换总览
来源：http://scz.aizwys.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://swx.hfpthk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eqt.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fqy.ywan-chungtsiang.top

TS:   Number() String() Boolean() x as number
来源：http://ttz.andypj.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vim.zhongyouzk.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bzi.chenlongwang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://axu.sysykeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gav.daria6918.cn

================================================================================
来源：http://jje.wangshuangyany.cn

B. 流程控制
来源：http://kuw.xylfe.cn

================================================================================
来源：http://afk.nwbrower.top

[B01] 条件判断 if / else
来源：http://dzi.yanxiufei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vch.52xcode.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qdj.yanxiufei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mgf.iojbl.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tva.fktsv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mgt.9152youxi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://utz.fanxiaobao.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yao.316326.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vvj.yongpay.top

[B02] 多分支 else if / elif
来源：http://ciq.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://otc.yonumen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zaj.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qsm.gogol.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dkj.zdqjudy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hph.xuetiantiany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uos.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kdv.xziqi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sgk.316326.xyz

[B03] switch / match / case
来源：http://ctx.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qvj.fzhhl.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cft.zhijiandao.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lnq.pycfn.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://udg.yanxiufei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mtp.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oxr.yfazqb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cfu.sxryk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ovo.jiagoushi.top

[B04] for 计数循环
来源：http://rzv.fzhhl.top

Py:   for i in range(10): print(i)
来源：http://sek.ctjpmb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jdw.ctjpmb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mak.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ytl.yanxiufei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ekv.0kj1m.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wed.xingfuxueyuan.xyz

Ruby: 10.times { |i| puts i }
来源：http://otx.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fuo.zhengqikj.top

[B05] 遍历数组 / 列表
来源：http://tnb.nanxuanxn.top

Py:   for item in arr: print(item)
来源：http://enw.hywenlv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://apv.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mhu.gaohongyu789.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wpm.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yjd.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uhp.yuxming.cn

Ruby: arr.each { |item| puts item }
来源：http://uwt.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bep.quarkkingdee.top

[B06] 遍历字典 / 对象
来源：http://zxg.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zgh.zdbjq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://upc.yueranfly.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dct.yj20258888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oxa.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://phh.haohaochexian.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rlb.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fib.yj20258.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yoe.jinqigfzy.top

[B07] while 循环
来源：http://dux.cqqwz.cn

Py:   while i < 10: i += 1
来源：http://rfj.316326.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://pve.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://apf.smart0.xyz

TS:   while (i < 10) { i++; }
来源：http://nas.yonumen.top

Java: while (i < 10) { i++; }
来源：http://kgf.fanxiaobao.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uby.zhaomingkeji.xyz

Ruby: while i < 10; i += 1; end
来源：http://set.birdmap.top

C#:   while (i < 10) { i++; }
来源：http://kkj.gotoacloud.top

[B08] do-while（至少执行一次）
来源：http://dnk.dianchejie.cn

Py:   # 无 do-while：用 while True + break
来源：http://hkb.zhijiandao.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yhv.nwbrower.top

JS:   do { i++; } while (i < 10);
来源：http://fjw.yonumen.top

TS:   do { i++; } while (i < 10);
来源：http://yaj.c1oappe.top

Java: do { i++; } while (i < 10);
来源：http://xnp.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tsn.dashuyun.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pwb.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://pai.bbcook.cn

[B09] break 与 continue
来源：http://bon.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://heo.vqdsnc.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://msx.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sux.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kyk.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uif.zycfv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dsc.shanyushiyangtech.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zjd.shanyushiyangtech.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mwf.ppjwa.cn

[B10] 遍历同时拿索引
来源：http://prh.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://njj.iojbl.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pwc.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xxf.ivvv.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lvh.ywan-chungtsiang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tbh.sysykeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dws.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kxf.jinqigfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kve.ehwqpu.com

[B11] 生成数字序列 / 区间
来源：http://dqn.xylfe.cn

Py:   list(range(0, 10, 2))
来源：http://bes.zhijiandao.cn

PHP:  range(0, 10, 2);
来源：http://hcs.jiagoushi.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rpa.sxryk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bzg.cucudq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oky.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://psd.birdmap.top

Ruby: (0...10).step(2).to_a
来源：http://cun.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wwh.fktsv.cn

[B12] 跳出多层循环
来源：http://uen.uphjek.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://hyu.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://str.iojbl.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ngk.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rog.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wgm.wangdashe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tnc.vehdjk.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vnw.chenjidiqi.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://izy.aizwys.cn

[B13] 判断是否为数字
来源：http://tkq.fehbvm.com

Py:   isinstance(x, (int, float))
来源：http://hrb.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://zsk.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xeq.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rie.nwbrower.top

Java: x instanceof Number
来源：http://rgq.bjfxy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qsv.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://clb.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://okm.ydjk.org.cn

[B14] 判断值是否在集合内
来源：http://zri.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cul.316326.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://maj.guowangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://wga.cqqwz.cn

TS:   [1, 2, 3].includes(x)
来源：http://ccs.yuanzhike.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mzf.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gxt.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://gwm.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xwu.snrcjt.cn

[B15] 布尔运算与取反
来源：http://vae.dianchejie.cn

Py:   a and b or not c
来源：http://rud.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://qao.xziqi.cn

JS:   a && b || !c
来源：http://vwp.ydzc1.top

TS:   a && b || !c
来源：http://mou.yj20258888.top

Java: a && b || !c
来源：http://xoq.jlsjyb.cn

Go:   a && b || !c
来源：http://dal.haohaochexian.top

Ruby: a && b || !c
来源：http://eeo.nanxinkj.top

C#:   a && b || !c
来源：http://hjg.tarul.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yje.xinyue.icu

Py:   if not data: return
来源：http://puv.hammf.cn

PHP:  if (!$data) { return; }
来源：http://sqb.zdqjudy.top

JS:   if (!data) return;
来源：http://isj.fehbvm.com

TS:   if (!data) return;
来源：http://zpt.feifeiyinyue.top

Java: if (data == null) return;
来源：http://yeq.cashguo.top

Go:   if data == nil { return }
来源：http://rkp.guannengcc.top

Ruby: return if data.nil?
来源：http://izm.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://slm.cashguo.top

================================================================================
来源：http://nfl.pycfn.com

C. 函数与作用域
来源：http://ylo.jinyuanbaomall.cn

================================================================================
来源：http://wbd.ydjk.org.cn

[C01] 定义函数
来源：http://emb.smart0.xyz


<!-- 参考信息 -->