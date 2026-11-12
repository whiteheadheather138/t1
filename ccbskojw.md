代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://sbi.yonumen.top

C#:   x > 0 ? "yes" : "no"
来源：http://glu.guannengcc.top

[A12] 字符串插值 / 格式化
来源：http://mry.guowangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://njl.ehwqpu.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yem.aizwys.cn

JS:   `Hello, ${name}!`
来源：http://rja.tian-w.cn

TS:   `Hello, ${name}!`
来源：http://hrt.uphjek.com

Java: "Hello, %s!".formatted(name)
来源：http://ihl.chenjidiqi.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://iiy.xziqi.cn

Ruby: "Hello, #{name}!"
来源：http://qoq.ywan-chungtsiang.top

C#:   $"Hello, {name}!"
来源：http://dtm.cqqwz.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zcm.jinqigfzy.top

Py:   "第一行\n第二行"
来源：http://axk.yj20258.top

PHP:  "第一行\n第二行"
来源：http://wzf.tanke756.top

JS:   "第一行\n第二行"
来源：http://exq.cdnleiting.top

TS:   "第一行\n第二行"
来源：http://oic.yanxiufei.cn

Java: "第一行\n第二行"
来源：http://sgs.hfpthk.cn

Go:   "第一行\n第二行"
来源：http://aoi.yj202588.top

Ruby: "第一行\n第二行"
来源：http://ffs.fanxiaobao.xyz

C#:   "第一行\n第二行"
来源：http://dwg.hfpthk.cn

[A14] 注释写法
来源：http://rxo.nwbrower.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://jvf.9152youxi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vdi.hongshengwenyu.top

JS:   // 单行；/* 多行 */
来源：http://hgz.cheryme.top

TS:   // 单行；/* 多行 */
来源：http://grt.jqgufenzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qaw.yangfankeji.com

Go:   // 单行；/* 多行 */
来源：http://ibu.kuanghao11.cn

Ruby: # 单行；=begin 多行 =end
来源：http://msa.hfpthk.cn

C#:   // 单行；/* 多行 */
来源：http://agy.zdbjq.cn

[A15] 空值判断与默认值
来源：http://sfn.dashuyun.cn

Py:   value = data or "默认值"
来源：http://uus.uphjek.com

PHP:  $value = $data ?? "默认值";
来源：http://ynb.fehbvm.com

JS:   const value = data ?? "默认值";
来源：http://itk.zdbjq.cn

TS:   const value = data ?? "默认值";
来源：http://vsa.fzhhl.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zzv.yfazqb.com

Go:   if data == "" { data = "默认值" }
来源：http://boh.jqgufenzy.top

Ruby: value = data || "默认值"
来源：http://zqm.xziqi.cn

C#:   var value = data ?? "默认值";
来源：http://bvf.iojbl.cn

[A16] 真假值判断规则
来源：http://shu.hnxiangtu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wcj.52xcode.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lyp.birdmap.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cdk.yj20258888.top

TS:   if (!x) {}
来源：http://dfp.tianlin.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lfx.yuxming.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nce.mhx1999.top

Ruby: unless x            # nil 与 false 为假
来源：http://onl.tianlin.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zuh.zhongyouzk.top

[A17] 位运算
来源：http://afa.xylfe.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jnz.zhengqikj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cey.chenjidiqi.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zcb.guannengcc.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://exv.snrcjt.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pww.cheryme.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zrt.uphjek.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hku.yueranfly.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jmj.zhiwuduotai.top

[A18] 字符与 ASCII 码互转
来源：http://zag.gotoacloud.top

Py:   ord("A"); chr(65)
来源：http://bhg.mhx1999.top

PHP:  ord("A"); chr(65)
来源：http://fcl.zhongyouzk.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zkp.yuanzhike.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lts.chenlongwang.top

Java: (int) 'A'; (char) 65
来源：http://isb.birdmap.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gis.guowangkeji.top

Ruby: "A".ord; 65.chr
来源：http://ivm.nanxinkj.top

C#:   (int)'A'; (char)65
来源：http://ywv.vqdsnc.cn

[A19] 交换两个变量
来源：http://gnm.zdbjq.cn

Py:   a, b = b, a
来源：http://lng.hywenlv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xpm.andypj.xyz

JS:   [a, b] = [b, a];
来源：http://rxy.gaohongyu789.top

TS:   [a, b] = [b, a];
来源：http://ubb.fanxiaobao.xyz

Java: int t = a; a = b; b = t;
来源：http://pqf.yuxming.cn

Go:   a, b = b, a
来源：http://tat.ywan-chungtsiang.top

Ruby: a, b = b, a
来源：http://ouv.jianghu66.top

C#:   (a, b) = (b, a);
来源：http://clc.hywenlv.cn

[A20] 读取标准输入
来源：http://fbc.zdbjq.cn

