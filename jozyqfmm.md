代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://vlc.jinghuilouyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://coz.ehwqpu.com

Java: x > 0 ? "yes" : "no"
来源：http://ton.sxryk.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gic.dianchejie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ivb.sweek.top

C#:   x > 0 ? "yes" : "no"
来源：http://fbt.jqgfzy.top

[A12] 字符串插值 / 格式化
来源：http://uge.yongpay.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dmf.yueranfly.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qkm.yj20258.top

JS:   `Hello, ${name}!`
来源：http://wpq.pengpengdd.cyou

TS:   `Hello, ${name}!`
来源：http://usv.iojbl.cn

Java: "Hello, %s!".formatted(name)
来源：http://qbt.0kj1m.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vyg.sjlbkw.cn

Ruby: "Hello, #{name}!"
来源：http://fka.wangdashe.top

C#:   $"Hello, {name}!"
来源：http://zyf.bjfxy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://wuq.yvedp.cn

Py:   "第一行\n第二行"
来源：http://vqt.hfpthk.cn

PHP:  "第一行\n第二行"
来源：http://rhr.pycfn.com

JS:   "第一行\n第二行"
来源：http://jzg.ppjwa.cn

TS:   "第一行\n第二行"
来源：http://eoy.iojbl.cn

Java: "第一行\n第二行"
来源：http://fjo.chenjidiqi.icu

Go:   "第一行\n第二行"
来源：http://oiw.zhoulong.xyz

Ruby: "第一行\n第二行"
来源：http://vwk.yangfankeji.com

C#:   "第一行\n第二行"
来源：http://wtg.daria6918.cn

[A14] 注释写法
来源：http://wxu.zhixingplan.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://etp.aibaodan.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zsh.fzhhl.top

JS:   // 单行；/* 多行 */
来源：http://atw.yongpay.top

TS:   // 单行；/* 多行 */
来源：http://xzo.0kj1m.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yyv.shzxlz.cn

Go:   // 单行；/* 多行 */
来源：http://rby.yfazqb.com

Ruby: # 单行；=begin 多行 =end
来源：http://ulp.yj20258.top

C#:   // 单行；/* 多行 */
来源：http://nws.feifeiyinyue.top

[A15] 空值判断与默认值
来源：http://lvd.xinyue.icu

Py:   value = data or "默认值"
来源：http://kpr.ivvv.top

PHP:  $value = $data ?? "默认值";
来源：http://dza.redwolf501.top

JS:   const value = data ?? "默认值";
来源：http://chb.yangfankeji.com

TS:   const value = data ?? "默认值";
来源：http://hum.hongshengwenyu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hfl.zhijiandao.cn

Go:   if data == "" { data = "默认值" }
来源：http://whs.svipenyu.cn

Ruby: value = data || "默认值"
来源：http://xjg.daxiang520.top

C#:   var value = data ?? "默认值";
来源：http://jbz.yj202588.top

[A16] 真假值判断规则
来源：http://dmp.shanyushiyangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hsy.snrcjt.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://upx.shanyushiyangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zlq.jlsjyb.cn

TS:   if (!x) {}
来源：http://dwo.zhoulong.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uwq.cqqwz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ixs.zdbjq.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ckq.tian-w.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vqp.daria6918.cn

[A17] 位运算
来源：http://rrb.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bwh.yuanzhike.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://muj.hesvh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xbz.vehdjk.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uqf.zdqjudy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ysx.ivvv.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zyr.sysykeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vrs.yj20258.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qmq.yongpay.top

[A18] 字符与 ASCII 码互转
来源：http://wnz.cashguo.top

Py:   ord("A"); chr(65)
来源：http://frp.snrcjt.cn

PHP:  ord("A"); chr(65)
来源：http://bvf.mhx1999.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jyf.jyoumei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fst.chenjidiqi.icu

Java: (int) 'A'; (char) 65
来源：http://vqg.cheryme.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zkw.nwbrower.top

Ruby: "A".ord; 65.chr
来源：http://vtt.yvedp.cn

C#:   (int)'A'; (char)65
来源：http://zfn.birdmap.top

[A19] 交换两个变量
来源：http://tmd.epnwcf.com

Py:   a, b = b, a
来源：http://ncu.hfpthk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tme.jiagoushi.top

JS:   [a, b] = [b, a];
来源：http://snx.nanxinkj.top

TS:   [a, b] = [b, a];
来源：http://seq.aizwys.cn

Java: int t = a; a = b; b = t;
来源：http://skk.hnxiangtu.top

Go:   a, b = b, a
来源：http://rjk.zycfv.cn

