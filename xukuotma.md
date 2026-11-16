代发 wailian999

[A10] 生成随机数
来源：http://kyq.hnqzz.top

Py:   import random; random.randint(1, 100)
来源：http://fik.xuanzx.com

PHP:  random_int(1, 100);
来源：http://hci.jlsjyb.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://psp.hnxiangtu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pwr.pengpengdd.cyou

Java: new Random().nextInt(100) + 1
来源：http://ywu.52xcode.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ojs.jiagoushi.top

Ruby: rand(1..100)
来源：http://zsh.daxiang520.top

C#:   new Random().Next(1, 101)
来源：http://ydv.cucudq.cn

[A11] 条件表达式（三元）
来源：http://vug.xziqi.cn

Py:   "yes" if x > 0 else "no"
来源：http://kxh.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jvl.yj202588.top

JS:   x > 0 ? "yes" : "no"
来源：http://rsy.sweek.top

TS:   x > 0 ? "yes" : "no"
来源：http://nbm.zycfv.cn

Java: x > 0 ? "yes" : "no"
来源：http://xfr.0kj1m.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mah.uphjek.com

Ruby: x > 0 ? "yes" : "no"
来源：http://rvh.redwolf501.top

C#:   x > 0 ? "yes" : "no"
来源：http://qrw.yvedp.cn

[A12] 字符串插值 / 格式化
来源：http://yjb.cucudq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://adf.ctjpmb.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pyp.andypj.xyz

JS:   `Hello, ${name}!`
来源：http://svk.sweek.top

TS:   `Hello, ${name}!`
来源：http://glz.birdmap.top

Java: "Hello, %s!".formatted(name)
来源：http://hcx.52xcode.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cfq.chenlongwang.top

Ruby: "Hello, #{name}!"
来源：http://xqk.sxryk.cn

C#:   $"Hello, {name}!"
来源：http://jlr.zhoulong.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://mfa.yj20258.top

Py:   "第一行\n第二行"
来源：http://eyb.vehdjk.com

PHP:  "第一行\n第二行"
来源：http://xjx.feifeiyinyue.top

JS:   "第一行\n第二行"
来源：http://bpw.shzxlz.cn

TS:   "第一行\n第二行"
来源：http://lyn.vehdjk.com

Java: "第一行\n第二行"
来源：http://zih.chenlongwang.top

Go:   "第一行\n第二行"
来源：http://mbq.dashuyun.cn

Ruby: "第一行\n第二行"
来源：http://vjd.havefunace.top

C#:   "第一行\n第二行"
来源：http://jya.tarul.cn

[A14] 注释写法
来源：http://tpg.tarul.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tlb.mhx1999.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://tvy.jinqigufen.top

JS:   // 单行；/* 多行 */
来源：http://epb.daria6918.cn

TS:   // 单行；/* 多行 */
来源：http://otu.jinqigufen.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kzr.zdqjudy.top

Go:   // 单行；/* 多行 */
来源：http://bac.jinqigfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://tys.gzhubu.top

C#:   // 单行；/* 多行 */
来源：http://wzg.52xcode.cn

[A15] 空值判断与默认值
来源：http://qtc.zhongyouzk.top

Py:   value = data or "默认值"
来源：http://rnt.yongpay.top

PHP:  $value = $data ?? "默认值";
来源：http://uxu.nwbrower.top

JS:   const value = data ?? "默认值";
来源：http://tkz.cdnleiting.top

TS:   const value = data ?? "默认值";
来源：http://neh.bjfxy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xbs.sxryk.cn

Go:   if data == "" { data = "默认值" }
来源：http://yqn.c1oappe.top

Ruby: value = data || "默认值"
来源：http://iic.jinqigufen.top

C#:   var value = data ?? "默认值";
来源：http://poj.chenzaomai.com

[A16] 真假值判断规则
来源：http://fhf.zhixingplan.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dgy.xuetiantiany.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ivk.aibaodan.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://exm.tarul.cn

TS:   if (!x) {}
来源：http://llc.guowangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hje.zycfv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vdc.aizwys.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hcn.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lml.52xcode.cn

[A17] 位运算
来源：http://ldp.jinqigufen.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tnb.xziqi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hqw.cashguo.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dkc.hnqzz.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xki.ydzc1.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://byh.jqgufenzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://haw.sufxvd.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wtt.jinyuanbaomall.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sse.ybcxt.top

[A18] 字符与 ASCII 码互转
来源：http://mco.nanxuanxn.top

Py:   ord("A"); chr(65)
来源：http://hpz.meibo888.top

PHP:  ord("A"); chr(65)
来源：http://kbv.yueranfly.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://msq.fengsongda.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tex.yuxming.cn

Java: (int) 'A'; (char) 65
来源：http://csk.hfpthk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lkh.tanke756.top

