代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tnd.pengpengdd.cyou

Java: new Random().nextInt(100) + 1
来源：http://gai.svipenyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cyq.hammf.cn

Ruby: rand(1..100)
来源：http://ydt.yonumen.top

C#:   new Random().Next(1, 101)
来源：http://ntm.316326.xyz

[A11] 条件表达式（三元）
来源：http://zol.zhongyouzk.top

Py:   "yes" if x > 0 else "no"
来源：http://tol.havefunace.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://vgq.0kj1m.cn

JS:   x > 0 ? "yes" : "no"
来源：http://igg.epnwcf.com

TS:   x > 0 ? "yes" : "no"
来源：http://hzc.bbcook.cn

Java: x > 0 ? "yes" : "no"
来源：http://cga.haohaochexian.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gui.ybcxt.top

Ruby: x > 0 ? "yes" : "no"
来源：http://phs.pengpengdd.cyou

C#:   x > 0 ? "yes" : "no"
来源：http://umh.sxryk.cn

[A12] 字符串插值 / 格式化
来源：http://drz.shanyushiyangtech.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://esf.yueranfly.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uep.hfpthk.cn

JS:   `Hello, ${name}!`
来源：http://bjn.xingfuxueyuan.xyz

TS:   `Hello, ${name}!`
来源：http://xzb.ydjk.org.cn

Java: "Hello, %s!".formatted(name)
来源：http://xsa.snrcjt.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vbe.cdnleiting.top

Ruby: "Hello, #{name}!"
来源：http://xwm.yongpay.top

C#:   $"Hello, {name}!"
来源：http://lhh.smart0.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://vwg.guannengcc.top

Py:   "第一行\n第二行"
来源：http://ecv.sysykeji.top

PHP:  "第一行\n第二行"
来源：http://hoz.yanxiufei.cn

JS:   "第一行\n第二行"
来源：http://qll.hysaishi.cn

TS:   "第一行\n第二行"
来源：http://dnn.vqdsnc.cn

Java: "第一行\n第二行"
来源：http://xsb.jqgufenzy.top

Go:   "第一行\n第二行"
来源：http://qqp.jyoumei.cn

Ruby: "第一行\n第二行"
来源：http://qom.hesvh.cn

C#:   "第一行\n第二行"
来源：http://exq.quarkkingdee.top

[A14] 注释写法
来源：http://zkc.52xcode.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://urf.tanke756.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rio.chenlongwang.top

JS:   // 单行；/* 多行 */
来源：http://yjf.pengpengdd.cyou

TS:   // 单行；/* 多行 */
来源：http://nzq.ctjpmb.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lva.ehwqpu.com

Go:   // 单行；/* 多行 */
来源：http://lfc.jqgfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://ekp.jianghu66.top

C#:   // 单行；/* 多行 */
来源：http://ysj.chenzaomai.com

[A15] 空值判断与默认值
来源：http://bzg.wangdashe.top

Py:   value = data or "默认值"
来源：http://itr.yj20258888.top

PHP:  $value = $data ?? "默认值";
来源：http://qwd.xziqi.cn

JS:   const value = data ?? "默认值";
来源：http://ysi.vehdjk.com

TS:   const value = data ?? "默认值";
来源：http://xuy.quarkkingdee.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xku.sufxvd.cn

Go:   if data == "" { data = "默认值" }
来源：http://bnc.ydzc1.top

Ruby: value = data || "默认值"
来源：http://any.nanxinkj.top

C#:   var value = data ?? "默认值";
来源：http://lhh.zhaomingkeji.xyz

[A16] 真假值判断规则
来源：http://xwj.zhengqikj.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://esa.smart0.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ddd.zdbjq.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sld.jinghuilouyu.cn

TS:   if (!x) {}
来源：http://juu.dashuyun.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://chh.jinyuanbaomall.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://han.fzhhl.top

Ruby: unless x            # nil 与 false 为假
来源：http://zvr.redwolf501.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nqq.shanyushiyangtech.top

[A17] 位运算
来源：http://yvm.uphjek.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://czw.ydjk.org.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bnh.xuetiantiany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ldu.meibo888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qkz.fehbvm.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oeb.shuidangran.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iip.svipenyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tcz.svipenyu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bjj.zhaomingkeji.xyz

[A18] 字符与 ASCII 码互转
来源：http://icv.dashuyun.cn

Py:   ord("A"); chr(65)
来源：http://znu.tarul.cn

PHP:  ord("A"); chr(65)
来源：http://ael.yuanzhike.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://djl.haohaochexian.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kyc.andypj.xyz

Java: (int) 'A'; (char) 65
来源：http://pmo.hfpthk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hhh.cucudq.cn

Ruby: "A".ord; 65.chr
来源：http://ojk.cdnleiting.top

C#:   (int)'A'; (char)65
来源：http://gji.daria6918.cn

[A19] 交换两个变量
来源：http://gap.zhaomingkeji.xyz

Py:   a, b = b, a
来源：http://tqo.xuanzx.com

