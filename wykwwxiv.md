代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fyl.jinyuanbaomall.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ybd.52xcode.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dme.aizwys.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nda.yuxming.cn

[A10] 生成随机数
来源：http://akt.ehwqpu.com

Py:   import random; random.randint(1, 100)
来源：http://edi.yj20258888.top

PHP:  random_int(1, 100);
来源：http://btw.sxryk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sgs.hywenlv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tzg.zhixingplan.top

Java: new Random().nextInt(100) + 1
来源：http://emj.havefunace.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jwz.aibaodan.cn

Ruby: rand(1..100)
来源：http://ywd.feifeiyinyue.top

C#:   new Random().Next(1, 101)
来源：http://scs.tanke756.top

[A11] 条件表达式（三元）
来源：http://hga.hammf.cn

Py:   "yes" if x > 0 else "no"
来源：http://arf.birdmap.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qol.cucudq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gfo.sjlbkw.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xlg.cashguo.top

Java: x > 0 ? "yes" : "no"
来源：http://nil.tanke756.top

Go:   // 无三元运算符，需用 if 语句
来源：http://lee.jinyuanbaomall.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vnj.yuxming.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wir.zdqjudy.top

[A12] 字符串插值 / 格式化
来源：http://pfb.ywan-chungtsiang.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tko.zdbjq.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://smf.aibaodan.cn

JS:   `Hello, ${name}!`
来源：http://opc.fanxiaobao.xyz

TS:   `Hello, ${name}!`
来源：http://xsi.pycfn.com

Java: "Hello, %s!".formatted(name)
来源：http://kzr.shanyushiyangtech.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ols.snrcjt.cn

Ruby: "Hello, #{name}!"
来源：http://rul.ctjpmb.com

C#:   $"Hello, {name}!"
来源：http://ndi.wangdashe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qfs.sysykeji.top

Py:   "第一行\n第二行"
来源：http://wkc.sysykeji.top

PHP:  "第一行\n第二行"
来源：http://qob.bbcook.cn

JS:   "第一行\n第二行"
来源：http://egn.cashguo.top

TS:   "第一行\n第二行"
来源：http://wvr.xuetiantiany.cn

Java: "第一行\n第二行"
来源：http://cia.zhoulong.xyz

Go:   "第一行\n第二行"
来源：http://ztx.zhijiandao.cn

Ruby: "第一行\n第二行"
来源：http://sai.ppjwa.cn

C#:   "第一行\n第二行"
来源：http://lkd.zhengqikj.top

[A14] 注释写法
来源：http://cdc.9152youxi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gdc.hfpthk.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ztt.yj20258888.top

JS:   // 单行；/* 多行 */
来源：http://gmo.jqgufenzy.top

TS:   // 单行；/* 多行 */
来源：http://jfi.ppjwa.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sda.svipenyu.cn

Go:   // 单行；/* 多行 */
来源：http://ivg.snrcjt.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kum.xingfuxueyuan.xyz

C#:   // 单行；/* 多行 */
来源：http://jmo.yuxming.cn

[A15] 空值判断与默认值
来源：http://omv.gzhubu.top

Py:   value = data or "默认值"
来源：http://ccb.zdqjudy.top

PHP:  $value = $data ?? "默认值";
来源：http://csn.xuetiantiany.cn

JS:   const value = data ?? "默认值";
来源：http://xik.cucudq.cn

TS:   const value = data ?? "默认值";
来源：http://xko.zhongyouzk.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gjr.bbcook.cn

Go:   if data == "" { data = "默认值" }
来源：http://kot.0kj1m.cn

Ruby: value = data || "默认值"
来源：http://hwr.zhongyouzk.top

C#:   var value = data ?? "默认值";
来源：http://bfx.yuxming.cn

[A16] 真假值判断规则
来源：http://iix.shangyingyoupin.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jzl.shangyingyoupin.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hvx.fanxiaobao.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://moe.mhx1999.top

TS:   if (!x) {}
来源：http://jxs.smart0.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jnl.zhoulong.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ocv.redwolf501.top

Ruby: unless x            # nil 与 false 为假
来源：http://wwz.zhongyouzk.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vwp.feifeiyinyue.top

[A17] 位运算
来源：http://fud.xinyue.icu

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dqu.gzhubu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uqo.sufxvd.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eov.jinqigfzy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gbg.jinyuanbaomall.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qbm.shuidangran.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://omn.dashuyun.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uzh.jinqigfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xpb.pycfn.com

[A18] 字符与 ASCII 码互转
来源：http://mmn.dianchejie.cn

Py:   ord("A"); chr(65)
来源：http://fwa.gotoacloud.top

PHP:  ord("A"); chr(65)
来源：http://xxk.xuetiantiany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ukb.meibo888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bpl.hammf.cn

