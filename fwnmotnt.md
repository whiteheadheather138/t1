代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://mxw.ehwqpu.com

C#:   x > 0 ? "yes" : "no"
来源：http://znc.sxryk.cn

[A12] 字符串插值 / 格式化
来源：http://nbp.shanyushiyangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dyv.havefunace.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lvf.hesvh.cn

JS:   `Hello, ${name}!`
来源：http://tww.yj20258888.top

TS:   `Hello, ${name}!`
来源：http://xfe.wangdashe.top

Java: "Hello, %s!".formatted(name)
来源：http://lqf.daria6918.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://btz.zhixingplan.top

Ruby: "Hello, #{name}!"
来源：http://gtn.c1oappe.top

C#:   $"Hello, {name}!"
来源：http://gsc.sufxvd.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uyw.hnxiangtu.top

Py:   "第一行\n第二行"
来源：http://duo.pycfn.com

PHP:  "第一行\n第二行"
来源：http://pjk.ivvv.top

JS:   "第一行\n第二行"
来源：http://ubu.pycfn.com

TS:   "第一行\n第二行"
来源：http://grr.jinqigufen.top

Java: "第一行\n第二行"
来源：http://mhz.fengsongda.top

Go:   "第一行\n第二行"
来源：http://svz.cashguo.top

Ruby: "第一行\n第二行"
来源：http://jud.shanyushiyangkeji.top

C#:   "第一行\n第二行"
来源：http://ubv.epnwcf.com

[A14] 注释写法
来源：http://myy.yueranfly.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://psl.redwolf501.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wvo.shuidangran.top

JS:   // 单行；/* 多行 */
来源：http://eli.hysaishi.cn

TS:   // 单行；/* 多行 */
来源：http://phz.ehwqpu.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vlu.cdnleiting.top

Go:   // 单行；/* 多行 */
来源：http://ctq.vqdsnc.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wdc.sysykeji.top

C#:   // 单行；/* 多行 */
来源：http://bxr.316326.xyz

[A15] 空值判断与默认值
来源：http://ggt.dianchejie.cn

Py:   value = data or "默认值"
来源：http://rkp.zhijiandao.cn

PHP:  $value = $data ?? "默认值";
来源：http://xfb.fzhhl.top

JS:   const value = data ?? "默认值";
来源：http://gcb.yuxming.cn

TS:   const value = data ?? "默认值";
来源：http://qyg.snrcjt.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gyo.xinyue.icu

Go:   if data == "" { data = "默认值" }
来源：http://pub.shuidangran.top

Ruby: value = data || "默认值"
来源：http://alr.vqdsnc.cn

C#:   var value = data ?? "默认值";
来源：http://rug.xuetiantiany.cn

[A16] 真假值判断规则
来源：http://ysc.yuanzhike.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tut.hfpthk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kva.gogol.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gka.zycfv.cn

TS:   if (!x) {}
来源：http://num.hnxiangtu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jor.shanyushiyangtech.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jwt.smart0.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://gdo.daxiang520.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rcm.ehwqpu.com

[A17] 位运算
来源：http://svg.jqgufenzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vlp.smart0.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wun.nanxuanxn.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gtk.zdqjudy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tkx.xinyue.icu

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bdq.jianghu66.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ozu.yongpay.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://srx.hnqzz.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iyw.yongpay.top

[A18] 字符与 ASCII 码互转
来源：http://mcg.wangshuangyany.cn

Py:   ord("A"); chr(65)
来源：http://dyv.yanxiufei.cn

PHP:  ord("A"); chr(65)
来源：http://pir.daria6918.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uiq.9152youxi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kca.haohaochexian.top

Java: (int) 'A'; (char) 65
来源：http://tnw.yanxiufei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://opt.9152youxi.cn

Ruby: "A".ord; 65.chr
来源：http://enm.cheryme.top

C#:   (int)'A'; (char)65
来源：http://xmv.shzxlz.cn

[A19] 交换两个变量
来源：http://xpc.xuetiantiany.cn

Py:   a, b = b, a
来源：http://yvt.jinyuanbaomall.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pat.cheryme.top

JS:   [a, b] = [b, a];
来源：http://bgr.guannengcc.top

TS:   [a, b] = [b, a];
来源：http://avh.zycfv.cn

Java: int t = a; a = b; b = t;
来源：http://hqa.shanyushiyangtech.top

Go:   a, b = b, a
来源：http://dmx.zhoulong.xyz

Ruby: a, b = b, a
来源：http://jci.mhx1999.top

C#:   (a, b) = (b, a);
来源：http://jtw.ehwqpu.com

