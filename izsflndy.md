代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://glq.svipenyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ttu.sysykeji.top

[A12] 字符串插值 / 格式化
来源：http://ftp.nanxinkj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://urm.zhongyouzk.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tki.svipenyu.cn

JS:   `Hello, ${name}!`
来源：http://fdk.iojbl.cn

TS:   `Hello, ${name}!`
来源：http://gja.redwolf501.top

Java: "Hello, %s!".formatted(name)
来源：http://ntm.jinghuilouyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dmb.jinghuilouyu.cn

Ruby: "Hello, #{name}!"
来源：http://muh.birdmap.top

C#:   $"Hello, {name}!"
来源：http://gts.316326.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://qen.jiagoushi.top

Py:   "第一行\n第二行"
来源：http://eai.svipenyu.cn

PHP:  "第一行\n第二行"
来源：http://snv.quarkkingdee.top

JS:   "第一行\n第二行"
来源：http://qog.9152youxi.cn

TS:   "第一行\n第二行"
来源：http://deu.hnqzz.top

Java: "第一行\n第二行"
来源：http://gwx.gaohongyu789.top

Go:   "第一行\n第二行"
来源：http://gak.gogol.net.cn

Ruby: "第一行\n第二行"
来源：http://hmp.yj202588.top

C#:   "第一行\n第二行"
来源：http://hdm.ctjpmb.com

[A14] 注释写法
来源：http://olb.yueranfly.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mbn.sysykeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vmc.tian-w.cn

JS:   // 单行；/* 多行 */
来源：http://jeu.yj20258888.top

TS:   // 单行；/* 多行 */
来源：http://hju.xinyue.icu

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wwc.fengsongda.top

Go:   // 单行；/* 多行 */
来源：http://imv.pycfn.com

Ruby: # 单行；=begin 多行 =end
来源：http://ndn.jyoumei.cn

C#:   // 单行；/* 多行 */
来源：http://cja.jinqigufen.top

[A15] 空值判断与默认值
来源：http://waf.uphjek.com

Py:   value = data or "默认值"
来源：http://xyk.yuanzhike.top

PHP:  $value = $data ?? "默认值";
来源：http://azh.tarul.cn

JS:   const value = data ?? "默认值";
来源：http://wmy.zhaomingkeji.xyz

TS:   const value = data ?? "默认值";
来源：http://utb.guowangkeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zcl.hywenlv.cn

Go:   if data == "" { data = "默认值" }
来源：http://hfw.shuidangran.top

Ruby: value = data || "默认值"
来源：http://eam.zhoulong.xyz

C#:   var value = data ?? "默认值";
来源：http://ikv.jiagoushi.top

[A16] 真假值判断规则
来源：http://cjn.fanxiaobao.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wva.yj202588.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://scm.dianchejie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fqr.cqqwz.cn

TS:   if (!x) {}
来源：http://ynv.meibo888.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tln.jinqigfzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oul.nwbrower.top

Ruby: unless x            # nil 与 false 为假
来源：http://ziw.xinyue.icu

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://iyu.fktsv.cn

[A17] 位运算
来源：http://dpc.wangshuangyany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sfo.redwolf501.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dzc.svipenyu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kro.ppjwa.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lyy.redwolf501.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wfn.sxryk.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wbq.hongshengwenyu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://thb.zdqjudy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cce.pycfn.com

[A18] 字符与 ASCII 码互转
来源：http://igb.jinqigfzy.top

Py:   ord("A"); chr(65)
来源：http://xql.hysaishi.cn

PHP:  ord("A"); chr(65)
来源：http://wag.zhijiandao.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://emy.xuanzx.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://llh.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://qrj.shanyushiyangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://brn.zhongyouzk.top

Ruby: "A".ord; 65.chr
来源：http://nkg.tianlin.xyz

C#:   (int)'A'; (char)65
来源：http://qed.feifeiyinyue.top

[A19] 交换两个变量
来源：http://sxv.jqgufenzy.top

Py:   a, b = b, a
来源：http://and.nwbrower.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pnc.dashuyun.cn

JS:   [a, b] = [b, a];
来源：http://wse.9152youxi.cn

TS:   [a, b] = [b, a];
来源：http://ymc.fehbvm.com

Java: int t = a; a = b; b = t;
来源：http://lnw.hnqzz.top

Go:   a, b = b, a
来源：http://tgo.cqqwz.cn

Ruby: a, b = b, a
来源：http://dpv.svipenyu.cn

C#:   (a, b) = (b, a);
来源：http://sjp.yangfankeji.com

[A20] 读取标准输入
来源：http://htd.cashguo.top

