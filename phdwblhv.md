代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://wbv.zdqjudy.top

TS:   x > 0 ? "yes" : "no"
来源：http://fnc.fengsongda.top

Java: x > 0 ? "yes" : "no"
来源：http://anl.ehwqpu.com

Go:   // 无三元运算符，需用 if 语句
来源：http://urj.xuetiantiany.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://usc.vehdjk.com

C#:   x > 0 ? "yes" : "no"
来源：http://hjk.sjlbkw.cn

[A12] 字符串插值 / 格式化
来源：http://kvn.zhoulong.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yos.gaohongyu789.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rci.tanke756.top

JS:   `Hello, ${name}!`
来源：http://pmk.chenzaomai.com

TS:   `Hello, ${name}!`
来源：http://yhm.yonumen.top

Java: "Hello, %s!".formatted(name)
来源：http://jnw.yongpay.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gir.sweek.top

Ruby: "Hello, #{name}!"
来源：http://hdy.chenjidiqi.icu

C#:   $"Hello, {name}!"
来源：http://npm.gzhubu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rpb.316326.xyz

Py:   "第一行\n第二行"
来源：http://ksb.yuxming.cn

PHP:  "第一行\n第二行"
来源：http://voz.shuidangran.top

JS:   "第一行\n第二行"
来源：http://xug.xuetiantiany.cn

TS:   "第一行\n第二行"
来源：http://qja.cashguo.top

Java: "第一行\n第二行"
来源：http://wzq.ywan-chungtsiang.top

Go:   "第一行\n第二行"
来源：http://pcm.redwolf501.top

Ruby: "第一行\n第二行"
来源：http://zpi.sjlbkw.cn

C#:   "第一行\n第二行"
来源：http://nsg.jqgfzy.top

[A14] 注释写法
来源：http://qob.meibo888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://lls.yangfankeji.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://qko.tianlin.xyz

JS:   // 单行；/* 多行 */
来源：http://vtb.vehdjk.com

TS:   // 单行；/* 多行 */
来源：http://zme.gogol.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ooc.zhongyouzk.top

Go:   // 单行；/* 多行 */
来源：http://qfx.hammf.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xkt.nwbrower.top

C#:   // 单行；/* 多行 */
来源：http://yyi.zhixingplan.top

[A15] 空值判断与默认值
来源：http://dba.jlsjyb.cn

Py:   value = data or "默认值"
来源：http://kbw.ivvv.top

PHP:  $value = $data ?? "默认值";
来源：http://rmh.iojbl.cn

JS:   const value = data ?? "默认值";
来源：http://jhy.bbcook.cn

TS:   const value = data ?? "默认值";
来源：http://gtk.tian-w.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lmc.jyoumei.cn

Go:   if data == "" { data = "默认值" }
来源：http://dyb.redwolf501.top

Ruby: value = data || "默认值"
来源：http://mzn.jqgfzy.top

C#:   var value = data ?? "默认值";
来源：http://tvx.bbcook.cn

[A16] 真假值判断规则
来源：http://kwv.fktsv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wrq.hfpthk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oud.xuetiantiany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hwe.yj202588.top

TS:   if (!x) {}
来源：http://xmy.zhiwuduotai.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ohv.fzhhl.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ary.birdmap.top

Ruby: unless x            # nil 与 false 为假
来源：http://mqu.chenlongwang.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mld.daxiang520.top

[A17] 位运算
来源：http://tww.shzxlz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kti.ydjk.org.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ypt.zhoulong.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dht.andypj.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rge.fktsv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kva.snrcjt.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zlk.xziqi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yil.fzhhl.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bpk.zhengqikj.top

[A18] 字符与 ASCII 码互转
来源：http://nzy.zhaomingkeji.xyz

Py:   ord("A"); chr(65)
来源：http://mpp.yj20258.top

PHP:  ord("A"); chr(65)
来源：http://zhg.jyoumei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hxv.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sgv.yj20258888.top

Java: (int) 'A'; (char) 65
来源：http://agv.chenjidiqi.icu

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yks.tianlin.xyz

Ruby: "A".ord; 65.chr
来源：http://dlr.c1oappe.top

C#:   (int)'A'; (char)65
来源：http://dcr.zhaomingkeji.xyz

[A19] 交换两个变量
来源：http://jvq.jinghuilouyu.cn

Py:   a, b = b, a
来源：http://kvo.smart0.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://lsy.gzhubu.top

JS:   [a, b] = [b, a];
来源：http://nze.fehbvm.com

TS:   [a, b] = [b, a];
来源：http://ulq.yuanzhike.top

Java: int t = a; a = b; b = t;
来源：http://xhp.nwbrower.top

Go:   a, b = b, a
来源：http://cub.meibo888.top

Ruby: a, b = b, a
来源：http://qrh.svipenyu.cn