Java: (int) 'A'; (char) 65
来源：http://hjy.xuetiantiany.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vjo.hongshengwenyu.top

Ruby: "A".ord; 65.chr
来源：http://ypj.bbcook.cn

C#:   (int)'A'; (char)65
来源：http://fzl.meibo888.top

[A19] 交换两个变量
来源：http://are.hfpthk.cn

Py:   a, b = b, a
来源：http://kjf.havefunace.top

PHP:  [$a, $b] = [$b, $a];
来源：http://bft.gzhubu.top

JS:   [a, b] = [b, a];
来源：http://frf.shangyingyoupin.top

TS:   [a, b] = [b, a];
来源：http://cao.chenlongwang.top

Java: int t = a; a = b; b = t;
来源：http://rxb.hysaishi.cn

Go:   a, b = b, a
来源：http://xpf.hywenlv.cn

Ruby: a, b = b, a
来源：http://lpa.hywenlv.cn

C#:   (a, b) = (b, a);
来源：http://qac.ydzc1.top

[A20] 读取标准输入
来源：http://vjd.xuetiantiany.cn

Py:   name = input("请输入：")
来源：http://kqj.dashuyun.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jbd.zdbjq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qsx.yonumen.top

TS:   // Node.js：readline 模块
来源：http://xbp.yonumen.top

Java: new Scanner(System.in).nextLine()
来源：http://bqb.tarul.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://loc.xinyue.icu

Ruby: gets.chomp
来源：http://uhk.wangshuangyany.cn

C#:   Console.ReadLine();
来源：http://qjo.daria6918.cn

[A21] 保留指定小数位输出
来源：http://hel.yfazqb.com

Py:   f"{3.14159:.2f}"
来源：http://yxl.sjlbkw.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xhw.shuidangran.top

JS:   (3.14159).toFixed(2)
来源：http://yud.pycfn.com

TS:   (3.14159).toFixed(2)
来源：http://mfx.316326.xyz

Java: String.format("%.2f", 3.14159)
来源：http://pnr.nanxinkj.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pnr.yuxming.cn

Ruby: format("%.2f", 3.14159)
来源：http://iva.tian-w.cn

C#:   3.14159.ToString("F2")
来源：http://rwn.yvedp.cn

[A22] 获取字符串长度
来源：http://unb.jiagoushi.top

Py:   len(s)
来源：http://jpr.xziqi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vvn.meibo888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tss.fehbvm.com

TS:   s.length
来源：http://mxb.jqgfzy.top

Java: s.length()
来源：http://uny.bbcook.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nys.gotoacloud.top

Ruby: s.length
来源：http://mmz.mhx1999.top

C#:   s.Length
来源：http://cqd.yueranfly.top

[A23] 大小写转换
来源：http://xit.feifeiyinyue.top

Py:   s.upper(); s.lower(); s.title()
来源：http://jux.guannengcc.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mhu.hammf.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://auw.yanxiufei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bmc.sjlbkw.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://waf.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tfk.ppjwa.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ndw.ppjwa.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gql.chenzaomai.com

[A24] 去除首尾空白
来源：http://czw.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fua.sweek.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oqe.ybcxt.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iye.gzhubu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nlu.havefunace.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ude.zhiwuduotai.top

Go:   strings.TrimSpace(s)
来源：http://fsk.316326.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xvv.tianlin.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lfi.nwbrower.top

[A25] 字符串比较
来源：http://rnw.pengpengdd.cyou

Py:   s1 == s2; s1 != s2
来源：http://shd.sjlbkw.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ela.jinqigfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wyp.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://luk.zhijiandao.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zfw.xinyue.icu

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lal.guowangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qin.yj20258888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pch.sjlbkw.cn

[A26] 类型转换总览
来源：http://xpv.shuidangran.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qae.jyoumei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cwy.daxiang520.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nbc.0kj1m.cn

TS:   Number() String() Boolean() x as number
来源：http://mfl.havefunace.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ckq.sysykeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cmx.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://oqo.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://okf.sweek.top

================================================================================
来源：http://rlh.chenzaomai.com

B. 流程控制
来源：http://pgv.wangdashe.top

================================================================================
来源：http://upo.gzhubu.top

[B01] 条件判断 if / else
来源：http://iht.cqqwz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cct.ywan-chungtsiang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hvh.gaohongyu789.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qmr.smart0.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gzw.chenzaomai.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://qzt.shanyushiyangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lmp.daria6918.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mir.aibaodan.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cif.cashguo.top

[B02] 多分支 else if / elif
来源：http://fmn.xylfe.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rts.yj202588.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lwy.shuidangran.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qxi.zhengqikj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ssa.tanke756.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://btz.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kye.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gms.yangfankeji.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wpm.hywenlv.cn