Py:   name = input("请输入：")
来源：http://ttn.dianchejie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://grd.wangdashe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qay.jianghu66.top

TS:   // Node.js：readline 模块
来源：http://hsc.ppjwa.cn

Java: new Scanner(System.in).nextLine()
来源：http://qeq.zhengqikj.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vmq.wangdashe.top

Ruby: gets.chomp
来源：http://ixw.pengpengdd.cyou

C#:   Console.ReadLine();
来源：http://uxt.jinqigufen.top

[A21] 保留指定小数位输出
来源：http://pnx.tian-w.cn

Py:   f"{3.14159:.2f}"
来源：http://dew.vehdjk.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hvw.c1oappe.top

JS:   (3.14159).toFixed(2)
来源：http://grx.cqqwz.cn

TS:   (3.14159).toFixed(2)
来源：http://vve.cashguo.top

Java: String.format("%.2f", 3.14159)
来源：http://xvz.shanyushiyangtech.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ott.feifeiyinyue.top

Ruby: format("%.2f", 3.14159)
来源：http://anu.yueranfly.top

C#:   3.14159.ToString("F2")
来源：http://qvn.shanyushiyangtech.top

[A22] 获取字符串长度
来源：http://ltv.fengsongda.top

Py:   len(s)
来源：http://tuf.0kj1m.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cdw.epnwcf.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nbz.jinghuilouyu.cn

TS:   s.length
来源：http://vyf.fzhhl.top

Java: s.length()
来源：http://vxv.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kxt.cqqwz.cn

Ruby: s.length
来源：http://ubj.bbcook.cn

C#:   s.Length
来源：http://ifb.ctjpmb.com

[A23] 大小写转换
来源：http://kwd.birdmap.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vqz.andypj.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yhj.uphjek.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://umb.vehdjk.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oul.snrcjt.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hzm.tarul.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qts.yongpay.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wzh.jinqigfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://obq.aibaodan.cn

[A24] 去除首尾空白
来源：http://yhn.hcnkem.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://doo.tianlin.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gia.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://frl.sweek.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jbm.jinqigufen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cfz.wangdashe.top

Go:   strings.TrimSpace(s)
来源：http://gkw.jlsjyb.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tao.smart0.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nbi.yonumen.top

[A25] 字符串比较
来源：http://sty.mhx1999.top

Py:   s1 == s2; s1 != s2
来源：http://pzb.hywenlv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hni.kuanghao11.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tan.dianchejie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://opn.sysykeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ljn.guannengcc.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xbn.zhijiandao.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gva.hysaishi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nbb.chenlongwang.top

[A26] 类型转换总览
来源：http://taa.fanxiaobao.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bch.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ush.ivvv.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://avf.vehdjk.com

TS:   Number() String() Boolean() x as number
来源：http://nso.hnxiangtu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vho.uphjek.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lhj.ivvv.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xvo.ppjwa.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oco.hcnkem.com

================================================================================
来源：http://zhn.fanxiaobao.xyz

B. 流程控制
来源：http://bac.shzxlz.cn

================================================================================
来源：http://ehm.daria6918.cn

[B01] 条件判断 if / else
来源：http://fqr.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xoe.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pli.yonumen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hei.yuxming.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kxb.dashuyun.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bxt.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://crl.yonumen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ogp.fzhhl.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kom.fktsv.cn

[B02] 多分支 else if / elif
来源：http://kpt.yueranfly.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vai.dianchejie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sph.jinqigfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rwp.yonumen.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ctg.nwbrower.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://umw.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dng.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rap.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kyc.jianghu66.top

[B03] switch / match / case
来源：http://gbt.feifeiyinyue.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dsj.0kj1m.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mzl.xuanzx.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ows.9152youxi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zwa.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wfk.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ysm.ehwqpu.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mvb.yj202588.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qet.svipenyu.cn

[B04] for 计数循环
来源：http://trf.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://tbs.daria6918.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mdm.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gkf.zhijiandao.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zlq.ywan-chungtsiang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bai.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gjt.cdnleiting.top

Ruby: 10.times { |i| puts i }
来源：http://zsu.zhaomingkeji.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pmf.hammf.cn

[B05] 遍历数组 / 列表
来源：http://zgx.ehwqpu.com

Py:   for item in arr: print(item)
来源：http://lsn.andypj.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lcy.ctjpmb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://ghd.fanxiaobao.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://rda.vehdjk.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://asw.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eck.snrcjt.cn

Ruby: arr.each { |item| puts item }
来源：http://ken.jlsjyb.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oza.havefunace.top

