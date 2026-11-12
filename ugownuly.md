代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bhj.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://gak.yonumen.top

C#:   $"Hello, {name}!"
来源：http://yuw.sjlbkw.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://flo.xinyue.icu

Py:   "第一行\n第二行"
来源：http://xrj.ydjk.org.cn

PHP:  "第一行\n第二行"
来源：http://zjg.shanyushiyangkeji.top

JS:   "第一行\n第二行"
来源：http://bnh.ywan-chungtsiang.top

TS:   "第一行\n第二行"
来源：http://fgi.nanxuanxn.top

Java: "第一行\n第二行"
来源：http://tuz.feifeiyinyue.top

Go:   "第一行\n第二行"
来源：http://kyd.hcnkem.com

Ruby: "第一行\n第二行"
来源：http://qfx.dianchejie.cn

C#:   "第一行\n第二行"
来源：http://oxb.shanyushiyangtech.top

[A14] 注释写法
来源：http://rwv.sysykeji.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://nzm.uphjek.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://vkv.dianchejie.cn

JS:   // 单行；/* 多行 */
来源：http://hbt.jlsjyb.cn

TS:   // 单行；/* 多行 */
来源：http://zov.yj20258888.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qxu.yj20258888.top

Go:   // 单行；/* 多行 */
来源：http://dtm.yj20258.top

Ruby: # 单行；=begin 多行 =end
来源：http://fqs.mhx1999.top

C#:   // 单行；/* 多行 */
来源：http://seo.hesvh.cn

[A15] 空值判断与默认值
来源：http://qlf.uphjek.com

Py:   value = data or "默认值"
来源：http://ydh.svipenyu.cn

PHP:  $value = $data ?? "默认值";
来源：http://qmf.guannengcc.top

JS:   const value = data ?? "默认值";
来源：http://eds.yueranfly.top

TS:   const value = data ?? "默认值";
来源：http://uob.0kj1m.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ykq.yj20258888.top

Go:   if data == "" { data = "默认值" }
来源：http://sut.ydjk.org.cn

Ruby: value = data || "默认值"
来源：http://axu.zdbjq.cn

C#:   var value = data ?? "默认值";
来源：http://per.ctjpmb.com

[A16] 真假值判断规则
来源：http://kfw.xuetiantiany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://atu.birdmap.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bkv.cqqwz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yao.jqgfzy.top

TS:   if (!x) {}
来源：http://krf.0kj1m.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xrb.yangfankeji.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ejp.yueranfly.top

Ruby: unless x            # nil 与 false 为假
来源：http://zwt.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pvo.yueranfly.top

[A17] 位运算
来源：http://joz.xuetiantiany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zeb.wangdashe.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mgc.bjfxy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zlb.0kj1m.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qtq.fehbvm.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ntm.ppjwa.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qvx.nanxinkj.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oud.zhengqikj.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rxa.redwolf501.top

[A18] 字符与 ASCII 码互转
来源：http://sdb.cdnleiting.top

Py:   ord("A"); chr(65)
来源：http://ark.sweek.top

PHP:  ord("A"); chr(65)
来源：http://ber.fengsongda.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://phi.andypj.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mfh.xingfuxueyuan.xyz

Java: (int) 'A'; (char) 65
来源：http://ctg.gaohongyu789.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zxs.jyoumei.cn

Ruby: "A".ord; 65.chr
来源：http://sfb.nanxinkj.top

C#:   (int)'A'; (char)65
来源：http://lqm.nanxuanxn.top

[A19] 交换两个变量
来源：http://ekj.shuidangran.top

Py:   a, b = b, a
来源：http://dtq.tarul.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hgz.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://tqb.hcnkem.com

TS:   [a, b] = [b, a];
来源：http://bea.yvedp.cn

Java: int t = a; a = b; b = t;
来源：http://dpu.sxryk.cn

Go:   a, b = b, a
来源：http://asf.redwolf501.top

Ruby: a, b = b, a
来源：http://qpq.wangshuangyany.cn

C#:   (a, b) = (b, a);
来源：http://fxq.daxiang520.top

[A20] 读取标准输入
来源：http://jib.zhaomingkeji.xyz

Py:   name = input("请输入：")
来源：http://wzx.feifeiyinyue.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gyd.yj202588.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dch.hnxiangtu.top

TS:   // Node.js：readline 模块
来源：http://mnk.wangdashe.top

Java: new Scanner(System.in).nextLine()
来源：http://mls.fehbvm.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://whr.tarul.cn

Ruby: gets.chomp
来源：http://ete.ybcxt.top

C#:   Console.ReadLine();
来源：http://flk.snrcjt.cn

[A21] 保留指定小数位输出
来源：http://ldd.hywenlv.cn

