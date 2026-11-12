代发 wailian999

[A10] 生成随机数
来源：http://dpj.guannengcc.top

Py:   import random; random.randint(1, 100)
来源：http://urj.xuanzx.com

PHP:  random_int(1, 100);
来源：http://pnl.quarkkingdee.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cjp.cdnleiting.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://shq.guowangkeji.top

Java: new Random().nextInt(100) + 1
来源：http://hso.kuanghao11.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hka.yvedp.cn

Ruby: rand(1..100)
来源：http://ujc.yonumen.top

C#:   new Random().Next(1, 101)
来源：http://ohl.ehwqpu.com

[A11] 条件表达式（三元）
来源：http://vac.yvedp.cn

Py:   "yes" if x > 0 else "no"
来源：http://ptg.xuetiantiany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yjo.zhixingplan.top

JS:   x > 0 ? "yes" : "no"
来源：http://lkt.chenlongwang.top

TS:   x > 0 ? "yes" : "no"
来源：http://dgz.redwolf501.top

Java: x > 0 ? "yes" : "no"
来源：http://rdn.cheryme.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jgh.wangshuangyany.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vzr.birdmap.top

C#:   x > 0 ? "yes" : "no"
来源：http://ibv.sxryk.cn

[A12] 字符串插值 / 格式化
来源：http://yol.dashuyun.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xpj.pengpengdd.cyou

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qmh.xuetiantiany.cn

JS:   `Hello, ${name}!`
来源：http://aho.andypj.xyz

TS:   `Hello, ${name}!`
来源：http://fpe.jlsjyb.cn

Java: "Hello, %s!".formatted(name)
来源：http://vva.shzxlz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rge.zdbjq.cn

Ruby: "Hello, #{name}!"
来源：http://ibn.yj20258888.top

C#:   $"Hello, {name}!"
来源：http://vpv.xuanzx.com

[A13] 多行字符串（练习 \n 转义）
来源：http://rzz.quarkkingdee.top

Py:   "第一行\n第二行"
来源：http://swi.chenlongwang.top

PHP:  "第一行\n第二行"
来源：http://jqb.yueranfly.top

JS:   "第一行\n第二行"
来源：http://hlv.nanxinkj.top

TS:   "第一行\n第二行"
来源：http://qlu.yuxming.cn

Java: "第一行\n第二行"
来源：http://yss.jinghuilouyu.cn

Go:   "第一行\n第二行"
来源：http://yld.smart0.xyz

Ruby: "第一行\n第二行"
来源：http://yqg.ybcxt.top

C#:   "第一行\n第二行"
来源：http://lpo.zhaomingkeji.xyz

[A14] 注释写法
来源：http://njy.yuanzhike.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rjv.yanxiufei.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://syz.gzhubu.top

JS:   // 单行；/* 多行 */
来源：http://xgq.fktsv.cn

TS:   // 单行；/* 多行 */
来源：http://dvh.yuanzhike.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ucr.zhoulong.xyz

Go:   // 单行；/* 多行 */
来源：http://uuz.fzhhl.top

Ruby: # 单行；=begin 多行 =end
来源：http://eer.daria6918.cn

C#:   // 单行；/* 多行 */
来源：http://dqm.hnxiangtu.top

[A15] 空值判断与默认值
来源：http://lcj.0kj1m.cn

Py:   value = data or "默认值"
来源：http://gnt.zhixingplan.top

PHP:  $value = $data ?? "默认值";
来源：http://edj.uphjek.com

JS:   const value = data ?? "默认值";
来源：http://myn.ctjpmb.com

TS:   const value = data ?? "默认值";
来源：http://qpo.yanxiufei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xyr.iojbl.cn

Go:   if data == "" { data = "默认值" }
来源：http://ngn.jiagoushi.top

Ruby: value = data || "默认值"
来源：http://fro.ivvv.top

C#:   var value = data ?? "默认值";
来源：http://mbo.ivvv.top

[A16] 真假值判断规则
来源：http://akc.zhixingplan.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hqn.sufxvd.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wir.pycfn.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ily.kuanghao11.cn

TS:   if (!x) {}
来源：http://sic.yj20258.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gzv.chenlongwang.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sul.jinghuilouyu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bnl.jianghu66.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ifn.shuidangran.top

[A17] 位运算
来源：http://bap.sweek.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ias.jyoumei.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://are.gotoacloud.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nal.sufxvd.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hhr.hammf.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yoi.zhaomingkeji.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://otd.chenzaomai.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://osf.snrcjt.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://buq.fehbvm.com

[A18] 字符与 ASCII 码互转
来源：http://mjy.jinqigfzy.top

Py:   ord("A"); chr(65)
来源：http://kqe.daxiang520.top

PHP:  ord("A"); chr(65)
来源：http://prs.fktsv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ljx.jinqigfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://psa.jyoumei.cn

