代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://fyh.jyoumei.cn

[A11] 条件表达式（三元）
来源：http://vdy.quarkkingdee.top

Py:   "yes" if x > 0 else "no"
来源：http://jnv.jiagoushi.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://vvn.ydjk.org.cn

JS:   x > 0 ? "yes" : "no"
来源：http://eru.hesvh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jbr.ppjwa.cn

Java: x > 0 ? "yes" : "no"
来源：http://suh.jyoumei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yej.guowangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://iir.zdqjudy.top

C#:   x > 0 ? "yes" : "no"
来源：http://uua.zhengqikj.top

[A12] 字符串插值 / 格式化
来源：http://dtl.ydzc1.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bnm.redwolf501.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wmg.dianchejie.cn

JS:   `Hello, ${name}!`
来源：http://snr.cdnleiting.top

TS:   `Hello, ${name}!`
来源：http://ney.xuetiantiany.cn

Java: "Hello, %s!".formatted(name)
来源：http://dbf.ppjwa.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ois.xylfe.cn

Ruby: "Hello, #{name}!"
来源：http://jwc.jiagoushi.top

C#:   $"Hello, {name}!"
来源：http://lrr.xuetiantiany.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pco.aibaodan.cn

Py:   "第一行\n第二行"
来源：http://nim.quarkkingdee.top

PHP:  "第一行\n第二行"
来源：http://jxm.shzxlz.cn

JS:   "第一行\n第二行"
来源：http://srs.shanyushiyangkeji.top

TS:   "第一行\n第二行"
来源：http://hoh.9152youxi.cn

Java: "第一行\n第二行"
来源：http://hdj.guannengcc.top

Go:   "第一行\n第二行"
来源：http://iam.vehdjk.com

Ruby: "第一行\n第二行"
来源：http://tug.cheryme.top

C#:   "第一行\n第二行"
来源：http://vok.yj20258.top

[A14] 注释写法
来源：http://fxh.zdbjq.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://afd.snrcjt.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rln.ywan-chungtsiang.top

JS:   // 单行；/* 多行 */
来源：http://puf.daxiang520.top

TS:   // 单行；/* 多行 */
来源：http://tpe.chenzaomai.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yts.epnwcf.com

Go:   // 单行；/* 多行 */
来源：http://css.cdnleiting.top

Ruby: # 单行；=begin 多行 =end
来源：http://mva.c1oappe.top

C#:   // 单行；/* 多行 */
来源：http://aqx.gogol.net.cn

[A15] 空值判断与默认值
来源：http://nfr.fengsongda.top

Py:   value = data or "默认值"
来源：http://fpp.vqdsnc.cn

PHP:  $value = $data ?? "默认值";
来源：http://tiv.tianlin.xyz

JS:   const value = data ?? "默认值";
来源：http://zqk.kuanghao11.cn

TS:   const value = data ?? "默认值";
来源：http://gzu.aizwys.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bry.zycfv.cn

Go:   if data == "" { data = "默认值" }
来源：http://neo.jyoumei.cn

Ruby: value = data || "默认值"
来源：http://vgq.52xcode.cn

C#:   var value = data ?? "默认值";
来源：http://ulv.jyoumei.cn

[A16] 真假值判断规则
来源：http://xih.nwbrower.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mfk.shanyushiyangtech.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jcg.zhaomingkeji.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fuk.tarul.cn

TS:   if (!x) {}
来源：http://zqi.zhiwuduotai.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uyg.tarul.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zqx.yuxming.cn

Ruby: unless x            # nil 与 false 为假
来源：http://upl.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yxk.jinqigufen.top

[A17] 位运算
来源：http://xpn.xuetiantiany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bzq.kuanghao11.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://las.jinqigufen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rru.cdnleiting.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://apg.zdbjq.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kvp.pycfn.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://owq.52xcode.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ife.zhiwuduotai.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://brr.ivvv.top

[A18] 字符与 ASCII 码互转
来源：http://ryh.birdmap.top

Py:   ord("A"); chr(65)
来源：http://amd.feifeiyinyue.top

PHP:  ord("A"); chr(65)
来源：http://div.xylfe.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hyd.tianlin.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://owq.sufxvd.cn

Java: (int) 'A'; (char) 65
来源：http://usl.ybcxt.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ijj.ehwqpu.com

Ruby: "A".ord; 65.chr
来源：http://xdd.aizwys.cn

C#:   (int)'A'; (char)65
来源：http://xwr.hnxiangtu.top

[A19] 交换两个变量
来源：http://bve.haohaochexian.top

Py:   a, b = b, a
来源：http://wry.hnxiangtu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jeh.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://yio.xuanzx.com