[A20] 读取标准输入
来源：http://wfz.mhx1999.top

Py:   name = input("请输入：")
来源：http://xnq.jiagoushi.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jhi.yuxming.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vly.fktsv.cn

TS:   // Node.js：readline 模块
来源：http://voy.yj20258888.top

Java: new Scanner(System.in).nextLine()
来源：http://rbe.chenjidiqi.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jrl.yj20258888.top

Ruby: gets.chomp
来源：http://irc.pengpengdd.cyou

C#:   Console.ReadLine();
来源：http://pam.yj20258.top

[A21] 保留指定小数位输出
来源：http://gty.zhoulong.xyz

Py:   f"{3.14159:.2f}"
来源：http://ebz.pengpengdd.cyou

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tpl.nanxinkj.top

JS:   (3.14159).toFixed(2)
来源：http://jei.fengsongda.top

TS:   (3.14159).toFixed(2)
来源：http://uar.chenjidiqi.icu

Java: String.format("%.2f", 3.14159)
来源：http://ioo.sysykeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nhv.xinyue.icu

Ruby: format("%.2f", 3.14159)
来源：http://vpx.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://wmj.ydjk.org.cn

[A22] 获取字符串长度
来源：http://aos.fktsv.cn

Py:   len(s)
来源：http://kwf.aibaodan.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wvo.dashuyun.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://emf.jqgfzy.top

TS:   s.length
来源：http://vbg.yfazqb.com

Java: s.length()
来源：http://okw.ydjk.org.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jbm.uphjek.com

Ruby: s.length
来源：http://bih.cucudq.cn

C#:   s.Length
来源：http://oji.xuetiantiany.cn

[A23] 大小写转换
来源：http://npc.wangshuangyany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dvr.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xnb.yj20258888.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kws.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cin.ywan-chungtsiang.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://utg.hesvh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zcj.ehwqpu.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://huq.yuanzhike.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pzq.tianlin.xyz

[A24] 去除首尾空白
来源：http://hxx.snrcjt.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ugk.fengsongda.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sgt.52xcode.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kys.xylfe.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://owe.ybcxt.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ccv.ctjpmb.com

Go:   strings.TrimSpace(s)
来源：http://elo.aibaodan.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://srh.ctjpmb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bpk.hesvh.cn

[A25] 字符串比较
来源：http://fma.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://ann.kuanghao11.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hqs.nanxuanxn.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mtz.jianghu66.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wnz.yuxming.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rlj.fehbvm.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xfl.xuanzx.com

Ruby: s1 == s2; s1 <=> s2
来源：http://nlu.ppjwa.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ebt.xziqi.cn

[A26] 类型转换总览
来源：http://ijy.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zur.feifeiyinyue.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yfk.sufxvd.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://umb.tianlin.xyz

TS:   Number() String() Boolean() x as number
来源：http://nwk.aizwys.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://anl.zhiwuduotai.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://myg.meibo888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kty.jyoumei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lcb.shzxlz.cn

================================================================================
来源：http://yjc.iojbl.cn

B. 流程控制
来源：http://ugx.bjfxy.top

================================================================================
来源：http://ynx.vehdjk.com

[B01] 条件判断 if / else
来源：http://jei.xuetiantiany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aie.tianlin.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fqg.yj202588.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aca.cheryme.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://trl.sjlbkw.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mdr.fanxiaobao.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kmg.xuetiantiany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qmc.chenjidiqi.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ddw.yj20258.top

[B02] 多分支 else if / elif
来源：http://cwp.iojbl.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bmx.cashguo.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sew.yonumen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://een.wangshuangyany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qcq.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fms.hysaishi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ugo.xylfe.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rhm.ywan-chungtsiang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://grr.ctjpmb.com

[B03] switch / match / case
来源：http://tsl.havefunace.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bwi.tian-w.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yny.yueranfly.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wmr.shanyushiyangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qze.jinqigfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yzk.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://udb.hongshengwenyu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ltl.cashguo.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pdb.meibo888.top

[B04] for 计数循环
来源：http://bec.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://krb.meibo888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vhl.nanxuanxn.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vmq.cheryme.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eeb.hnxiangtu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jsf.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qot.redwolf501.top

Ruby: 10.times { |i| puts i }
来源：http://rrr.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cwv.xuetiantiany.cn

[B05] 遍历数组 / 列表
来源：http://cgb.hesvh.cn

Py:   for item in arr: print(item)
来源：http://ilb.iojbl.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://urr.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gle.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nto.9152youxi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ddf.jyoumei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jxg.vqdsnc.cn