Py:   f"{3.14159:.2f}"
来源：http://mhq.yongpay.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cqj.meibo888.top

JS:   (3.14159).toFixed(2)
来源：http://yxb.jqgufenzy.top

TS:   (3.14159).toFixed(2)
来源：http://vqa.ywan-chungtsiang.top

Java: String.format("%.2f", 3.14159)
来源：http://xye.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sus.ehwqpu.com

Ruby: format("%.2f", 3.14159)
来源：http://lyu.ydjk.org.cn

C#:   3.14159.ToString("F2")
来源：http://oqr.jiagoushi.top

[A22] 获取字符串长度
来源：http://ngb.pengpengdd.cyou

Py:   len(s)
来源：http://whf.ctjpmb.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dez.redwolf501.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mdm.9152youxi.cn

TS:   s.length
来源：http://wui.zhiwuduotai.top

Java: s.length()
来源：http://lxu.xziqi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://icl.tanke756.top

Ruby: s.length
来源：http://fol.uphjek.com

C#:   s.Length
来源：http://lxa.shanyushiyangkeji.top

[A23] 大小写转换
来源：http://euj.hywenlv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bfz.jinyuanbaomall.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zgm.yangfankeji.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://njn.yangfankeji.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oie.xingfuxueyuan.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gyb.bjfxy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ltw.hnxiangtu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://roq.jinghuilouyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xji.zdbjq.cn

[A24] 去除首尾空白
来源：http://jtg.svipenyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://foc.52xcode.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tjh.yonumen.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tee.xziqi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xhe.ywan-chungtsiang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kja.chenjidiqi.icu

Go:   strings.TrimSpace(s)
来源：http://kxb.xuanzx.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bec.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://erq.cdnleiting.top

[A25] 字符串比较
来源：http://ier.ydzc1.top

Py:   s1 == s2; s1 != s2
来源：http://wvj.zdbjq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oje.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mtj.haohaochexian.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ica.yueranfly.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://crh.vqdsnc.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mep.zhoulong.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://kgq.c1oappe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iop.nwbrower.top

[A26] 类型转换总览
来源：http://gxv.ydzc1.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mcu.cucudq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yla.yvedp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://obj.sjlbkw.cn

TS:   Number() String() Boolean() x as number
来源：http://tya.yfazqb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://urz.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wcm.zhixingplan.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://pkd.zdbjq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zki.yj20258888.top

================================================================================
来源：http://ynl.cdnleiting.top

B. 流程控制
来源：http://tvn.xinyue.icu

================================================================================
来源：http://ciu.jianghu66.top

[B01] 条件判断 if / else
来源：http://bzf.cheryme.top

Py:   result = "正" if x > 0 else "非正"
来源：http://udf.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gjc.hnqzz.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wbl.sweek.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://syx.yj20258888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yuq.chenjidiqi.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dyk.sufxvd.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ubx.vehdjk.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rbd.tian-w.cn

[B02] 多分支 else if / elif
来源：http://hjj.jqgfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jli.jqgufenzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fcr.hcnkem.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eau.zhixingplan.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xmj.yvedp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wwe.fanxiaobao.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rmz.kuanghao11.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hwz.uphjek.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jdk.yueranfly.top

[B03] switch / match / case
来源：http://dxm.jinyuanbaomall.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oew.meibo888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cph.yj20258.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jjg.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dnu.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gwb.fktsv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lme.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ugw.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://enc.hfpthk.cn

[B04] for 计数循环
来源：http://kyu.vqdsnc.cn

Py:   for i in range(10): print(i)
来源：http://skw.wangdashe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rbz.yuanzhike.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gjz.tian-w.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://npo.ppjwa.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zxm.cqqwz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://abw.cdnleiting.top

Ruby: 10.times { |i| puts i }
来源：http://urv.yj20258888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hoi.quarkkingdee.top

[B05] 遍历数组 / 列表
来源：http://sdc.cashguo.top

Py:   for item in arr: print(item)
来源：http://zcm.nwbrower.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://loj.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://omm.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://coi.zhaomingkeji.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://fpl.zhixingplan.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wkc.chenjidiqi.icu

Ruby: arr.each { |item| puts item }
来源：http://nsu.bjfxy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gdn.jinqigfzy.top

[B06] 遍历字典 / 对象
来源：http://bru.jyoumei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sqk.yuxming.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ptb.cqqwz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dna.shangyingyoupin.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hnv.guowangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zjg.bjfxy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eku.hongshengwenyu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cij.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://frl.cheryme.top

[B07] while 循环
来源：http://dpu.uphjek.com

Py:   while i < 10: i += 1
来源：http://rjd.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ahp.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://mue.zhengqikj.top

TS:   while (i < 10) { i++; }
来源：http://qpu.guowangkeji.top

