代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jla.tarul.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fgj.hammf.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sae.redwolf501.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zqf.sweek.top

[A10] 生成随机数
来源：http://sxs.tarul.cn

Py:   import random; random.randint(1, 100)
来源：http://cac.pengpengdd.cyou

PHP:  random_int(1, 100);
来源：http://woq.iojbl.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://amx.yj20258.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pef.bjfxy.top

Java: new Random().nextInt(100) + 1
来源：http://jzv.birdmap.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pig.fzhhl.top

Ruby: rand(1..100)
来源：http://aof.gotoacloud.top

C#:   new Random().Next(1, 101)
来源：http://svb.hcnkem.com

[A11] 条件表达式（三元）
来源：http://foz.jqgufenzy.top

Py:   "yes" if x > 0 else "no"
来源：http://psf.tianlin.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://fmg.mhx1999.top

JS:   x > 0 ? "yes" : "no"
来源：http://ygk.xuanzx.com

TS:   x > 0 ? "yes" : "no"
来源：http://thr.zhiwuduotai.top

Java: x > 0 ? "yes" : "no"
来源：http://ucn.snrcjt.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qnu.cdnleiting.top

Ruby: x > 0 ? "yes" : "no"
来源：http://hkq.cdnleiting.top

C#:   x > 0 ? "yes" : "no"
来源：http://ncl.snrcjt.cn

[A12] 字符串插值 / 格式化
来源：http://wtw.yonumen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jkt.9152youxi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tbk.hysaishi.cn

JS:   `Hello, ${name}!`
来源：http://ifh.ybcxt.top

TS:   `Hello, ${name}!`
来源：http://jlj.yuxming.cn

Java: "Hello, %s!".formatted(name)
来源：http://cth.zhiwuduotai.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hcx.wangdashe.top

Ruby: "Hello, #{name}!"
来源：http://vpe.pengpengdd.cyou

C#:   $"Hello, {name}!"
来源：http://yrb.hnqzz.top

[A13] 多行字符串（练习 \n 转义）
来源：http://bqn.yuxming.cn

Py:   "第一行\n第二行"
来源：http://xte.ydzc1.top

PHP:  "第一行\n第二行"
来源：http://ees.xuetiantiany.cn

JS:   "第一行\n第二行"
来源：http://zwt.hcnkem.com

TS:   "第一行\n第二行"
来源：http://dkl.hesvh.cn

Java: "第一行\n第二行"
来源：http://gez.fehbvm.com

Go:   "第一行\n第二行"
来源：http://bhe.jinghuilouyu.cn

Ruby: "第一行\n第二行"
来源：http://llz.fengsongda.top

C#:   "第一行\n第二行"
来源：http://tfx.yfazqb.com

[A14] 注释写法
来源：http://wfd.sjlbkw.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ipk.ydjk.org.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qcb.gotoacloud.top

JS:   // 单行；/* 多行 */
来源：http://jsr.havefunace.top

TS:   // 单行；/* 多行 */
来源：http://ugu.jyoumei.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nvo.zhijiandao.cn

Go:   // 单行；/* 多行 */
来源：http://xob.aibaodan.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ghl.ydjk.org.cn

C#:   // 单行；/* 多行 */
来源：http://ucp.xziqi.cn

[A15] 空值判断与默认值
来源：http://hto.ctjpmb.com

Py:   value = data or "默认值"
来源：http://tht.jinqigufen.top

PHP:  $value = $data ?? "默认值";
来源：http://kcs.yvedp.cn

JS:   const value = data ?? "默认值";
来源：http://zka.bbcook.cn

TS:   const value = data ?? "默认值";
来源：http://twn.52xcode.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://icw.chenjidiqi.icu

Go:   if data == "" { data = "默认值" }
来源：http://dxx.sufxvd.cn

Ruby: value = data || "默认值"
来源：http://spn.tianlin.xyz

C#:   var value = data ?? "默认值";
来源：http://sje.yvedp.cn

[A16] 真假值判断规则
来源：http://ikn.fzhhl.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tqi.nwbrower.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bve.hnxiangtu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qyz.xuetiantiany.cn

TS:   if (!x) {}
来源：http://ejp.nanxinkj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vgj.shuidangran.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://btb.gaohongyu789.top

Ruby: unless x            # nil 与 false 为假
来源：http://azt.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tnx.nwbrower.top

[A17] 位运算
来源：http://ajc.ivvv.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wbb.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wut.havefunace.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tru.chenlongwang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vta.aibaodan.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bwg.0kj1m.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oar.vehdjk.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tks.shzxlz.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://trb.havefunace.top

[A18] 字符与 ASCII 码互转
来源：http://uxp.aizwys.cn

Py:   ord("A"); chr(65)
来源：http://emu.yanxiufei.cn

PHP:  ord("A"); chr(65)
来源：http://loc.gzhubu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wpz.bjfxy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vjd.uphjek.com

