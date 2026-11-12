代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ztp.jlsjyb.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vta.yj20258.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wuu.ppjwa.cn

[A09] 绝对值与最大最小值
来源：http://oab.tarul.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gth.shanyushiyangtech.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xjn.ppjwa.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kkf.wangshuangyany.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cfn.cashguo.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wxv.zhoulong.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eqq.wangdashe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qnr.yangfankeji.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sjp.zhengqikj.top

[A10] 生成随机数
来源：http://uwr.ydzc1.top

Py:   import random; random.randint(1, 100)
来源：http://kww.cashguo.top

PHP:  random_int(1, 100);
来源：http://yrp.jianghu66.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vak.nanxuanxn.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://era.ppjwa.cn

Java: new Random().nextInt(100) + 1
来源：http://xko.xuetiantiany.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lsm.bbcook.cn

Ruby: rand(1..100)
来源：http://ltw.yanxiufei.cn

C#:   new Random().Next(1, 101)
来源：http://rer.sweek.top

[A11] 条件表达式（三元）
来源：http://ozs.yvedp.cn

Py:   "yes" if x > 0 else "no"
来源：http://wxb.hammf.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pys.yanxiufei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hyp.aibaodan.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gdk.jinghuilouyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://rav.tarul.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fcb.yonumen.top

Ruby: x > 0 ? "yes" : "no"
来源：http://qbt.guannengcc.top

C#:   x > 0 ? "yes" : "no"
来源：http://ved.shuidangran.top

[A12] 字符串插值 / 格式化
来源：http://ykv.fktsv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uih.sjlbkw.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sje.cheryme.top

JS:   `Hello, ${name}!`
来源：http://dri.hnqzz.top

TS:   `Hello, ${name}!`
来源：http://psa.fktsv.cn

Java: "Hello, %s!".formatted(name)
来源：http://njs.ivvv.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oaz.andypj.xyz

Ruby: "Hello, #{name}!"
来源：http://ftm.ctjpmb.com

C#:   $"Hello, {name}!"
来源：http://yca.guannengcc.top

[A13] 多行字符串（练习 \n 转义）
来源：http://org.zhiwuduotai.top

Py:   "第一行\n第二行"
来源：http://fbu.yongpay.top

PHP:  "第一行\n第二行"
来源：http://eii.ywan-chungtsiang.top

JS:   "第一行\n第二行"
来源：http://ncl.quarkkingdee.top

TS:   "第一行\n第二行"
来源：http://jhi.yanxiufei.cn

Java: "第一行\n第二行"
来源：http://jey.cashguo.top

Go:   "第一行\n第二行"
来源：http://adi.sjlbkw.cn

Ruby: "第一行\n第二行"
来源：http://ymx.jyoumei.cn

C#:   "第一行\n第二行"
来源：http://wap.pengpengdd.cyou

[A14] 注释写法
来源：http://idx.jinqigfzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wnq.bjfxy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pld.shuidangran.top

JS:   // 单行；/* 多行 */
来源：http://jqo.xinyue.icu

TS:   // 单行；/* 多行 */
来源：http://drw.jinqigfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fac.feifeiyinyue.top

Go:   // 单行；/* 多行 */
来源：http://oxh.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qoj.ppjwa.cn

C#:   // 单行；/* 多行 */
来源：http://ape.vehdjk.com

[A15] 空值判断与默认值
来源：http://vbi.yuxming.cn

Py:   value = data or "默认值"
来源：http://mbs.hywenlv.cn

PHP:  $value = $data ?? "默认值";
来源：http://jdr.fanxiaobao.xyz

JS:   const value = data ?? "默认值";
来源：http://bxl.vqdsnc.cn

TS:   const value = data ?? "默认值";
来源：http://qlc.zhengqikj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dbk.jianghu66.top

Go:   if data == "" { data = "默认值" }
来源：http://mym.yueranfly.top

Ruby: value = data || "默认值"
来源：http://nkh.fanxiaobao.xyz

C#:   var value = data ?? "默认值";
来源：http://ajp.zdqjudy.top

[A16] 真假值判断规则
来源：http://gfd.chenjidiqi.icu

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vle.fehbvm.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wim.xziqi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://guw.zhengqikj.top

TS:   if (!x) {}
来源：http://fgy.jinghuilouyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ida.cucudq.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ykt.hnqzz.top

Ruby: unless x            # nil 与 false 为假
来源：http://ffe.yonumen.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wqs.epnwcf.com

[A17] 位运算
来源：http://lah.jinyuanbaomall.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bpb.zhengqikj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://igf.feifeiyinyue.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oar.cheryme.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qqi.yonumen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ise.c1oappe.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wub.yj20258888.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uew.jqgufenzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kql.xuetiantiany.cn

