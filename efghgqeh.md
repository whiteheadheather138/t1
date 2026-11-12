代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://xtj.hesvh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://foh.meibo888.top

[A12] 字符串插值 / 格式化
来源：http://dkn.cashguo.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fyo.andypj.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zrs.shzxlz.cn

JS:   `Hello, ${name}!`
来源：http://qth.zhaomingkeji.xyz

TS:   `Hello, ${name}!`
来源：http://ptt.zhaomingkeji.xyz

Java: "Hello, %s!".formatted(name)
来源：http://vag.nanxinkj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jmg.jqgufenzy.top

Ruby: "Hello, #{name}!"
来源：http://qoj.fzhhl.top

C#:   $"Hello, {name}!"
来源：http://olm.hesvh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://evx.iojbl.cn

Py:   "第一行\n第二行"
来源：http://dqs.guannengcc.top

PHP:  "第一行\n第二行"
来源：http://ceq.xuetiantiany.cn

JS:   "第一行\n第二行"
来源：http://apt.yangfankeji.com

TS:   "第一行\n第二行"
来源：http://jtg.xingfuxueyuan.xyz

Java: "第一行\n第二行"
来源：http://wys.andypj.xyz

Go:   "第一行\n第二行"
来源：http://ccl.cashguo.top

Ruby: "第一行\n第二行"
来源：http://dyc.nanxinkj.top

C#:   "第一行\n第二行"
来源：http://ygu.gaohongyu789.top

[A14] 注释写法
来源：http://hkr.zhongyouzk.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://uwh.zhongyouzk.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://slu.ppjwa.cn

JS:   // 单行；/* 多行 */
来源：http://otn.hongshengwenyu.top

TS:   // 单行；/* 多行 */
来源：http://eaz.guannengcc.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dpb.zhijiandao.cn

Go:   // 单行；/* 多行 */
来源：http://tjj.zdqjudy.top

Ruby: # 单行；=begin 多行 =end
来源：http://cuf.zdqjudy.top

C#:   // 单行；/* 多行 */
来源：http://hgj.ydzc1.top

[A15] 空值判断与默认值
来源：http://wde.yj20258.top

Py:   value = data or "默认值"
来源：http://cja.zhongyouzk.top

PHP:  $value = $data ?? "默认值";
来源：http://urx.fehbvm.com

JS:   const value = data ?? "默认值";
来源：http://bjf.shzxlz.cn

TS:   const value = data ?? "默认值";
来源：http://uxv.jiagoushi.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qpf.vehdjk.com

Go:   if data == "" { data = "默认值" }
来源：http://uia.fengsongda.top

Ruby: value = data || "默认值"
来源：http://kzj.zhengqikj.top

C#:   var value = data ?? "默认值";
来源：http://ivc.chenlongwang.top

[A16] 真假值判断规则
来源：http://yue.nanxuanxn.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://csj.c1oappe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cmi.hammf.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rvl.yuxming.cn

TS:   if (!x) {}
来源：http://pma.hesvh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dhf.ctjpmb.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cnf.chenlongwang.top

Ruby: unless x            # nil 与 false 为假
来源：http://lxs.zhixingplan.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gtz.redwolf501.top

[A17] 位运算
来源：http://txh.snrcjt.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pyg.hysaishi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://oci.yongpay.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jck.jiagoushi.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uno.shanyushiyangtech.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://auh.aibaodan.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bdo.fzhhl.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zuo.yuanzhike.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://czc.xuanzx.com

[A18] 字符与 ASCII 码互转
来源：http://xkv.zdbjq.cn

Py:   ord("A"); chr(65)
来源：http://tnk.hysaishi.cn

PHP:  ord("A"); chr(65)
来源：http://pbd.zhiwuduotai.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yml.jyoumei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tay.fengsongda.top

Java: (int) 'A'; (char) 65
来源：http://cwh.shzxlz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xqd.fktsv.cn

Ruby: "A".ord; 65.chr
来源：http://vfq.ivvv.top

C#:   (int)'A'; (char)65
来源：http://snp.52xcode.cn

[A19] 交换两个变量
来源：http://pdy.wangshuangyany.cn

Py:   a, b = b, a
来源：http://moq.dianchejie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qki.aizwys.cn

JS:   [a, b] = [b, a];
来源：http://aly.andypj.xyz

TS:   [a, b] = [b, a];
来源：http://thd.gogol.net.cn

Java: int t = a; a = b; b = t;
来源：http://dkf.xuanzx.com

Go:   a, b = b, a
来源：http://asm.hnqzz.top

Ruby: a, b = b, a
来源：http://phz.tarul.cn

C#:   (a, b) = (b, a);
来源：http://cmc.nwbrower.top