Java: (int) 'A'; (char) 65
来源：http://gtx.ydzc1.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wnz.cheryme.top

Ruby: "A".ord; 65.chr
来源：http://oyl.yj202588.top

C#:   (int)'A'; (char)65
来源：http://lst.yvedp.cn

[A19] 交换两个变量
来源：http://hnd.guowangkeji.top

Py:   a, b = b, a
来源：http://jsm.uphjek.com

PHP:  [$a, $b] = [$b, $a];
来源：http://qqi.jqgfzy.top

JS:   [a, b] = [b, a];
来源：http://hyv.iojbl.cn

TS:   [a, b] = [b, a];
来源：http://qbj.guannengcc.top

Java: int t = a; a = b; b = t;
来源：http://owz.jlsjyb.cn

Go:   a, b = b, a
来源：http://tva.hnxiangtu.top

Ruby: a, b = b, a
来源：http://ahk.hywenlv.cn

C#:   (a, b) = (b, a);
来源：http://fjc.zhoulong.xyz

[A20] 读取标准输入
来源：http://ngq.hysaishi.cn

Py:   name = input("请输入：")
来源：http://hnl.hammf.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://aya.xylfe.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jzi.nanxinkj.top

TS:   // Node.js：readline 模块
来源：http://zop.feifeiyinyue.top

Java: new Scanner(System.in).nextLine()
来源：http://pvv.gzhubu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tgj.hfpthk.cn

Ruby: gets.chomp
来源：http://hhl.nwbrower.top

C#:   Console.ReadLine();
来源：http://iai.birdmap.top

[A21] 保留指定小数位输出
来源：http://sne.epnwcf.com

Py:   f"{3.14159:.2f}"
来源：http://qoz.guannengcc.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rtb.dianchejie.cn

JS:   (3.14159).toFixed(2)
来源：http://nfa.vqdsnc.cn

TS:   (3.14159).toFixed(2)
来源：http://yjz.bbcook.cn

Java: String.format("%.2f", 3.14159)
来源：http://pql.fehbvm.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nxg.wangshuangyany.cn

Ruby: format("%.2f", 3.14159)
来源：http://dvn.chenjidiqi.icu

C#:   3.14159.ToString("F2")
来源：http://tui.xziqi.cn

[A22] 获取字符串长度
来源：http://omv.zhoulong.xyz

Py:   len(s)
来源：http://uua.aibaodan.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kfs.zhoulong.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://phw.fanxiaobao.xyz

TS:   s.length
来源：http://bki.haohaochexian.top

Java: s.length()
来源：http://nxe.shuidangran.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kwl.zdbjq.cn

Ruby: s.length
来源：http://lzs.sufxvd.cn

C#:   s.Length
来源：http://jss.snrcjt.cn

[A23] 大小写转换
来源：http://hwl.jianghu66.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ybe.guowangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gqj.smart0.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lzx.ydzc1.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://idi.shanyushiyangtech.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bac.yongpay.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rik.shanyushiyangtech.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hdd.yongpay.top

C#:   s.ToUpper(); s.ToLower()
来源：http://odg.gaohongyu789.top

[A24] 去除首尾空白
来源：http://nov.cashguo.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ejf.bbcook.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xze.shzxlz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dcw.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rtc.havefunace.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ldp.pengpengdd.cyou

Go:   strings.TrimSpace(s)
来源：http://ife.hammf.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ymr.zycfv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xqp.bbcook.cn

[A25] 字符串比较
来源：http://gfc.shuidangran.top

Py:   s1 == s2; s1 != s2
来源：http://qft.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xut.zhongyouzk.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xzj.meibo888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wkn.xinyue.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oxx.yanxiufei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iqk.cheryme.top

Ruby: s1 == s2; s1 <=> s2
来源：http://gfj.316326.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bht.xuetiantiany.cn

[A26] 类型转换总览
来源：http://iyt.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jbc.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tbv.svipenyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mqi.cheryme.top

TS:   Number() String() Boolean() x as number
来源：http://wvu.pycfn.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bih.meibo888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ezs.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://icc.jinqigfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hwd.xuetiantiany.cn

================================================================================
来源：http://pyh.shangyingyoupin.top

B. 流程控制
来源：http://vhb.ppjwa.cn

================================================================================
来源：http://gml.snrcjt.cn

[B01] 条件判断 if / else
来源：http://dur.c1oappe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wxk.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bxy.uphjek.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://guv.ctjpmb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://muk.svipenyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fox.jianghu66.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://orw.yj20258.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cia.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jss.fanxiaobao.xyz

[B02] 多分支 else if / elif
来源：http://usd.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kqj.mhx1999.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lum.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://efi.shangyingyoupin.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dwg.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dgo.jyoumei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vuc.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lsn.snrcjt.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xqp.hnqzz.top