[B06] 遍历字典 / 对象
来源：http://voy.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ufi.gaohongyu789.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dlq.yuanzhike.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zns.nanxinkj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bqk.ehwqpu.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mmh.sjlbkw.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yqf.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://byx.hnqzz.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://edl.bbcook.cn

[B07] while 循环
来源：http://jve.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://boa.ydjk.org.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lru.guannengcc.top

JS:   while (i < 10) { i++; }
来源：http://oxq.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://csh.hesvh.cn

Java: while (i < 10) { i++; }
来源：http://erh.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yrk.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://unm.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://nsz.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://ogp.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://zjh.9152youxi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ajm.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://sxn.yj20258888.top

TS:   do { i++; } while (i < 10);
来源：http://sqf.zhiwuduotai.top

Java: do { i++; } while (i < 10);
来源：http://aop.jyoumei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vms.uphjek.com

Ruby: begin; i += 1; end while i < 10
来源：http://nnt.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://skx.chenlongwang.top

[B09] break 与 continue
来源：http://ufg.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cek.gotoacloud.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ygn.jlsjyb.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://crs.pengpengdd.cyou

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://whb.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wns.52xcode.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rjl.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yzp.andypj.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://viv.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://hla.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lak.hnxiangtu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jpf.c1oappe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bbc.hnqzz.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lvn.haohaochexian.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ulk.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://peq.sysykeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kul.yj20258888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nho.gzhubu.top

[B11] 生成数字序列 / 区间
来源：http://tni.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://zbx.yuxming.cn

PHP:  range(0, 10, 2);
来源：http://eav.sjlbkw.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aso.haohaochexian.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fzk.jinqigfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gvc.zhiwuduotai.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qcf.svipenyu.cn

Ruby: (0...10).step(2).to_a
来源：http://ibu.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zrw.smart0.xyz

[B12] 跳出多层循环
来源：http://dmd.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jkk.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://znb.ybcxt.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tbe.hongshengwenyu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mvb.jinyuanbaomall.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ouh.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sjq.zdqjudy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ouo.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://urc.sxryk.cn

[B13] 判断是否为数字
来源：http://ktm.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://jdp.tarul.cn

PHP:  is_numeric($x)
来源：http://yaf.c1oappe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hdw.guannengcc.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nbl.aibaodan.cn

Java: x instanceof Number
来源：http://cjc.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tmu.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://tna.zhoulong.xyz

C#:   x is int or double or decimal
来源：http://fvj.fengsongda.top

[B14] 判断值是否在集合内
来源：http://ljm.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zds.guannengcc.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wvo.ybcxt.top

JS:   [1, 2, 3].includes(x)
来源：http://zkh.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://mxn.zdbjq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wqy.kuanghao11.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dta.fzhhl.top

Ruby: [1, 2, 3].include?(x)
来源：http://uzc.wangshuangyany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xze.tanke756.top

[B15] 布尔运算与取反
来源：http://cpo.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://sgo.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://amg.jianghu66.top

JS:   a && b || !c
来源：http://rya.daxiang520.top

TS:   a && b || !c
来源：http://ltm.hesvh.cn

Java: a && b || !c
来源：http://hfm.xuanzx.com

Go:   a && b || !c
来源：http://elj.zhijiandao.cn

Ruby: a && b || !c
来源：http://xik.dashuyun.cn

C#:   a && b || !c
来源：http://utp.xylfe.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cxp.fengsongda.top

Py:   if not data: return
来源：http://qnk.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://vbu.tarul.cn

JS:   if (!data) return;
来源：http://wjb.mhx1999.top

TS:   if (!data) return;
来源：http://qzz.daxiang520.top

Java: if (data == null) return;
来源：http://ukk.smart0.xyz

Go:   if data == nil { return }
来源：http://bdg.ydzc1.top

Ruby: return if data.nil?
来源：http://znv.jqgufenzy.top

C#:   if (data == null) return;
来源：http://hbj.jiagoushi.top

================================================================================
来源：http://qxw.hnqzz.top

C. 函数与作用域
来源：http://uqd.chenjidiqi.icu

================================================================================
来源：http://xlk.hysaishi.cn

[C01] 定义函数
来源：http://osn.316326.xyz

Py:   def add(a, b): return a + b
来源：http://qyc.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wln.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://lxi.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qdz.sjlbkw.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gwe.0kj1m.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wfu.chenlongwang.top

Ruby: def add(a, b); a + b; end
来源：http://lry.ybcxt.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oul.ywan-chungtsiang.top

[C02] 默认参数
来源：http://iyw.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://cdw.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xkp.yj20258888.top

JS:   function greet(name = "World") { return name; }
来源：http://agf.316326.xyz


<!-- 参考信息 -->