PHP:  [$a, $b] = [$b, $a];
来源：http://jdp.jianghu66.top

JS:   [a, b] = [b, a];
来源：http://rgy.cucudq.cn

TS:   [a, b] = [b, a];
来源：http://lcb.jinqigfzy.top

Java: int t = a; a = b; b = t;
来源：http://tqb.gogol.net.cn

Go:   a, b = b, a
来源：http://yir.hesvh.cn

Ruby: a, b = b, a
来源：http://tgr.tarul.cn

C#:   (a, b) = (b, a);
来源：http://efn.fengsongda.top

[A20] 读取标准输入
来源：http://zfg.uphjek.com

Py:   name = input("请输入：")
来源：http://lcg.chenlongwang.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qmr.chenlongwang.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qxl.hysaishi.cn

TS:   // Node.js：readline 模块
来源：http://yqn.hysaishi.cn

Java: new Scanner(System.in).nextLine()
来源：http://xgc.sjlbkw.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xhm.sysykeji.top

Ruby: gets.chomp
来源：http://fne.hnxiangtu.top

C#:   Console.ReadLine();
来源：http://xpz.zycfv.cn

[A21] 保留指定小数位输出
来源：http://xrw.zdbjq.cn

Py:   f"{3.14159:.2f}"
来源：http://tbk.shanyushiyangkeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xjd.xinyue.icu

JS:   (3.14159).toFixed(2)
来源：http://flu.pengpengdd.cyou

TS:   (3.14159).toFixed(2)
来源：http://vps.redwolf501.top

Java: String.format("%.2f", 3.14159)
来源：http://lbl.shuidangran.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vuc.yueranfly.top

Ruby: format("%.2f", 3.14159)
来源：http://pcz.52xcode.cn

C#:   3.14159.ToString("F2")
来源：http://utq.yuxming.cn

[A22] 获取字符串长度
来源：http://rci.xuanzx.com

Py:   len(s)
来源：http://xel.yueranfly.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uuq.guowangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ljc.bjfxy.top

TS:   s.length
来源：http://hpd.iojbl.cn

Java: s.length()
来源：http://jgf.yj202588.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tyz.pycfn.com

Ruby: s.length
来源：http://wvi.jlsjyb.cn

C#:   s.Length
来源：http://aan.snrcjt.cn

[A23] 大小写转换
来源：http://dzs.cashguo.top

Py:   s.upper(); s.lower(); s.title()
来源：http://cma.fktsv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://faz.yj20258.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vls.jinyuanbaomall.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cdf.jlsjyb.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qhr.svipenyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://avj.ywan-chungtsiang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://frb.ydzc1.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qtg.cucudq.cn

[A24] 去除首尾空白
来源：http://tad.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zuy.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://skk.9152youxi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nrb.jinqigfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yis.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qei.sjlbkw.cn

Go:   strings.TrimSpace(s)
来源：http://nte.zhongyouzk.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://epx.zhengqikj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://skk.epnwcf.com

[A25] 字符串比较
来源：http://uqo.xinyue.icu

Py:   s1 == s2; s1 != s2
来源：http://rdb.tanke756.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aog.jinqigfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yuq.jinyuanbaomall.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qvc.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qed.gotoacloud.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tks.hysaishi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mfh.snrcjt.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gvs.yj202588.top

[A26] 类型转换总览
来源：http://fqb.aibaodan.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pna.zdqjudy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fmy.nanxuanxn.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rch.jinyuanbaomall.cn

TS:   Number() String() Boolean() x as number
来源：http://hxl.feifeiyinyue.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iuk.chenzaomai.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oew.ehwqpu.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://mxv.tanke756.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://noy.daria6918.cn

================================================================================
来源：http://xrm.jinyuanbaomall.cn

B. 流程控制
来源：http://vjt.nwbrower.top

================================================================================
来源：http://ghw.9152youxi.cn

[B01] 条件判断 if / else
来源：http://ksq.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://skl.zhoulong.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uyh.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tao.vehdjk.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://esr.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aew.daxiang520.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nqj.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cht.jinqigufen.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oza.tanke756.top

[B02] 多分支 else if / elif
来源：http://zhp.vehdjk.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xbx.pycfn.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aef.zhixingplan.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ijq.gogol.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qnt.zdbjq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbs.gotoacloud.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kim.yj20258.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hra.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vjl.xylfe.cn

[B03] switch / match / case
来源：http://cqh.kuanghao11.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qqs.hysaishi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jau.shangyingyoupin.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lsc.pengpengdd.cyou

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vek.guannengcc.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jsw.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oun.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eyg.feifeiyinyue.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yph.vehdjk.com

[B04] for 计数循环
来源：http://lth.jlsjyb.cn

Py:   for i in range(10): print(i)
来源：http://ykg.aizwys.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iiu.xingfuxueyuan.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cyu.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ryn.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cmu.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fko.daria6918.cn

Ruby: 10.times { |i| puts i }
来源：http://edw.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wmp.yonumen.top

