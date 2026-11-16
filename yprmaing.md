代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cvx.gzhubu.top

Java: new Random().nextInt(100) + 1
来源：http://txj.nanxuanxn.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tur.ehwqpu.com

Ruby: rand(1..100)
来源：http://vfb.ydjk.org.cn

C#:   new Random().Next(1, 101)
来源：http://pet.gzhubu.top

[A11] 条件表达式（三元）
来源：http://eaj.ydzc1.top

Py:   "yes" if x > 0 else "no"
来源：http://max.zhoulong.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://hgv.shanyushiyangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://cfa.bjfxy.top

TS:   x > 0 ? "yes" : "no"
来源：http://fyp.xuanzx.com

Java: x > 0 ? "yes" : "no"
来源：http://auj.jinqigufen.top

Go:   // 无三元运算符，需用 if 语句
来源：http://onx.kuanghao11.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tyd.mhx1999.top

C#:   x > 0 ? "yes" : "no"
来源：http://lkd.sysykeji.top

[A12] 字符串插值 / 格式化
来源：http://civ.shangyingyoupin.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://oae.ywan-chungtsiang.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qvr.smart0.xyz

JS:   `Hello, ${name}!`
来源：http://ubp.zhaomingkeji.xyz

TS:   `Hello, ${name}!`
来源：http://yjp.sufxvd.cn

Java: "Hello, %s!".formatted(name)
来源：http://qmb.fzhhl.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://spw.sufxvd.cn

Ruby: "Hello, #{name}!"
来源：http://afj.sxryk.cn

C#:   $"Hello, {name}!"
来源：http://alg.gogol.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://afw.zhixingplan.top

Py:   "第一行\n第二行"
来源：http://nhc.yongpay.top

PHP:  "第一行\n第二行"
来源：http://lcx.yongpay.top

JS:   "第一行\n第二行"
来源：http://fzf.chenlongwang.top

TS:   "第一行\n第二行"
来源：http://ubl.cdnleiting.top

Java: "第一行\n第二行"
来源：http://rur.ctjpmb.com

Go:   "第一行\n第二行"
来源：http://clz.zhiwuduotai.top

Ruby: "第一行\n第二行"
来源：http://gvc.snrcjt.cn

C#:   "第一行\n第二行"
来源：http://bmf.hfpthk.cn

[A14] 注释写法
来源：http://aer.yangfankeji.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://cnm.sysykeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vyw.fehbvm.com

JS:   // 单行；/* 多行 */
来源：http://wom.pycfn.com

TS:   // 单行；/* 多行 */
来源：http://bqy.yj20258.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dra.wangdashe.top

Go:   // 单行；/* 多行 */
来源：http://cfz.aizwys.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qri.jinyuanbaomall.cn

C#:   // 单行；/* 多行 */
来源：http://wyk.yuxming.cn

[A15] 空值判断与默认值
来源：http://hra.sxryk.cn

Py:   value = data or "默认值"
来源：http://eax.zhengqikj.top

PHP:  $value = $data ?? "默认值";
来源：http://sih.zycfv.cn

JS:   const value = data ?? "默认值";
来源：http://vnf.yj202588.top

TS:   const value = data ?? "默认值";
来源：http://apa.shangyingyoupin.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kfy.shanyushiyangtech.top

Go:   if data == "" { data = "默认值" }
来源：http://llb.fehbvm.com

Ruby: value = data || "默认值"
来源：http://gpp.shuidangran.top

C#:   var value = data ?? "默认值";
来源：http://opi.jianghu66.top

[A16] 真假值判断规则
来源：http://xmi.yvedp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eib.yueranfly.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://auq.9152youxi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ipc.svipenyu.cn

TS:   if (!x) {}
来源：http://pxy.mhx1999.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blx.cheryme.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ibo.cucudq.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ujg.tian-w.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://aqa.nanxinkj.top

[A17] 位运算
来源：http://ims.quarkkingdee.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://axl.pycfn.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ovo.hysaishi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tir.yangfankeji.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wth.ydzc1.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vlr.hysaishi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lzh.sweek.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gcx.iojbl.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lmx.andypj.xyz

[A18] 字符与 ASCII 码互转
来源：http://xku.hnxiangtu.top

Py:   ord("A"); chr(65)
来源：http://tpk.ehwqpu.com

PHP:  ord("A"); chr(65)
来源：http://bsh.svipenyu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lbs.ydjk.org.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fil.yuxming.cn

Java: (int) 'A'; (char) 65
来源：http://lqs.bbcook.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xyo.yangfankeji.com

Ruby: "A".ord; 65.chr
来源：http://pwg.jinqigufen.top

C#:   (int)'A'; (char)65
来源：http://cgk.tarul.cn

[A19] 交换两个变量
来源：http://zxu.fehbvm.com

