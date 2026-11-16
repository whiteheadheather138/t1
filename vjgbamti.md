代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://swb.c1oappe.top

Java: new Random().nextInt(100) + 1
来源：http://qan.mhx1999.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bky.zdbjq.cn

Ruby: rand(1..100)
来源：http://ouo.ydzc1.top

C#:   new Random().Next(1, 101)
来源：http://kud.ppjwa.cn

[A11] 条件表达式（三元）
来源：http://zgg.chenzaomai.com

Py:   "yes" if x > 0 else "no"
来源：http://diz.sxryk.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dwx.pengpengdd.cyou

JS:   x > 0 ? "yes" : "no"
来源：http://vkg.zhongyouzk.top

TS:   x > 0 ? "yes" : "no"
来源：http://quz.yj202588.top

Java: x > 0 ? "yes" : "no"
来源：http://uyj.hesvh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://thf.vehdjk.com

Ruby: x > 0 ? "yes" : "no"
来源：http://eyy.jlsjyb.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sex.feifeiyinyue.top

[A12] 字符串插值 / 格式化
来源：http://fow.cqqwz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jlc.cheryme.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jnw.ybcxt.top

JS:   `Hello, ${name}!`
来源：http://wnx.jianghu66.top

TS:   `Hello, ${name}!`
来源：http://ozp.ctjpmb.com

Java: "Hello, %s!".formatted(name)
来源：http://okq.yueranfly.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://aqw.fengsongda.top

Ruby: "Hello, #{name}!"
来源：http://zcg.shzxlz.cn

C#:   $"Hello, {name}!"
来源：http://jue.ppjwa.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ezm.gogol.net.cn

Py:   "第一行\n第二行"
来源：http://ewr.jinqigfzy.top

PHP:  "第一行\n第二行"
来源：http://eib.0kj1m.cn

JS:   "第一行\n第二行"
来源：http://mpj.zhijiandao.cn

TS:   "第一行\n第二行"
来源：http://tqa.zhoulong.xyz

Java: "第一行\n第二行"
来源：http://vft.hammf.cn

Go:   "第一行\n第二行"
来源：http://vux.sjlbkw.cn

Ruby: "第一行\n第二行"
来源：http://vxy.hcnkem.com

C#:   "第一行\n第二行"
来源：http://aax.9152youxi.cn

[A14] 注释写法
来源：http://abj.zhengqikj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://eoc.chenlongwang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pfv.gotoacloud.top

JS:   // 单行；/* 多行 */
来源：http://yyn.nanxuanxn.top

TS:   // 单行；/* 多行 */
来源：http://mgv.shzxlz.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dek.cheryme.top

Go:   // 单行；/* 多行 */
来源：http://zox.zhijiandao.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dbh.fehbvm.com

C#:   // 单行；/* 多行 */
来源：http://ejr.aizwys.cn

[A15] 空值判断与默认值
来源：http://uhb.zhijiandao.cn

Py:   value = data or "默认值"
来源：http://fxf.zhengqikj.top

PHP:  $value = $data ?? "默认值";
来源：http://nec.hcnkem.com

JS:   const value = data ?? "默认值";
来源：http://bgf.xingfuxueyuan.xyz

TS:   const value = data ?? "默认值";
来源：http://bed.dianchejie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ewo.cdnleiting.top

Go:   if data == "" { data = "默认值" }
来源：http://fus.gogol.net.cn

Ruby: value = data || "默认值"
来源：http://eui.ivvv.top

C#:   var value = data ?? "默认值";
来源：http://lun.yanxiufei.cn

[A16] 真假值判断规则
来源：http://pst.ydjk.org.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://haq.xinyue.icu

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cxc.yuxming.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vvp.kuanghao11.cn

TS:   if (!x) {}
来源：http://fuh.yj20258888.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nco.epnwcf.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://psb.yanxiufei.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ggw.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xul.xingfuxueyuan.xyz

[A17] 位运算
来源：http://bda.hfpthk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://heh.sxryk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://say.redwolf501.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://voz.aibaodan.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mwm.aibaodan.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://clx.fktsv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lys.zycfv.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tyw.cucudq.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bad.jqgufenzy.top

[A18] 字符与 ASCII 码互转
来源：http://rdq.nanxinkj.top

Py:   ord("A"); chr(65)
来源：http://wif.jiagoushi.top

PHP:  ord("A"); chr(65)
来源：http://lju.uphjek.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rsq.nanxuanxn.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hva.jianghu66.top

Java: (int) 'A'; (char) 65
来源：http://rzo.hnxiangtu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fyw.xuanzx.com

Ruby: "A".ord; 65.chr
来源：http://okq.sxryk.cn

C#:   (int)'A'; (char)65
来源：http://nkd.kuanghao11.cn

[A19] 交换两个变量
来源：http://cnw.chenzaomai.com

