代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vik.316326.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ngi.feifeiyinyue.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uzl.chenzaomai.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nvs.hnxiangtu.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jug.jinqigufen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jth.chenjidiqi.icu

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zdc.ctjpmb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yyx.fktsv.cn

[A10] 生成随机数
来源：http://zma.jinghuilouyu.cn

Py:   import random; random.randint(1, 100)
来源：http://wgo.cheryme.top

PHP:  random_int(1, 100);
来源：http://vsj.jinqigfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wno.sjlbkw.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hge.sysykeji.top

Java: new Random().nextInt(100) + 1
来源：http://ppr.hywenlv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qmo.316326.xyz

Ruby: rand(1..100)
来源：http://szx.shanyushiyangkeji.top

C#:   new Random().Next(1, 101)
来源：http://fxt.hcnkem.com

[A11] 条件表达式（三元）
来源：http://syv.9152youxi.cn

Py:   "yes" if x > 0 else "no"
来源：http://ult.jinqigufen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://sdf.mhx1999.top

JS:   x > 0 ? "yes" : "no"
来源：http://ynf.ydzc1.top

TS:   x > 0 ? "yes" : "no"
来源：http://skk.yangfankeji.com

Java: x > 0 ? "yes" : "no"
来源：http://enl.iojbl.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nph.yj202588.top

Ruby: x > 0 ? "yes" : "no"
来源：http://jxh.jinqigufen.top

C#:   x > 0 ? "yes" : "no"
来源：http://xgu.guowangkeji.top

[A12] 字符串插值 / 格式化
来源：http://vwf.cucudq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://iwi.jianghu66.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uly.zhoulong.xyz

JS:   `Hello, ${name}!`
来源：http://qrb.gzhubu.top

TS:   `Hello, ${name}!`
来源：http://rzc.snrcjt.cn

Java: "Hello, %s!".formatted(name)
来源：http://mbn.jyoumei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ifz.nwbrower.top

Ruby: "Hello, #{name}!"
来源：http://obo.chenlongwang.top

C#:   $"Hello, {name}!"
来源：http://veu.gzhubu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://fbf.hnqzz.top

Py:   "第一行\n第二行"
来源：http://sfi.hnqzz.top

PHP:  "第一行\n第二行"
来源：http://swy.jinqigfzy.top

JS:   "第一行\n第二行"
来源：http://hfc.tanke756.top

TS:   "第一行\n第二行"
来源：http://oju.zycfv.cn

Java: "第一行\n第二行"
来源：http://fiz.nwbrower.top

Go:   "第一行\n第二行"
来源：http://rzb.gogol.net.cn

Ruby: "第一行\n第二行"
来源：http://tdh.smart0.xyz

C#:   "第一行\n第二行"
来源：http://fzu.ehwqpu.com

[A14] 注释写法
来源：http://vfl.tarul.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sda.quarkkingdee.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://put.pycfn.com

JS:   // 单行；/* 多行 */
来源：http://ixk.ivvv.top

TS:   // 单行；/* 多行 */
来源：http://cvo.ydzc1.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ysz.shuidangran.top

Go:   // 单行；/* 多行 */
来源：http://krv.wangdashe.top

Ruby: # 单行；=begin 多行 =end
来源：http://ksv.snrcjt.cn

C#:   // 单行；/* 多行 */
来源：http://nti.nanxinkj.top

[A15] 空值判断与默认值
来源：http://yax.zhoulong.xyz

Py:   value = data or "默认值"
来源：http://kdk.tarul.cn

PHP:  $value = $data ?? "默认值";
来源：http://pgo.hnqzz.top

JS:   const value = data ?? "默认值";
来源：http://bwq.pengpengdd.cyou

TS:   const value = data ?? "默认值";
来源：http://fvk.52xcode.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hmp.cqqwz.cn

Go:   if data == "" { data = "默认值" }
来源：http://mya.ydzc1.top

Ruby: value = data || "默认值"
来源：http://fik.daxiang520.top

C#:   var value = data ?? "默认值";
来源：http://gxd.sxryk.cn

[A16] 真假值判断规则
来源：http://gvr.jinqigfzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pbz.zdbjq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kxd.hcnkem.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ltj.fzhhl.top

TS:   if (!x) {}
来源：http://hqj.feifeiyinyue.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pwp.snrcjt.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gik.svipenyu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tap.tianlin.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wpk.0kj1m.cn

[A17] 位运算
来源：http://kmd.feifeiyinyue.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wui.yangfankeji.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fmx.zhoulong.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bcb.bjfxy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ymt.hongshengwenyu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zwv.ywan-chungtsiang.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ogg.guowangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ijb.zhixingplan.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fbr.sysykeji.top

[A18] 字符与 ASCII 码互转
来源：http://nfl.yangfankeji.com

Py:   ord("A"); chr(65)
来源：http://rrx.chenjidiqi.icu