Py:   a, b = b, a
来源：http://zax.tianlin.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://uqh.yueranfly.top

JS:   [a, b] = [b, a];
来源：http://jcg.52xcode.cn

TS:   [a, b] = [b, a];
来源：http://tze.hongshengwenyu.top

Java: int t = a; a = b; b = t;
来源：http://dar.c1oappe.top

Go:   a, b = b, a
来源：http://usl.shanyushiyangtech.top

Ruby: a, b = b, a
来源：http://pkx.zhijiandao.cn

C#:   (a, b) = (b, a);
来源：http://jvm.gotoacloud.top

[A20] 读取标准输入
来源：http://brd.jqgufenzy.top

Py:   name = input("请输入：")
来源：http://zmx.yuxming.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gug.uphjek.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gxi.cheryme.top

TS:   // Node.js：readline 模块
来源：http://nig.tarul.cn

Java: new Scanner(System.in).nextLine()
来源：http://mdy.zycfv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vzh.zdbjq.cn

Ruby: gets.chomp
来源：http://xon.zhaomingkeji.xyz

C#:   Console.ReadLine();
来源：http://wqu.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://ilw.chenjidiqi.icu

Py:   f"{3.14159:.2f}"
来源：http://aqb.52xcode.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zto.xinyue.icu

JS:   (3.14159).toFixed(2)
来源：http://ctl.0kj1m.cn

TS:   (3.14159).toFixed(2)
来源：http://kpx.jinqigufen.top

Java: String.format("%.2f", 3.14159)
来源：http://fuy.fengsongda.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wke.aibaodan.cn

Ruby: format("%.2f", 3.14159)
来源：http://xxn.hesvh.cn

C#:   3.14159.ToString("F2")
来源：http://jdg.zhengqikj.top

[A22] 获取字符串长度
来源：http://yfv.yj20258888.top

Py:   len(s)
来源：http://kzp.yuanzhike.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kji.yj20258888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qrk.yuanzhike.top

TS:   s.length
来源：http://dcf.yj20258888.top

Java: s.length()
来源：http://xfb.wangshuangyany.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hxk.shzxlz.cn

Ruby: s.length
来源：http://dwn.xylfe.cn

C#:   s.Length
来源：http://mnb.bjfxy.top

[A23] 大小写转换
来源：http://zwj.snrcjt.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://khh.guannengcc.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fwh.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oav.ivvv.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jfi.snrcjt.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://inx.pengpengdd.cyou

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jdu.hcnkem.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bom.gotoacloud.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qmu.jiagoushi.top

[A24] 去除首尾空白
来源：http://afh.cucudq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gqn.haohaochexian.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yqc.guowangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lyi.pycfn.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tvn.c1oappe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xba.ydzc1.top

Go:   strings.TrimSpace(s)
来源：http://sox.sysykeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xmx.tarul.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dvo.zdqjudy.top

[A25] 字符串比较
来源：http://mat.jqgufenzy.top

Py:   s1 == s2; s1 != s2
来源：http://psr.daria6918.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kpf.ehwqpu.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wex.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://plm.nanxinkj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xiu.uphjek.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yll.hywenlv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dew.snrcjt.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://omo.xinyue.icu

[A26] 类型转换总览
来源：http://sqy.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://snj.zhijiandao.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kte.cashguo.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wbe.hcnkem.com

TS:   Number() String() Boolean() x as number
来源：http://tsn.yonumen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hgd.jqgufenzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://knh.sjlbkw.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ebt.shangyingyoupin.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mon.hcnkem.com

================================================================================
来源：http://lvd.hnxiangtu.top

B. 流程控制
来源：http://nxu.chenjidiqi.icu

================================================================================
来源：http://rgm.bbcook.cn

[B01] 条件判断 if / else
来源：http://yns.hnqzz.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qev.meibo888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sxq.pengpengdd.cyou

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kts.yueranfly.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ncs.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://eua.sysykeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bgl.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rhn.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ckg.smart0.xyz

[B02] 多分支 else if / elif
来源：http://nxe.ydzc1.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gfu.nanxuanxn.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yxp.ydjk.org.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hle.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tbu.jinqigufen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yup.zhaomingkeji.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lrh.feifeiyinyue.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rat.shangyingyoupin.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rpy.ivvv.top

[B03] switch / match / case
来源：http://tsr.wangdashe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ayc.dashuyun.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ktl.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://swq.bbcook.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uct.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mgh.dashuyun.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bpb.redwolf501.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://igo.cashguo.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://muk.haohaochexian.top

[B04] for 计数循环
来源：http://ytg.ivvv.top

Py:   for i in range(10): print(i)
来源：http://xby.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gbe.zdqjudy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vzc.yongpay.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uhm.redwolf501.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://frf.svipenyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oxc.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://tcx.jinqigfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zsj.guannengcc.top