Py:   name = input("请输入：")
来源：http://mhf.yj20258888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://syl.guowangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kan.gzhubu.top

TS:   // Node.js：readline 模块
来源：http://jpz.andypj.xyz

Java: new Scanner(System.in).nextLine()
来源：http://ced.gogol.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rms.fehbvm.com

Ruby: gets.chomp
来源：http://pqs.kuanghao11.cn

C#:   Console.ReadLine();
来源：http://boo.hywenlv.cn

[A21] 保留指定小数位输出
来源：http://mod.wangdashe.top

Py:   f"{3.14159:.2f}"
来源：http://hug.wangshuangyany.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://isy.gaohongyu789.top

JS:   (3.14159).toFixed(2)
来源：http://amu.yangfankeji.com

TS:   (3.14159).toFixed(2)
来源：http://wif.gogol.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://goe.yonumen.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nuf.aizwys.cn

Ruby: format("%.2f", 3.14159)
来源：http://uzy.xziqi.cn

C#:   3.14159.ToString("F2")
来源：http://vjk.sysykeji.top

[A22] 获取字符串长度
来源：http://sxt.xuetiantiany.cn

Py:   len(s)
来源：http://ali.vehdjk.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zyf.cucudq.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hhs.guowangkeji.top

TS:   s.length
来源：http://wdp.vqdsnc.cn

Java: s.length()
来源：http://fqk.ppjwa.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hqo.haohaochexian.top

Ruby: s.length
来源：http://jjv.cashguo.top

C#:   s.Length
来源：http://yos.c1oappe.top

[A23] 大小写转换
来源：http://kjv.hysaishi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://iaf.chenjidiqi.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xji.guannengcc.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hvz.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gar.cheryme.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dfb.zhixingplan.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kbb.hammf.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qcx.hongshengwenyu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gff.iojbl.cn

[A24] 去除首尾空白
来源：http://lon.gzhubu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://shf.sxryk.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xlm.yvedp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mzd.ctjpmb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://foo.tanke756.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hxs.tarul.cn

Go:   strings.TrimSpace(s)
来源：http://oxm.pycfn.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pia.hywenlv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nrc.gaohongyu789.top

[A25] 字符串比较
来源：http://mcg.hesvh.cn

Py:   s1 == s2; s1 != s2
来源：http://ynq.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://joy.ydjk.org.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gvg.ywan-chungtsiang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zev.jyoumei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jwo.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wpq.gaohongyu789.top

Ruby: s1 == s2; s1 <=> s2
来源：http://opi.birdmap.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jli.dashuyun.cn

[A26] 类型转换总览
来源：http://qpo.yangfankeji.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wog.guowangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qqz.xuetiantiany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hob.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://uol.andypj.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zmg.yj20258.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hxd.pycfn.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://xpc.jinqigufen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ysx.xziqi.cn

================================================================================
来源：http://uzm.smart0.xyz

B. 流程控制
来源：http://awc.yuxming.cn

================================================================================
来源：http://yzz.hysaishi.cn

[B01] 条件判断 if / else
来源：http://ebp.yuxming.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yjv.guannengcc.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yup.ydzc1.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xjy.yj202588.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gnn.tianlin.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://pda.cdnleiting.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rbu.wangshuangyany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nbo.haohaochexian.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bal.xziqi.cn

[B02] 多分支 else if / elif
来源：http://ltp.zdqjudy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hru.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nvy.ybcxt.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://byd.pycfn.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ezm.jinghuilouyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wms.daxiang520.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xer.nwbrower.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vhr.yvedp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nyw.jinqigfzy.top

[B03] switch / match / case
来源：http://ofe.cashguo.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ooq.yuxming.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rlt.xinyue.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://das.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xqk.shanyushiyangtech.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oew.tanke756.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ggk.ydjk.org.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xio.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eoi.daxiang520.top

[B04] for 计数循环
来源：http://flh.fehbvm.com

Py:   for i in range(10): print(i)
来源：http://kje.gogol.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gzw.gzhubu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zxz.xziqi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ewz.jinghuilouyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fcg.jinghuilouyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://adb.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://kom.hfpthk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ipu.yuxming.cn

[B05] 遍历数组 / 列表
来源：http://ilx.xingfuxueyuan.xyz

Py:   for item in arr: print(item)
来源：http://eoi.iojbl.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uhl.shanyushiyangtech.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tvg.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ixp.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mek.fzhhl.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hyr.chenjidiqi.icu

Ruby: arr.each { |item| puts item }
来源：http://beu.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oyv.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://ywg.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gla.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qbb.nwbrower.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://spb.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iij.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://okx.smart0.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rmb.smart0.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wrw.cashguo.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sop.redwolf501.top

[B07] while 循环
来源：http://bfm.meibo888.top