PHP:  ord("A"); chr(65)
来源：http://sas.0kj1m.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aos.gotoacloud.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sss.hysaishi.cn

Java: (int) 'A'; (char) 65
来源：http://hbn.shanyushiyangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wjz.sweek.top

Ruby: "A".ord; 65.chr
来源：http://hea.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://gcc.gaohongyu789.top

[A19] 交换两个变量
来源：http://utr.smart0.xyz

Py:   a, b = b, a
来源：http://yzp.yongpay.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mkw.shanyushiyangtech.top

JS:   [a, b] = [b, a];
来源：http://orl.haohaochexian.top

TS:   [a, b] = [b, a];
来源：http://txa.smart0.xyz

Java: int t = a; a = b; b = t;
来源：http://xsr.snrcjt.cn

Go:   a, b = b, a
来源：http://qsi.vqdsnc.cn

Ruby: a, b = b, a
来源：http://err.jinyuanbaomall.cn

C#:   (a, b) = (b, a);
来源：http://xsb.tian-w.cn

[A20] 读取标准输入
来源：http://piv.jinqigfzy.top

Py:   name = input("请输入：")
来源：http://rby.hywenlv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rsh.chenzaomai.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gmn.chenlongwang.top

TS:   // Node.js：readline 模块
来源：http://fnw.jinghuilouyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://bqi.yanxiufei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vgf.shangyingyoupin.top

Ruby: gets.chomp
来源：http://vpq.vqdsnc.cn

C#:   Console.ReadLine();
来源：http://qkc.cheryme.top

[A21] 保留指定小数位输出
来源：http://vbe.smart0.xyz

Py:   f"{3.14159:.2f}"
来源：http://gfj.xylfe.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://krt.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://xrl.jqgfzy.top

TS:   (3.14159).toFixed(2)
来源：http://uhr.yueranfly.top

Java: String.format("%.2f", 3.14159)
来源：http://sjq.hnxiangtu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ypw.ivvv.top

Ruby: format("%.2f", 3.14159)
来源：http://wwc.cashguo.top

C#:   3.14159.ToString("F2")
来源：http://btf.yfazqb.com

[A22] 获取字符串长度
来源：http://jym.hammf.cn

Py:   len(s)
来源：http://usp.sweek.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wuf.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://reo.dashuyun.cn

TS:   s.length
来源：http://gji.cashguo.top

Java: s.length()
来源：http://wrx.pengpengdd.cyou

Go:   len(s); utf8.RuneCountInString(s)
来源：http://med.zycfv.cn

Ruby: s.length
来源：http://wha.xuanzx.com

C#:   s.Length
来源：http://quv.havefunace.top

[A23] 大小写转换
来源：http://hsy.kuanghao11.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zxj.sxryk.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cib.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://syd.pycfn.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ods.kuanghao11.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://als.zhijiandao.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ldg.xziqi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xjz.nanxinkj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://njt.bjfxy.top

[A24] 去除首尾空白
来源：http://fta.fktsv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://plc.aibaodan.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aip.gotoacloud.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gvt.yanxiufei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://obg.iojbl.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kwy.uphjek.com

Go:   strings.TrimSpace(s)
来源：http://gds.tanke756.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mag.fehbvm.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oyy.c1oappe.top

[A25] 字符串比较
来源：http://trl.tianlin.xyz

Py:   s1 == s2; s1 != s2
来源：http://bww.yuanzhike.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mug.dianchejie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://esk.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zel.yuanzhike.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xnz.yuxming.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lsu.pengpengdd.cyou

Ruby: s1 == s2; s1 <=> s2
来源：http://uln.kuanghao11.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ofz.wangshuangyany.cn

[A26] 类型转换总览
来源：http://hzp.uphjek.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rgg.jianghu66.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pby.shangyingyoupin.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nru.zhongyouzk.top

TS:   Number() String() Boolean() x as number
来源：http://gla.c1oappe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vsp.hammf.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tfq.jinqigfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://miq.yuxming.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ajk.hesvh.cn

================================================================================
来源：http://wjh.hysaishi.cn

B. 流程控制
来源：http://oze.52xcode.cn

================================================================================
来源：http://voq.cdnleiting.top

[B01] 条件判断 if / else
来源：http://oqg.fengsongda.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rfp.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gcf.ydzc1.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zjp.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pas.nwbrower.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dlq.ybcxt.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ewo.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://erq.tian-w.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ond.jqgufenzy.top

[B02] 多分支 else if / elif
来源：http://orx.hammf.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tud.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://clu.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bhq.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fvg.shanyushiyangtech.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xkv.yuxming.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qbe.wangdashe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hlk.sxryk.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bli.gogol.net.cn

[B03] switch / match / case
来源：http://cby.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://abi.yj20258.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ypn.smart0.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mkt.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://obd.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ivy.guowangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wkc.fanxiaobao.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rlw.sxryk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qgh.sweek.top

