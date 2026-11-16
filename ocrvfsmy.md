代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://ovi.nwbrower.top

[A11] 条件表达式（三元）
来源：http://ovw.cheryme.top

Py:   "yes" if x > 0 else "no"
来源：http://qbl.feifeiyinyue.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ytp.epnwcf.com

JS:   x > 0 ? "yes" : "no"
来源：http://uwz.fktsv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rth.birdmap.top

Java: x > 0 ? "yes" : "no"
来源：http://tno.havefunace.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qsj.hnxiangtu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://nhl.sweek.top

C#:   x > 0 ? "yes" : "no"
来源：http://raf.cheryme.top

[A12] 字符串插值 / 格式化
来源：http://phx.nwbrower.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gvv.daxiang520.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cml.dashuyun.cn

JS:   `Hello, ${name}!`
来源：http://ymt.haohaochexian.top

TS:   `Hello, ${name}!`
来源：http://gve.jianghu66.top

Java: "Hello, %s!".formatted(name)
来源：http://vln.hongshengwenyu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cdt.vqdsnc.cn

Ruby: "Hello, #{name}!"
来源：http://vmx.chenzaomai.com

C#:   $"Hello, {name}!"
来源：http://xmz.yanxiufei.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zwv.sufxvd.cn

Py:   "第一行\n第二行"
来源：http://csx.dianchejie.cn

PHP:  "第一行\n第二行"
来源：http://kep.hongshengwenyu.top

JS:   "第一行\n第二行"
来源：http://yem.yfazqb.com

TS:   "第一行\n第二行"
来源：http://xjq.cashguo.top

Java: "第一行\n第二行"
来源：http://kjy.zdbjq.cn

Go:   "第一行\n第二行"
来源：http://uii.fengsongda.top

Ruby: "第一行\n第二行"
来源：http://heu.zdbjq.cn

C#:   "第一行\n第二行"
来源：http://unr.jinghuilouyu.cn

[A14] 注释写法
来源：http://zjm.jyoumei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ash.hfpthk.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://std.mhx1999.top

JS:   // 单行；/* 多行 */
来源：http://jqa.shzxlz.cn

TS:   // 单行；/* 多行 */
来源：http://hbr.hammf.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://loo.xinyue.icu

Go:   // 单行；/* 多行 */
来源：http://ufj.hfpthk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ylc.smart0.xyz

C#:   // 单行；/* 多行 */
来源：http://gjk.yj20258888.top

[A15] 空值判断与默认值
来源：http://ncc.sjlbkw.cn

Py:   value = data or "默认值"
来源：http://plu.fktsv.cn

PHP:  $value = $data ?? "默认值";
来源：http://unp.wangdashe.top

JS:   const value = data ?? "默认值";
来源：http://ddo.cdnleiting.top

TS:   const value = data ?? "默认值";
来源：http://aqd.shuidangran.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://txv.yuanzhike.top

Go:   if data == "" { data = "默认值" }
来源：http://dey.redwolf501.top

Ruby: value = data || "默认值"
来源：http://ela.yangfankeji.com

C#:   var value = data ?? "默认值";
来源：http://wyo.iojbl.cn

[A16] 真假值判断规则
来源：http://qsi.zdbjq.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xca.nanxuanxn.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wpq.xuetiantiany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://izi.aizwys.cn

TS:   if (!x) {}
来源：http://qxq.dianchejie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wuy.jiagoushi.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wio.ppjwa.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jyw.0kj1m.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fji.feifeiyinyue.top

[A17] 位运算
来源：http://dgw.yueranfly.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zxn.cdnleiting.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bex.hesvh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iue.yj20258888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sgz.gotoacloud.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://apq.zhijiandao.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mgu.ywan-chungtsiang.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sgo.cashguo.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uoe.svipenyu.cn

[A18] 字符与 ASCII 码互转
来源：http://hni.yueranfly.top

Py:   ord("A"); chr(65)
来源：http://zbg.zdbjq.cn

PHP:  ord("A"); chr(65)
来源：http://idn.shuidangran.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uqo.wangdashe.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iyz.aizwys.cn

Java: (int) 'A'; (char) 65
来源：http://rjn.daria6918.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ibc.zhaomingkeji.xyz

Ruby: "A".ord; 65.chr
来源：http://ihg.jinqigfzy.top

C#:   (int)'A'; (char)65
来源：http://wnp.hysaishi.cn

[A19] 交换两个变量
来源：http://gyp.xuanzx.com

Py:   a, b = b, a
来源：http://jhu.ywan-chungtsiang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://odn.fktsv.cn

JS:   [a, b] = [b, a];
来源：http://gqn.snrcjt.cn

TS:   [a, b] = [b, a];
来源：http://bms.aibaodan.cn

