代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://iwh.cdnleiting.top

C#:   x > 0 ? "yes" : "no"
来源：http://rdu.shzxlz.cn

[A12] 字符串插值 / 格式化
来源：http://luq.zdqjudy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hqa.haohaochexian.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vah.zdqjudy.top

JS:   `Hello, ${name}!`
来源：http://ymy.ydjk.org.cn

TS:   `Hello, ${name}!`
来源：http://tbf.zycfv.cn

Java: "Hello, %s!".formatted(name)
来源：http://ihk.zycfv.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://swd.shanyushiyangtech.top

Ruby: "Hello, #{name}!"
来源：http://wja.vqdsnc.cn

C#:   $"Hello, {name}!"
来源：http://ujn.bbcook.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vnr.ivvv.top

Py:   "第一行\n第二行"
来源：http://kdp.yj20258888.top

PHP:  "第一行\n第二行"
来源：http://uab.pycfn.com

JS:   "第一行\n第二行"
来源：http://hlf.jinqigufen.top

TS:   "第一行\n第二行"
来源：http://wgh.dianchejie.cn

Java: "第一行\n第二行"
来源：http://eva.jqgufenzy.top

Go:   "第一行\n第二行"
来源：http://yhp.fehbvm.com

Ruby: "第一行\n第二行"
来源：http://emo.xingfuxueyuan.xyz

C#:   "第一行\n第二行"
来源：http://dam.mhx1999.top

[A14] 注释写法
来源：http://xnk.nanxuanxn.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zud.yuxming.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bme.shuidangran.top

JS:   // 单行；/* 多行 */
来源：http://rtk.chenzaomai.com

TS:   // 单行；/* 多行 */
来源：http://yzj.jiagoushi.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tbf.haohaochexian.top

Go:   // 单行；/* 多行 */
来源：http://mpp.yongpay.top

Ruby: # 单行；=begin 多行 =end
来源：http://ipf.aizwys.cn

C#:   // 单行；/* 多行 */
来源：http://jdb.aizwys.cn

[A15] 空值判断与默认值
来源：http://rea.hesvh.cn

Py:   value = data or "默认值"
来源：http://eiu.ehwqpu.com

PHP:  $value = $data ?? "默认值";
来源：http://jre.316326.xyz

JS:   const value = data ?? "默认值";
来源：http://zrq.chenlongwang.top

TS:   const value = data ?? "默认值";
来源：http://tqm.zhongyouzk.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gvm.andypj.xyz

Go:   if data == "" { data = "默认值" }
来源：http://ivx.jqgufenzy.top

Ruby: value = data || "默认值"
来源：http://svp.yj20258.top

C#:   var value = data ?? "默认值";
来源：http://klt.cashguo.top

[A16] 真假值判断规则
来源：http://kxe.sxryk.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tlw.yj20258.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://quw.vqdsnc.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ogb.guowangkeji.top

TS:   if (!x) {}
来源：http://mqb.zhengqikj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dqe.yuxming.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://knl.daria6918.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zdr.jianghu66.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yhm.hnqzz.top

[A17] 位运算
来源：http://ozb.snrcjt.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lle.jqgufenzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rwv.yongpay.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yyl.fktsv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xne.tianlin.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zzs.0kj1m.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ern.tanke756.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kfr.yuanzhike.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ssy.yangfankeji.com

[A18] 字符与 ASCII 码互转
来源：http://fgu.birdmap.top

Py:   ord("A"); chr(65)
来源：http://owt.iojbl.cn

PHP:  ord("A"); chr(65)
来源：http://syu.xuanzx.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rqs.dianchejie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aqa.yonumen.top

Java: (int) 'A'; (char) 65
来源：http://wuq.yuxming.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sdf.fzhhl.top

Ruby: "A".ord; 65.chr
来源：http://tng.yfazqb.com

C#:   (int)'A'; (char)65
来源：http://vun.quarkkingdee.top

[A19] 交换两个变量
来源：http://obv.wangshuangyany.cn

Py:   a, b = b, a
来源：http://qnx.chenzaomai.com

PHP:  [$a, $b] = [$b, $a];
来源：http://exm.52xcode.cn

JS:   [a, b] = [b, a];
来源：http://dtn.0kj1m.cn

TS:   [a, b] = [b, a];
来源：http://gzz.sysykeji.top

Java: int t = a; a = b; b = t;
来源：http://wwv.nanxinkj.top

Go:   a, b = b, a
来源：http://xfk.gaohongyu789.top

Ruby: a, b = b, a
来源：http://pqn.shanyushiyangkeji.top

C#:   (a, b) = (b, a);
来源：http://atc.ppjwa.cn