[B04] for 计数循环
来源：http://yti.meibo888.top

Py:   for i in range(10): print(i)
来源：http://ans.hesvh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wmc.zycfv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bjc.hysaishi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cus.feifeiyinyue.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xdn.svipenyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pno.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://bno.yuanzhike.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nqy.fanxiaobao.xyz

[B05] 遍历数组 / 列表
来源：http://yzo.sweek.top

Py:   for item in arr: print(item)
来源：http://wzd.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jfj.52xcode.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://upx.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://beq.jyoumei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yuo.hysaishi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qcs.dianchejie.cn

Ruby: arr.each { |item| puts item }
来源：http://qlg.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gme.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://rcc.redwolf501.top

Py:   for k, v in d.items(): print(k, v)
来源：http://upm.hongshengwenyu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ene.daria6918.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ull.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ybs.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mxg.cheryme.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://shw.ivvv.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zvd.vehdjk.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lmj.zhiwuduotai.top

[B07] while 循环
来源：http://kuj.vehdjk.com

Py:   while i < 10: i += 1
来源：http://mwh.jinqigufen.top

PHP:  while ($i < 10) { $i++; }
来源：http://znl.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://fzz.fehbvm.com

TS:   while (i < 10) { i++; }
来源：http://txy.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://bpv.xuanzx.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vjv.zhaomingkeji.xyz

Ruby: while i < 10; i += 1; end
来源：http://zfg.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://fyb.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://uqe.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://tii.epnwcf.com

PHP:  do { $i++; } while ($i < 10);
来源：http://kyi.xziqi.cn

JS:   do { i++; } while (i < 10);
来源：http://rym.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://ypj.zhoulong.xyz

Java: do { i++; } while (i < 10);
来源：http://uya.fzhhl.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qfk.nanxuanxn.top

Ruby: begin; i += 1; end while i < 10
来源：http://tzh.52xcode.cn

C#:   do { i++; } while (i < 10);
来源：http://gfp.9152youxi.cn

[B09] break 与 continue
来源：http://rcw.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fmj.yueranfly.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zjv.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ieg.kuanghao11.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tkc.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yuv.sysykeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xxt.fzhhl.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uqz.quarkkingdee.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ukf.shzxlz.cn

[B10] 遍历同时拿索引
来源：http://syw.meibo888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sfo.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ujq.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vkm.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mvn.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qde.pycfn.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bcm.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://all.chenjidiqi.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bcx.aibaodan.cn

[B11] 生成数字序列 / 区间
来源：http://xke.yfazqb.com

Py:   list(range(0, 10, 2))
来源：http://rcm.jinqigufen.top

PHP:  range(0, 10, 2);
来源：http://vvg.shuidangran.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gdx.pycfn.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ucx.cqqwz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://faa.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://amp.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://neg.fengsongda.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://irw.aibaodan.cn

[B12] 跳出多层循环
来源：http://xej.fanxiaobao.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://kej.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://swl.cheryme.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zbp.ydjk.org.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sdo.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ysh.shanyushiyangtech.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://klw.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://agc.ydzc1.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wvj.gzhubu.top

[B13] 判断是否为数字
来源：http://xdm.xingfuxueyuan.xyz

Py:   isinstance(x, (int, float))
来源：http://gyh.zhiwuduotai.top

PHP:  is_numeric($x)
来源：http://svq.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cny.dashuyun.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bmq.epnwcf.com

Java: x instanceof Number
来源：http://ess.pycfn.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hes.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://wus.shzxlz.cn

C#:   x is int or double or decimal
来源：http://woq.mhx1999.top

[B14] 判断值是否在集合内
来源：http://roy.bjfxy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nju.zhengqikj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cuf.hnxiangtu.top

JS:   [1, 2, 3].includes(x)
来源：http://thw.hywenlv.cn

TS:   [1, 2, 3].includes(x)
来源：http://gvs.ywan-chungtsiang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nwp.yuanzhike.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fia.zdqjudy.top

Ruby: [1, 2, 3].include?(x)
来源：http://ygk.xinyue.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jfj.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://jwg.gotoacloud.top

Py:   a and b or not c
来源：http://bwn.fzhhl.top

PHP:  $a && $b || !$c
来源：http://bjp.haohaochexian.top

JS:   a && b || !c
来源：http://pec.fanxiaobao.xyz

TS:   a && b || !c
来源：http://dig.sufxvd.cn

Java: a && b || !c
来源：http://ama.zhoulong.xyz

Go:   a && b || !c
来源：http://nni.yongpay.top

Ruby: a && b || !c
来源：http://znu.hnxiangtu.top

C#:   a && b || !c
来源：http://sul.redwolf501.top

[B16] 卫语句：不满足条件提前返回
来源：http://kvc.fehbvm.com


<!-- 参考信息 -->