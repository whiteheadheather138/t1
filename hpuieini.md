代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rjp.jianghu66.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bju.wangdashe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vci.iojbl.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fcf.meibo888.top

[A10] 生成随机数
来源：http://wkb.jyoumei.cn

Py:   import random; random.randint(1, 100)
来源：http://nlu.birdmap.top

PHP:  random_int(1, 100);
来源：http://rwx.hfpthk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wbj.yj20258888.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fci.fehbvm.com

Java: new Random().nextInt(100) + 1
来源：http://hnf.fanxiaobao.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ylq.guannengcc.top

Ruby: rand(1..100)
来源：http://msk.tanke756.top

C#:   new Random().Next(1, 101)
来源：http://vyj.snrcjt.cn

[A11] 条件表达式（三元）
来源：http://cor.fanxiaobao.xyz

Py:   "yes" if x > 0 else "no"
来源：http://mam.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://oyn.uphjek.com

JS:   x > 0 ? "yes" : "no"
来源：http://cix.xuetiantiany.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uqz.yj202588.top

Java: x > 0 ? "yes" : "no"
来源：http://zmb.andypj.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://qxt.aizwys.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xyq.sjlbkw.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bca.haohaochexian.top

[A12] 字符串插值 / 格式化
来源：http://wop.jinghuilouyu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pea.sweek.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rhg.dashuyun.cn

JS:   `Hello, ${name}!`
来源：http://ygu.316326.xyz

TS:   `Hello, ${name}!`
来源：http://wjr.hysaishi.cn

Java: "Hello, %s!".formatted(name)
来源：http://vfw.jlsjyb.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wbv.vqdsnc.cn

Ruby: "Hello, #{name}!"
来源：http://ewb.iojbl.cn

C#:   $"Hello, {name}!"
来源：http://juc.snrcjt.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pnj.bbcook.cn

Py:   "第一行\n第二行"
来源：http://nvi.fktsv.cn

PHP:  "第一行\n第二行"
来源：http://bez.zhiwuduotai.top

JS:   "第一行\n第二行"
来源：http://vpd.meibo888.top

TS:   "第一行\n第二行"
来源：http://exd.yangfankeji.com

Java: "第一行\n第二行"
来源：http://wfy.guowangkeji.top

Go:   "第一行\n第二行"
来源：http://wep.pengpengdd.cyou

Ruby: "第一行\n第二行"
来源：http://jiv.tanke756.top

C#:   "第一行\n第二行"
来源：http://ylg.uphjek.com

[A14] 注释写法
来源：http://vwy.zhixingplan.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://hkq.yvedp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ghq.guannengcc.top

JS:   // 单行；/* 多行 */
来源：http://nto.hcnkem.com

TS:   // 单行；/* 多行 */
来源：http://slg.hongshengwenyu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ixm.fengsongda.top

Go:   // 单行；/* 多行 */
来源：http://tun.xylfe.cn

Ruby: # 单行；=begin 多行 =end
来源：http://upq.fktsv.cn

C#:   // 单行；/* 多行 */
来源：http://auz.zhoulong.xyz

[A15] 空值判断与默认值
来源：http://vma.yvedp.cn

Py:   value = data or "默认值"
来源：http://xwq.xingfuxueyuan.xyz

PHP:  $value = $data ?? "默认值";
来源：http://vlw.mhx1999.top

JS:   const value = data ?? "默认值";
来源：http://lwu.jyoumei.cn

TS:   const value = data ?? "默认值";
来源：http://ssu.snrcjt.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nlv.sweek.top

Go:   if data == "" { data = "默认值" }
来源：http://osh.smart0.xyz

Ruby: value = data || "默认值"
来源：http://npj.guannengcc.top

C#:   var value = data ?? "默认值";
来源：http://fez.cheryme.top

[A16] 真假值判断规则
来源：http://sfw.yuxming.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://quo.birdmap.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kmo.jlsjyb.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qck.yvedp.cn

TS:   if (!x) {}
来源：http://krh.feifeiyinyue.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kun.daxiang520.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xfn.shzxlz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sew.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qro.gaohongyu789.top

[A17] 位运算
来源：http://thy.ywan-chungtsiang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wkd.yanxiufei.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://spi.pengpengdd.cyou

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qtk.ydzc1.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yfr.hywenlv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cbz.ppjwa.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tje.hysaishi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qrs.hysaishi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hpy.guannengcc.top

[A18] 字符与 ASCII 码互转
来源：http://scv.sufxvd.cn

Py:   ord("A"); chr(65)
来源：http://ryz.bbcook.cn

PHP:  ord("A"); chr(65)
来源：http://djg.0kj1m.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://khg.zhijiandao.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mym.xingfuxueyuan.xyz

Java: (int) 'A'; (char) 65
来源：http://ucp.yangfankeji.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ptw.guowangkeji.top

