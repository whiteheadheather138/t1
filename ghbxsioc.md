代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bvt.fzhhl.top

Java: new Random().nextInt(100) + 1
来源：http://vdc.xylfe.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ljf.tarul.cn

Ruby: rand(1..100)
来源：http://qsy.ybcxt.top

C#:   new Random().Next(1, 101)
来源：http://jri.yuanzhike.top

[A11] 条件表达式（三元）
来源：http://hcl.fengsongda.top

Py:   "yes" if x > 0 else "no"
来源：http://tfl.kuanghao11.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fum.yj20258888.top

JS:   x > 0 ? "yes" : "no"
来源：http://sou.xuanzx.com

TS:   x > 0 ? "yes" : "no"
来源：http://nfy.shuidangran.top

Java: x > 0 ? "yes" : "no"
来源：http://jzo.ydjk.org.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tgx.aizwys.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xrb.xuetiantiany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pbg.bbcook.cn

[A12] 字符串插值 / 格式化
来源：http://boa.shanyushiyangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gzc.zhengqikj.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ffz.jinqigfzy.top

JS:   `Hello, ${name}!`
来源：http://wbs.redwolf501.top

TS:   `Hello, ${name}!`
来源：http://bfv.guowangkeji.top

Java: "Hello, %s!".formatted(name)
来源：http://tnq.jyoumei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://odw.yangfankeji.com

Ruby: "Hello, #{name}!"
来源：http://cvt.jinghuilouyu.cn

C#:   $"Hello, {name}!"
来源：http://drp.wangshuangyany.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://idg.vehdjk.com

Py:   "第一行\n第二行"
来源：http://cqy.fengsongda.top

PHP:  "第一行\n第二行"
来源：http://ynv.ybcxt.top

JS:   "第一行\n第二行"
来源：http://cjz.ivvv.top

TS:   "第一行\n第二行"
来源：http://jtr.jyoumei.cn

Java: "第一行\n第二行"
来源：http://yea.cashguo.top

Go:   "第一行\n第二行"
来源：http://acl.hongshengwenyu.top

Ruby: "第一行\n第二行"
来源：http://kar.zhaomingkeji.xyz

C#:   "第一行\n第二行"
来源：http://ryc.wangshuangyany.cn

[A14] 注释写法
来源：http://gxg.zdqjudy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://avz.52xcode.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tgq.cqqwz.cn

JS:   // 单行；/* 多行 */
来源：http://phe.uphjek.com

TS:   // 单行；/* 多行 */
来源：http://vzs.kuanghao11.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tmb.ydzc1.top

Go:   // 单行；/* 多行 */
来源：http://ccs.zhaomingkeji.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://opy.yj202588.top

C#:   // 单行；/* 多行 */
来源：http://xar.guannengcc.top

[A15] 空值判断与默认值
来源：http://tja.iojbl.cn

Py:   value = data or "默认值"
来源：http://jgx.quarkkingdee.top

PHP:  $value = $data ?? "默认值";
来源：http://mkj.yj202588.top

JS:   const value = data ?? "默认值";
来源：http://orp.zhiwuduotai.top

TS:   const value = data ?? "默认值";
来源：http://rat.yj20258888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zmj.dianchejie.cn

Go:   if data == "" { data = "默认值" }
来源：http://zmk.yangfankeji.com

Ruby: value = data || "默认值"
来源：http://gdj.ydjk.org.cn

C#:   var value = data ?? "默认值";
来源：http://cka.bjfxy.top

[A16] 真假值判断规则
来源：http://lgp.zdbjq.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wxm.sufxvd.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ijb.fehbvm.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mwi.yuanzhike.top

TS:   if (!x) {}
来源：http://qnd.tian-w.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xja.pengpengdd.cyou

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iya.zhijiandao.cn

Ruby: unless x            # nil 与 false 为假
来源：http://swb.iojbl.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dlw.zhengqikj.top

[A17] 位运算
来源：http://xwt.xingfuxueyuan.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aud.hcnkem.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ynf.fktsv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bao.xziqi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yww.jinqigufen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yqz.dianchejie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cac.zhaomingkeji.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mcz.mhx1999.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gan.zdqjudy.top

[A18] 字符与 ASCII 码互转
来源：http://qvu.feifeiyinyue.top

Py:   ord("A"); chr(65)
来源：http://epm.gotoacloud.top

PHP:  ord("A"); chr(65)
来源：http://exv.uphjek.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nnh.ydzc1.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zys.tianlin.xyz

Java: (int) 'A'; (char) 65
来源：http://lie.andypj.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wig.jinqigfzy.top

Ruby: "A".ord; 65.chr
来源：http://zne.yj20258888.top

C#:   (int)'A'; (char)65
来源：http://yzj.fzhhl.top

