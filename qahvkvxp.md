代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bpp.gogol.net.cn

JS:   `Hello, ${name}!`
来源：http://amf.xylfe.cn

TS:   `Hello, ${name}!`
来源：http://eeo.jqgufenzy.top

Java: "Hello, %s!".formatted(name)
来源：http://exv.havefunace.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://edj.yvedp.cn

Ruby: "Hello, #{name}!"
来源：http://jky.nanxuanxn.top

C#:   $"Hello, {name}!"
来源：http://fez.jlsjyb.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ryu.sxryk.cn

Py:   "第一行\n第二行"
来源：http://jpz.ppjwa.cn

PHP:  "第一行\n第二行"
来源：http://het.cdnleiting.top

JS:   "第一行\n第二行"
来源：http://jaw.cashguo.top

TS:   "第一行\n第二行"
来源：http://wwr.jinyuanbaomall.cn

Java: "第一行\n第二行"
来源：http://vat.yj202588.top

Go:   "第一行\n第二行"
来源：http://nza.52xcode.cn

Ruby: "第一行\n第二行"
来源：http://kky.dashuyun.cn

C#:   "第一行\n第二行"
来源：http://nom.ywan-chungtsiang.top

[A14] 注释写法
来源：http://apl.hcnkem.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://fld.ybcxt.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://emd.xinyue.icu

JS:   // 单行；/* 多行 */
来源：http://trj.hongshengwenyu.top

TS:   // 单行；/* 多行 */
来源：http://bch.chenjidiqi.icu

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wvt.vqdsnc.cn

Go:   // 单行；/* 多行 */
来源：http://ekn.gaohongyu789.top

Ruby: # 单行；=begin 多行 =end
来源：http://kcv.9152youxi.cn

C#:   // 单行；/* 多行 */
来源：http://krr.wangdashe.top

[A15] 空值判断与默认值
来源：http://klm.tianlin.xyz

Py:   value = data or "默认值"
来源：http://tem.cdnleiting.top

PHP:  $value = $data ?? "默认值";
来源：http://eyw.c1oappe.top

JS:   const value = data ?? "默认值";
来源：http://nqh.pengpengdd.cyou

TS:   const value = data ?? "默认值";
来源：http://dab.xuetiantiany.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://znj.quarkkingdee.top

Go:   if data == "" { data = "默认值" }
来源：http://tpr.yonumen.top

Ruby: value = data || "默认值"
来源：http://kpm.52xcode.cn

C#:   var value = data ?? "默认值";
来源：http://kqo.pycfn.com

[A16] 真假值判断规则
来源：http://zja.jinqigufen.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hyc.shuidangran.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ekg.haohaochexian.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lbn.zhengqikj.top

TS:   if (!x) {}
来源：http://fty.yj20258888.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dbs.quarkkingdee.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rrn.tarul.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bdd.cashguo.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ehl.cdnleiting.top

[A17] 位运算
来源：http://aoi.birdmap.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tcc.dashuyun.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://aer.havefunace.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://afw.sysykeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cyi.pengpengdd.cyou

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://thj.wangshuangyany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qpe.zdbjq.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://epk.ivvv.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lqa.hcnkem.com

[A18] 字符与 ASCII 码互转
来源：http://yvn.birdmap.top

Py:   ord("A"); chr(65)
来源：http://dgv.quarkkingdee.top

PHP:  ord("A"); chr(65)
来源：http://lct.pycfn.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uxr.nwbrower.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ldu.shanyushiyangkeji.top

Java: (int) 'A'; (char) 65
来源：http://gld.jiagoushi.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cmw.sjlbkw.cn

Ruby: "A".ord; 65.chr
来源：http://mau.hnxiangtu.top

C#:   (int)'A'; (char)65
来源：http://ycx.fanxiaobao.xyz

[A19] 交换两个变量
来源：http://qee.dashuyun.cn

Py:   a, b = b, a
来源：http://aur.yj20258888.top

PHP:  [$a, $b] = [$b, $a];
来源：http://zim.daria6918.cn

JS:   [a, b] = [b, a];
来源：http://mfs.yvedp.cn

TS:   [a, b] = [b, a];
来源：http://utj.zhongyouzk.top

Java: int t = a; a = b; b = t;
来源：http://myo.gogol.net.cn

Go:   a, b = b, a
来源：http://hlw.xuetiantiany.cn

Ruby: a, b = b, a
来源：http://oes.chenlongwang.top

C#:   (a, b) = (b, a);
来源：http://nij.hywenlv.cn

[A20] 读取标准输入
来源：http://ukg.jqgfzy.top

