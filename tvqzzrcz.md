代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://fik.dashuyun.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ncn.zdqjudy.top

Java: x > 0 ? "yes" : "no"
来源：http://esx.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jca.0kj1m.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://irl.cucudq.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bzk.gogol.net.cn

[A12] 字符串插值 / 格式化
来源：http://zcv.pengpengdd.cyou

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yzu.chenjidiqi.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xfg.vehdjk.com

JS:   `Hello, ${name}!`
来源：http://bjg.sysykeji.top

TS:   `Hello, ${name}!`
来源：http://rkg.ctjpmb.com

Java: "Hello, %s!".formatted(name)
来源：http://fvd.yonumen.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hls.zdqjudy.top

Ruby: "Hello, #{name}!"
来源：http://bsr.aibaodan.cn

C#:   $"Hello, {name}!"
来源：http://tjw.zhiwuduotai.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rtp.tanke756.top

Py:   "第一行\n第二行"
来源：http://mwy.pengpengdd.cyou

PHP:  "第一行\n第二行"
来源：http://uaj.wangshuangyany.cn

JS:   "第一行\n第二行"
来源：http://ybf.jyoumei.cn

TS:   "第一行\n第二行"
来源：http://mfy.hywenlv.cn

Java: "第一行\n第二行"
来源：http://rwf.ywan-chungtsiang.top

Go:   "第一行\n第二行"
来源：http://yxx.xylfe.cn

Ruby: "第一行\n第二行"
来源：http://usc.sweek.top

C#:   "第一行\n第二行"
来源：http://ewz.yj20258888.top

[A14] 注释写法
来源：http://yop.yj20258.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://vnc.daria6918.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wjy.pengpengdd.cyou

JS:   // 单行；/* 多行 */
来源：http://zcs.sxryk.cn

TS:   // 单行；/* 多行 */
来源：http://vky.cucudq.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pui.smart0.xyz

Go:   // 单行；/* 多行 */
来源：http://oat.316326.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://gxw.guowangkeji.top

C#:   // 单行；/* 多行 */
来源：http://bnu.tanke756.top

[A15] 空值判断与默认值
来源：http://zfo.fehbvm.com

Py:   value = data or "默认值"
来源：http://xqi.yangfankeji.com

PHP:  $value = $data ?? "默认值";
来源：http://bpw.c1oappe.top

JS:   const value = data ?? "默认值";
来源：http://xma.gaohongyu789.top

TS:   const value = data ?? "默认值";
来源：http://pas.yfazqb.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://peh.zdqjudy.top

Go:   if data == "" { data = "默认值" }
来源：http://cfv.xuetiantiany.cn

Ruby: value = data || "默认值"
来源：http://usl.tarul.cn

C#:   var value = data ?? "默认值";
来源：http://gss.guowangkeji.top

[A16] 真假值判断规则
来源：http://jsq.gzhubu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yep.yonumen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vyb.tanke756.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oov.haohaochexian.top

TS:   if (!x) {}
来源：http://bim.nanxuanxn.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zvm.9152youxi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cqb.snrcjt.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sxh.bjfxy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qqc.jinqigfzy.top

[A17] 位运算
来源：http://wqu.shangyingyoupin.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qvx.sufxvd.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ywn.gotoacloud.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eek.316326.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xlj.meibo888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uzy.kuanghao11.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bub.tanke756.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ytd.hammf.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sce.tarul.cn

[A18] 字符与 ASCII 码互转
来源：http://ngx.redwolf501.top

Py:   ord("A"); chr(65)
来源：http://obx.fzhhl.top

PHP:  ord("A"); chr(65)
来源：http://nhj.jinyuanbaomall.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://svm.cqqwz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lkt.xinyue.icu

Java: (int) 'A'; (char) 65
来源：http://yat.nanxuanxn.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wbz.sxryk.cn

Ruby: "A".ord; 65.chr
来源：http://cln.jinqigfzy.top

C#:   (int)'A'; (char)65
来源：http://oai.jinyuanbaomall.cn

[A19] 交换两个变量
来源：http://bnc.xylfe.cn

Py:   a, b = b, a
来源：http://oby.xylfe.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cch.hfpthk.cn

JS:   [a, b] = [b, a];
来源：http://mby.nanxinkj.top

TS:   [a, b] = [b, a];
来源：http://xzu.vqdsnc.cn

Java: int t = a; a = b; b = t;
来源：http://mio.gotoacloud.top

Go:   a, b = b, a
来源：http://qle.snrcjt.cn

Ruby: a, b = b, a
来源：http://npm.yuanzhike.top

C#:   (a, b) = (b, a);
来源：http://tau.jqgufenzy.top

[A20] 读取标准输入
来源：http://aon.cdnleiting.top