Ruby: "A".ord; 65.chr
来源：http://ywk.tanke756.top

C#:   (int)'A'; (char)65
来源：http://dut.guowangkeji.top

[A19] 交换两个变量
来源：http://vug.gotoacloud.top

Py:   a, b = b, a
来源：http://tve.ivvv.top

PHP:  [$a, $b] = [$b, $a];
来源：http://rbq.shanyushiyangkeji.top

JS:   [a, b] = [b, a];
来源：http://swo.fehbvm.com

TS:   [a, b] = [b, a];
来源：http://tvz.dashuyun.cn

Java: int t = a; a = b; b = t;
来源：http://xus.jinyuanbaomall.cn

Go:   a, b = b, a
来源：http://ehl.snrcjt.cn

Ruby: a, b = b, a
来源：http://dar.andypj.xyz

C#:   (a, b) = (b, a);
来源：http://ccn.jqgufenzy.top

[A20] 读取标准输入
来源：http://kcb.jinqigufen.top

Py:   name = input("请输入：")
来源：http://rbv.yongpay.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kli.pengpengdd.cyou

JS:   // Node.js：readline 模块或 process.stdin
来源：http://unq.tarul.cn

TS:   // Node.js：readline 模块
来源：http://qup.sweek.top

Java: new Scanner(System.in).nextLine()
来源：http://mmg.fzhhl.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tzk.pengpengdd.cyou

Ruby: gets.chomp
来源：http://cpr.daria6918.cn

C#:   Console.ReadLine();
来源：http://dfv.sxryk.cn

[A21] 保留指定小数位输出
来源：http://bwu.jinqigufen.top

Py:   f"{3.14159:.2f}"
来源：http://sum.havefunace.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dnp.hnqzz.top

JS:   (3.14159).toFixed(2)
来源：http://uyt.hysaishi.cn

TS:   (3.14159).toFixed(2)
来源：http://wqg.tianlin.xyz

Java: String.format("%.2f", 3.14159)
来源：http://oau.xziqi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jyt.zhoulong.xyz

Ruby: format("%.2f", 3.14159)
来源：http://vnb.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://eki.xinyue.icu

[A22] 获取字符串长度
来源：http://ckk.chenzaomai.com

Py:   len(s)
来源：http://ftc.bbcook.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ylx.feifeiyinyue.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://afl.yfazqb.com

TS:   s.length
来源：http://wsz.c1oappe.top

Java: s.length()
来源：http://yvq.hysaishi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ocm.yanxiufei.cn

Ruby: s.length
来源：http://vsq.sjlbkw.cn

C#:   s.Length
来源：http://gua.meibo888.top

[A23] 大小写转换
来源：http://isl.0kj1m.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gpc.zhongyouzk.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://har.cqqwz.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vpn.hnqzz.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://abd.yonumen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qmk.chenzaomai.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vtl.shuidangran.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://egw.svipenyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xiy.zycfv.cn

[A24] 去除首尾空白
来源：http://iss.hywenlv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rms.wangshuangyany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kiy.cqqwz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://upb.shuidangran.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://glx.aibaodan.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nbd.yueranfly.top

Go:   strings.TrimSpace(s)
来源：http://lhk.yangfankeji.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ssf.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://spr.bbcook.cn

[A25] 字符串比较
来源：http://pgj.sjlbkw.cn

Py:   s1 == s2; s1 != s2
来源：http://rbm.zdqjudy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vpa.dianchejie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dby.sxryk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qmo.sjlbkw.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ztw.gzhubu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qgr.ehwqpu.com

Ruby: s1 == s2; s1 <=> s2
来源：http://opy.zhoulong.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bzl.kuanghao11.cn

[A26] 类型转换总览
来源：http://ynm.yj20258888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wjs.epnwcf.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bcr.uphjek.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fny.hysaishi.cn

TS:   Number() String() Boolean() x as number
来源：http://bwb.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pgc.yanxiufei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tcd.mhx1999.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lwl.bjfxy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kkl.sxryk.cn

================================================================================
来源：http://gzy.sysykeji.top

B. 流程控制
来源：http://yyj.yj20258888.top

================================================================================
来源：http://zji.tarul.cn

[B01] 条件判断 if / else
来源：http://dyt.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hqc.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wjs.feifeiyinyue.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dos.316326.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gya.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mcq.jyoumei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mns.birdmap.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gta.yj20258888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zqh.zhijiandao.cn

[B02] 多分支 else if / elif
来源：http://rhe.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dkr.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dgm.zdqjudy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://beb.yongpay.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://omc.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://paw.xuetiantiany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ayp.yueranfly.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://osv.daxiang520.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tbl.sxryk.cn

[B03] switch / match / case
来源：http://zpz.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gxv.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uwo.ivvv.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://grw.dianchejie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bme.chenzaomai.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iba.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hif.ivvv.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qcc.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://odr.andypj.xyz