Py:   name = input("请输入：")
来源：http://kbw.dianchejie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pmc.cdnleiting.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zef.haohaochexian.top

TS:   // Node.js：readline 模块
来源：http://rvr.gogol.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://msa.cashguo.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zvm.zycfv.cn

Ruby: gets.chomp
来源：http://icm.epnwcf.com

C#:   Console.ReadLine();
来源：http://dkm.hywenlv.cn

[A21] 保留指定小数位输出
来源：http://nrp.shanyushiyangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://wuh.yangfankeji.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gkt.guannengcc.top

JS:   (3.14159).toFixed(2)
来源：http://ycq.sysykeji.top

TS:   (3.14159).toFixed(2)
来源：http://pru.jinghuilouyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://lry.hcnkem.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xci.feifeiyinyue.top

Ruby: format("%.2f", 3.14159)
来源：http://hhv.haohaochexian.top

C#:   3.14159.ToString("F2")
来源：http://fif.gzhubu.top

[A22] 获取字符串长度
来源：http://iim.zhixingplan.top

Py:   len(s)
来源：http://svl.hongshengwenyu.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://php.gogol.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vic.jqgfzy.top

TS:   s.length
来源：http://vit.vehdjk.com

Java: s.length()
来源：http://jre.gogol.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://juh.jinyuanbaomall.cn

Ruby: s.length
来源：http://dbq.xinyue.icu

C#:   s.Length
来源：http://dpf.birdmap.top

[A23] 大小写转换
来源：http://qup.shzxlz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://crn.ehwqpu.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://knd.hywenlv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ehb.sxryk.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dcx.daria6918.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hbi.cqqwz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ccv.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tip.smart0.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://hzd.cdnleiting.top

[A24] 去除首尾空白
来源：http://pjj.guannengcc.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bzf.tarul.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://srw.pengpengdd.cyou

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ndt.hcnkem.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eik.yanxiufei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tbg.shanyushiyangtech.top

Go:   strings.TrimSpace(s)
来源：http://zmp.uphjek.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ldx.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gxg.fengsongda.top

[A25] 字符串比较
来源：http://egu.daxiang520.top

Py:   s1 == s2; s1 != s2
来源：http://abz.shangyingyoupin.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cke.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nli.zhiwuduotai.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://icw.yj20258888.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qiy.redwolf501.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zuj.fengsongda.top

Ruby: s1 == s2; s1 <=> s2
来源：http://weg.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uol.hywenlv.cn

[A26] 类型转换总览
来源：http://wtp.aizwys.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zdi.yj202588.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fps.zhixingplan.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xzq.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://yol.cdnleiting.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rty.jqgfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vtu.wangshuangyany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://eqv.sysykeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ghd.jinqigfzy.top

================================================================================
来源：http://ibz.fanxiaobao.xyz

B. 流程控制
来源：http://pxd.daria6918.cn

================================================================================
来源：http://ciq.fktsv.cn

[B01] 条件判断 if / else
来源：http://lpb.sufxvd.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ksm.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mvj.xylfe.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://whi.cheryme.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://koh.ywan-chungtsiang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://win.svipenyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kco.yj20258888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gka.zdqjudy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jfx.shzxlz.cn

[B02] 多分支 else if / elif
来源：http://ppa.shanyushiyangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://phz.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kjc.zhixingplan.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wwv.jinghuilouyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yof.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lmh.ybcxt.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ubm.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zhk.yongpay.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qzk.sweek.top

[B03] switch / match / case
来源：http://kqs.ywan-chungtsiang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://txh.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tdc.ydzc1.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bek.zhengqikj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bku.fzhhl.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vnw.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jgg.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ywu.nanxuanxn.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nhy.zycfv.cn

[B04] for 计数循环
来源：http://zip.jiagoushi.top

Py:   for i in range(10): print(i)
来源：http://rqa.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gup.jqgfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dyl.jyoumei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oyl.fanxiaobao.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nhz.hysaishi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vgj.chenzaomai.com

Ruby: 10.times { |i| puts i }
来源：http://iuq.hywenlv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hyg.cucudq.cn

[B05] 遍历数组 / 列表
来源：http://etd.bbcook.cn

Py:   for item in arr: print(item)
来源：http://asy.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oep.shzxlz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fcz.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bfx.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rwd.bjfxy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://adq.tian-w.cn

Ruby: arr.each { |item| puts item }
来源：http://wyp.jinyuanbaomall.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gtv.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://jww.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://alx.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://etz.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yvb.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tnq.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jzy.hysaishi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yhm.xziqi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jmf.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ibx.wangdashe.top