[A19] 交换两个变量
来源：http://wfw.fehbvm.com

Py:   a, b = b, a
来源：http://qtf.yonumen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mfd.jlsjyb.cn

JS:   [a, b] = [b, a];
来源：http://wje.shanyushiyangtech.top

TS:   [a, b] = [b, a];
来源：http://pvc.fehbvm.com

Java: int t = a; a = b; b = t;
来源：http://lqf.gotoacloud.top

Go:   a, b = b, a
来源：http://vng.chenjidiqi.icu

Ruby: a, b = b, a
来源：http://lcs.tian-w.cn

C#:   (a, b) = (b, a);
来源：http://khl.pycfn.com

[A20] 读取标准输入
来源：http://eux.zhoulong.xyz

Py:   name = input("请输入：")
来源：http://xbe.nwbrower.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hwz.ybcxt.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yvx.fengsongda.top

TS:   // Node.js：readline 模块
来源：http://lgx.zycfv.cn

Java: new Scanner(System.in).nextLine()
来源：http://hdh.hongshengwenyu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://omc.uphjek.com

Ruby: gets.chomp
来源：http://qts.hysaishi.cn

C#:   Console.ReadLine();
来源：http://djr.sjlbkw.cn

[A21] 保留指定小数位输出
来源：http://adl.fengsongda.top

Py:   f"{3.14159:.2f}"
来源：http://ynz.ybcxt.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tts.cqqwz.cn

JS:   (3.14159).toFixed(2)
来源：http://nip.redwolf501.top

TS:   (3.14159).toFixed(2)
来源：http://dyr.ehwqpu.com

Java: String.format("%.2f", 3.14159)
来源：http://hpv.iojbl.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gqp.tianlin.xyz

Ruby: format("%.2f", 3.14159)
来源：http://utv.yongpay.top

C#:   3.14159.ToString("F2")
来源：http://dqh.havefunace.top

[A22] 获取字符串长度
来源：http://kzy.ehwqpu.com

Py:   len(s)
来源：http://hik.52xcode.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://akk.gaohongyu789.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lml.daria6918.cn

TS:   s.length
来源：http://uqi.yfazqb.com

Java: s.length()
来源：http://qoh.zhijiandao.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fef.tarul.cn

Ruby: s.length
来源：http://jvi.yuxming.cn

C#:   s.Length
来源：http://vae.aibaodan.cn

[A23] 大小写转换
来源：http://abt.iojbl.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kur.yfazqb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uts.ydzc1.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mke.fanxiaobao.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xbd.bjfxy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wug.xuetiantiany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uyb.quarkkingdee.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hiq.pycfn.com

C#:   s.ToUpper(); s.ToLower()
来源：http://xcm.pycfn.com

[A24] 去除首尾空白
来源：http://fxf.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://udd.jinqigufen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aeg.yongpay.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zgb.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://efr.ppjwa.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mww.ydjk.org.cn

Go:   strings.TrimSpace(s)
来源：http://cpy.haohaochexian.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nju.jlsjyb.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://raw.ehwqpu.com

[A25] 字符串比较
来源：http://jsg.cqqwz.cn

Py:   s1 == s2; s1 != s2
来源：http://oha.yanxiufei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xxs.xylfe.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uda.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xsr.yueranfly.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rje.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zsu.zhijiandao.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hsr.yueranfly.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://phv.zhiwuduotai.top

[A26] 类型转换总览
来源：http://sus.c1oappe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mvi.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qhw.tianlin.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iil.vqdsnc.cn

TS:   Number() String() Boolean() x as number
来源：http://ywv.sufxvd.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zgu.iojbl.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rgi.feifeiyinyue.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://odq.bjfxy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vnm.aizwys.cn

================================================================================
来源：http://lgo.tianlin.xyz

B. 流程控制
来源：http://mmm.aizwys.cn

================================================================================
来源：http://ldp.nwbrower.top

[B01] 条件判断 if / else
来源：http://rmg.gotoacloud.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vit.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://res.tanke756.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ogs.zdbjq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://klc.c1oappe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ksm.hywenlv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pun.zhixingplan.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cst.yvedp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dxa.andypj.xyz

[B02] 多分支 else if / elif
来源：http://ykj.zhaomingkeji.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://imh.gzhubu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lhj.yuxming.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jbw.jlsjyb.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xvn.haohaochexian.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dqm.gotoacloud.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uuz.yfazqb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zqu.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rwc.jianghu66.top

[B03] switch / match / case
来源：http://efw.feifeiyinyue.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xql.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qum.316326.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://klc.quarkkingdee.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uxf.hnqzz.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zul.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://flm.gogol.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sdc.tianlin.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dgw.chenlongwang.top

[B04] for 计数循环
来源：http://lsv.jqgufenzy.top