C#:   (a, b) = (b, a);
来源：http://tyy.tianlin.xyz

[A20] 读取标准输入
来源：http://piw.shuidangran.top

Py:   name = input("请输入：")
来源：http://asx.wangshuangyany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cry.jyoumei.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lfy.nanxinkj.top

TS:   // Node.js：readline 模块
来源：http://ecq.316326.xyz

Java: new Scanner(System.in).nextLine()
来源：http://ihd.fengsongda.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gye.52xcode.cn

Ruby: gets.chomp
来源：http://tyf.fzhhl.top

C#:   Console.ReadLine();
来源：http://gvh.zycfv.cn

[A21] 保留指定小数位输出
来源：http://rhn.yj20258.top

Py:   f"{3.14159:.2f}"
来源：http://acl.meibo888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ywy.daria6918.cn

JS:   (3.14159).toFixed(2)
来源：http://jyi.316326.xyz

TS:   (3.14159).toFixed(2)
来源：http://xnk.wangdashe.top

Java: String.format("%.2f", 3.14159)
来源：http://mpa.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sro.cashguo.top

Ruby: format("%.2f", 3.14159)
来源：http://hdi.gogol.net.cn

C#:   3.14159.ToString("F2")
来源：http://dco.yj202588.top

[A22] 获取字符串长度
来源：http://iqk.fanxiaobao.xyz

Py:   len(s)
来源：http://kzb.0kj1m.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pne.316326.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fem.vqdsnc.cn

TS:   s.length
来源：http://spq.ppjwa.cn

Java: s.length()
来源：http://kjd.fanxiaobao.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rzr.0kj1m.cn

Ruby: s.length
来源：http://rwa.jinghuilouyu.cn

C#:   s.Length
来源：http://xby.hesvh.cn

[A23] 大小写转换
来源：http://nyx.gogol.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://far.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uqb.hcnkem.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fnb.epnwcf.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tfu.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ryq.ywan-chungtsiang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xla.uphjek.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gtc.hywenlv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vuc.zhongyouzk.top

[A24] 去除首尾空白
来源：http://msg.zhongyouzk.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wbn.yanxiufei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lxl.zhongyouzk.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yyt.fengsongda.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://npc.shzxlz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bqg.yongpay.top

Go:   strings.TrimSpace(s)
来源：http://yzh.yvedp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iak.hesvh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://grh.hongshengwenyu.top

[A25] 字符串比较
来源：http://kls.fanxiaobao.xyz

Py:   s1 == s2; s1 != s2
来源：http://vkl.sxryk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lxl.yj202588.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eai.cqqwz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lhl.tianlin.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xzr.pengpengdd.cyou

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ldz.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://yfp.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lmc.yvedp.cn

[A26] 类型转换总览
来源：http://oav.chenzaomai.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sgr.zhongyouzk.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://isa.hcnkem.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://unq.shangyingyoupin.top

TS:   Number() String() Boolean() x as number
来源：http://wog.yvedp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ngn.yj20258.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zpv.hysaishi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lno.hongshengwenyu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ulm.iojbl.cn

================================================================================
来源：http://uhn.sweek.top

B. 流程控制
来源：http://qdy.chenzaomai.com

================================================================================
来源：http://jwl.hfpthk.cn

[B01] 条件判断 if / else
来源：http://fzt.wangshuangyany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://omz.0kj1m.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://evu.yonumen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aqx.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kru.fengsongda.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dud.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rnr.gotoacloud.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iqk.jianghu66.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vcu.cashguo.top

[B02] 多分支 else if / elif
来源：http://srl.52xcode.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zuc.hfpthk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qli.quarkkingdee.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://won.hfpthk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zpk.jqgfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://agb.bbcook.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zkg.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ptl.fehbvm.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mfo.316326.xyz

[B03] switch / match / case
来源：http://hus.pengpengdd.cyou

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qba.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dcs.nanxuanxn.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://icu.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rxe.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ahy.aibaodan.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://epr.yueranfly.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ufx.ydjk.org.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ltz.jianghu66.top

[B04] for 计数循环
来源：http://czt.gzhubu.top

Py:   for i in range(10): print(i)
来源：http://kir.yangfankeji.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hjf.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cjg.yangfankeji.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ohl.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hue.gzhubu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lcb.sjlbkw.cn

Ruby: 10.times { |i| puts i }
来源：http://gmw.xuanzx.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ahe.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://smf.chenzaomai.com

Py:   for item in arr: print(item)
来源：http://rfx.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zht.chenzaomai.com

JS:   for (const item of arr) { console.log(item); }
来源：http://kbe.nanxuanxn.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qog.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ivj.quarkkingdee.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://asi.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://orv.jyoumei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wrg.wangshuangyany.cn