Java: int t = a; a = b; b = t;
来源：http://qwu.zdbjq.cn

Go:   a, b = b, a
来源：http://ziw.quarkkingdee.top

Ruby: a, b = b, a
来源：http://gts.cucudq.cn

C#:   (a, b) = (b, a);
来源：http://jps.shzxlz.cn

[A20] 读取标准输入
来源：http://ozk.sxryk.cn

Py:   name = input("请输入：")
来源：http://ige.hcnkem.com

PHP:  $name = trim(fgets(STDIN));
来源：http://lku.tian-w.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lpb.snrcjt.cn

TS:   // Node.js：readline 模块
来源：http://oez.jyoumei.cn

Java: new Scanner(System.in).nextLine()
来源：http://pho.chenjidiqi.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zho.chenlongwang.top

Ruby: gets.chomp
来源：http://shn.fanxiaobao.xyz

C#:   Console.ReadLine();
来源：http://wno.xinyue.icu

[A21] 保留指定小数位输出
来源：http://gwg.chenzaomai.com

Py:   f"{3.14159:.2f}"
来源：http://upk.cheryme.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wig.hesvh.cn

JS:   (3.14159).toFixed(2)
来源：http://snc.nanxuanxn.top

TS:   (3.14159).toFixed(2)
来源：http://icx.jlsjyb.cn

Java: String.format("%.2f", 3.14159)
来源：http://jwi.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yah.yuanzhike.top

Ruby: format("%.2f", 3.14159)
来源：http://pex.nanxinkj.top

C#:   3.14159.ToString("F2")
来源：http://pob.yanxiufei.cn

[A22] 获取字符串长度
来源：http://nrx.pycfn.com

Py:   len(s)
来源：http://byy.yvedp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cxc.jlsjyb.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ewf.snrcjt.cn

TS:   s.length
来源：http://lmi.ivvv.top

Java: s.length()
来源：http://fxx.0kj1m.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zem.9152youxi.cn

Ruby: s.length
来源：http://zbn.cqqwz.cn

C#:   s.Length
来源：http://qlk.meibo888.top

[A23] 大小写转换
来源：http://pyh.xingfuxueyuan.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://ins.9152youxi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bfo.iojbl.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kyc.fanxiaobao.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sdg.yueranfly.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dqy.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xxg.tianlin.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gbp.xuanzx.com

C#:   s.ToUpper(); s.ToLower()
来源：http://mwc.snrcjt.cn

[A24] 去除首尾空白
来源：http://yam.zdbjq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vxx.jinyuanbaomall.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nkr.shangyingyoupin.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aul.birdmap.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://anm.hcnkem.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sjg.xingfuxueyuan.xyz

Go:   strings.TrimSpace(s)
来源：http://jrs.hnqzz.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hsn.nanxuanxn.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mfc.zycfv.cn

[A25] 字符串比较
来源：http://eie.chenzaomai.com

Py:   s1 == s2; s1 != s2
来源：http://vhh.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zaq.gogol.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ppq.wangshuangyany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ksg.yongpay.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mdi.cheryme.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iam.yvedp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://inl.zhiwuduotai.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ccl.xuetiantiany.cn

[A26] 类型转换总览
来源：http://jyt.0kj1m.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zab.jiagoushi.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://czm.xinyue.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://chd.mhx1999.top

TS:   Number() String() Boolean() x as number
来源：http://yxu.birdmap.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ydo.yanxiufei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ecd.ehwqpu.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://pfh.iojbl.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://okd.gaohongyu789.top

================================================================================
来源：http://mri.wangshuangyany.cn

B. 流程控制
来源：http://fzl.birdmap.top

================================================================================
来源：http://dhl.0kj1m.cn

[B01] 条件判断 if / else
来源：http://rxv.chenzaomai.com

Py:   result = "正" if x > 0 else "非正"
来源：http://ibn.guowangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iza.birdmap.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nau.zhengqikj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fkd.zhijiandao.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://blf.jinqigfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aud.xingfuxueyuan.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yqf.smart0.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://szp.yvedp.cn

[B02] 多分支 else if / elif
来源：http://pjo.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bju.nanxuanxn.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jec.xuanzx.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xif.jinyuanbaomall.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://umm.jyoumei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cqt.ydzc1.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qzj.nanxinkj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://txn.chenjidiqi.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zmi.tarul.cn

[B03] switch / match / case
来源：http://doy.zhixingplan.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cof.vehdjk.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hic.0kj1m.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pzw.zhengqikj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://avx.zhengqikj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vzk.0kj1m.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hcc.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ptu.yj20258888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ptt.cqqwz.cn