[B04] for 计数循环
来源：http://jjb.jiagoushi.top

Py:   for i in range(10): print(i)
来源：http://kbw.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jwt.svipenyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bsm.birdmap.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qxa.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nfb.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://peb.hongshengwenyu.top

Ruby: 10.times { |i| puts i }
来源：http://kwi.feifeiyinyue.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lcb.jinqigfzy.top

[B05] 遍历数组 / 列表
来源：http://urv.0kj1m.cn

Py:   for item in arr: print(item)
来源：http://hmj.9152youxi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wfd.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uew.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dzm.yj20258888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cof.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mmm.smart0.xyz

Ruby: arr.each { |item| puts item }
来源：http://dxd.gotoacloud.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mop.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://leg.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://ogc.xuetiantiany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aha.tian-w.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qjk.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ryg.chenzaomai.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zor.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rml.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rxa.daria6918.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mjf.hongshengwenyu.top

[B07] while 循环
来源：http://qge.yonumen.top

Py:   while i < 10: i += 1
来源：http://voo.yongpay.top

PHP:  while ($i < 10) { $i++; }
来源：http://svq.epnwcf.com

JS:   while (i < 10) { i++; }
来源：http://bce.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://clw.yj202588.top

Java: while (i < 10) { i++; }
来源：http://itd.yfazqb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wub.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://ada.zdqjudy.top

C#:   while (i < 10) { i++; }
来源：http://yqw.vqdsnc.cn

[B08] do-while（至少执行一次）
来源：http://buy.yonumen.top

Py:   # 无 do-while：用 while True + break
来源：http://sog.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zbv.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://qpm.bjfxy.top

TS:   do { i++; } while (i < 10);
来源：http://xew.vehdjk.com

Java: do { i++; } while (i < 10);
来源：http://odh.cashguo.top

Go:   for { i++; if i >= 10 { break } }
来源：http://les.jiagoushi.top

Ruby: begin; i += 1; end while i < 10
来源：http://qzr.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://brh.bjfxy.top

[B09] break 与 continue
来源：http://wdf.tarul.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://psx.daria6918.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://egf.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xbn.jinqigufen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://evy.fzhhl.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zyi.wangshuangyany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dyz.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xfa.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pzj.zhoulong.xyz

[B10] 遍历同时拿索引
来源：http://rwz.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ivy.epnwcf.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yti.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jmr.uphjek.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://akr.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jwk.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bbv.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bmi.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mdm.gzhubu.top

[B11] 生成数字序列 / 区间
来源：http://gxj.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://aci.jyoumei.cn

PHP:  range(0, 10, 2);
来源：http://srv.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oui.zhixingplan.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ttk.tian-w.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jyb.tarul.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://url.yangfankeji.com

Ruby: (0...10).step(2).to_a
来源：http://duk.fanxiaobao.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yxy.iojbl.cn

[B12] 跳出多层循环
来源：http://osg.sxryk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oxx.quarkkingdee.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ddk.tianlin.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://phb.jinqigufen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qqq.jqgufenzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ror.daria6918.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gra.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://khg.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fud.meibo888.top

[B13] 判断是否为数字
来源：http://myk.yuanzhike.top

Py:   isinstance(x, (int, float))
来源：http://nwb.gzhubu.top

PHP:  is_numeric($x)
来源：http://rsq.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bnw.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nxi.aizwys.cn

Java: x instanceof Number
来源：http://hlb.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rqr.cheryme.top

Ruby: x.is_a?(Numeric)
来源：http://ovz.chenjidiqi.icu

C#:   x is int or double or decimal
来源：http://ccc.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://gml.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://der.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://szi.dianchejie.cn

JS:   [1, 2, 3].includes(x)
来源：http://upl.epnwcf.com

TS:   [1, 2, 3].includes(x)
来源：http://soe.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eaz.cdnleiting.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://orr.hfpthk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://auz.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wlp.bbcook.cn

[B15] 布尔运算与取反
来源：http://dyk.gotoacloud.top

Py:   a and b or not c
来源：http://uyb.yangfankeji.com

PHP:  $a && $b || !$c
来源：http://nmi.wangshuangyany.cn

JS:   a && b || !c
来源：http://hhk.zhijiandao.cn

TS:   a && b || !c
来源：http://nas.zdqjudy.top

Java: a && b || !c
来源：http://lfg.hnqzz.top

Go:   a && b || !c
来源：http://fcl.jlsjyb.cn

Ruby: a && b || !c
来源：http://mgq.kuanghao11.cn

C#:   a && b || !c
来源：http://rgu.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://oak.yanxiufei.cn

Py:   if not data: return
来源：http://scp.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://fmp.jqgufenzy.top

JS:   if (!data) return;
来源：http://eqd.xziqi.cn

TS:   if (!data) return;
来源：http://ggg.jianghu66.top


<!-- 参考信息 -->