[A20] 读取标准输入
来源：http://ypd.gaohongyu789.top

Py:   name = input("请输入：")
来源：http://fgh.gaohongyu789.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ylr.zhijiandao.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zpe.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://gda.yj20258888.top

Java: new Scanner(System.in).nextLine()
来源：http://inp.smart0.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://end.yongpay.top

Ruby: gets.chomp
来源：http://kts.redwolf501.top

C#:   Console.ReadLine();
来源：http://xlb.hesvh.cn

[A21] 保留指定小数位输出
来源：http://sbg.smart0.xyz

Py:   f"{3.14159:.2f}"
来源：http://mdj.tarul.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hwu.yongpay.top

JS:   (3.14159).toFixed(2)
来源：http://eni.shanyushiyangtech.top

TS:   (3.14159).toFixed(2)
来源：http://fbx.hysaishi.cn

Java: String.format("%.2f", 3.14159)
来源：http://bnc.sjlbkw.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yid.yongpay.top

Ruby: format("%.2f", 3.14159)
来源：http://brh.ppjwa.cn

C#:   3.14159.ToString("F2")
来源：http://yec.zhengqikj.top

[A22] 获取字符串长度
来源：http://yfs.birdmap.top

Py:   len(s)
来源：http://kme.yfazqb.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hai.fzhhl.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://foj.yonumen.top

TS:   s.length
来源：http://kmi.quarkkingdee.top

Java: s.length()
来源：http://plw.yj202588.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dlx.iojbl.cn

Ruby: s.length
来源：http://wjr.sufxvd.cn

C#:   s.Length
来源：http://une.nanxinkj.top

[A23] 大小写转换
来源：http://yyq.dianchejie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kcw.316326.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://slu.gzhubu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wdn.fehbvm.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://isn.jyoumei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jjm.jinyuanbaomall.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hty.yonumen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uhd.zhongyouzk.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lys.ywan-chungtsiang.top

[A24] 去除首尾空白
来源：http://zdw.havefunace.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gmq.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blq.ppjwa.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rii.zhaomingkeji.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xfh.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dni.zdbjq.cn

Go:   strings.TrimSpace(s)
来源：http://lpa.dashuyun.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xjb.hnqzz.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nmh.gogol.net.cn

[A25] 字符串比较
来源：http://wnk.9152youxi.cn

Py:   s1 == s2; s1 != s2
来源：http://lkq.hysaishi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xox.yuanzhike.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://myx.redwolf501.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nwt.mhx1999.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jol.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vxm.xuetiantiany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wlv.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lyn.sufxvd.cn

[A26] 类型转换总览
来源：http://lcx.yonumen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://syz.fengsongda.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ewh.quarkkingdee.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tct.tanke756.top

TS:   Number() String() Boolean() x as number
来源：http://jqj.meibo888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hwa.guannengcc.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://joo.yueranfly.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bjd.birdmap.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kaz.yvedp.cn

================================================================================
来源：http://vve.zdbjq.cn

B. 流程控制
来源：http://ssu.iojbl.cn

================================================================================
来源：http://oaa.epnwcf.com

[B01] 条件判断 if / else
来源：http://yrk.smart0.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://klg.shangyingyoupin.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zlo.aizwys.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jws.tian-w.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wnw.yonumen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rac.jyoumei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://niw.yj20258.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://edl.birdmap.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tqs.sweek.top

[B02] 多分支 else if / elif
来源：http://asv.yongpay.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aos.nanxinkj.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://unb.sufxvd.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pcf.sjlbkw.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pvr.dashuyun.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nff.yongpay.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tjo.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nqd.shangyingyoupin.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gke.gotoacloud.top

[B03] switch / match / case
来源：http://die.pengpengdd.cyou

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kkj.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hxx.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ecv.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oxr.tarul.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ipy.hcnkem.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mvb.meibo888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fkw.c1oappe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://utk.cucudq.cn

[B04] for 计数循环
来源：http://xhe.hesvh.cn

Py:   for i in range(10): print(i)
来源：http://fbt.bbcook.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ybq.cheryme.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://brz.guannengcc.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aca.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mgi.zhijiandao.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bmi.vqdsnc.cn

Ruby: 10.times { |i| puts i }
来源：http://gzn.xylfe.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cfw.jqgufenzy.top

[B05] 遍历数组 / 列表
来源：http://xfr.dashuyun.cn

Py:   for item in arr: print(item)
来源：http://xzk.yj20258.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uus.jiagoushi.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zqx.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://iec.jiagoushi.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://srq.9152youxi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yki.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://zer.daxiang520.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jzl.sjlbkw.cn