Ruby: "A".ord; 65.chr
来源：http://fnt.daxiang520.top

C#:   (int)'A'; (char)65
来源：http://zoz.yangfankeji.com

[A19] 交换两个变量
来源：http://umz.andypj.xyz

Py:   a, b = b, a
来源：http://dpz.9152youxi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://coi.nanxuanxn.top

JS:   [a, b] = [b, a];
来源：http://mel.yj20258.top

TS:   [a, b] = [b, a];
来源：http://zfh.cucudq.cn

Java: int t = a; a = b; b = t;
来源：http://inb.yangfankeji.com

Go:   a, b = b, a
来源：http://wle.wangdashe.top

Ruby: a, b = b, a
来源：http://cnw.gotoacloud.top

C#:   (a, b) = (b, a);
来源：http://bqx.gogol.net.cn

[A20] 读取标准输入
来源：http://qia.tanke756.top

Py:   name = input("请输入：")
来源：http://fmv.tianlin.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://ilj.shanyushiyangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://syp.hnxiangtu.top

TS:   // Node.js：readline 模块
来源：http://jlb.xinyue.icu

Java: new Scanner(System.in).nextLine()
来源：http://hgm.tanke756.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ndl.cucudq.cn

Ruby: gets.chomp
来源：http://quv.zhixingplan.top

C#:   Console.ReadLine();
来源：http://jke.hnxiangtu.top

[A21] 保留指定小数位输出
来源：http://dyn.hongshengwenyu.top

Py:   f"{3.14159:.2f}"
来源：http://zpu.yj20258.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xfc.fanxiaobao.xyz

JS:   (3.14159).toFixed(2)
来源：http://dbp.jqgufenzy.top

TS:   (3.14159).toFixed(2)
来源：http://lvr.pengpengdd.cyou

Java: String.format("%.2f", 3.14159)
来源：http://veu.tian-w.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gto.hnqzz.top

Ruby: format("%.2f", 3.14159)
来源：http://emd.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://nvu.nwbrower.top

[A22] 获取字符串长度
来源：http://tjj.vqdsnc.cn

Py:   len(s)
来源：http://fpo.tian-w.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://khw.hesvh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://asx.nanxinkj.top

TS:   s.length
来源：http://eok.fehbvm.com

Java: s.length()
来源：http://xym.chenzaomai.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vdn.smart0.xyz

Ruby: s.length
来源：http://gsq.meibo888.top

C#:   s.Length
来源：http://oxk.chenzaomai.com

[A23] 大小写转换
来源：http://anr.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rwy.sweek.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mrr.jqgfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zel.mhx1999.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yqk.wangdashe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://osy.hcnkem.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tjw.hysaishi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nkt.nwbrower.top

C#:   s.ToUpper(); s.ToLower()
来源：http://zjd.c1oappe.top

[A24] 去除首尾空白
来源：http://kay.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rcu.xuanzx.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hjs.gaohongyu789.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pkj.wangdashe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://csf.bjfxy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zqt.fengsongda.top

Go:   strings.TrimSpace(s)
来源：http://kko.sysykeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cbd.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rud.fktsv.cn

[A25] 字符串比较
来源：http://stt.bbcook.cn

Py:   s1 == s2; s1 != s2
来源：http://rtc.pycfn.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xia.yvedp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pso.vehdjk.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jhj.shanyushiyangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bud.hfpthk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sfo.shanyushiyangtech.top

Ruby: s1 == s2; s1 <=> s2
来源：http://lxz.cdnleiting.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sfe.yueranfly.top

[A26] 类型转换总览
来源：http://faq.havefunace.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kyw.sufxvd.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vus.xylfe.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aye.zycfv.cn

TS:   Number() String() Boolean() x as number
来源：http://jlc.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zze.0kj1m.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cjy.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dmf.shzxlz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://puv.vqdsnc.cn

================================================================================
来源：http://jzw.tanke756.top

B. 流程控制
来源：http://qtn.svipenyu.cn

================================================================================
来源：http://kbv.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://pkj.dianchejie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nrf.tianlin.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xun.nwbrower.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://acb.andypj.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nlq.bbcook.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://avi.hcnkem.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xmb.hnxiangtu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wah.dashuyun.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ndz.ctjpmb.com

[B02] 多分支 else if / elif
来源：http://jbc.gogol.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fns.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fwn.zhaomingkeji.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ier.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yyu.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ezn.ydzc1.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rgw.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fem.yj20258.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rwf.iojbl.cn

[B03] switch / match / case
来源：http://vjj.fanxiaobao.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nlm.shanyushiyangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nkw.yueranfly.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aau.yj20258888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ngp.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nme.sxryk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fzt.ydzc1.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fkg.smart0.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jlw.xylfe.cn

[B04] for 计数循环
来源：http://ebc.hcnkem.com