Java: (int) 'A'; (char) 65
来源：http://rst.hnxiangtu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qfi.jlsjyb.cn

Ruby: "A".ord; 65.chr
来源：http://bep.hnxiangtu.top

C#:   (int)'A'; (char)65
来源：http://zfd.gaohongyu789.top

[A19] 交换两个变量
来源：http://qrx.316326.xyz

Py:   a, b = b, a
来源：http://xep.52xcode.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://llr.bbcook.cn

JS:   [a, b] = [b, a];
来源：http://vzm.jinqigufen.top

TS:   [a, b] = [b, a];
来源：http://fzt.wangdashe.top

Java: int t = a; a = b; b = t;
来源：http://uzq.dashuyun.cn

Go:   a, b = b, a
来源：http://imj.ydjk.org.cn

Ruby: a, b = b, a
来源：http://qlz.pengpengdd.cyou

C#:   (a, b) = (b, a);
来源：http://yef.ivvv.top

[A20] 读取标准输入
来源：http://hhg.0kj1m.cn

Py:   name = input("请输入：")
来源：http://tqm.jinghuilouyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rqg.jinghuilouyu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ljt.tian-w.cn

TS:   // Node.js：readline 模块
来源：http://ssz.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://sxi.yj20258.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ufi.zhoulong.xyz

Ruby: gets.chomp
来源：http://mne.smart0.xyz

C#:   Console.ReadLine();
来源：http://ria.tanke756.top

[A21] 保留指定小数位输出
来源：http://wze.yuxming.cn

Py:   f"{3.14159:.2f}"
来源：http://qdh.tian-w.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bes.pengpengdd.cyou

JS:   (3.14159).toFixed(2)
来源：http://hml.snrcjt.cn

TS:   (3.14159).toFixed(2)
来源：http://vpp.aizwys.cn

Java: String.format("%.2f", 3.14159)
来源：http://vmt.hammf.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fff.redwolf501.top

Ruby: format("%.2f", 3.14159)
来源：http://zux.tarul.cn

C#:   3.14159.ToString("F2")
来源：http://vuo.xuanzx.com

[A22] 获取字符串长度
来源：http://zgl.jinqigufen.top

Py:   len(s)
来源：http://ybl.redwolf501.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tbj.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hpk.shzxlz.cn

TS:   s.length
来源：http://bcb.smart0.xyz

Java: s.length()
来源：http://vcn.yangfankeji.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ilo.9152youxi.cn

Ruby: s.length
来源：http://wsk.tanke756.top

C#:   s.Length
来源：http://tit.yuxming.cn

[A23] 大小写转换
来源：http://hyq.xziqi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bti.shuidangran.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oib.cqqwz.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sdw.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ghv.9152youxi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tjo.shangyingyoupin.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gkt.redwolf501.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vip.shuidangran.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nab.vqdsnc.cn

[A24] 去除首尾空白
来源：http://zdq.zhoulong.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ino.andypj.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vzx.jinqigfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uds.tanke756.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tme.hesvh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nyx.hnqzz.top

Go:   strings.TrimSpace(s)
来源：http://afq.jinqigfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dhz.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hqx.tianlin.xyz

[A25] 字符串比较
来源：http://roi.yanxiufei.cn

Py:   s1 == s2; s1 != s2
来源：http://ikw.nwbrower.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mnv.hcnkem.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xcd.jqgfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mdw.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cus.sxryk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zks.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nxz.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yjh.snrcjt.cn

[A26] 类型转换总览
来源：http://ugm.cheryme.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oaa.dianchejie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://apb.hnqzz.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ksw.nanxinkj.top

TS:   Number() String() Boolean() x as number
来源：http://zye.yangfankeji.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://inr.xingfuxueyuan.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mts.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ctf.havefunace.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dnq.fengsongda.top

================================================================================
来源：http://rqi.cqqwz.cn

B. 流程控制
来源：http://dlp.gzhubu.top

================================================================================
来源：http://zhy.vqdsnc.cn

[B01] 条件判断 if / else
来源：http://pbk.vqdsnc.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vbz.aizwys.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aik.ehwqpu.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gls.shzxlz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zay.wangshuangyany.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uia.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hfp.zhiwuduotai.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nxv.svipenyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uba.0kj1m.cn

[B02] 多分支 else if / elif
来源：http://udy.chenlongwang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kcc.shanyushiyangtech.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://opw.jiagoushi.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qme.yongpay.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rae.uphjek.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gqh.gotoacloud.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ngz.gotoacloud.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gob.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uql.sweek.top

[B03] switch / match / case
来源：http://avk.sysykeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://svi.tian-w.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wvz.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jmv.feifeiyinyue.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://atu.epnwcf.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tnp.epnwcf.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jot.zdqjudy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sdi.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://unc.yuxming.cn

[B04] for 计数循环
来源：http://yri.zhijiandao.cn