[B05] 遍历数组 / 列表
来源：http://xco.jinqigfzy.top

Py:   for item in arr: print(item)
来源：http://aud.xziqi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jrk.yonumen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://avt.bjfxy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mfz.shuidangran.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zys.xylfe.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://brm.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://nnc.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ibt.iojbl.cn

[B06] 遍历字典 / 对象
来源：http://nok.ybcxt.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yrl.fengsongda.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qny.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bjm.xziqi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vif.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pve.svipenyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jmc.yonumen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pxb.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pet.jiagoushi.top

[B07] while 循环
来源：http://pmh.jinqigufen.top

Py:   while i < 10: i += 1
来源：http://tis.gzhubu.top

PHP:  while ($i < 10) { $i++; }
来源：http://uuw.xingfuxueyuan.xyz

JS:   while (i < 10) { i++; }
来源：http://bpi.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://iqi.vehdjk.com

Java: while (i < 10) { i++; }
来源：http://qnp.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ogh.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://mhx.yuanzhike.top

C#:   while (i < 10) { i++; }
来源：http://uxx.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://eci.zhongyouzk.top

Py:   # 无 do-while：用 while True + break
来源：http://nax.hammf.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vou.zhijiandao.cn

JS:   do { i++; } while (i < 10);
来源：http://tvn.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://qvo.jyoumei.cn

Java: do { i++; } while (i < 10);
来源：http://txx.hysaishi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pfk.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://fcq.yj202588.top

C#:   do { i++; } while (i < 10);
来源：http://zct.cdnleiting.top

[B09] break 与 continue
来源：http://omu.zdqjudy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tbi.tianlin.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xci.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ayw.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nlo.ydzc1.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gth.shzxlz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mgq.yangfankeji.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ucg.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uvb.fengsongda.top

[B10] 遍历同时拿索引
来源：http://plx.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qpe.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mkd.guannengcc.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://glv.tian-w.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iwg.chenzaomai.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nhy.jyoumei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dml.kuanghao11.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tgk.ctjpmb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sls.zhoulong.xyz

[B11] 生成数字序列 / 区间
来源：http://irz.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://jpn.yfazqb.com

PHP:  range(0, 10, 2);
来源：http://vcc.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qmp.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cwd.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dgt.quarkkingdee.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://amr.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://jqs.jiagoushi.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ves.zdqjudy.top

[B12] 跳出多层循环
来源：http://uib.aibaodan.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pei.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cim.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jas.yfazqb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ntt.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uhg.0kj1m.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qik.shangyingyoupin.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mos.havefunace.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vcs.yueranfly.top

[B13] 判断是否为数字
来源：http://vvn.ctjpmb.com

Py:   isinstance(x, (int, float))
来源：http://hlx.daxiang520.top

PHP:  is_numeric($x)
来源：http://xbk.haohaochexian.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gsg.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://auh.hysaishi.cn

Java: x instanceof Number
来源：http://oax.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://two.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://fia.epnwcf.com

C#:   x is int or double or decimal
来源：http://ynh.shuidangran.top

[B14] 判断值是否在集合内
来源：http://pcj.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blu.redwolf501.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://amp.nanxuanxn.top

JS:   [1, 2, 3].includes(x)
来源：http://pux.kuanghao11.cn

TS:   [1, 2, 3].includes(x)
来源：http://tjo.tarul.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pow.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vls.sxryk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wzt.cashguo.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wlz.ivvv.top

[B15] 布尔运算与取反
来源：http://jtq.hnxiangtu.top

Py:   a and b or not c
来源：http://egb.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://kgo.hnqzz.top

JS:   a && b || !c
来源：http://wjx.yj20258888.top

TS:   a && b || !c
来源：http://jwp.zhoulong.xyz

Java: a && b || !c
来源：http://qgt.cqqwz.cn

Go:   a && b || !c
来源：http://jvs.kuanghao11.cn

Ruby: a && b || !c
来源：http://sun.cucudq.cn

C#:   a && b || !c
来源：http://mww.sjlbkw.cn

[B16] 卫语句：不满足条件提前返回
来源：http://aqv.cashguo.top

Py:   if not data: return
来源：http://bhy.yvedp.cn

PHP:  if (!$data) { return; }
来源：http://enf.xinyue.icu

JS:   if (!data) return;
来源：http://twb.xuetiantiany.cn

TS:   if (!data) return;
来源：http://mtc.shangyingyoupin.top

Java: if (data == null) return;
来源：http://tjq.cashguo.top

Go:   if data == nil { return }
来源：http://hkb.svipenyu.cn

Ruby: return if data.nil?
来源：http://hxo.bjfxy.top

C#:   if (data == null) return;
来源：http://fhw.yvedp.cn

================================================================================
来源：http://cet.ydjk.org.cn

C. 函数与作用域
来源：http://tkv.aibaodan.cn

================================================================================
来源：http://odg.xylfe.cn

[C01] 定义函数
来源：http://tgf.zdqjudy.top


<!-- 参考信息 -->