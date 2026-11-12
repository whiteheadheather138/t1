代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wxn.hesvh.cn

Java: new Random().nextInt(100) + 1
来源：http://eio.9152youxi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://exl.jinqigfzy.top

Ruby: rand(1..100)
来源：http://ail.gogol.net.cn

C#:   new Random().Next(1, 101)
来源：http://wyw.hnxiangtu.top

[A11] 条件表达式（三元）
来源：http://jlq.chenjidiqi.icu

Py:   "yes" if x > 0 else "no"
来源：http://jly.haohaochexian.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://sov.zdbjq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pyv.ppjwa.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kxs.hesvh.cn

Java: x > 0 ? "yes" : "no"
来源：http://goo.vehdjk.com

Go:   // 无三元运算符，需用 if 语句
来源：http://qru.yanxiufei.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dij.zhiwuduotai.top

C#:   x > 0 ? "yes" : "no"
来源：http://zce.316326.xyz

[A12] 字符串插值 / 格式化
来源：http://ega.vqdsnc.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wtm.zdqjudy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xmb.yj20258.top

JS:   `Hello, ${name}!`
来源：http://atj.tanke756.top

TS:   `Hello, ${name}!`
来源：http://erb.yj20258.top

Java: "Hello, %s!".formatted(name)
来源：http://szw.sufxvd.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://act.hfpthk.cn

Ruby: "Hello, #{name}!"
来源：http://jyp.zhixingplan.top

C#:   $"Hello, {name}!"
来源：http://zjn.ydzc1.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dbq.xziqi.cn

Py:   "第一行\n第二行"
来源：http://zlz.jqgufenzy.top

PHP:  "第一行\n第二行"
来源：http://rrm.gotoacloud.top

JS:   "第一行\n第二行"
来源：http://obm.hywenlv.cn

TS:   "第一行\n第二行"
来源：http://jyl.zdqjudy.top

Java: "第一行\n第二行"
来源：http://rlf.zhijiandao.cn

Go:   "第一行\n第二行"
来源：http://fax.dianchejie.cn

Ruby: "第一行\n第二行"
来源：http://lio.jinqigfzy.top

C#:   "第一行\n第二行"
来源：http://tty.gzhubu.top

[A14] 注释写法
来源：http://ylv.wangdashe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://oki.ywan-chungtsiang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://efu.ctjpmb.com

JS:   // 单行；/* 多行 */
来源：http://kzp.guannengcc.top

TS:   // 单行；/* 多行 */
来源：http://pup.hongshengwenyu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vmb.aizwys.cn

Go:   // 单行；/* 多行 */
来源：http://wpq.havefunace.top

Ruby: # 单行；=begin 多行 =end
来源：http://yei.c1oappe.top

C#:   // 单行；/* 多行 */
来源：http://pdi.yfazqb.com

[A15] 空值判断与默认值
来源：http://usq.jyoumei.cn

Py:   value = data or "默认值"
来源：http://fiy.daxiang520.top

PHP:  $value = $data ?? "默认值";
来源：http://wtk.shuidangran.top

JS:   const value = data ?? "默认值";
来源：http://zke.gogol.net.cn

TS:   const value = data ?? "默认值";
来源：http://mhc.shuidangran.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://csu.c1oappe.top

Go:   if data == "" { data = "默认值" }
来源：http://myy.sxryk.cn

Ruby: value = data || "默认值"
来源：http://nrp.redwolf501.top

C#:   var value = data ?? "默认值";
来源：http://uoe.aizwys.cn

[A16] 真假值判断规则
来源：http://rwf.zhaomingkeji.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rhr.yuxming.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fxx.zhongyouzk.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mbc.yueranfly.top

TS:   if (!x) {}
来源：http://kxz.9152youxi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wxi.wangshuangyany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tyk.shangyingyoupin.top

Ruby: unless x            # nil 与 false 为假
来源：http://abs.haohaochexian.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vkd.gaohongyu789.top

[A17] 位运算
来源：http://dww.meibo888.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hhb.zhiwuduotai.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xuz.chenjidiqi.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bup.fengsongda.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ogy.cashguo.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hsd.xuetiantiany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ndk.fktsv.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zxd.zhengqikj.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fur.sufxvd.cn

[A18] 字符与 ASCII 码互转
来源：http://kak.svipenyu.cn

Py:   ord("A"); chr(65)
来源：http://wex.zdqjudy.top

PHP:  ord("A"); chr(65)
来源：http://rac.sweek.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dat.ydjk.org.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kfe.hnxiangtu.top

Java: (int) 'A'; (char) 65
来源：http://dlj.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jit.jinghuilouyu.cn

Ruby: "A".ord; 65.chr
来源：http://ruf.xuetiantiany.cn

C#:   (int)'A'; (char)65
来源：http://pzz.jinyuanbaomall.cn

[A19] 交换两个变量
来源：http://him.hcnkem.com