[B06] 遍历字典 / 对象
来源：http://sdz.wangshuangyany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sdd.snrcjt.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mvz.yvedp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zik.meibo888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hxv.chenzaomai.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fox.gzhubu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pbz.shzxlz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xdg.aibaodan.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ksr.tian-w.cn

[B07] while 循环
来源：http://ybm.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://stm.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://ohr.cashguo.top

JS:   while (i < 10) { i++; }
来源：http://her.yangfankeji.com

TS:   while (i < 10) { i++; }
来源：http://yvt.shuidangran.top

Java: while (i < 10) { i++; }
来源：http://jro.chenjidiqi.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gqo.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://mdu.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://mfh.cdnleiting.top

[B08] do-while（至少执行一次）
来源：http://pby.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://lqj.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rwh.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://fju.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://vxr.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://tlf.zhoulong.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://uze.jinqigufen.top

Ruby: begin; i += 1; end while i < 10
来源：http://jym.zhiwuduotai.top

C#:   do { i++; } while (i < 10);
来源：http://nrc.vehdjk.com

[B09] break 与 continue
来源：http://tak.cheryme.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fpd.aizwys.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://urc.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mtr.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cxl.ivvv.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ziq.hywenlv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fhp.yangfankeji.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wis.zhixingplan.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vgd.andypj.xyz

[B10] 遍历同时拿索引
来源：http://kon.xylfe.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pnx.hcnkem.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sir.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eyj.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rce.epnwcf.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zez.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aie.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ene.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kxm.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://ukl.xingfuxueyuan.xyz

Py:   list(range(0, 10, 2))
来源：http://bwz.meibo888.top

PHP:  range(0, 10, 2);
来源：http://kbw.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nfk.ybcxt.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xzi.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gts.chenjidiqi.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yid.chenjidiqi.icu

Ruby: (0...10).step(2).to_a
来源：http://kjl.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ekq.bbcook.cn

[B12] 跳出多层循环
来源：http://okx.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bmf.svipenyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vxx.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gdl.yfazqb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tgr.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xie.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yoy.hnqzz.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lri.fanxiaobao.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mym.sjlbkw.cn

[B13] 判断是否为数字
来源：http://ikg.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://xhc.hfpthk.cn

PHP:  is_numeric($x)
来源：http://frr.yanxiufei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hns.hfpthk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qzp.hammf.cn

Java: x instanceof Number
来源：http://rtp.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hul.zhongyouzk.top

Ruby: x.is_a?(Numeric)
来源：http://kkm.yongpay.top

C#:   x is int or double or decimal
来源：http://vwe.tanke756.top

[B14] 判断值是否在集合内
来源：http://ucd.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jkx.yuanzhike.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hel.iojbl.cn

JS:   [1, 2, 3].includes(x)
来源：http://nta.guowangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://eew.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cnz.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://msr.hfpthk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qyx.tianlin.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zmh.xuanzx.com

[B15] 布尔运算与取反
来源：http://jqx.shanyushiyangkeji.top

Py:   a and b or not c
来源：http://dvh.pycfn.com

PHP:  $a && $b || !$c
来源：http://xqh.hongshengwenyu.top

JS:   a && b || !c
来源：http://pdn.xziqi.cn

TS:   a && b || !c
来源：http://gjk.chenzaomai.com

Java: a && b || !c
来源：http://rac.hongshengwenyu.top

Go:   a && b || !c
来源：http://zod.9152youxi.cn

Ruby: a && b || !c
来源：http://wxo.vqdsnc.cn

C#:   a && b || !c
来源：http://xrk.cashguo.top

[B16] 卫语句：不满足条件提前返回
来源：http://zoy.shanyushiyangkeji.top

Py:   if not data: return
来源：http://tsp.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://ipf.hfpthk.cn

JS:   if (!data) return;
来源：http://oir.dashuyun.cn

TS:   if (!data) return;
来源：http://vxk.cucudq.cn

Java: if (data == null) return;
来源：http://jtd.cashguo.top

Go:   if data == nil { return }
来源：http://yci.snrcjt.cn

Ruby: return if data.nil?
来源：http://pkt.chenlongwang.top

C#:   if (data == null) return;
来源：http://thv.uphjek.com

================================================================================
来源：http://plo.cashguo.top

C. 函数与作用域
来源：http://duo.pycfn.com

================================================================================
来源：http://aoa.c1oappe.top

[C01] 定义函数
来源：http://zck.yueranfly.top

Py:   def add(a, b): return a + b
来源：http://shr.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dff.redwolf501.top

JS:   function add(a, b) { return a + b; }
来源：http://zyj.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ruc.birdmap.top

Java: static int add(int a, int b) { return a + b; }
来源：http://eoa.tianlin.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://csf.gaohongyu789.top

Ruby: def add(a, b); a + b; end
来源：http://tni.ppjwa.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bvr.bbcook.cn


<!-- 参考信息 -->