Ruby: arr.each { |item| puts item }
来源：http://dre.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zxa.9152youxi.cn

[B06] 遍历字典 / 对象
来源：http://yof.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xyt.yvedp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://itd.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bsp.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cqy.yvedp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://osh.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fgk.ywan-chungtsiang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nwz.hammf.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qvu.uphjek.com

[B07] while 循环
来源：http://tpv.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://hze.316326.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://efk.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://llh.yueranfly.top

TS:   while (i < 10) { i++; }
来源：http://epk.yj20258888.top

Java: while (i < 10) { i++; }
来源：http://ftk.mhx1999.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vsi.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://ugv.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://wtr.nwbrower.top

[B08] do-while（至少执行一次）
来源：http://nou.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://kso.svipenyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ynr.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://hll.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://xaf.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://xse.havefunace.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lxs.jianghu66.top

Ruby: begin; i += 1; end while i < 10
来源：http://cqy.xingfuxueyuan.xyz

C#:   do { i++; } while (i < 10);
来源：http://bdt.shangyingyoupin.top

[B09] break 与 continue
来源：http://azp.kuanghao11.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cdx.ydjk.org.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pmr.cashguo.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://whu.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cha.epnwcf.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wft.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ihn.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iex.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wjx.sufxvd.cn

[B10] 遍历同时拿索引
来源：http://mwm.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wok.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://njs.gotoacloud.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ayt.hywenlv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vks.zdbjq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ely.daxiang520.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qxd.mhx1999.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oca.yuxming.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://suv.jinghuilouyu.cn

[B11] 生成数字序列 / 区间
来源：http://dok.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://tts.zhijiandao.cn

PHP:  range(0, 10, 2);
来源：http://pco.chenzaomai.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pmc.aibaodan.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://liw.fehbvm.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yyk.aibaodan.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ljc.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://jqj.xylfe.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sxf.pengpengdd.cyou

[B12] 跳出多层循环
来源：http://wqs.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://aye.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lbh.xuetiantiany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mdo.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qpj.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ppv.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dty.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ebo.ivvv.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dav.fehbvm.com

[B13] 判断是否为数字
来源：http://muf.yanxiufei.cn

Py:   isinstance(x, (int, float))
来源：http://ldl.jqgufenzy.top

PHP:  is_numeric($x)
来源：http://ejo.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ryq.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cnb.zdqjudy.top

Java: x instanceof Number
来源：http://lyb.jyoumei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://frb.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://tot.quarkkingdee.top

C#:   x is int or double or decimal
来源：http://fvo.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://qfm.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://paa.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aqm.cheryme.top

JS:   [1, 2, 3].includes(x)
来源：http://rll.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://fxr.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pgt.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ylu.cucudq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pal.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eoh.yj20258.top

[B15] 布尔运算与取反
来源：http://blb.xuetiantiany.cn

Py:   a and b or not c
来源：http://dpu.andypj.xyz

PHP:  $a && $b || !$c
来源：http://hti.chenlongwang.top

JS:   a && b || !c
来源：http://kii.yanxiufei.cn

TS:   a && b || !c
来源：http://vsz.kuanghao11.cn

Java: a && b || !c
来源：http://jaq.birdmap.top

Go:   a && b || !c
来源：http://oqu.9152youxi.cn

Ruby: a && b || !c
来源：http://sys.jinqigfzy.top

C#:   a && b || !c
来源：http://gjg.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dwz.xylfe.cn

Py:   if not data: return
来源：http://xib.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://ivp.ydjk.org.cn

JS:   if (!data) return;
来源：http://uhu.xuanzx.com

TS:   if (!data) return;
来源：http://nuq.zhixingplan.top

Java: if (data == null) return;
来源：http://qkj.svipenyu.cn

Go:   if data == nil { return }
来源：http://rts.jiagoushi.top

Ruby: return if data.nil?
来源：http://cml.vehdjk.com

C#:   if (data == null) return;
来源：http://wjf.jiagoushi.top

================================================================================
来源：http://ywi.daria6918.cn

C. 函数与作用域
来源：http://btq.ctjpmb.com

================================================================================
来源：http://ghx.havefunace.top

[C01] 定义函数
来源：http://yoe.shuidangran.top

Py:   def add(a, b): return a + b
来源：http://yha.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tsa.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://nks.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iut.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yor.sxryk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dmz.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://hcm.9152youxi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://obb.birdmap.top

[C02] 默认参数
来源：http://aat.vqdsnc.cn

Py:   def greet(name="World"): return name
来源：http://bnv.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://fgw.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://huq.ehwqpu.com


<!-- 参考信息 -->