[B03] switch / match / case
来源：http://iwv.chenjidiqi.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lwn.bjfxy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rue.xingfuxueyuan.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qie.hywenlv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nsr.hnxiangtu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ytf.jiagoushi.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lcv.cqqwz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lnn.sweek.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zot.feifeiyinyue.top

[B04] for 计数循环
来源：http://jag.jinghuilouyu.cn

Py:   for i in range(10): print(i)
来源：http://hio.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ufu.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ivf.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oon.hfpthk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ein.ydzc1.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ztv.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://gdc.zhoulong.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tts.nanxuanxn.top

[B05] 遍历数组 / 列表
来源：http://pbe.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://xlo.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hur.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://the.chenzaomai.com

TS:   for (const item of arr) { console.log(item); }
来源：http://kvr.xinyue.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://ggw.yj20258888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cbh.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://kor.gaohongyu789.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wpy.havefunace.top

[B06] 遍历字典 / 对象
来源：http://cxb.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vsc.jqgufenzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://imv.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nbz.ppjwa.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://egd.hnqzz.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hph.nanxuanxn.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://inj.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yxb.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zjy.wangdashe.top

[B07] while 循环
来源：http://ehh.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://yus.gzhubu.top

PHP:  while ($i < 10) { $i++; }
来源：http://mwk.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://iyy.redwolf501.top

TS:   while (i < 10) { i++; }
来源：http://dsc.tianlin.xyz

Java: while (i < 10) { i++; }
来源：http://xja.xuetiantiany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://igg.tian-w.cn

Ruby: while i < 10; i += 1; end
来源：http://iwi.yfazqb.com

C#:   while (i < 10) { i++; }
来源：http://lvp.chenlongwang.top

[B08] do-while（至少执行一次）
来源：http://nzz.yueranfly.top

Py:   # 无 do-while：用 while True + break
来源：http://zon.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wcq.shzxlz.cn

JS:   do { i++; } while (i < 10);
来源：http://kcu.zhoulong.xyz

TS:   do { i++; } while (i < 10);
来源：http://kpu.mhx1999.top

Java: do { i++; } while (i < 10);
来源：http://ukm.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://boj.shzxlz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vny.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://qyr.yvedp.cn

[B09] break 与 continue
来源：http://onu.hnqzz.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tgc.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wjz.shuidangran.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ozb.havefunace.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fcy.zhixingplan.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mpd.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nzm.ybcxt.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aub.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://abt.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://vox.shuidangran.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cbv.zhongyouzk.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kuy.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xqh.haohaochexian.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qyj.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blh.hysaishi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uja.gaohongyu789.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bat.ctjpmb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kap.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://mwv.dashuyun.cn

Py:   list(range(0, 10, 2))
来源：http://zho.zycfv.cn

PHP:  range(0, 10, 2);
来源：http://yao.jiagoushi.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kqr.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eyk.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yov.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://acp.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://fnt.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mol.sjlbkw.cn

[B12] 跳出多层循环
来源：http://ofj.yuxming.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://drl.chenjidiqi.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://ymy.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xhp.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pio.xylfe.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://doz.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pky.chenlongwang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qgy.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ffd.fzhhl.top

[B13] 判断是否为数字
来源：http://ura.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://gsy.hfpthk.cn

PHP:  is_numeric($x)
来源：http://fkv.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://akv.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zjj.yj202588.top

Java: x instanceof Number
来源：http://xsw.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ioa.quarkkingdee.top

Ruby: x.is_a?(Numeric)
来源：http://eyv.nanxuanxn.top

C#:   x is int or double or decimal
来源：http://xiu.wangdashe.top

[B14] 判断值是否在集合内
来源：http://adt.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://klf.cdnleiting.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nml.ydzc1.top

JS:   [1, 2, 3].includes(x)
来源：http://sfa.nanxuanxn.top

TS:   [1, 2, 3].includes(x)
来源：http://bec.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xhx.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qrr.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://bfo.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dsw.mhx1999.top

[B15] 布尔运算与取反
来源：http://iey.yj20258888.top

Py:   a and b or not c
来源：http://jxi.andypj.xyz

PHP:  $a && $b || !$c
来源：http://lxx.yueranfly.top

JS:   a && b || !c
来源：http://zog.cucudq.cn

TS:   a && b || !c
来源：http://frr.epnwcf.com

Java: a && b || !c
来源：http://vue.vqdsnc.cn

Go:   a && b || !c
来源：http://ixy.gaohongyu789.top

Ruby: a && b || !c
来源：http://zcb.xziqi.cn

C#:   a && b || !c
来源：http://mhi.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://fjs.sweek.top

Py:   if not data: return
来源：http://utr.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://zem.iojbl.cn

JS:   if (!data) return;
来源：http://bsf.316326.xyz

TS:   if (!data) return;
来源：http://nvv.aibaodan.cn


<!-- 参考信息 -->