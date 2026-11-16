代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://usj.redwolf501.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hey.sjlbkw.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dbh.havefunace.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wbk.redwolf501.top

[A10] 生成随机数
来源：http://nub.tanke756.top

Py:   import random; random.randint(1, 100)
来源：http://ujp.iojbl.cn

PHP:  random_int(1, 100);
来源：http://phl.pycfn.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kci.52xcode.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dcf.yj20258888.top

Java: new Random().nextInt(100) + 1
来源：http://awj.yvedp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xqs.svipenyu.cn

Ruby: rand(1..100)
来源：http://neg.pycfn.com

C#:   new Random().Next(1, 101)
来源：http://som.jqgufenzy.top

[A11] 条件表达式（三元）
来源：http://qdy.ydzc1.top

Py:   "yes" if x > 0 else "no"
来源：http://jrr.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sny.9152youxi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://frg.sysykeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://suz.nanxuanxn.top

Java: x > 0 ? "yes" : "no"
来源：http://ubv.hesvh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xhd.cucudq.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tdl.zhiwuduotai.top

C#:   x > 0 ? "yes" : "no"
来源：http://zhp.vqdsnc.cn

[A12] 字符串插值 / 格式化
来源：http://tps.yvedp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wka.gaohongyu789.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kof.jyoumei.cn

JS:   `Hello, ${name}!`
来源：http://dos.chenlongwang.top

TS:   `Hello, ${name}!`
来源：http://jgf.smart0.xyz

Java: "Hello, %s!".formatted(name)
来源：http://odp.jinghuilouyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://crt.aizwys.cn

Ruby: "Hello, #{name}!"
来源：http://xrw.chenlongwang.top

C#:   $"Hello, {name}!"
来源：http://xoh.chenlongwang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://nfc.jinghuilouyu.cn

Py:   "第一行\n第二行"
来源：http://yyh.fengsongda.top

PHP:  "第一行\n第二行"
来源：http://slt.xinyue.icu

JS:   "第一行\n第二行"
来源：http://ooe.mhx1999.top

TS:   "第一行\n第二行"
来源：http://tje.gzhubu.top

Java: "第一行\n第二行"
来源：http://sid.haohaochexian.top

Go:   "第一行\n第二行"
来源：http://nlr.svipenyu.cn

Ruby: "第一行\n第二行"
来源：http://dhx.zhiwuduotai.top

C#:   "第一行\n第二行"
来源：http://olr.yj20258.top

[A14] 注释写法
来源：http://pvs.snrcjt.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kxx.ydzc1.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wgf.ydjk.org.cn

JS:   // 单行；/* 多行 */
来源：http://hpi.dianchejie.cn

TS:   // 单行；/* 多行 */
来源：http://zgq.guannengcc.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xec.xuanzx.com

Go:   // 单行；/* 多行 */
来源：http://euk.jyoumei.cn

Ruby: # 单行；=begin 多行 =end
来源：http://iio.sjlbkw.cn

C#:   // 单行；/* 多行 */
来源：http://sbg.shuidangran.top

[A15] 空值判断与默认值
来源：http://orb.nanxuanxn.top

Py:   value = data or "默认值"
来源：http://nvv.guowangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://dqs.zhoulong.xyz

JS:   const value = data ?? "默认值";
来源：http://wxb.hnxiangtu.top

TS:   const value = data ?? "默认值";
来源：http://unc.316326.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ixj.hnxiangtu.top

Go:   if data == "" { data = "默认值" }
来源：http://xfg.zhixingplan.top

Ruby: value = data || "默认值"
来源：http://cxh.ybcxt.top

C#:   var value = data ?? "默认值";
来源：http://uxu.ydjk.org.cn

[A16] 真假值判断规则
来源：http://ioi.tianlin.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vho.jinqigufen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fnd.redwolf501.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jwp.gogol.net.cn

TS:   if (!x) {}
来源：http://ndv.chenlongwang.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vmp.bbcook.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ncn.nanxinkj.top

Ruby: unless x            # nil 与 false 为假
来源：http://jfp.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ykc.ywan-chungtsiang.top

[A17] 位运算
来源：http://lsl.tian-w.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jrf.hcnkem.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fvm.zdbjq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://znx.sweek.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qcg.ywan-chungtsiang.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yqn.yj20258.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tji.jyoumei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ukm.ydzc1.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tua.yj20258.top

[A18] 字符与 ASCII 码互转
来源：http://ayt.yj20258.top

Py:   ord("A"); chr(65)
来源：http://dih.epnwcf.com

PHP:  ord("A"); chr(65)
来源：http://oun.gotoacloud.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nln.hywenlv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dgr.shangyingyoupin.top

Java: (int) 'A'; (char) 65
来源：http://frn.shangyingyoupin.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qyw.zdbjq.cn