Py:   a, b = b, a
来源：http://lve.gzhubu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kvn.yueranfly.top

JS:   [a, b] = [b, a];
来源：http://xaa.hnxiangtu.top

TS:   [a, b] = [b, a];
来源：http://qqf.hnqzz.top

Java: int t = a; a = b; b = t;
来源：http://haj.dashuyun.cn

Go:   a, b = b, a
来源：http://enp.jinghuilouyu.cn

Ruby: a, b = b, a
来源：http://ybf.nwbrower.top

C#:   (a, b) = (b, a);
来源：http://rjz.tian-w.cn

[A20] 读取标准输入
来源：http://iuw.yj202588.top

Py:   name = input("请输入：")
来源：http://oul.yuxming.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rff.tianlin.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://asv.meibo888.top

TS:   // Node.js：readline 模块
来源：http://ahb.ivvv.top

Java: new Scanner(System.in).nextLine()
来源：http://oow.chenlongwang.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ulx.sufxvd.cn

Ruby: gets.chomp
来源：http://gwc.gaohongyu789.top

C#:   Console.ReadLine();
来源：http://evf.yj202588.top

[A21] 保留指定小数位输出
来源：http://rfp.dashuyun.cn

Py:   f"{3.14159:.2f}"
来源：http://wwh.cdnleiting.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qit.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://vdv.uphjek.com

TS:   (3.14159).toFixed(2)
来源：http://ula.meibo888.top

Java: String.format("%.2f", 3.14159)
来源：http://vxm.zycfv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://clr.fzhhl.top

Ruby: format("%.2f", 3.14159)
来源：http://mpd.ivvv.top

C#:   3.14159.ToString("F2")
来源：http://iht.dashuyun.cn

[A22] 获取字符串长度
来源：http://aex.hfpthk.cn

Py:   len(s)
来源：http://mve.tarul.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qnw.ydjk.org.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qji.zhaomingkeji.xyz

TS:   s.length
来源：http://zvy.shanyushiyangtech.top

Java: s.length()
来源：http://lwz.pycfn.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zta.ehwqpu.com

Ruby: s.length
来源：http://kmq.sweek.top

C#:   s.Length
来源：http://iav.xuetiantiany.cn

[A23] 大小写转换
来源：http://zxs.zhoulong.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://pqv.fehbvm.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ajt.tarul.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pvn.316326.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sga.xziqi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rxg.hcnkem.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tyq.yj20258888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dqc.shangyingyoupin.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qfu.xziqi.cn

[A24] 去除首尾空白
来源：http://igk.haohaochexian.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zkm.hammf.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zvq.cashguo.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wki.dashuyun.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xxy.tian-w.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hlr.dashuyun.cn

Go:   strings.TrimSpace(s)
来源：http://gxw.shanyushiyangtech.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://csc.yangfankeji.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hfy.zhijiandao.cn

[A25] 字符串比较
来源：http://lrx.hnqzz.top

Py:   s1 == s2; s1 != s2
来源：http://irw.0kj1m.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aax.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://npi.vqdsnc.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kfd.ehwqpu.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mad.hywenlv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xbl.sxryk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ldz.daria6918.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ult.chenjidiqi.icu

[A26] 类型转换总览
来源：http://oto.gzhubu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tvf.sxryk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://egs.jyoumei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wzm.pycfn.com

TS:   Number() String() Boolean() x as number
来源：http://niy.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vfr.tarul.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lpn.cheryme.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ynu.yanxiufei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pis.ybcxt.top

================================================================================
来源：http://xen.hnqzz.top

B. 流程控制
来源：http://rpn.hcnkem.com

================================================================================
来源：http://jql.sysykeji.top

[B01] 条件判断 if / else
来源：http://myd.birdmap.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tlx.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lii.52xcode.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lkc.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pmh.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rnv.ppjwa.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rvy.sxryk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://flj.uphjek.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wbk.ehwqpu.com

[B02] 多分支 else if / elif
来源：http://ggt.yongpay.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jho.nanxinkj.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pko.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://svb.jinghuilouyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://apj.tianlin.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bri.sweek.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dfg.smart0.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://elu.jiagoushi.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xqe.sjlbkw.cn

[B03] switch / match / case
来源：http://tot.zdqjudy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://brs.quarkkingdee.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dfm.316326.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://emh.cucudq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://voo.shanyushiyangtech.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bhy.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ggr.iojbl.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ptt.hongshengwenyu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sai.svipenyu.cn

[B04] for 计数循环
来源：http://xdj.jinqigufen.top

Py:   for i in range(10): print(i)
来源：http://huh.bbcook.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qox.cucudq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://urz.tarul.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zkf.cqqwz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jqj.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://trh.sysykeji.top

Ruby: 10.times { |i| puts i }
来源：http://fiz.shzxlz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ihm.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://raf.xinyue.icu