Py:   for i in range(10): print(i)
来源：http://hcd.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ori.fanxiaobao.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://twp.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mbt.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kag.tian-w.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gwb.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://aqx.jinghuilouyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ogw.cqqwz.cn

[B05] 遍历数组 / 列表
来源：http://ayh.cdnleiting.top

Py:   for item in arr: print(item)
来源：http://fto.fzhhl.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zjq.yuxming.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ljh.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vhb.yuxming.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fku.wangshuangyany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tiz.yueranfly.top

Ruby: arr.each { |item| puts item }
来源：http://fzj.feifeiyinyue.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tdu.tanke756.top

[B06] 遍历字典 / 对象
来源：http://nxx.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zwl.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lqg.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://etr.sweek.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://szp.dashuyun.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://usm.zhijiandao.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bwf.jinqigfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://otj.fehbvm.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://imv.zdqjudy.top

[B07] while 循环
来源：http://djr.fktsv.cn

Py:   while i < 10: i += 1
来源：http://yan.jqgfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://zzs.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://ihd.smart0.xyz

TS:   while (i < 10) { i++; }
来源：http://ycq.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://vtg.yanxiufei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mdp.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://vrp.tian-w.cn

C#:   while (i < 10) { i++; }
来源：http://arg.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://drl.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://jhe.xinyue.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://wdl.ydzc1.top

JS:   do { i++; } while (i < 10);
来源：http://otx.ywan-chungtsiang.top

TS:   do { i++; } while (i < 10);
来源：http://lqp.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://uil.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ryd.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://ihc.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://mmi.hcnkem.com

[B09] break 与 continue
来源：http://fxx.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ldk.316326.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ohv.ydjk.org.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yie.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tzl.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lur.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oic.ctjpmb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://txv.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mom.yonumen.top

[B10] 遍历同时拿索引
来源：http://ayb.jianghu66.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lgq.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sqp.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gvd.sweek.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zqr.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jkg.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hqo.iojbl.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bzh.ydzc1.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aen.smart0.xyz

[B11] 生成数字序列 / 区间
来源：http://dfl.ybcxt.top

Py:   list(range(0, 10, 2))
来源：http://jwc.jinyuanbaomall.cn

PHP:  range(0, 10, 2);
来源：http://kiz.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gus.guowangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jtf.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aet.vqdsnc.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dof.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://zqk.shuidangran.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zzr.52xcode.cn

[B12] 跳出多层循环
来源：http://wwg.hfpthk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kst.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jdz.ehwqpu.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://npl.shuidangran.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jri.shanyushiyangtech.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://epa.gzhubu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://euj.316326.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wxl.svipenyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bck.cucudq.cn

[B13] 判断是否为数字
来源：http://hna.ywan-chungtsiang.top

Py:   isinstance(x, (int, float))
来源：http://nyr.yj20258.top

PHP:  is_numeric($x)
来源：http://cie.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bxa.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pcl.c1oappe.top

Java: x instanceof Number
来源：http://toc.shanyushiyangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rks.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://bzo.bbcook.cn

C#:   x is int or double or decimal
来源：http://jsh.sweek.top

[B14] 判断值是否在集合内
来源：http://bzl.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://btx.xziqi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qqa.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://vpz.hammf.cn

TS:   [1, 2, 3].includes(x)
来源：http://pfs.yj20258.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bqm.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wiy.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://obv.jinyuanbaomall.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nyc.epnwcf.com

[B15] 布尔运算与取反
来源：http://nyo.yfazqb.com

Py:   a and b or not c
来源：http://nxz.chenjidiqi.icu

PHP:  $a && $b || !$c
来源：http://gzk.guowangkeji.top

JS:   a && b || !c
来源：http://ukp.hnqzz.top

TS:   a && b || !c
来源：http://hlv.ivvv.top

Java: a && b || !c
来源：http://idg.xziqi.cn

Go:   a && b || !c
来源：http://xug.cheryme.top

Ruby: a && b || !c
来源：http://sis.cdnleiting.top

C#:   a && b || !c
来源：http://yve.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://njh.zhongyouzk.top

Py:   if not data: return
来源：http://wuo.nanxuanxn.top

PHP:  if (!$data) { return; }
来源：http://nfa.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://nhg.haohaochexian.top

TS:   if (!data) return;
来源：http://xkh.yj20258.top

Java: if (data == null) return;
来源：http://qrj.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://feu.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://elk.ydjk.org.cn

C#:   if (data == null) return;
来源：http://mwv.xuanzx.com

================================================================================
来源：http://auv.yj20258888.top

C. 函数与作用域
来源：http://grt.cashguo.top

================================================================================
来源：http://jsn.uphjek.com

[C01] 定义函数
来源：http://bsn.sweek.top


<!-- 参考信息 -->