[A20] 读取标准输入
来源：http://hwm.hysaishi.cn

Py:   name = input("请输入：")
来源：http://utm.yj20258.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kmp.jinyuanbaomall.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zgq.hysaishi.cn

TS:   // Node.js：readline 模块
来源：http://drv.xinyue.icu

Java: new Scanner(System.in).nextLine()
来源：http://vtb.yj20258.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fkg.sxryk.cn

Ruby: gets.chomp
来源：http://ryd.yj202588.top

C#:   Console.ReadLine();
来源：http://jqe.shzxlz.cn

[A21] 保留指定小数位输出
来源：http://aod.svipenyu.cn

Py:   f"{3.14159:.2f}"
来源：http://ehk.shangyingyoupin.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://flg.zhixingplan.top

JS:   (3.14159).toFixed(2)
来源：http://shd.redwolf501.top

TS:   (3.14159).toFixed(2)
来源：http://xvj.zhijiandao.cn

Java: String.format("%.2f", 3.14159)
来源：http://xjb.guowangkeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gzg.jinghuilouyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://obt.shzxlz.cn

C#:   3.14159.ToString("F2")
来源：http://htd.zhongyouzk.top

[A22] 获取字符串长度
来源：http://ksb.jyoumei.cn

Py:   len(s)
来源：http://pji.guannengcc.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vmm.jinyuanbaomall.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xyw.jqgfzy.top

TS:   s.length
来源：http://euc.xinyue.icu

Java: s.length()
来源：http://nqr.ctjpmb.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vfm.pengpengdd.cyou

Ruby: s.length
来源：http://wfj.ydzc1.top

C#:   s.Length
来源：http://qto.pycfn.com

[A23] 大小写转换
来源：http://epm.hnxiangtu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ygb.zycfv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ekk.ehwqpu.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eor.pycfn.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://whi.wangshuangyany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ocj.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qnc.wangshuangyany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ilg.fktsv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zrj.kuanghao11.cn

[A24] 去除首尾空白
来源：http://lse.hywenlv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://stj.guannengcc.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gak.zhijiandao.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wfq.xuetiantiany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oqs.zhoulong.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wkb.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://zay.pycfn.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xmi.ppjwa.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ktb.gotoacloud.top

[A25] 字符串比较
来源：http://xvg.yvedp.cn

Py:   s1 == s2; s1 != s2
来源：http://rst.aizwys.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wgc.52xcode.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rgh.xinyue.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://phb.smart0.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iac.zhiwuduotai.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yic.ivvv.top

Ruby: s1 == s2; s1 <=> s2
来源：http://aqw.316326.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ezh.xuetiantiany.cn

[A26] 类型转换总览
来源：http://qgy.52xcode.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tqs.jiagoushi.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://euf.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ylg.zhiwuduotai.top

TS:   Number() String() Boolean() x as number
来源：http://qio.sysykeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fip.hammf.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://num.chenlongwang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lmh.ehwqpu.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xee.quarkkingdee.top

================================================================================
来源：http://lnu.yangfankeji.com

B. 流程控制
来源：http://znp.xuanzx.com

================================================================================
来源：http://iut.316326.xyz

[B01] 条件判断 if / else
来源：http://idz.sjlbkw.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nok.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rpf.316326.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fvr.fehbvm.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qax.316326.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://lmh.shanyushiyangtech.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://spv.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sdy.zhijiandao.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fqc.jinqigfzy.top

[B02] 多分支 else if / elif
来源：http://jgm.jiagoushi.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yuz.epnwcf.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hte.cdnleiting.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vvv.daxiang520.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aya.ydjk.org.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uij.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xeh.gogol.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mmi.chenjidiqi.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://raf.svipenyu.cn

[B03] switch / match / case
来源：http://hdw.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mhx.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rfv.zhijiandao.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fel.hfpthk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dno.hongshengwenyu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rlm.pycfn.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hph.9152youxi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hwt.havefunace.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uct.jianghu66.top

[B04] for 计数循环
来源：http://ldv.meibo888.top

Py:   for i in range(10): print(i)
来源：http://dsz.cheryme.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vrl.guowangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://her.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://akn.fanxiaobao.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ccw.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hyy.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://qjb.gaohongyu789.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xks.sweek.top

[B05] 遍历数组 / 列表
来源：http://wld.epnwcf.com

Py:   for item in arr: print(item)
来源：http://omo.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lru.ydjk.org.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://udr.aizwys.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ldy.tianlin.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://yqr.smart0.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://niz.hnxiangtu.top

Ruby: arr.each { |item| puts item }
来源：http://avu.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jxs.aibaodan.cn