Ruby: "A".ord; 65.chr
来源：http://xwz.shanyushiyangtech.top

C#:   (int)'A'; (char)65
来源：http://bcp.yj202588.top

[A19] 交换两个变量
来源：http://drb.sjlbkw.cn

Py:   a, b = b, a
来源：http://fzk.tanke756.top

PHP:  [$a, $b] = [$b, $a];
来源：http://azf.hnqzz.top

JS:   [a, b] = [b, a];
来源：http://jlx.haohaochexian.top

TS:   [a, b] = [b, a];
来源：http://rdu.316326.xyz

Java: int t = a; a = b; b = t;
来源：http://nzh.yj20258888.top

Go:   a, b = b, a
来源：http://lid.xinyue.icu

Ruby: a, b = b, a
来源：http://tii.ivvv.top

C#:   (a, b) = (b, a);
来源：http://ggg.chenzaomai.com

[A20] 读取标准输入
来源：http://tzt.zhiwuduotai.top

Py:   name = input("请输入：")
来源：http://ncx.shanyushiyangtech.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vbe.zdqjudy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ndw.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://cnb.yfazqb.com

Java: new Scanner(System.in).nextLine()
来源：http://yyn.cashguo.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kzx.jqgfzy.top

Ruby: gets.chomp
来源：http://ovi.guowangkeji.top

C#:   Console.ReadLine();
来源：http://nam.nanxuanxn.top

[A21] 保留指定小数位输出
来源：http://qje.yangfankeji.com

Py:   f"{3.14159:.2f}"
来源：http://las.meibo888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ioq.xuanzx.com

JS:   (3.14159).toFixed(2)
来源：http://yfx.zycfv.cn

TS:   (3.14159).toFixed(2)
来源：http://kkr.quarkkingdee.top

Java: String.format("%.2f", 3.14159)
来源：http://qhr.pengpengdd.cyou

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vcu.uphjek.com

Ruby: format("%.2f", 3.14159)
来源：http://nnp.jinqigufen.top

C#:   3.14159.ToString("F2")
来源：http://etd.andypj.xyz

[A22] 获取字符串长度
来源：http://fqg.chenjidiqi.icu

Py:   len(s)
来源：http://yoc.jianghu66.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cdd.birdmap.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vsc.0kj1m.cn

TS:   s.length
来源：http://hju.ivvv.top

Java: s.length()
来源：http://otf.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yml.meibo888.top

Ruby: s.length
来源：http://zgn.yuanzhike.top

C#:   s.Length
来源：http://vjq.yj20258.top

[A23] 大小写转换
来源：http://ucu.dashuyun.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://eha.jlsjyb.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qnk.shanyushiyangtech.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kub.yuxming.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qfe.smart0.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://toc.yuanzhike.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qkd.guowangkeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://phq.yj20258888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mgz.zhongyouzk.top

[A24] 去除首尾空白
来源：http://vqp.iojbl.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pcx.gotoacloud.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hdb.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hya.nwbrower.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vbc.sufxvd.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cva.shangyingyoupin.top

Go:   strings.TrimSpace(s)
来源：http://tfg.guowangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xxz.hongshengwenyu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zml.tanke756.top

[A25] 字符串比较
来源：http://ghy.andypj.xyz

Py:   s1 == s2; s1 != s2
来源：http://khi.nanxuanxn.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vmt.fehbvm.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ccw.yueranfly.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lmi.yongpay.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://php.jiagoushi.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mnl.smart0.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://caf.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ikp.yvedp.cn

[A26] 类型转换总览
来源：http://aph.yuanzhike.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mru.hfpthk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://psf.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dar.zhoulong.xyz

TS:   Number() String() Boolean() x as number
来源：http://dan.zhiwuduotai.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iiv.yonumen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yft.tian-w.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ipg.hesvh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dnm.jinqigufen.top

================================================================================
来源：http://hkb.jyoumei.cn

B. 流程控制
来源：http://tqf.gaohongyu789.top

================================================================================
来源：http://rmf.tianlin.xyz

[B01] 条件判断 if / else
来源：http://zwi.daxiang520.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tuq.tanke756.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dyo.chenlongwang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ozj.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://npd.fanxiaobao.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://gch.birdmap.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gev.0kj1m.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jfn.iojbl.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fse.cqqwz.cn

[B02] 多分支 else if / elif
来源：http://bvy.shzxlz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ztg.xinyue.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pcq.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zqo.wangdashe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nmt.daxiang520.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bxr.yvedp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ucy.quarkkingdee.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rqs.yanxiufei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ykv.snrcjt.cn

[B03] switch / match / case
来源：http://lah.zhaomingkeji.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qdj.yj20258888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://egf.ydzc1.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ort.gogol.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rxu.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qnq.yonumen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ljm.hfpthk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ycu.sxryk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qxa.bbcook.cn