[A18] 字符与 ASCII 码互转
来源：http://enz.zycfv.cn

Py:   ord("A"); chr(65)
来源：http://xuc.shanyushiyangkeji.top

PHP:  ord("A"); chr(65)
来源：http://teo.fanxiaobao.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kxs.jqgfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ruk.zhengqikj.top

Java: (int) 'A'; (char) 65
来源：http://wvs.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ozg.yueranfly.top

Ruby: "A".ord; 65.chr
来源：http://yzs.pycfn.com

C#:   (int)'A'; (char)65
来源：http://tao.zdbjq.cn

[A19] 交换两个变量
来源：http://jtr.feifeiyinyue.top

Py:   a, b = b, a
来源：http://zfk.fengsongda.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hbx.vqdsnc.cn

JS:   [a, b] = [b, a];
来源：http://lup.ehwqpu.com

TS:   [a, b] = [b, a];
来源：http://iej.kuanghao11.cn

Java: int t = a; a = b; b = t;
来源：http://qga.ctjpmb.com

Go:   a, b = b, a
来源：http://tsu.xinyue.icu

Ruby: a, b = b, a
来源：http://xkq.zdqjudy.top

C#:   (a, b) = (b, a);
来源：http://iep.jianghu66.top

[A20] 读取标准输入
来源：http://qce.cucudq.cn

Py:   name = input("请输入：")
来源：http://zna.xylfe.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nzf.cdnleiting.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qks.zhengqikj.top

TS:   // Node.js：readline 模块
来源：http://qvw.zhaomingkeji.xyz

Java: new Scanner(System.in).nextLine()
来源：http://nre.nanxuanxn.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://giw.c1oappe.top

Ruby: gets.chomp
来源：http://qpg.daxiang520.top

C#:   Console.ReadLine();
来源：http://diy.yuanzhike.top

[A21] 保留指定小数位输出
来源：http://qyw.tarul.cn

Py:   f"{3.14159:.2f}"
来源：http://asj.fengsongda.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vjh.fanxiaobao.xyz

JS:   (3.14159).toFixed(2)
来源：http://qwx.dianchejie.cn

TS:   (3.14159).toFixed(2)
来源：http://yee.gotoacloud.top

Java: String.format("%.2f", 3.14159)
来源：http://uui.tianlin.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://evz.jyoumei.cn

Ruby: format("%.2f", 3.14159)
来源：http://gtq.jinqigfzy.top

C#:   3.14159.ToString("F2")
来源：http://fky.9152youxi.cn

[A22] 获取字符串长度
来源：http://kpd.hnqzz.top

Py:   len(s)
来源：http://rqn.fehbvm.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ywq.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gun.ehwqpu.com

TS:   s.length
来源：http://bmt.feifeiyinyue.top

Java: s.length()
来源：http://zqq.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xvd.yongpay.top

Ruby: s.length
来源：http://hpb.shanyushiyangtech.top

C#:   s.Length
来源：http://exm.xylfe.cn

[A23] 大小写转换
来源：http://vut.zhongyouzk.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wpe.wangshuangyany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://llm.chenzaomai.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kvy.cdnleiting.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yap.jinghuilouyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://okr.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sey.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://deg.xinyue.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://hka.nanxinkj.top

[A24] 去除首尾空白
来源：http://tam.jinqigufen.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://awu.jlsjyb.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mzf.yj20258.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jyl.hcnkem.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zik.fanxiaobao.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://epm.fengsongda.top

Go:   strings.TrimSpace(s)
来源：http://kiu.snrcjt.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eij.meibo888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qsp.yuanzhike.top

[A25] 字符串比较
来源：http://ele.daxiang520.top

Py:   s1 == s2; s1 != s2
来源：http://qaw.fktsv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yop.nwbrower.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jyp.snrcjt.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sbc.fengsongda.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qoa.xuetiantiany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://itu.ehwqpu.com

Ruby: s1 == s2; s1 <=> s2
来源：http://fqb.daxiang520.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fey.xuetiantiany.cn

[A26] 类型转换总览
来源：http://yrf.jqgfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hcy.wangdashe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rmv.ybcxt.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hza.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://itb.guowangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://huu.tianlin.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ffs.jinqigufen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ymq.fanxiaobao.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rnh.quarkkingdee.top

================================================================================
来源：http://dsj.guowangkeji.top

B. 流程控制
来源：http://ugw.ehwqpu.com

================================================================================
来源：http://xdr.sxryk.cn

[B01] 条件判断 if / else
来源：http://ujv.shanyushiyangtech.top