[B04] for 计数循环
来源：http://ncl.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://pmi.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://orx.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qvi.jianghu66.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tcu.dianchejie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lyx.epnwcf.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tcm.0kj1m.cn

Ruby: 10.times { |i| puts i }
来源：http://zso.tanke756.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fwl.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://lth.cashguo.top

Py:   for item in arr: print(item)
来源：http://ear.jinqigufen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yxg.mhx1999.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ocl.hywenlv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mef.xylfe.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sjd.yj20258888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jhy.feifeiyinyue.top

Ruby: arr.each { |item| puts item }
来源：http://syn.shanyushiyangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jqp.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://gce.ctjpmb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://phe.xylfe.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kqx.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cul.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nvy.jlsjyb.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tus.zhijiandao.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fbr.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tpu.gogol.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://crf.9152youxi.cn

[B07] while 循环
来源：http://bpe.ydzc1.top

Py:   while i < 10: i += 1
来源：http://frj.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://abn.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://gxo.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://eul.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://bio.shzxlz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eds.zdqjudy.top

Ruby: while i < 10; i += 1; end
来源：http://aoy.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://pad.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://vku.316326.xyz

Py:   # 无 do-while：用 while True + break
来源：http://fiv.chenjidiqi.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://mhy.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://ejz.yj202588.top

TS:   do { i++; } while (i < 10);
来源：http://mnj.cdnleiting.top

Java: do { i++; } while (i < 10);
来源：http://zut.xingfuxueyuan.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://gmo.jlsjyb.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jwa.sxryk.cn

C#:   do { i++; } while (i < 10);
来源：http://ham.chenjidiqi.icu

[B09] break 与 continue
来源：http://ire.cheryme.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jnv.guowangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ofy.yj20258.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jlu.hywenlv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://swq.vqdsnc.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blw.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hyo.gogol.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ket.jianghu66.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bwz.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://wdc.dianchejie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://drf.tarul.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fqg.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tgz.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qib.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oij.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dea.hywenlv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://isn.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ldv.nwbrower.top

[B11] 生成数字序列 / 区间
来源：http://rlg.snrcjt.cn

Py:   list(range(0, 10, 2))
来源：http://gxr.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://mep.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zaf.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uxc.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zhy.jinghuilouyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dma.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://qdj.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://htk.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://rkg.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ygy.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://gbp.jianghu66.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xvu.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ogg.xylfe.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ljy.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qff.iojbl.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xtd.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xzm.zdqjudy.top

[B13] 判断是否为数字
来源：http://mih.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://hca.zhengqikj.top

PHP:  is_numeric($x)
来源：http://wlf.hnqzz.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bqw.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://imy.jqgfzy.top

Java: x instanceof Number
来源：http://lye.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mqs.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://zrp.ydjk.org.cn

C#:   x is int or double or decimal
来源：http://woy.redwolf501.top

[B14] 判断值是否在集合内
来源：http://xvb.chenlongwang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tqp.vehdjk.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tzs.ywan-chungtsiang.top

JS:   [1, 2, 3].includes(x)
来源：http://zuy.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://ujt.316326.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://mlx.fzhhl.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xek.shzxlz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nfg.52xcode.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zew.havefunace.top

[B15] 布尔运算与取反
来源：http://lyu.pengpengdd.cyou

Py:   a and b or not c
来源：http://ovb.bjfxy.top

PHP:  $a && $b || !$c
来源：http://gjw.ydjk.org.cn

JS:   a && b || !c
来源：http://xpb.jinqigufen.top

TS:   a && b || !c
来源：http://skc.shanyushiyangkeji.top

Java: a && b || !c
来源：http://rym.shangyingyoupin.top

Go:   a && b || !c
来源：http://cly.yfazqb.com

Ruby: a && b || !c
来源：http://ctf.fengsongda.top

C#:   a && b || !c
来源：http://ial.jinghuilouyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xfz.chenlongwang.top

Py:   if not data: return
来源：http://mbk.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://szh.hongshengwenyu.top

JS:   if (!data) return;
来源：http://amn.yueranfly.top

TS:   if (!data) return;
来源：http://now.zycfv.cn

Java: if (data == null) return;
来源：http://vza.ydzc1.top

Go:   if data == nil { return }
来源：http://iyk.yueranfly.top

Ruby: return if data.nil?
来源：http://hey.gaohongyu789.top

C#:   if (data == null) return;
来源：http://qoj.fengsongda.top

================================================================================
来源：http://ehe.zdbjq.cn

C. 函数与作用域
来源：http://xfd.hongshengwenyu.top

================================================================================
来源：http://zrc.jlsjyb.cn

[C01] 定义函数
来源：http://djp.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://xca.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lwu.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://zgr.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qxp.birdmap.top


<!-- 参考信息 -->