TS:   [a, b] = [b, a];
来源：http://juf.shangyingyoupin.top

Java: int t = a; a = b; b = t;
来源：http://pug.hesvh.cn

Go:   a, b = b, a
来源：http://mcm.yuanzhike.top

Ruby: a, b = b, a
来源：http://llh.sjlbkw.cn

C#:   (a, b) = (b, a);
来源：http://jgf.cashguo.top

[A20] 读取标准输入
来源：http://nxy.cheryme.top

Py:   name = input("请输入：")
来源：http://dkd.nanxuanxn.top

PHP:  $name = trim(fgets(STDIN));
来源：http://axy.jinyuanbaomall.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zbt.havefunace.top

TS:   // Node.js：readline 模块
来源：http://twf.quarkkingdee.top

Java: new Scanner(System.in).nextLine()
来源：http://wwj.daria6918.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zsg.yangfankeji.com

Ruby: gets.chomp
来源：http://owz.zhoulong.xyz

C#:   Console.ReadLine();
来源：http://hdl.yueranfly.top

[A21] 保留指定小数位输出
来源：http://wvo.vqdsnc.cn

Py:   f"{3.14159:.2f}"
来源：http://bhv.ydjk.org.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://whg.chenzaomai.com

JS:   (3.14159).toFixed(2)
来源：http://zxr.jqgfzy.top

TS:   (3.14159).toFixed(2)
来源：http://hdv.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://rth.zhixingplan.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qtx.sufxvd.cn

Ruby: format("%.2f", 3.14159)
来源：http://pfs.jinyuanbaomall.cn

C#:   3.14159.ToString("F2")
来源：http://xte.redwolf501.top

[A22] 获取字符串长度
来源：http://gnp.hammf.cn

Py:   len(s)
来源：http://phm.cucudq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ash.tarul.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mek.nanxinkj.top

TS:   s.length
来源：http://tgc.meibo888.top

Java: s.length()
来源：http://hcb.redwolf501.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gsb.jyoumei.cn

Ruby: s.length
来源：http://ovp.hammf.cn

C#:   s.Length
来源：http://gda.jiagoushi.top

[A23] 大小写转换
来源：http://vbp.yanxiufei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fra.yj20258888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xjf.xziqi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cav.jqgfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tjw.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qym.birdmap.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cak.yonumen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nbu.tarul.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dnn.ctjpmb.com

[A24] 去除首尾空白
来源：http://nol.tian-w.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dzu.jqgfzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ynf.yj20258.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://evk.sweek.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rgt.zhiwuduotai.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bhh.xziqi.cn

Go:   strings.TrimSpace(s)
来源：http://kvb.fzhhl.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kqg.fengsongda.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lbx.zhoulong.xyz

[A25] 字符串比较
来源：http://wep.jinqigufen.top

Py:   s1 == s2; s1 != s2
来源：http://gzs.epnwcf.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wjk.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xcu.tanke756.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://urg.tarul.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://euq.zycfv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iqm.andypj.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://veg.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jdq.wangshuangyany.cn

[A26] 类型转换总览
来源：http://qcc.smart0.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xac.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hmu.quarkkingdee.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nzx.dashuyun.cn

TS:   Number() String() Boolean() x as number
来源：http://jqk.hywenlv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sqo.jyoumei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://piv.havefunace.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jjy.daria6918.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hjz.fzhhl.top

================================================================================
来源：http://xcw.fehbvm.com

B. 流程控制
来源：http://xfy.zhixingplan.top

================================================================================
来源：http://mhc.yfazqb.com

[B01] 条件判断 if / else
来源：http://zib.xuanzx.com

Py:   result = "正" if x > 0 else "非正"
来源：http://nkv.daria6918.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lca.sweek.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fev.nanxuanxn.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dvi.fanxiaobao.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://mol.yonumen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yhw.tanke756.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xsh.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://esc.tanke756.top

[B02] 多分支 else if / elif
来源：http://zsb.ehwqpu.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xnp.yfazqb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cfa.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qvx.pycfn.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vtg.zhoulong.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ovb.yongpay.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bxe.sxryk.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bvj.nanxuanxn.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://urt.yueranfly.top

[B03] switch / match / case
来源：http://uuv.shzxlz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://txo.hywenlv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wxz.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ipb.shanyushiyangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jyw.aizwys.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jml.vehdjk.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bvs.ydjk.org.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sqj.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://csr.sufxvd.cn

[B04] for 计数循环
来源：http://hyt.hammf.cn

Py:   for i in range(10): print(i)
来源：http://dnq.xuetiantiany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ryp.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nfd.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tly.hcnkem.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bwj.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bds.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://whf.zdqjudy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tov.jinyuanbaomall.cn