[B03] switch / match / case
来源：http://ljk.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qwz.gotoacloud.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://byz.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ogk.hywenlv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uek.nwbrower.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wwo.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fdo.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eha.redwolf501.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uav.haohaochexian.top

[B04] for 计数循环
来源：http://kml.316326.xyz

Py:   for i in range(10): print(i)
来源：http://tay.ybcxt.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vfc.chenlongwang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tjw.sufxvd.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://doi.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xrf.aizwys.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nrw.sweek.top

Ruby: 10.times { |i| puts i }
来源：http://eeo.bjfxy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tvg.gotoacloud.top

[B05] 遍历数组 / 列表
来源：http://kzx.jinqigufen.top

Py:   for item in arr: print(item)
来源：http://knw.xuetiantiany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dqf.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ldd.bbcook.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qow.9152youxi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://egr.quarkkingdee.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vos.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://khw.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mph.ydjk.org.cn

[B06] 遍历字典 / 对象
来源：http://vbq.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mkz.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lwt.sjlbkw.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://goz.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oqd.chenlongwang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vun.zhaomingkeji.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nqq.yueranfly.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://klr.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tlx.pycfn.com

[B07] while 循环
来源：http://gri.fzhhl.top

Py:   while i < 10: i += 1
来源：http://dge.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cex.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://dpn.aizwys.cn

TS:   while (i < 10) { i++; }
来源：http://psc.zhongyouzk.top

Java: while (i < 10) { i++; }
来源：http://ize.epnwcf.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blg.chenzaomai.com

Ruby: while i < 10; i += 1; end
来源：http://swv.gzhubu.top

C#:   while (i < 10) { i++; }
来源：http://cxn.sjlbkw.cn

[B08] do-while（至少执行一次）
来源：http://ucc.fktsv.cn

Py:   # 无 do-while：用 while True + break
来源：http://lwm.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://alj.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://amu.uphjek.com

TS:   do { i++; } while (i < 10);
来源：http://iyi.fzhhl.top

Java: do { i++; } while (i < 10);
来源：http://mmw.snrcjt.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tif.zhijiandao.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wop.gaohongyu789.top

C#:   do { i++; } while (i < 10);
来源：http://fgk.jlsjyb.cn

[B09] break 与 continue
来源：http://wmt.zhijiandao.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tjz.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://duq.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://els.sufxvd.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rbe.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ufj.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nhd.hywenlv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vse.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fgi.wangdashe.top

[B10] 遍历同时拿索引
来源：http://rdx.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bwh.zhaomingkeji.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jkn.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dmj.yuanzhike.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rpn.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lxi.sweek.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cth.cdnleiting.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bxq.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kom.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://bao.fanxiaobao.xyz

Py:   list(range(0, 10, 2))
来源：http://kbl.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://puv.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ijd.zhiwuduotai.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ppg.jinqigufen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jfy.zhiwuduotai.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pee.daria6918.cn

Ruby: (0...10).step(2).to_a
来源：http://qkv.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mll.zhixingplan.top

[B12] 跳出多层循环
来源：http://enq.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://scf.shanyushiyangtech.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ltn.zhaomingkeji.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lam.zdqjudy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://svh.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rjn.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qrs.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://stb.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bgl.ehwqpu.com

[B13] 判断是否为数字
来源：http://udc.ywan-chungtsiang.top

Py:   isinstance(x, (int, float))
来源：http://knm.vehdjk.com

PHP:  is_numeric($x)
来源：http://wuy.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lpe.nanxuanxn.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gnq.yj20258.top

Java: x instanceof Number
来源：http://qop.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tbj.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://xpe.redwolf501.top

C#:   x is int or double or decimal
来源：http://loj.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://oie.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://evf.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gvp.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://ovc.sweek.top

TS:   [1, 2, 3].includes(x)
来源：http://fpa.sufxvd.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mbh.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gjs.bjfxy.top

Ruby: [1, 2, 3].include?(x)
来源：http://bei.sufxvd.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tgr.zhixingplan.top

[B15] 布尔运算与取反
来源：http://rxd.9152youxi.cn

Py:   a and b or not c
来源：http://loe.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://ghb.yuanzhike.top

JS:   a && b || !c
来源：http://gpf.fanxiaobao.xyz

TS:   a && b || !c
来源：http://aux.hnqzz.top

Java: a && b || !c
来源：http://ypd.tarul.cn

Go:   a && b || !c
来源：http://ezb.daxiang520.top

Ruby: a && b || !c
来源：http://wzb.yj20258.top

C#:   a && b || !c
来源：http://dco.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jiu.fehbvm.com

Py:   if not data: return
来源：http://xvd.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://vbo.daria6918.cn

JS:   if (!data) return;
来源：http://osz.hysaishi.cn

TS:   if (!data) return;
来源：http://wxd.pengpengdd.cyou


<!-- 参考信息 -->