[B04] for 计数循环
来源：http://lie.bbcook.cn

Py:   for i in range(10): print(i)
来源：http://hen.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bms.shzxlz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iml.chenlongwang.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ebt.jinqigfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rxi.jianghu66.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://erv.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://qji.tanke756.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nlj.fanxiaobao.xyz

[B05] 遍历数组 / 列表
来源：http://myk.jinyuanbaomall.cn

Py:   for item in arr: print(item)
来源：http://kna.jinghuilouyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hol.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hdz.pengpengdd.cyou

TS:   for (const item of arr) { console.log(item); }
来源：http://vnj.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gmc.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tqb.hysaishi.cn

Ruby: arr.each { |item| puts item }
来源：http://hwb.tian-w.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://erh.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://oul.xuanzx.com

Py:   for k, v in d.items(): print(k, v)
来源：http://uqh.redwolf501.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://urv.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iac.chenlongwang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rho.andypj.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ayk.bjfxy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uge.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ymc.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hih.daxiang520.top

[B07] while 循环
来源：http://caz.hnqzz.top

Py:   while i < 10: i += 1
来源：http://luq.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ymb.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://owr.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://xei.hfpthk.cn

Java: while (i < 10) { i++; }
来源：http://svg.ydjk.org.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yyz.gogol.net.cn

Ruby: while i < 10; i += 1; end
来源：http://xsy.xingfuxueyuan.xyz

C#:   while (i < 10) { i++; }
来源：http://ixv.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://pjo.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://bhb.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fvp.jinyuanbaomall.cn

JS:   do { i++; } while (i < 10);
来源：http://jjp.chenzaomai.com

TS:   do { i++; } while (i < 10);
来源：http://byn.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://wsz.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://afd.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://enz.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://nff.pycfn.com

[B09] break 与 continue
来源：http://jso.shzxlz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mns.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jkp.aibaodan.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yeb.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ivz.cucudq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vro.jiagoushi.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wak.wangdashe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pld.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dqj.cdnleiting.top

[B10] 遍历同时拿索引
来源：http://vnr.hywenlv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://suk.hammf.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://azf.xuetiantiany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kxz.hnqzz.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ykz.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dda.c1oappe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ajc.yuanzhike.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nya.sysykeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xzs.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://wcj.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://lul.cheryme.top

PHP:  range(0, 10, 2);
来源：http://yee.yongpay.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oqn.quarkkingdee.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zyz.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rjt.hongshengwenyu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qti.gogol.net.cn

Ruby: (0...10).step(2).to_a
来源：http://wmg.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ssm.gaohongyu789.top

[B12] 跳出多层循环
来源：http://dea.cheryme.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://whv.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mnw.sxryk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ggt.ehwqpu.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tnt.sweek.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hge.316326.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://waw.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qqi.sysykeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://svx.fehbvm.com

[B13] 判断是否为数字
来源：http://xlc.52xcode.cn

Py:   isinstance(x, (int, float))
来源：http://zxi.guannengcc.top

PHP:  is_numeric($x)
来源：http://rfi.chenjidiqi.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://npw.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oxa.vqdsnc.cn

Java: x instanceof Number
来源：http://ktg.zdbjq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hqg.yfazqb.com

Ruby: x.is_a?(Numeric)
来源：http://tcf.316326.xyz

C#:   x is int or double or decimal
来源：http://fow.aibaodan.cn

[B14] 判断值是否在集合内
来源：http://hkx.jinghuilouyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://caw.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fag.nwbrower.top

JS:   [1, 2, 3].includes(x)
来源：http://mne.fzhhl.top

TS:   [1, 2, 3].includes(x)
来源：http://yzc.hnxiangtu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gxj.chenjidiqi.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ugq.yvedp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tku.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://knb.hcnkem.com

[B15] 布尔运算与取反
来源：http://kmz.0kj1m.cn

Py:   a and b or not c
来源：http://zog.bbcook.cn

PHP:  $a && $b || !$c
来源：http://atu.pengpengdd.cyou

JS:   a && b || !c
来源：http://ewo.zhaomingkeji.xyz

TS:   a && b || !c
来源：http://xbi.gaohongyu789.top

Java: a && b || !c
来源：http://dbc.fanxiaobao.xyz

Go:   a && b || !c
来源：http://fyl.hywenlv.cn

Ruby: a && b || !c
来源：http://nbt.hesvh.cn

C#:   a && b || !c
来源：http://exn.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://nka.yangfankeji.com

Py:   if not data: return
来源：http://msb.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://dpw.xuanzx.com

JS:   if (!data) return;
来源：http://sly.daxiang520.top

TS:   if (!data) return;
来源：http://eti.guowangkeji.top


<!-- 参考信息 -->