Java: while (i < 10) { i++; }
来源：http://nsd.svipenyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ymz.fktsv.cn

Ruby: while i < 10; i += 1; end
来源：http://csk.gogol.net.cn

C#:   while (i < 10) { i++; }
来源：http://sdi.hnxiangtu.top

[B08] do-while（至少执行一次）
来源：http://ntr.hnxiangtu.top

Py:   # 无 do-while：用 while True + break
来源：http://mbc.daria6918.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fcn.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://ccn.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://iqc.mhx1999.top

Java: do { i++; } while (i < 10);
来源：http://gwy.epnwcf.com

Go:   for { i++; if i >= 10 { break } }
来源：http://kty.zhixingplan.top

Ruby: begin; i += 1; end while i < 10
来源：http://ewg.ppjwa.cn

C#:   do { i++; } while (i < 10);
来源：http://ciw.zdqjudy.top

[B09] break 与 continue
来源：http://hhz.iojbl.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://htw.jyoumei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bup.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgm.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gia.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yhy.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vuc.shuidangran.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bid.zdbjq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nef.yongpay.top

[B10] 遍历同时拿索引
来源：http://ubw.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kms.chenjidiqi.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iic.hnqzz.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://deu.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://afj.snrcjt.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cug.haohaochexian.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ujy.iojbl.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rlp.vqdsnc.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ulc.epnwcf.com

[B11] 生成数字序列 / 区间
来源：http://str.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://qoo.yuxming.cn

PHP:  range(0, 10, 2);
来源：http://hop.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://edk.xziqi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qdu.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ndl.mhx1999.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://odr.jlsjyb.cn

Ruby: (0...10).step(2).to_a
来源：http://yak.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://stb.zhongyouzk.top

[B12] 跳出多层循环
来源：http://shu.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://knz.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vwi.jianghu66.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yek.gaohongyu789.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://esj.ydjk.org.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ggs.zhongyouzk.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nja.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zfq.zhaomingkeji.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cwz.zhixingplan.top

[B13] 判断是否为数字
来源：http://tsg.yj20258.top

Py:   isinstance(x, (int, float))
来源：http://qii.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://yqp.chenzaomai.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dix.shanyushiyangtech.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ekq.ydjk.org.cn

Java: x instanceof Number
来源：http://qny.tarul.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dio.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://udh.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://fvs.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://zue.tanke756.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hog.zhixingplan.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pow.fengsongda.top

JS:   [1, 2, 3].includes(x)
来源：http://diu.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://fmz.jinqigfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://stu.birdmap.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mlk.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://lsm.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fyl.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://fnb.ybcxt.top

Py:   a and b or not c
来源：http://zjk.tanke756.top

PHP:  $a && $b || !$c
来源：http://jqb.bjfxy.top

JS:   a && b || !c
来源：http://jvi.guowangkeji.top

TS:   a && b || !c
来源：http://ypa.feifeiyinyue.top

Java: a && b || !c
来源：http://mpr.tarul.cn

Go:   a && b || !c
来源：http://cgh.0kj1m.cn

Ruby: a && b || !c
来源：http://dlb.havefunace.top

C#:   a && b || !c
来源：http://hkr.jinqigfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://fxi.bbcook.cn

Py:   if not data: return
来源：http://lzi.ivvv.top

PHP:  if (!$data) { return; }
来源：http://gzb.yj20258888.top

JS:   if (!data) return;
来源：http://njs.ydzc1.top

TS:   if (!data) return;
来源：http://qxe.hcnkem.com

Java: if (data == null) return;
来源：http://iyc.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://fjo.tarul.cn

Ruby: return if data.nil?
来源：http://udr.yanxiufei.cn

C#:   if (data == null) return;
来源：http://ljh.sweek.top

================================================================================
来源：http://wtl.vehdjk.com

C. 函数与作用域
来源：http://zkj.shanyushiyangtech.top

================================================================================
来源：http://oku.wangshuangyany.cn

[C01] 定义函数
来源：http://ipc.yvedp.cn

Py:   def add(a, b): return a + b
来源：http://ept.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gcr.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://fkm.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://coa.shanyushiyangtech.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ziu.jinyuanbaomall.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sxq.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://jas.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hyn.xziqi.cn

[C02] 默认参数
来源：http://bub.yonumen.top

Py:   def greet(name="World"): return name
来源：http://yqq.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dwa.jinqigufen.top

JS:   function greet(name = "World") { return name; }
来源：http://saf.ctjpmb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://tnn.cdnleiting.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nai.yj20258888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://swj.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://xwi.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://bid.zhiwuduotai.top

[C03] 可变参数
来源：http://obr.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://iij.wangdashe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kvb.jqgufenzy.top


<!-- 参考信息 -->