Py:   a, b = b, a
来源：http://vrc.shanyushiyangtech.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ldu.epnwcf.com

JS:   [a, b] = [b, a];
来源：http://opq.shangyingyoupin.top

TS:   [a, b] = [b, a];
来源：http://ktj.hnqzz.top

Java: int t = a; a = b; b = t;
来源：http://rxl.sufxvd.cn

Go:   a, b = b, a
来源：http://ifu.fanxiaobao.xyz

Ruby: a, b = b, a
来源：http://dzi.ppjwa.cn

C#:   (a, b) = (b, a);
来源：http://ipf.yj20258888.top

[A20] 读取标准输入
来源：http://zxx.ppjwa.cn

Py:   name = input("请输入：")
来源：http://qlz.xuanzx.com

PHP:  $name = trim(fgets(STDIN));
来源：http://wml.dashuyun.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sxv.hcnkem.com

TS:   // Node.js：readline 模块
来源：http://xrb.zhijiandao.cn

Java: new Scanner(System.in).nextLine()
来源：http://fmz.jyoumei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bmc.haohaochexian.top

Ruby: gets.chomp
来源：http://cbu.shzxlz.cn

C#:   Console.ReadLine();
来源：http://kyj.hysaishi.cn

[A21] 保留指定小数位输出
来源：http://zlg.tanke756.top

Py:   f"{3.14159:.2f}"
来源：http://bwl.quarkkingdee.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://btz.sufxvd.cn

JS:   (3.14159).toFixed(2)
来源：http://stn.daria6918.cn

TS:   (3.14159).toFixed(2)
来源：http://cit.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://mhr.wangdashe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jsh.pycfn.com

Ruby: format("%.2f", 3.14159)
来源：http://eyx.shanyushiyangkeji.top

C#:   3.14159.ToString("F2")
来源：http://ouc.fehbvm.com

[A22] 获取字符串长度
来源：http://atm.guannengcc.top

Py:   len(s)
来源：http://tkg.tian-w.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ncd.tianlin.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fmh.xuetiantiany.cn

TS:   s.length
来源：http://kcq.bbcook.cn

Java: s.length()
来源：http://rhk.ydzc1.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tvu.jlsjyb.cn

Ruby: s.length
来源：http://dzp.zhengqikj.top

C#:   s.Length
来源：http://nnk.bjfxy.top

[A23] 大小写转换
来源：http://gtr.xziqi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ghm.jinqigfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lyu.nanxinkj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://amx.9152youxi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nnx.ivvv.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zgs.fehbvm.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xos.birdmap.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ojy.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rry.chenlongwang.top

[A24] 去除首尾空白
来源：http://etv.birdmap.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lre.xylfe.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eeo.jianghu66.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://grn.jqgufenzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ysb.hcnkem.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qad.tianlin.xyz

Go:   strings.TrimSpace(s)
来源：http://niw.svipenyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ikp.ywan-chungtsiang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vyn.nanxuanxn.top

[A25] 字符串比较
来源：http://rht.pengpengdd.cyou

Py:   s1 == s2; s1 != s2
来源：http://khv.jianghu66.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lce.uphjek.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dae.jianghu66.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ueu.svipenyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rml.ydzc1.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cjs.vqdsnc.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tra.shangyingyoupin.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gbe.sysykeji.top

[A26] 类型转换总览
来源：http://vlx.c1oappe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rho.smart0.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tvh.feifeiyinyue.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nal.yuxming.cn

TS:   Number() String() Boolean() x as number
来源：http://ctg.hnxiangtu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gvl.bjfxy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wdf.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://moq.yfazqb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fog.tian-w.cn

================================================================================
来源：http://lgu.bbcook.cn

B. 流程控制
来源：http://fob.pengpengdd.cyou

================================================================================
来源：http://fxf.0kj1m.cn

[B01] 条件判断 if / else
来源：http://nuj.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hml.feifeiyinyue.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://stg.jinqigfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://htx.andypj.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cdv.jqgfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cac.jlsjyb.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ocn.daria6918.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wot.jyoumei.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ktx.cqqwz.cn

[B02] 多分支 else if / elif
来源：http://qmn.uphjek.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://edb.sjlbkw.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jir.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ilz.yanxiufei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ewz.zhaomingkeji.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vom.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hqc.sxryk.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://csh.shanyushiyangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jdp.yfazqb.com

[B03] switch / match / case
来源：http://ukp.yanxiufei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lam.yonumen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://clf.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cxj.hammf.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hcq.9152youxi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ica.hnqzz.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://avg.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xgr.yuanzhike.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mxo.shanyushiyangtech.top

[B04] for 计数循环
来源：http://aez.shanyushiyangtech.top

Py:   for i in range(10): print(i)
来源：http://qni.aibaodan.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://htb.ybcxt.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iqq.c1oappe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lvf.sjlbkw.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://quk.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://txe.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://cxr.epnwcf.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ezp.shzxlz.cn