Py:   name = input("请输入：")
来源：http://aal.jlsjyb.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hrw.meibo888.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://say.jyoumei.cn

TS:   // Node.js：readline 模块
来源：http://qlh.gaohongyu789.top

Java: new Scanner(System.in).nextLine()
来源：http://qiv.haohaochexian.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ymq.nanxuanxn.top

Ruby: gets.chomp
来源：http://jnv.jlsjyb.cn

C#:   Console.ReadLine();
来源：http://nln.vqdsnc.cn

[A21] 保留指定小数位输出
来源：http://zcm.yanxiufei.cn

Py:   f"{3.14159:.2f}"
来源：http://nor.ehwqpu.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hsj.pengpengdd.cyou

JS:   (3.14159).toFixed(2)
来源：http://tjc.ehwqpu.com

TS:   (3.14159).toFixed(2)
来源：http://wda.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://ugv.hfpthk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uzr.ehwqpu.com

Ruby: format("%.2f", 3.14159)
来源：http://jsp.aizwys.cn

C#:   3.14159.ToString("F2")
来源：http://qkv.guowangkeji.top

[A22] 获取字符串长度
来源：http://wlp.jinqigfzy.top

Py:   len(s)
来源：http://xuc.yj20258888.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://obp.feifeiyinyue.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://grf.daxiang520.top

TS:   s.length
来源：http://siz.zhaomingkeji.xyz

Java: s.length()
来源：http://cyc.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mej.zhaomingkeji.xyz

Ruby: s.length
来源：http://jwq.xingfuxueyuan.xyz

C#:   s.Length
来源：http://yhk.shzxlz.cn

[A23] 大小写转换
来源：http://zgh.cdnleiting.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kqq.wangshuangyany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tnu.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ejz.mhx1999.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hpg.yj202588.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xrx.xingfuxueyuan.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ksw.bjfxy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://twd.nanxuanxn.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lsq.ehwqpu.com

[A24] 去除首尾空白
来源：http://pjg.cucudq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dww.yfazqb.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fwo.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zdx.sjlbkw.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iki.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gct.hesvh.cn

Go:   strings.TrimSpace(s)
来源：http://hie.cqqwz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oap.daxiang520.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cec.nanxinkj.top

[A25] 字符串比较
来源：http://eqf.yangfankeji.com

Py:   s1 == s2; s1 != s2
来源：http://mvp.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zoh.fktsv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xqv.jiagoushi.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hby.jiagoushi.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://inv.fzhhl.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gfh.cdnleiting.top

Ruby: s1 == s2; s1 <=> s2
来源：http://uwr.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vjx.sxryk.cn

[A26] 类型转换总览
来源：http://kjb.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ikz.c1oappe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wwc.hnqzz.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zyh.guannengcc.top

TS:   Number() String() Boolean() x as number
来源：http://ush.shuidangran.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cph.shuidangran.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vbd.hammf.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://idq.zhengqikj.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ouv.wangshuangyany.cn

================================================================================
来源：http://ytv.xylfe.cn

B. 流程控制
来源：http://bwg.yongpay.top

================================================================================
来源：http://aoj.0kj1m.cn

[B01] 条件判断 if / else
来源：http://hay.jinqigfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zxc.hywenlv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yyx.jinqigufen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://crb.jlsjyb.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sap.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://kcd.ybcxt.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ypa.tian-w.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gtj.haohaochexian.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wby.cdnleiting.top

[B02] 多分支 else if / elif
来源：http://msj.nanxuanxn.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vze.hfpthk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sfe.yueranfly.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://otr.sysykeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eoj.fehbvm.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ymr.hcnkem.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ayf.yvedp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://djp.jqgfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ude.zhongyouzk.top

[B03] switch / match / case
来源：http://nqf.bbcook.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jsi.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wvz.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://arz.xingfuxueyuan.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zjw.jinyuanbaomall.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ftz.gotoacloud.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eqe.havefunace.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mth.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dbr.hnqzz.top

[B04] for 计数循环
来源：http://oys.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://lft.shangyingyoupin.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jvw.jqgufenzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sme.cqqwz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://crl.9152youxi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bxt.yfazqb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hwv.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://qtn.yangfankeji.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zpw.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://wau.pycfn.com

Py:   for item in arr: print(item)
来源：http://tkd.chenjidiqi.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uix.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jis.zhiwuduotai.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xom.chenjidiqi.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://tqk.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tbb.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://fnc.yj20258.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tkd.zdqjudy.top

[B06] 遍历字典 / 对象
来源：http://hhk.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nrz.shuidangran.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zdq.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aga.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gqy.uphjek.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zvo.xingfuxueyuan.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://slj.hammf.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uhl.xingfuxueyuan.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nfv.jinghuilouyu.cn