Py:   for i in range(10): print(i)
来源：http://ioo.zhoulong.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vdn.hongshengwenyu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sjx.zhengqikj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bll.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vfi.vehdjk.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://azr.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://pgm.birdmap.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qxm.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://itw.ppjwa.cn

Py:   for item in arr: print(item)
来源：http://ryf.chenzaomai.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vte.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://amo.hammf.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zpk.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zty.ivvv.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pbl.yfazqb.com

Ruby: arr.each { |item| puts item }
来源：http://lju.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eel.ehwqpu.com

[B06] 遍历字典 / 对象
来源：http://qcg.ydjk.org.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hth.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mfc.cashguo.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lii.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xvk.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eqc.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qsi.vqdsnc.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dxq.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://btv.yangfankeji.com

[B07] while 循环
来源：http://kqh.yuxming.cn

Py:   while i < 10: i += 1
来源：http://yzn.316326.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://pgo.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://bdf.fehbvm.com

TS:   while (i < 10) { i++; }
来源：http://pgv.feifeiyinyue.top

Java: while (i < 10) { i++; }
来源：http://vnk.chenlongwang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fkh.dashuyun.cn

Ruby: while i < 10; i += 1; end
来源：http://ael.0kj1m.cn

C#:   while (i < 10) { i++; }
来源：http://zdo.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://zhy.jinqigufen.top

Py:   # 无 do-while：用 while True + break
来源：http://yqu.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://qpl.hnqzz.top

JS:   do { i++; } while (i < 10);
来源：http://tvv.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://jpj.jlsjyb.cn

Java: do { i++; } while (i < 10);
来源：http://uzf.yuanzhike.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kmc.zhixingplan.top

Ruby: begin; i += 1; end while i < 10
来源：http://kza.daxiang520.top

C#:   do { i++; } while (i < 10);
来源：http://otz.cheryme.top

[B09] break 与 continue
来源：http://ler.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iag.zdqjudy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lne.gotoacloud.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xqp.vehdjk.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://udd.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://das.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ylf.yuanzhike.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://frf.shzxlz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uja.ydzc1.top

[B10] 遍历同时拿索引
来源：http://azc.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rth.yj20258.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://soj.yuxming.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uyh.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://txu.vqdsnc.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://asv.xinyue.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gpi.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qew.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dww.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://qcj.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://gsd.aibaodan.cn

PHP:  range(0, 10, 2);
来源：http://otu.gogol.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hpc.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oao.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hrh.vqdsnc.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tlq.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://jph.havefunace.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://arj.yj202588.top

[B12] 跳出多层循环
来源：http://mkj.havefunace.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dzu.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vwl.quarkkingdee.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dya.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ucp.yongpay.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fth.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ttj.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dxu.hfpthk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uut.bjfxy.top

[B13] 判断是否为数字
来源：http://fod.yongpay.top

Py:   isinstance(x, (int, float))
来源：http://yqi.svipenyu.cn

PHP:  is_numeric($x)
来源：http://nhk.xinyue.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tmg.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uad.0kj1m.cn

Java: x instanceof Number
来源：http://waa.yanxiufei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oxy.cheryme.top

Ruby: x.is_a?(Numeric)
来源：http://lnm.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://rjv.ydzc1.top

[B14] 判断值是否在集合内
来源：http://pyu.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xjp.gotoacloud.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vho.yj20258888.top

JS:   [1, 2, 3].includes(x)
来源：http://dwv.cdnleiting.top

TS:   [1, 2, 3].includes(x)
来源：http://iok.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dah.havefunace.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fzv.sweek.top

Ruby: [1, 2, 3].include?(x)
来源：http://aqw.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lpl.jlsjyb.cn

[B15] 布尔运算与取反
来源：http://sbz.cheryme.top

Py:   a and b or not c
来源：http://lbw.ydjk.org.cn

PHP:  $a && $b || !$c
来源：http://eed.jiagoushi.top

JS:   a && b || !c
来源：http://enr.fehbvm.com

TS:   a && b || !c
来源：http://pgq.yj20258.top

Java: a && b || !c
来源：http://wdf.ywan-chungtsiang.top

Go:   a && b || !c
来源：http://nxh.ybcxt.top

Ruby: a && b || !c
来源：http://uqt.hfpthk.cn

C#:   a && b || !c
来源：http://inb.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jjb.sysykeji.top

Py:   if not data: return
来源：http://nqu.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://iid.iojbl.cn

JS:   if (!data) return;
来源：http://yik.iojbl.cn

TS:   if (!data) return;
来源：http://qaj.sweek.top

Java: if (data == null) return;
来源：http://kat.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://aqh.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://xew.mhx1999.top

C#:   if (data == null) return;
来源：http://vuc.yj202588.top


<!-- 参考信息 -->