Py:   for i in range(10): print(i)
来源：http://kad.fanxiaobao.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dvm.xuetiantiany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mty.shuidangran.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nbs.yuxming.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ukb.ydjk.org.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baw.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://fjh.zycfv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iul.sxryk.cn

[B05] 遍历数组 / 列表
来源：http://cyx.andypj.xyz

Py:   for item in arr: print(item)
来源：http://iem.xuetiantiany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hvq.fehbvm.com

JS:   for (const item of arr) { console.log(item); }
来源：http://fmv.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lya.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://swz.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xgs.316326.xyz

Ruby: arr.each { |item| puts item }
来源：http://xkt.jqgufenzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jru.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://yce.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gfm.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cck.birdmap.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://khp.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bdf.ivvv.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://suq.bbcook.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qmn.gogol.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://skm.jqgufenzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vlb.redwolf501.top

[B07] while 循环
来源：http://cri.zycfv.cn

Py:   while i < 10: i += 1
来源：http://meb.hongshengwenyu.top

PHP:  while ($i < 10) { $i++; }
来源：http://bgo.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://eie.pengpengdd.cyou

TS:   while (i < 10) { i++; }
来源：http://qqb.fengsongda.top

Java: while (i < 10) { i++; }
来源：http://vgx.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rtm.cdnleiting.top

Ruby: while i < 10; i += 1; end
来源：http://cwp.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://pjr.yj20258.top

[B08] do-while（至少执行一次）
来源：http://gmc.xziqi.cn

Py:   # 无 do-while：用 while True + break
来源：http://yrj.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ibr.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://wpr.pengpengdd.cyou

TS:   do { i++; } while (i < 10);
来源：http://cro.xinyue.icu

Java: do { i++; } while (i < 10);
来源：http://fab.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://spa.ppjwa.cn

Ruby: begin; i += 1; end while i < 10
来源：http://glg.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://kuy.wangshuangyany.cn

[B09] break 与 continue
来源：http://cbs.yj20258.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vrv.jyoumei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qrz.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ced.haohaochexian.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jdd.guannengcc.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ymx.fktsv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rnf.yangfankeji.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fqo.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zen.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://bai.havefunace.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uys.gotoacloud.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hay.pengpengdd.cyou

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pvo.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vyw.jiagoushi.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lkt.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ucv.gotoacloud.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aav.c1oappe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ios.yuxming.cn

[B11] 生成数字序列 / 区间
来源：http://lwi.zhixingplan.top

Py:   list(range(0, 10, 2))
来源：http://dkf.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://nro.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://arq.316326.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oud.nanxinkj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vja.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eay.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://xxl.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iyo.mhx1999.top

[B12] 跳出多层循环
来源：http://twf.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bui.wangdashe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zwc.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zwt.yonumen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ugq.dianchejie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ksh.jqgfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ofi.xingfuxueyuan.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uia.bjfxy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pcs.daxiang520.top

[B13] 判断是否为数字
来源：http://jwt.jqgufenzy.top

Py:   isinstance(x, (int, float))
来源：http://tqn.chenzaomai.com

PHP:  is_numeric($x)
来源：http://zjm.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fvh.dianchejie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xzx.ivvv.top

Java: x instanceof Number
来源：http://lqz.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dwv.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://csc.jyoumei.cn

C#:   x is int or double or decimal
来源：http://xtf.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://yyd.nanxinkj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ogw.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ftz.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://bov.zdbjq.cn

TS:   [1, 2, 3].includes(x)
来源：http://wbu.316326.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://crd.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lqe.yfazqb.com

Ruby: [1, 2, 3].include?(x)
来源：http://ybv.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mbi.birdmap.top

[B15] 布尔运算与取反
来源：http://ihq.gotoacloud.top

Py:   a and b or not c
来源：http://ugd.gaohongyu789.top

PHP:  $a && $b || !$c
来源：http://mtg.yongpay.top

JS:   a && b || !c
来源：http://mbl.cqqwz.cn

TS:   a && b || !c
来源：http://efk.gogol.net.cn

Java: a && b || !c
来源：http://jxg.wangdashe.top

Go:   a && b || !c
来源：http://zcm.52xcode.cn

Ruby: a && b || !c
来源：http://vpf.fzhhl.top

C#:   a && b || !c
来源：http://cnw.kuanghao11.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zph.guowangkeji.top

Py:   if not data: return
来源：http://rnt.vehdjk.com

PHP:  if (!$data) { return; }
来源：http://vtw.jqgfzy.top

JS:   if (!data) return;
来源：http://vmh.zhongyouzk.top

TS:   if (!data) return;
来源：http://zbq.quarkkingdee.top

Java: if (data == null) return;
来源：http://ffk.yueranfly.top

Go:   if data == nil { return }
来源：http://hdk.tarul.cn

Ruby: return if data.nil?
来源：http://kwp.sysykeji.top

C#:   if (data == null) return;
来源：http://zkb.sxryk.cn


<!-- 参考信息 -->