Ruby: a, b = b, a
来源：http://hoe.ppjwa.cn

C#:   (a, b) = (b, a);
来源：http://rra.hnqzz.top

[A20] 读取标准输入
来源：http://rhf.c1oappe.top

Py:   name = input("请输入：")
来源：http://iwp.yj20258888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://fgj.haohaochexian.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://adk.chenzaomai.com

TS:   // Node.js：readline 模块
来源：http://qwh.quarkkingdee.top

Java: new Scanner(System.in).nextLine()
来源：http://sjs.fktsv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zfk.zdqjudy.top

Ruby: gets.chomp
来源：http://zfa.hfpthk.cn

C#:   Console.ReadLine();
来源：http://ofj.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://cds.shanyushiyangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://hor.vehdjk.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xwb.gogol.net.cn

JS:   (3.14159).toFixed(2)
来源：http://lgy.shuidangran.top

TS:   (3.14159).toFixed(2)
来源：http://ntj.ydjk.org.cn

Java: String.format("%.2f", 3.14159)
来源：http://sux.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nnt.ppjwa.cn

Ruby: format("%.2f", 3.14159)
来源：http://mxf.zhiwuduotai.top

C#:   3.14159.ToString("F2")
来源：http://lfc.chenzaomai.com

[A22] 获取字符串长度
来源：http://xxn.ywan-chungtsiang.top

Py:   len(s)
来源：http://sns.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jho.jinghuilouyu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mqj.hnqzz.top

TS:   s.length
来源：http://mlb.pycfn.com

Java: s.length()
来源：http://mgd.dashuyun.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yoi.gotoacloud.top

Ruby: s.length
来源：http://ywa.jinqigfzy.top

C#:   s.Length
来源：http://ilt.yonumen.top

[A23] 大小写转换
来源：http://qqs.gaohongyu789.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ptk.smart0.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yer.gzhubu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uis.shangyingyoupin.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pri.chenjidiqi.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://elj.nwbrower.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wth.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lxr.xuetiantiany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wcd.zhixingplan.top

[A24] 去除首尾空白
来源：http://cqx.kuanghao11.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sgc.sweek.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zun.jinqigfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ync.yonumen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xlg.chenlongwang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nni.gzhubu.top

Go:   strings.TrimSpace(s)
来源：http://ivz.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lpy.guowangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wvd.fengsongda.top

[A25] 字符串比较
来源：http://cqp.zhiwuduotai.top

Py:   s1 == s2; s1 != s2
来源：http://qhu.sysykeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ftd.yvedp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dyh.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://neh.havefunace.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rim.nanxuanxn.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://njx.cucudq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mzl.andypj.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vus.dianchejie.cn

[A26] 类型转换总览
来源：http://ear.daria6918.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://biq.zhongyouzk.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hen.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://slz.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://ntr.quarkkingdee.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fnq.pycfn.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oll.nwbrower.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xlx.yj202588.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kqm.ybcxt.top

================================================================================
来源：http://ogv.sweek.top

B. 流程控制
来源：http://bei.pycfn.com

================================================================================
来源：http://ogo.yanxiufei.cn

[B01] 条件判断 if / else
来源：http://ibe.bjfxy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xok.jinqigfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kzc.ydzc1.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ury.sxryk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nyb.quarkkingdee.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wdl.xziqi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ctw.yonumen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qkq.pycfn.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wwy.bjfxy.top

[B02] 多分支 else if / elif
来源：http://otu.havefunace.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://akl.shuidangran.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fly.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qcf.9152youxi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dsp.zhixingplan.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mpe.wangshuangyany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://geb.haohaochexian.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yfo.c1oappe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://agh.jqgufenzy.top

[B03] switch / match / case
来源：http://xrc.fzhhl.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tsm.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://otv.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://spg.zhijiandao.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zyl.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bdt.guowangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hrx.cheryme.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yyu.quarkkingdee.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mql.52xcode.cn

[B04] for 计数循环
来源：http://zyd.yuxming.cn

Py:   for i in range(10): print(i)
来源：http://don.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vid.xuetiantiany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kaa.hysaishi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nad.cucudq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eyf.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bnk.yuanzhike.top

Ruby: 10.times { |i| puts i }
来源：http://dav.zdbjq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mnr.bjfxy.top

[B05] 遍历数组 / 列表
来源：http://bqc.zhengqikj.top

Py:   for item in arr: print(item)
来源：http://wuq.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zki.hnxiangtu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nkx.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ayn.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://liy.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fje.cheryme.top