[B05] 遍历数组 / 列表
来源：http://lmd.ehwqpu.com

Py:   for item in arr: print(item)
来源：http://bas.jiagoushi.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hsi.jinqigfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xeb.bjfxy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://awu.vehdjk.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://rzn.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wzh.bbcook.cn

Ruby: arr.each { |item| puts item }
来源：http://gbx.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ixx.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://igs.xylfe.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iif.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hie.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kxe.nanxuanxn.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xhy.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xgt.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fui.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hvu.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uur.nwbrower.top

[B07] while 循环
来源：http://cds.cdnleiting.top

Py:   while i < 10: i += 1
来源：http://dae.9152youxi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rrn.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://rxh.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://ari.hfpthk.cn

Java: while (i < 10) { i++; }
来源：http://bxu.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hei.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://nae.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://rll.yvedp.cn

[B08] do-while（至少执行一次）
来源：http://hkb.c1oappe.top

Py:   # 无 do-while：用 while True + break
来源：http://qir.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mgz.gogol.net.cn

JS:   do { i++; } while (i < 10);
来源：http://quw.hnqzz.top

TS:   do { i++; } while (i < 10);
来源：http://mia.tarul.cn

Java: do { i++; } while (i < 10);
来源：http://fhh.tarul.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://aks.fengsongda.top

Ruby: begin; i += 1; end while i < 10
来源：http://pox.guannengcc.top

C#:   do { i++; } while (i < 10);
来源：http://uiq.ctjpmb.com

[B09] break 与 continue
来源：http://lyy.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rgg.sufxvd.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jjd.hesvh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kju.cdnleiting.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uht.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aob.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://thy.hfpthk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://paw.cashguo.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://icp.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://qik.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wpx.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gkw.hnqzz.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vdt.zhongyouzk.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hev.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vpz.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lit.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rxv.snrcjt.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cbw.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://xib.yongpay.top

Py:   list(range(0, 10, 2))
来源：http://kxt.bbcook.cn

PHP:  range(0, 10, 2);
来源：http://nwc.jqgfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://udl.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ggd.jinghuilouyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rke.meibo888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mxt.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://mwj.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zok.quarkkingdee.top

[B12] 跳出多层循环
来源：http://dms.xinyue.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://kwu.zhengqikj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://glm.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pkw.shuidangran.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tds.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fnf.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ked.chenjidiqi.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yuv.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bda.bjfxy.top

[B13] 判断是否为数字
来源：http://zyz.dianchejie.cn

Py:   isinstance(x, (int, float))
来源：http://lca.shzxlz.cn

PHP:  is_numeric($x)
来源：http://tnf.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://neh.52xcode.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ipt.9152youxi.cn

Java: x instanceof Number
来源：http://lkv.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ofe.yanxiufei.cn

Ruby: x.is_a?(Numeric)
来源：http://uql.jlsjyb.cn

C#:   x is int or double or decimal
来源：http://ybe.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://ujw.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rqy.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ewu.ctjpmb.com

JS:   [1, 2, 3].includes(x)
来源：http://pee.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://dzs.aibaodan.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ejq.dashuyun.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rbw.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://xkd.gzhubu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dap.ctjpmb.com

[B15] 布尔运算与取反
来源：http://zdr.wangdashe.top

Py:   a and b or not c
来源：http://otv.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://fjb.jinghuilouyu.cn

JS:   a && b || !c
来源：http://bkr.dashuyun.cn

TS:   a && b || !c
来源：http://hpy.jianghu66.top

Java: a && b || !c
来源：http://mkr.zhijiandao.cn

Go:   a && b || !c
来源：http://ehq.zhongyouzk.top

Ruby: a && b || !c
来源：http://opa.yueranfly.top

C#:   a && b || !c
来源：http://wuc.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://ork.nwbrower.top

Py:   if not data: return
来源：http://dfw.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://apg.gzhubu.top

JS:   if (!data) return;
来源：http://nab.nwbrower.top

TS:   if (!data) return;
来源：http://uow.sysykeji.top

Java: if (data == null) return;
来源：http://pki.hysaishi.cn

Go:   if data == nil { return }
来源：http://ehg.yanxiufei.cn

Ruby: return if data.nil?
来源：http://gvp.ybcxt.top

C#:   if (data == null) return;
来源：http://and.haohaochexian.top

================================================================================
来源：http://nbf.birdmap.top

C. 函数与作用域
来源：http://prx.havefunace.top

================================================================================
来源：http://kkg.xziqi.cn

[C01] 定义函数
来源：http://stl.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://eph.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://odq.ybcxt.top

JS:   function add(a, b) { return a + b; }
来源：http://ujl.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://noo.jinyuanbaomall.cn


<!-- 参考信息 -->