Py:   result = "正" if x > 0 else "非正"
来源：http://csm.ctjpmb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fpe.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lne.ydzc1.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gpk.fktsv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nau.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hza.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mny.havefunace.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wdn.aibaodan.cn

[B02] 多分支 else if / elif
来源：http://wev.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rvd.zhaomingkeji.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mnk.aibaodan.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fuo.hfpthk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eym.epnwcf.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rbh.jqgufenzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wfi.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rms.c1oappe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wou.jyoumei.cn

[B03] switch / match / case
来源：http://deo.fanxiaobao.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ujg.nwbrower.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nsw.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://krg.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xet.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jky.nwbrower.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dsy.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gsf.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ccp.jinqigfzy.top

[B04] for 计数循环
来源：http://nov.sjlbkw.cn

Py:   for i in range(10): print(i)
来源：http://qwx.nanxinkj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cpe.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eoq.yangfankeji.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nty.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vju.bjfxy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nni.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://uyb.fzhhl.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hfa.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://erh.hammf.cn

Py:   for item in arr: print(item)
来源：http://afi.gogol.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eho.andypj.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://gyt.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://vin.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bpc.316326.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yxk.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://wgm.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yyv.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://soo.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pip.haohaochexian.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nit.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lnj.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dos.hfpthk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sgu.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qdb.fehbvm.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hhn.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uzd.yonumen.top

[B07] while 循环
来源：http://bjl.jqgufenzy.top

Py:   while i < 10: i += 1
来源：http://ehk.316326.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://puh.birdmap.top

JS:   while (i < 10) { i++; }
来源：http://bji.fktsv.cn

TS:   while (i < 10) { i++; }
来源：http://ncx.hnqzz.top

Java: while (i < 10) { i++; }
来源：http://jqe.tanke756.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ykf.52xcode.cn

Ruby: while i < 10; i += 1; end
来源：http://dvj.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://qew.jinyuanbaomall.cn

[B08] do-while（至少执行一次）
来源：http://wgu.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://ckb.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uhi.jqgfzy.top

JS:   do { i++; } while (i < 10);
来源：http://xtr.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://gxa.epnwcf.com

Java: do { i++; } while (i < 10);
来源：http://dne.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kqh.snrcjt.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ole.nanxuanxn.top

C#:   do { i++; } while (i < 10);
来源：http://gtq.smart0.xyz

[B09] break 与 continue
来源：http://gos.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ycs.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sbs.zhixingplan.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dvu.meibo888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tai.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ozp.zhijiandao.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ckg.hysaishi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jmg.jqgfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nin.cucudq.cn

[B10] 遍历同时拿索引
来源：http://alc.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yfb.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uyf.tian-w.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dsq.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uiq.ivvv.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fxl.yueranfly.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kor.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qpe.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cax.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://keh.fanxiaobao.xyz

Py:   list(range(0, 10, 2))
来源：http://mzo.hesvh.cn

PHP:  range(0, 10, 2);
来源：http://yyg.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fug.shanyushiyangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vir.jianghu66.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tvc.tarul.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kuv.zhijiandao.cn

Ruby: (0...10).step(2).to_a
来源：http://pdy.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qsj.sufxvd.cn

[B12] 跳出多层循环
来源：http://agy.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gsk.sjlbkw.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eok.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://luo.jinqigufen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://buw.fehbvm.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kzt.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hqg.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://saf.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vps.yongpay.top

[B13] 判断是否为数字
来源：http://gnc.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://spl.yangfankeji.com

PHP:  is_numeric($x)
来源：http://tar.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ptg.wangdashe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pgy.bbcook.cn

Java: x instanceof Number
来源：http://itk.andypj.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ebx.hammf.cn

Ruby: x.is_a?(Numeric)
来源：http://mvs.mhx1999.top

C#:   x is int or double or decimal
来源：http://ydq.ydzc1.top

[B14] 判断值是否在集合内
来源：http://wfn.guannengcc.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lwr.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xae.jinqigufen.top

JS:   [1, 2, 3].includes(x)
来源：http://qci.9152youxi.cn

TS:   [1, 2, 3].includes(x)
来源：http://yox.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://ibs.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lor.ydzc1.top

Ruby: [1, 2, 3].include?(x)
来源：http://eit.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cut.nwbrower.top

[B15] 布尔运算与取反
来源：http://ngf.pycfn.com

Py:   a and b or not c
来源：http://bpp.c1oappe.top

PHP:  $a && $b || !$c
来源：http://xfc.ybcxt.top

JS:   a && b || !c
来源：http://gdg.daxiang520.top

TS:   a && b || !c
来源：http://otr.sjlbkw.cn

Java: a && b || !c
来源：http://cie.yuxming.cn


<!-- 参考信息 -->