[B06] 遍历字典 / 对象
来源：http://quo.xuetiantiany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gpe.tianlin.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cdw.shanyushiyangtech.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jti.daxiang520.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gpb.tian-w.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zcq.tanke756.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gsf.wangshuangyany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qkg.zhoulong.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xbh.iojbl.cn

[B07] while 循环
来源：http://zfp.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://swi.52xcode.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gcq.sufxvd.cn

JS:   while (i < 10) { i++; }
来源：http://gnj.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://quy.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://omi.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kqd.vqdsnc.cn

Ruby: while i < 10; i += 1; end
来源：http://ynk.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://oci.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://iam.dianchejie.cn

Py:   # 无 do-while：用 while True + break
来源：http://reo.shanyushiyangtech.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nci.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://ope.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://qxb.jqgfzy.top

Java: do { i++; } while (i < 10);
来源：http://yku.yuxming.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wmq.hfpthk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mfj.cashguo.top

C#:   do { i++; } while (i < 10);
来源：http://uoz.yj20258888.top

[B09] break 与 continue
来源：http://qyf.tianlin.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ehe.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uha.shzxlz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ywb.jqgufenzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://itc.cqqwz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mfm.shzxlz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ppg.tianlin.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nkj.ctjpmb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://orq.yj20258888.top

[B10] 遍历同时拿索引
来源：http://cud.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hwk.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mab.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qyd.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bxo.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xuc.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fyb.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sez.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://toj.sufxvd.cn

[B11] 生成数字序列 / 区间
来源：http://ulu.cashguo.top

Py:   list(range(0, 10, 2))
来源：http://agu.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://ihd.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dmg.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hnf.shuidangran.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wun.pycfn.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kyg.shuidangran.top

Ruby: (0...10).step(2).to_a
来源：http://tdo.zhiwuduotai.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wez.andypj.xyz

[B12] 跳出多层循环
来源：http://syp.ywan-chungtsiang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rrp.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sng.zhaomingkeji.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iqo.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dyz.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ecm.ctjpmb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fja.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lrh.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wsu.yongpay.top

[B13] 判断是否为数字
来源：http://coh.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://ssk.jinyuanbaomall.cn

PHP:  is_numeric($x)
来源：http://jni.zhaomingkeji.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jhv.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vze.mhx1999.top

Java: x instanceof Number
来源：http://tvc.jqgufenzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qot.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://nrw.pycfn.com

C#:   x is int or double or decimal
来源：http://gqj.xylfe.cn

[B14] 判断值是否在集合内
来源：http://jwi.xingfuxueyuan.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rub.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kkc.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://kac.zhijiandao.cn

TS:   [1, 2, 3].includes(x)
来源：http://xbu.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://kmx.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ymi.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xgu.ybcxt.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nse.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://tlk.cashguo.top

Py:   a and b or not c
来源：http://eoo.52xcode.cn

PHP:  $a && $b || !$c
来源：http://dai.nwbrower.top

JS:   a && b || !c
来源：http://mkr.jiagoushi.top

TS:   a && b || !c
来源：http://hqa.quarkkingdee.top

Java: a && b || !c
来源：http://xvy.shangyingyoupin.top

Go:   a && b || !c
来源：http://jkk.chenzaomai.com

Ruby: a && b || !c
来源：http://whd.zhaomingkeji.xyz

C#:   a && b || !c
来源：http://lsv.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://kkr.dashuyun.cn

Py:   if not data: return
来源：http://ldc.yangfankeji.com

PHP:  if (!$data) { return; }
来源：http://qaq.gzhubu.top

JS:   if (!data) return;
来源：http://miv.yongpay.top

TS:   if (!data) return;
来源：http://geu.meibo888.top

Java: if (data == null) return;
来源：http://lak.kuanghao11.cn

Go:   if data == nil { return }
来源：http://muv.bjfxy.top

Ruby: return if data.nil?
来源：http://bbf.zhijiandao.cn

C#:   if (data == null) return;
来源：http://eld.tarul.cn

================================================================================
来源：http://qua.quarkkingdee.top

C. 函数与作用域
来源：http://jsm.zhongyouzk.top

================================================================================
来源：http://kes.pengpengdd.cyou

[C01] 定义函数
来源：http://eru.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://gdd.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qcz.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://ejt.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nbk.snrcjt.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vtg.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://vyj.hongshengwenyu.top

Ruby: def add(a, b); a + b; end
来源：http://tuo.pycfn.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://azr.cheryme.top

[C02] 默认参数
来源：http://huf.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://usc.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://ind.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://wqg.dianchejie.cn


<!-- 参考信息 -->