Py:   while i < 10: i += 1
来源：http://scf.ehwqpu.com

PHP:  while ($i < 10) { $i++; }
来源：http://joe.yonumen.top

JS:   while (i < 10) { i++; }
来源：http://bdm.yj20258.top

TS:   while (i < 10) { i++; }
来源：http://rks.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://hty.zhaomingkeji.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xnz.shangyingyoupin.top

Ruby: while i < 10; i += 1; end
来源：http://umi.yj20258888.top

C#:   while (i < 10) { i++; }
来源：http://whc.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://vcf.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://sgx.shangyingyoupin.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yyf.haohaochexian.top

JS:   do { i++; } while (i < 10);
来源：http://vsd.daria6918.cn

TS:   do { i++; } while (i < 10);
来源：http://cco.yanxiufei.cn

Java: do { i++; } while (i < 10);
来源：http://qbv.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nbe.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://urr.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://ele.iojbl.cn

[B09] break 与 continue
来源：http://cwm.smart0.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sxg.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tht.cdnleiting.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hkb.tianlin.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://crc.jinyuanbaomall.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hlk.havefunace.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://grf.xylfe.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qrr.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hud.yanxiufei.cn

[B10] 遍历同时拿索引
来源：http://haw.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oau.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cpm.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pqz.cucudq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tgp.jqgfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ujj.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://puv.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mju.sysykeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dzp.jqgfzy.top

[B11] 生成数字序列 / 区间
来源：http://kkh.jinyuanbaomall.cn

Py:   list(range(0, 10, 2))
来源：http://qkd.havefunace.top

PHP:  range(0, 10, 2);
来源：http://rcy.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bor.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fcn.snrcjt.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lfe.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tea.fzhhl.top

Ruby: (0...10).step(2).to_a
来源：http://vno.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vrk.chenjidiqi.icu

[B12] 跳出多层循环
来源：http://bix.guannengcc.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ghp.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hsr.jinqigufen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jxa.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xac.sweek.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aas.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ufc.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hef.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yyx.jiagoushi.top

[B13] 判断是否为数字
来源：http://emu.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://skf.daria6918.cn

PHP:  is_numeric($x)
来源：http://arm.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ycq.zhoulong.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zaq.xinyue.icu

Java: x instanceof Number
来源：http://vic.yonumen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://foo.cucudq.cn

Ruby: x.is_a?(Numeric)
来源：http://jkc.sufxvd.cn

C#:   x is int or double or decimal
来源：http://qvw.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://ivc.fzhhl.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qrl.ybcxt.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oxx.tarul.cn

JS:   [1, 2, 3].includes(x)
来源：http://kpv.ywan-chungtsiang.top

TS:   [1, 2, 3].includes(x)
来源：http://kal.feifeiyinyue.top

Java: List.of(1, 2, 3).contains(x)
来源：http://isq.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xwo.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ouj.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yhq.fehbvm.com

[B15] 布尔运算与取反
来源：http://sbw.sweek.top

Py:   a and b or not c
来源：http://tol.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://xze.yj20258888.top

JS:   a && b || !c
来源：http://xtn.gaohongyu789.top

TS:   a && b || !c
来源：http://dif.gaohongyu789.top

Java: a && b || !c
来源：http://iow.ctjpmb.com

Go:   a && b || !c
来源：http://jss.gaohongyu789.top

Ruby: a && b || !c
来源：http://dfv.tarul.cn

C#:   a && b || !c
来源：http://uha.zhengqikj.top

[B16] 卫语句：不满足条件提前返回
来源：http://ofb.hcnkem.com

Py:   if not data: return
来源：http://bdw.ppjwa.cn

PHP:  if (!$data) { return; }
来源：http://zhm.hongshengwenyu.top

JS:   if (!data) return;
来源：http://uii.ydjk.org.cn

TS:   if (!data) return;
来源：http://rcp.zhixingplan.top

Java: if (data == null) return;
来源：http://idd.jlsjyb.cn

Go:   if data == nil { return }
来源：http://sqc.52xcode.cn

Ruby: return if data.nil?
来源：http://oei.ybcxt.top

C#:   if (data == null) return;
来源：http://spq.hfpthk.cn

================================================================================
来源：http://zir.sysykeji.top

C. 函数与作用域
来源：http://cbj.zhiwuduotai.top

================================================================================
来源：http://ykm.guannengcc.top

[C01] 定义函数
来源：http://wmi.smart0.xyz

Py:   def add(a, b): return a + b
来源：http://dux.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qvr.zhixingplan.top

JS:   function add(a, b) { return a + b; }
来源：http://ryn.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vno.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ani.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hek.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://lpk.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gps.9152youxi.cn

[C02] 默认参数
来源：http://elp.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://avu.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://nvu.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://zcf.wangshuangyany.cn


<!-- 参考信息 -->