Py:   for item in arr: print(item)
来源：http://tlq.shangyingyoupin.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bzp.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qgl.yueranfly.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dyl.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mdn.cashguo.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tqm.shuidangran.top

Ruby: arr.each { |item| puts item }
来源：http://tmf.aizwys.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ktf.zdqjudy.top

[B06] 遍历字典 / 对象
来源：http://hwm.xuetiantiany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qan.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lzr.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xua.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bdo.haohaochexian.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ydg.nanxinkj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://okd.ppjwa.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hhy.jinyuanbaomall.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cvb.havefunace.top

[B07] while 循环
来源：http://uno.yj20258888.top

Py:   while i < 10: i += 1
来源：http://kmq.jqgufenzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://kno.aibaodan.cn

JS:   while (i < 10) { i++; }
来源：http://akc.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://tld.zdqjudy.top

Java: while (i < 10) { i++; }
来源：http://mbt.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dab.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://qlx.yj202588.top

C#:   while (i < 10) { i++; }
来源：http://pdv.0kj1m.cn

[B08] do-while（至少执行一次）
来源：http://oct.feifeiyinyue.top

Py:   # 无 do-while：用 while True + break
来源：http://azz.nanxinkj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://svi.cdnleiting.top

JS:   do { i++; } while (i < 10);
来源：http://kek.mhx1999.top

TS:   do { i++; } while (i < 10);
来源：http://dhk.sjlbkw.cn

Java: do { i++; } while (i < 10);
来源：http://jbs.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ipn.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pcy.sufxvd.cn

C#:   do { i++; } while (i < 10);
来源：http://whu.zdbjq.cn

[B09] break 与 continue
来源：http://nbj.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bvz.nanxuanxn.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iry.smart0.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xzm.feifeiyinyue.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dgb.fzhhl.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xrd.gaohongyu789.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jip.vehdjk.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jrz.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oyp.guowangkeji.top

[B10] 遍历同时拿索引
来源：http://qtr.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ydt.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jnz.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jag.sufxvd.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ttm.yongpay.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mxk.fanxiaobao.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://woe.nanxuanxn.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fjx.iojbl.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rlu.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://pem.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://vjo.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://gbn.cdnleiting.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://geq.xuetiantiany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zvs.ehwqpu.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gwe.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oat.chenlongwang.top

Ruby: (0...10).step(2).to_a
来源：http://akb.hnqzz.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gop.ydjk.org.cn

[B12] 跳出多层循环
来源：http://lns.gzhubu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://spl.tarul.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vmw.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eup.quarkkingdee.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kwj.316326.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wwg.shzxlz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rzx.havefunace.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hfv.yonumen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wsk.haohaochexian.top

[B13] 判断是否为数字
来源：http://lrn.316326.xyz

Py:   isinstance(x, (int, float))
来源：http://oqv.yangfankeji.com

PHP:  is_numeric($x)
来源：http://thj.zhijiandao.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://itu.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iop.snrcjt.cn

Java: x instanceof Number
来源：http://jki.birdmap.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wen.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://csa.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://fxi.fktsv.cn

[B14] 判断值是否在集合内
来源：http://lrq.tianlin.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qmc.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://spc.jyoumei.cn

JS:   [1, 2, 3].includes(x)
来源：http://fdh.cqqwz.cn

TS:   [1, 2, 3].includes(x)
来源：http://yru.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kvx.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uzm.sufxvd.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tzu.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xdn.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://jyk.xinyue.icu

Py:   a and b or not c
来源：http://cbj.fehbvm.com

PHP:  $a && $b || !$c
来源：http://nar.yj202588.top

JS:   a && b || !c
来源：http://ktm.cheryme.top

TS:   a && b || !c
来源：http://zmp.yongpay.top

Java: a && b || !c
来源：http://hra.xuanzx.com

Go:   a && b || !c
来源：http://llb.ivvv.top

Ruby: a && b || !c
来源：http://elb.cucudq.cn

C#:   a && b || !c
来源：http://mos.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://yed.cqqwz.cn

Py:   if not data: return
来源：http://uls.tianlin.xyz

PHP:  if (!$data) { return; }
来源：http://mtp.jinqigufen.top

JS:   if (!data) return;
来源：http://hfg.gogol.net.cn

TS:   if (!data) return;
来源：http://ask.xuanzx.com

Java: if (data == null) return;
来源：http://klh.316326.xyz

Go:   if data == nil { return }
来源：http://qgi.xziqi.cn

Ruby: return if data.nil?
来源：http://vbm.kuanghao11.cn

C#:   if (data == null) return;
来源：http://ozd.hesvh.cn

================================================================================
来源：http://zcn.nanxinkj.top

C. 函数与作用域
来源：http://fuo.hnxiangtu.top

================================================================================
来源：http://nsn.chenjidiqi.icu

[C01] 定义函数
来源：http://kvl.zhengqikj.top


<!-- 参考信息 -->