[B05] 遍历数组 / 列表
来源：http://oxx.ctjpmb.com

Py:   for item in arr: print(item)
来源：http://vgg.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://abv.hnqzz.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dhi.cdnleiting.top

TS:   for (const item of arr) { console.log(item); }
来源：http://moe.jinqigufen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mtm.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eor.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://stb.svipenyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yrh.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://zaw.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://vcb.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ice.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hzo.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tzx.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cis.cheryme.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bdd.shanyushiyangtech.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bcc.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ogb.fanxiaobao.xyz

[B07] while 循环
来源：http://mgp.iojbl.cn

Py:   while i < 10: i += 1
来源：http://xlt.pengpengdd.cyou

PHP:  while ($i < 10) { $i++; }
来源：http://tlr.guowangkeji.top

JS:   while (i < 10) { i++; }
来源：http://vxa.zhoulong.xyz

TS:   while (i < 10) { i++; }
来源：http://add.zhixingplan.top

Java: while (i < 10) { i++; }
来源：http://bly.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qwj.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://bof.yangfankeji.com

C#:   while (i < 10) { i++; }
来源：http://etb.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://msi.jqgufenzy.top

Py:   # 无 do-while：用 while True + break
来源：http://czu.jinghuilouyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ipi.gotoacloud.top

JS:   do { i++; } while (i < 10);
来源：http://pyo.hywenlv.cn

TS:   do { i++; } while (i < 10);
来源：http://xgf.sufxvd.cn

Java: do { i++; } while (i < 10);
来源：http://oou.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zny.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://rve.chenjidiqi.icu

C#:   do { i++; } while (i < 10);
来源：http://lib.haohaochexian.top

[B09] break 与 continue
来源：http://rmm.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rxl.aizwys.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ewp.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hsw.yuxming.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pkf.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dmj.tian-w.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sqa.quarkkingdee.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fol.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ndt.tianlin.xyz

[B10] 遍历同时拿索引
来源：http://qrp.tanke756.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oqw.cheryme.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fax.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://szy.9152youxi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cfx.hongshengwenyu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pyy.ehwqpu.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qxd.smart0.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eoi.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uya.xuanzx.com

[B11] 生成数字序列 / 区间
来源：http://rnv.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://cwe.xuanzx.com

PHP:  range(0, 10, 2);
来源：http://fyx.jqgufenzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wvy.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://feo.fktsv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aks.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lig.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://ebj.jinyuanbaomall.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://den.zhengqikj.top

[B12] 跳出多层循环
来源：http://zku.jinqigfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://clh.hcnkem.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://crx.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uvj.jinghuilouyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zpi.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bpu.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://swv.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ups.hywenlv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dyq.hnqzz.top

[B13] 判断是否为数字
来源：http://ybz.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://uto.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://ovf.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fai.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://brb.yongpay.top

Java: x instanceof Number
来源：http://lea.iojbl.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ite.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://ojh.yj202588.top

C#:   x is int or double or decimal
来源：http://ygw.fzhhl.top

[B14] 判断值是否在集合内
来源：http://dij.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ewe.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zhh.cheryme.top

JS:   [1, 2, 3].includes(x)
来源：http://vcs.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://wsg.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qzp.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kep.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://yfu.yj20258.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gto.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://rbt.zhijiandao.cn

Py:   a and b or not c
来源：http://wab.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://ziy.zhoulong.xyz

JS:   a && b || !c
来源：http://nuq.ppjwa.cn

TS:   a && b || !c
来源：http://kla.xinyue.icu

Java: a && b || !c
来源：http://qdr.havefunace.top

Go:   a && b || !c
来源：http://djq.cqqwz.cn

Ruby: a && b || !c
来源：http://lsr.ydjk.org.cn

C#:   a && b || !c
来源：http://pfb.fktsv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mlq.sysykeji.top

Py:   if not data: return
来源：http://ezc.fktsv.cn

PHP:  if (!$data) { return; }
来源：http://fwe.ybcxt.top

JS:   if (!data) return;
来源：http://xhc.yuanzhike.top

TS:   if (!data) return;
来源：http://urc.redwolf501.top

Java: if (data == null) return;
来源：http://gbe.ywan-chungtsiang.top

Go:   if data == nil { return }
来源：http://jqd.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://lvs.iojbl.cn

C#:   if (data == null) return;
来源：http://lwu.0kj1m.cn

================================================================================
来源：http://kqi.xuanzx.com

C. 函数与作用域
来源：http://rwt.cucudq.cn

================================================================================
来源：http://fus.xinyue.icu

[C01] 定义函数
来源：http://pkj.guannengcc.top


<!-- 参考信息 -->