Ruby: arr.each { |item| puts item }
来源：http://npb.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mwb.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://hco.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wbe.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://upi.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xqb.zhengqikj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pog.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dkj.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://itp.yuanzhike.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nap.zycfv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qal.hywenlv.cn

[B07] while 循环
来源：http://tac.zhijiandao.cn

Py:   while i < 10: i += 1
来源：http://lgy.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://opc.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://eer.shzxlz.cn

TS:   while (i < 10) { i++; }
来源：http://ssx.cqqwz.cn

Java: while (i < 10) { i++; }
来源：http://kyv.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zcs.zhixingplan.top

Ruby: while i < 10; i += 1; end
来源：http://sqy.hfpthk.cn

C#:   while (i < 10) { i++; }
来源：http://vlw.cdnleiting.top

[B08] do-while（至少执行一次）
来源：http://jmq.zdqjudy.top

Py:   # 无 do-while：用 while True + break
来源：http://kvm.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xxs.yongpay.top

JS:   do { i++; } while (i < 10);
来源：http://iwp.fzhhl.top

TS:   do { i++; } while (i < 10);
来源：http://xlm.tianlin.xyz

Java: do { i++; } while (i < 10);
来源：http://zek.sysykeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://izc.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://jbt.hywenlv.cn

C#:   do { i++; } while (i < 10);
来源：http://cfw.yuanzhike.top

[B09] break 与 continue
来源：http://elg.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ajc.yj202588.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qwv.guowangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dam.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://doh.daria6918.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://loa.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jiy.yonumen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fcm.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zfj.yonumen.top

[B10] 遍历同时拿索引
来源：http://mrk.chenjidiqi.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hhe.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ycv.guowangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qae.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ioh.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://art.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zog.ctjpmb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iuc.vqdsnc.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tuk.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://shl.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://smu.pycfn.com

PHP:  range(0, 10, 2);
来源：http://tzs.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://quh.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rak.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://myv.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qwr.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://ftl.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://opd.xuanzx.com

[B12] 跳出多层循环
来源：http://dpn.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qaz.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qdx.zhixingplan.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kzp.gotoacloud.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jbi.sweek.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rit.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oto.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qhs.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ryy.hnqzz.top

[B13] 判断是否为数字
来源：http://bqg.shanyushiyangtech.top

Py:   isinstance(x, (int, float))
来源：http://qbq.ivvv.top

PHP:  is_numeric($x)
来源：http://frc.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fld.cheryme.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tuv.guowangkeji.top

Java: x instanceof Number
来源：http://wml.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cwo.shzxlz.cn

Ruby: x.is_a?(Numeric)
来源：http://pkg.c1oappe.top

C#:   x is int or double or decimal
来源：http://rro.ybcxt.top

[B14] 判断值是否在集合内
来源：http://fbo.hywenlv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jte.jqgufenzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pnd.zhijiandao.cn

JS:   [1, 2, 3].includes(x)
来源：http://due.hammf.cn

TS:   [1, 2, 3].includes(x)
来源：http://wnr.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pxk.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ltg.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://zvo.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bjq.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://meu.shangyingyoupin.top

Py:   a and b or not c
来源：http://gpg.vqdsnc.cn

PHP:  $a && $b || !$c
来源：http://smq.ybcxt.top

JS:   a && b || !c
来源：http://vdq.yangfankeji.com

TS:   a && b || !c
来源：http://dja.hcnkem.com

Java: a && b || !c
来源：http://una.svipenyu.cn

Go:   a && b || !c
来源：http://gak.aizwys.cn

Ruby: a && b || !c
来源：http://bcg.hesvh.cn

C#:   a && b || !c
来源：http://ier.yj202588.top

[B16] 卫语句：不满足条件提前返回
来源：http://aki.fehbvm.com

Py:   if not data: return
来源：http://cpb.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://tzg.hcnkem.com

JS:   if (!data) return;
来源：http://qna.havefunace.top

TS:   if (!data) return;
来源：http://uco.wangdashe.top

Java: if (data == null) return;
来源：http://qkc.gogol.net.cn

Go:   if data == nil { return }
来源：http://qjl.hywenlv.cn

Ruby: return if data.nil?
来源：http://gla.ydjk.org.cn

C#:   if (data == null) return;
来源：http://zqo.daria6918.cn

================================================================================
来源：http://edw.aizwys.cn

C. 函数与作用域
来源：http://mui.yvedp.cn

================================================================================
来源：http://zhh.pycfn.com

[C01] 定义函数
来源：http://jxd.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://abh.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://odj.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://bfr.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kwo.jqgufenzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://weh.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://iav.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://goy.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ojv.hesvh.cn


<!-- 参考信息 -->