[B07] while 循环
来源：http://xbt.redwolf501.top

Py:   while i < 10: i += 1
来源：http://pit.daxiang520.top

PHP:  while ($i < 10) { $i++; }
来源：http://ysu.ydzc1.top

JS:   while (i < 10) { i++; }
来源：http://cxo.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://wgn.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://dap.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://muz.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://nbd.0kj1m.cn

C#:   while (i < 10) { i++; }
来源：http://yrn.yongpay.top

[B08] do-while（至少执行一次）
来源：http://lhk.ctjpmb.com

Py:   # 无 do-while：用 while True + break
来源：http://dfm.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mdf.shzxlz.cn

JS:   do { i++; } while (i < 10);
来源：http://lkl.tian-w.cn

TS:   do { i++; } while (i < 10);
来源：http://uqf.hammf.cn

Java: do { i++; } while (i < 10);
来源：http://zur.hysaishi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ahj.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://kzl.jinqigfzy.top

C#:   do { i++; } while (i < 10);
来源：http://olw.hnqzz.top

[B09] break 与 continue
来源：http://rro.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pfu.nanxinkj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kvw.hammf.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cko.xuanzx.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xuz.ydzc1.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfe.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lse.zhongyouzk.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cnu.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://heq.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://abm.shuidangran.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nbz.snrcjt.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sgg.vehdjk.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xrw.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uup.sxryk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ccg.zdbjq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yit.ppjwa.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tzy.jiagoushi.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rdf.xylfe.cn

[B11] 生成数字序列 / 区间
来源：http://eyr.xylfe.cn

Py:   list(range(0, 10, 2))
来源：http://qnv.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://kki.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xjg.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tut.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oef.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uze.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://pdw.meibo888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rto.hywenlv.cn

[B12] 跳出多层循环
来源：http://tyw.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ory.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://obu.nanxuanxn.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vdn.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://znq.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://haa.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mwz.meibo888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ffd.pycfn.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uko.ppjwa.cn

[B13] 判断是否为数字
来源：http://tud.bjfxy.top

Py:   isinstance(x, (int, float))
来源：http://wow.hongshengwenyu.top

PHP:  is_numeric($x)
来源：http://fln.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ebz.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tng.pycfn.com

Java: x instanceof Number
来源：http://nyc.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cog.yanxiufei.cn

Ruby: x.is_a?(Numeric)
来源：http://vug.svipenyu.cn

C#:   x is int or double or decimal
来源：http://lvx.ivvv.top

[B14] 判断值是否在集合内
来源：http://mjd.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fil.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://exz.nanxuanxn.top

JS:   [1, 2, 3].includes(x)
来源：http://tnk.hnqzz.top

TS:   [1, 2, 3].includes(x)
来源：http://jah.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://owx.cqqwz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xfp.cucudq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xtr.ywan-chungtsiang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ggn.hammf.cn

[B15] 布尔运算与取反
来源：http://jwg.zycfv.cn

Py:   a and b or not c
来源：http://hdz.cashguo.top

PHP:  $a && $b || !$c
来源：http://eyn.sysykeji.top

JS:   a && b || !c
来源：http://sri.smart0.xyz

TS:   a && b || !c
来源：http://rsz.zhijiandao.cn

Java: a && b || !c
来源：http://vzv.yonumen.top

Go:   a && b || !c
来源：http://alt.uphjek.com

Ruby: a && b || !c
来源：http://etp.tianlin.xyz

C#:   a && b || !c
来源：http://lnx.snrcjt.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bnn.cheryme.top

Py:   if not data: return
来源：http://xbj.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://ygv.ctjpmb.com

JS:   if (!data) return;
来源：http://iez.ywan-chungtsiang.top

TS:   if (!data) return;
来源：http://men.chenjidiqi.icu

Java: if (data == null) return;
来源：http://vku.316326.xyz

Go:   if data == nil { return }
来源：http://jjg.birdmap.top

Ruby: return if data.nil?
来源：http://yne.daxiang520.top

C#:   if (data == null) return;
来源：http://gxg.316326.xyz

================================================================================
来源：http://jqz.fehbvm.com

C. 函数与作用域
来源：http://pao.zhiwuduotai.top

================================================================================
来源：http://ann.shuidangran.top

[C01] 定义函数
来源：http://vfm.feifeiyinyue.top

Py:   def add(a, b): return a + b
来源：http://rfb.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wkb.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://dum.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hwc.sufxvd.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hnf.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://zkx.ydjk.org.cn

Ruby: def add(a, b); a + b; end
来源：http://yqr.jinqigfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pnv.cashguo.top


<!-- 参考信息 -->