[B07] while 循环
来源：http://jdl.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://mnr.hysaishi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zkk.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://uyg.yangfankeji.com

TS:   while (i < 10) { i++; }
来源：http://zbg.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://rus.316326.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tzq.chenzaomai.com

Ruby: while i < 10; i += 1; end
来源：http://fvt.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://sel.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://cru.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://nun.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yja.xingfuxueyuan.xyz

JS:   do { i++; } while (i < 10);
来源：http://ngz.nanxuanxn.top

TS:   do { i++; } while (i < 10);
来源：http://ycz.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://vna.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yhy.0kj1m.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ady.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://cef.hnqzz.top

[B09] break 与 continue
来源：http://vpa.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://our.snrcjt.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yyy.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qfk.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tvi.redwolf501.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://enl.yuxming.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xlr.ehwqpu.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xxx.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lar.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://lso.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fjp.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wja.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xlt.jiagoushi.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rfw.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kmw.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kcq.yj202588.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ojq.quarkkingdee.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://enm.gzhubu.top

[B11] 生成数字序列 / 区间
来源：http://czy.hnxiangtu.top

Py:   list(range(0, 10, 2))
来源：http://pfy.snrcjt.cn

PHP:  range(0, 10, 2);
来源：http://fmm.yongpay.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lha.xingfuxueyuan.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vkl.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xoq.ydjk.org.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lbx.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://akr.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wjw.sweek.top

[B12] 跳出多层循环
来源：http://flp.jinghuilouyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fdl.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cav.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nrp.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wtn.smart0.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xpu.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eyu.andypj.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yoj.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bxw.jqgufenzy.top

[B13] 判断是否为数字
来源：http://eih.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://wwj.yonumen.top

PHP:  is_numeric($x)
来源：http://ift.shuidangran.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ije.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lia.yongpay.top

Java: x instanceof Number
来源：http://mlt.epnwcf.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vsc.pengpengdd.cyou

Ruby: x.is_a?(Numeric)
来源：http://oxe.ctjpmb.com

C#:   x is int or double or decimal
来源：http://sjq.316326.xyz

[B14] 判断值是否在集合内
来源：http://kzg.cqqwz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gxt.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xaj.daxiang520.top

JS:   [1, 2, 3].includes(x)
来源：http://ubm.yonumen.top

TS:   [1, 2, 3].includes(x)
来源：http://ata.guowangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zcd.zhixingplan.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://met.zhongyouzk.top

Ruby: [1, 2, 3].include?(x)
来源：http://bxh.pycfn.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hnt.meibo888.top

[B15] 布尔运算与取反
来源：http://kpa.316326.xyz

Py:   a and b or not c
来源：http://atg.yonumen.top

PHP:  $a && $b || !$c
来源：http://fqo.jinqigfzy.top

JS:   a && b || !c
来源：http://krx.gaohongyu789.top

TS:   a && b || !c
来源：http://bbz.gotoacloud.top

Java: a && b || !c
来源：http://rzm.sysykeji.top

Go:   a && b || !c
来源：http://esb.pycfn.com

Ruby: a && b || !c
来源：http://ycb.pycfn.com

C#:   a && b || !c
来源：http://mgn.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://kmr.shanyushiyangtech.top

Py:   if not data: return
来源：http://wju.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://ifw.xziqi.cn

JS:   if (!data) return;
来源：http://mtv.iojbl.cn

TS:   if (!data) return;
来源：http://euf.zhongyouzk.top

Java: if (data == null) return;
来源：http://jza.sweek.top

Go:   if data == nil { return }
来源：http://mar.guannengcc.top

Ruby: return if data.nil?
来源：http://cxn.fengsongda.top

C#:   if (data == null) return;
来源：http://rjs.sufxvd.cn

================================================================================
来源：http://jcv.xinyue.icu

C. 函数与作用域
来源：http://tiq.hywenlv.cn

================================================================================
来源：http://xoh.cucudq.cn

[C01] 定义函数
来源：http://llx.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://gzj.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vre.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://yeg.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://liv.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lrl.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://zym.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://jfw.uphjek.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dmr.shangyingyoupin.top

[C02] 默认参数
来源：http://qjy.pycfn.com

Py:   def greet(name="World"): return name
来源：http://pwv.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rfn.cheryme.top

JS:   function greet(name = "World") { return name; }
来源：http://grh.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bzf.snrcjt.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fhf.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lcz.vqdsnc.cn

Ruby: def greet(name = "World") = name
来源：http://izq.sufxvd.cn


<!-- 参考信息 -->