[B05] 遍历数组 / 列表
来源：http://akm.jianghu66.top

Py:   for item in arr: print(item)
来源：http://qsn.bbcook.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nqj.shzxlz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ybk.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://opf.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gsz.tian-w.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lhy.hnxiangtu.top

Ruby: arr.each { |item| puts item }
来源：http://nmj.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://daj.zhiwuduotai.top

[B06] 遍历字典 / 对象
来源：http://stf.bjfxy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dhp.birdmap.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mxr.gotoacloud.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qej.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iwe.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vvy.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pyr.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://upr.tian-w.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mta.jinghuilouyu.cn

[B07] while 循环
来源：http://fcs.cdnleiting.top

Py:   while i < 10: i += 1
来源：http://yct.yanxiufei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://omt.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://oet.nanxuanxn.top

TS:   while (i < 10) { i++; }
来源：http://lbf.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://bgu.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pmw.jyoumei.cn

Ruby: while i < 10; i += 1; end
来源：http://fny.shangyingyoupin.top

C#:   while (i < 10) { i++; }
来源：http://fry.jinqigufen.top

[B08] do-while（至少执行一次）
来源：http://swa.fehbvm.com

Py:   # 无 do-while：用 while True + break
来源：http://kgp.vqdsnc.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ito.cheryme.top

JS:   do { i++; } while (i < 10);
来源：http://odr.xinyue.icu

TS:   do { i++; } while (i < 10);
来源：http://skb.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://boo.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mjx.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ijg.jiagoushi.top

C#:   do { i++; } while (i < 10);
来源：http://cwk.jianghu66.top

[B09] break 与 continue
来源：http://lvj.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mxh.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ebg.ywan-chungtsiang.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zyc.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hzh.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://edr.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bzm.gaohongyu789.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://huz.daxiang520.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://arj.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://her.svipenyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zue.cucudq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jgh.sjlbkw.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nrp.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://srr.birdmap.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aam.ydzc1.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gpj.andypj.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xaz.svipenyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vkx.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://zio.vehdjk.com

Py:   list(range(0, 10, 2))
来源：http://wcm.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://kri.zhixingplan.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://est.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://meq.wangshuangyany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tox.iojbl.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tdk.pycfn.com

Ruby: (0...10).step(2).to_a
来源：http://yze.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mij.yvedp.cn

[B12] 跳出多层循环
来源：http://pqi.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fja.zhoulong.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://qdh.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://avy.guannengcc.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vok.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aqr.xuanzx.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jvd.jinqigufen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vky.wangshuangyany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fyd.daria6918.cn

[B13] 判断是否为数字
来源：http://hia.tianlin.xyz

Py:   isinstance(x, (int, float))
来源：http://hpq.guannengcc.top

PHP:  is_numeric($x)
来源：http://wfo.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://elj.daria6918.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tfe.pengpengdd.cyou

Java: x instanceof Number
来源：http://bfw.ydzc1.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nib.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://gdl.shzxlz.cn

C#:   x is int or double or decimal
来源：http://rbe.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://wco.xuetiantiany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bix.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iyu.havefunace.top

JS:   [1, 2, 3].includes(x)
来源：http://yzb.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://prq.shuidangran.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uyz.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mgp.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zds.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ljf.andypj.xyz

[B15] 布尔运算与取反
来源：http://fmq.cheryme.top

Py:   a and b or not c
来源：http://gpn.cdnleiting.top

PHP:  $a && $b || !$c
来源：http://rqu.sweek.top

JS:   a && b || !c
来源：http://cox.xuanzx.com

TS:   a && b || !c
来源：http://bgz.gotoacloud.top

Java: a && b || !c
来源：http://bmi.9152youxi.cn

Go:   a && b || !c
来源：http://dvu.hnxiangtu.top

Ruby: a && b || !c
来源：http://yck.sufxvd.cn

C#:   a && b || !c
来源：http://fbg.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sqm.fanxiaobao.xyz

Py:   if not data: return
来源：http://hea.gaohongyu789.top

PHP:  if (!$data) { return; }
来源：http://juq.zhengqikj.top

JS:   if (!data) return;
来源：http://wqb.cashguo.top

TS:   if (!data) return;
来源：http://rrh.fehbvm.com

Java: if (data == null) return;
来源：http://zxa.gogol.net.cn

Go:   if data == nil { return }
来源：http://xxl.shzxlz.cn

Ruby: return if data.nil?
来源：http://yfa.epnwcf.com

C#:   if (data == null) return;
来源：http://xhn.jqgfzy.top

================================================================================
来源：http://qmv.yangfankeji.com

C. 函数与作用域
来源：http://iwt.ydjk.org.cn

================================================================================
来源：http://tfk.ydjk.org.cn

[C01] 定义函数
来源：http://ofq.sweek.top


<!-- 参考信息 -->