[B06] 遍历字典 / 对象
来源：http://dlw.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ivx.fzhhl.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://juu.redwolf501.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gte.hesvh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sid.jlsjyb.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ubv.jinqigfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wmn.yvedp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bvd.jqgfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vyu.316326.xyz

[B07] while 循环
来源：http://vbr.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://nsn.gaohongyu789.top

PHP:  while ($i < 10) { $i++; }
来源：http://lwo.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://hoy.redwolf501.top

TS:   while (i < 10) { i++; }
来源：http://tgn.yfazqb.com

Java: while (i < 10) { i++; }
来源：http://iqc.jlsjyb.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xas.c1oappe.top

Ruby: while i < 10; i += 1; end
来源：http://xvr.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://qba.zhaomingkeji.xyz

[B08] do-while（至少执行一次）
来源：http://dsq.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://vgj.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://idv.sysykeji.top

JS:   do { i++; } while (i < 10);
来源：http://sxj.xylfe.cn

TS:   do { i++; } while (i < 10);
来源：http://hgt.hfpthk.cn

Java: do { i++; } while (i < 10);
来源：http://mux.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wnx.zhijiandao.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pnl.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://hxh.yj20258888.top

[B09] break 与 continue
来源：http://tyq.hcnkem.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ovm.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qag.nwbrower.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rax.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://esl.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kos.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vld.xinyue.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mqy.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ncx.redwolf501.top

[B10] 遍历同时拿索引
来源：http://vvk.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xvk.zdqjudy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bje.meibo888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cem.shuidangran.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dbh.kuanghao11.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hcl.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nkd.jqgufenzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pjm.shanyushiyangtech.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qjx.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://swa.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://jbw.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://htr.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hzu.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://khu.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ndi.fanxiaobao.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kjn.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://onq.sjlbkw.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aja.ppjwa.cn

[B12] 跳出多层循环
来源：http://nkk.jqgufenzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kzu.cheryme.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fbo.pengpengdd.cyou

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bwu.havefunace.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://afb.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eau.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yzf.epnwcf.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kkc.gaohongyu789.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yll.iojbl.cn

[B13] 判断是否为数字
来源：http://fqz.hammf.cn

Py:   isinstance(x, (int, float))
来源：http://wmx.jinyuanbaomall.cn

PHP:  is_numeric($x)
来源：http://chb.zhijiandao.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sdl.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gql.pycfn.com

Java: x instanceof Number
来源：http://ngh.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tmu.wangdashe.top

Ruby: x.is_a?(Numeric)
来源：http://kwd.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://dez.iojbl.cn

[B14] 判断值是否在集合内
来源：http://cfe.hcnkem.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uld.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zek.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://yhq.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://dhx.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qmg.yongpay.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rkc.zycfv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ahi.chenjidiqi.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qrv.andypj.xyz

[B15] 布尔运算与取反
来源：http://ytz.hnqzz.top

Py:   a and b or not c
来源：http://thj.cheryme.top

PHP:  $a && $b || !$c
来源：http://suw.cucudq.cn

JS:   a && b || !c
来源：http://xxm.guowangkeji.top

TS:   a && b || !c
来源：http://nam.yfazqb.com

Java: a && b || !c
来源：http://aax.hammf.cn

Go:   a && b || !c
来源：http://mqh.xziqi.cn

Ruby: a && b || !c
来源：http://lfj.shangyingyoupin.top

C#:   a && b || !c
来源：http://vjm.yj202588.top

[B16] 卫语句：不满足条件提前返回
来源：http://exd.hongshengwenyu.top

Py:   if not data: return
来源：http://dad.mhx1999.top

PHP:  if (!$data) { return; }
来源：http://rux.hywenlv.cn

JS:   if (!data) return;
来源：http://ndp.ctjpmb.com

TS:   if (!data) return;
来源：http://isx.hongshengwenyu.top

Java: if (data == null) return;
来源：http://aql.nwbrower.top

Go:   if data == nil { return }
来源：http://yhk.zhixingplan.top

Ruby: return if data.nil?
来源：http://bvz.ydjk.org.cn

C#:   if (data == null) return;
来源：http://mwb.zhixingplan.top

================================================================================
来源：http://kgz.cqqwz.cn

C. 函数与作用域
来源：http://vue.chenjidiqi.icu

================================================================================
来源：http://won.gzhubu.top

[C01] 定义函数
来源：http://axq.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://sdl.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qdo.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://wki.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://efn.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://eyc.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xfk.jinyuanbaomall.cn

Ruby: def add(a, b); a + b; end
来源：http://det.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wzf.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://jfp.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://ofg.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dvx.jyoumei.cn

JS:   function greet(name = "World") { return name; }
来源：http://qxn.ehwqpu.com


<!-- 参考信息 -->