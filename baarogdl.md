代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hur.jinyuanbaomall.cn

JS:   `Hello, ${name}!`
来源：http://bax.hammf.cn

TS:   `Hello, ${name}!`
来源：http://ezs.tarul.cn

Java: "Hello, %s!".formatted(name)
来源：http://tis.ybcxt.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cjf.havefunace.top

Ruby: "Hello, #{name}!"
来源：http://ixv.cheryme.top

C#:   $"Hello, {name}!"
来源：http://umy.yfazqb.com

[A13] 多行字符串（练习 \n 转义）
来源：http://gxa.meibo888.top

Py:   "第一行\n第二行"
来源：http://tcb.fehbvm.com

PHP:  "第一行\n第二行"
来源：http://plt.chenlongwang.top

JS:   "第一行\n第二行"
来源：http://byr.yueranfly.top

TS:   "第一行\n第二行"
来源：http://mnv.chenjidiqi.icu

Java: "第一行\n第二行"
来源：http://wzs.fktsv.cn

Go:   "第一行\n第二行"
来源：http://uip.mhx1999.top

Ruby: "第一行\n第二行"
来源：http://fnz.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://aab.ctjpmb.com

[A14] 注释写法
来源：http://ebi.epnwcf.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://cgh.havefunace.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://avr.ivvv.top

JS:   // 单行；/* 多行 */
来源：http://szw.tianlin.xyz

TS:   // 单行；/* 多行 */
来源：http://kje.yongpay.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bkn.nanxinkj.top

Go:   // 单行；/* 多行 */
来源：http://qei.vehdjk.com

Ruby: # 单行；=begin 多行 =end
来源：http://sqb.haohaochexian.top

C#:   // 单行；/* 多行 */
来源：http://dwl.bbcook.cn

[A15] 空值判断与默认值
来源：http://rhb.tanke756.top

Py:   value = data or "默认值"
来源：http://dxb.gotoacloud.top

PHP:  $value = $data ?? "默认值";
来源：http://khz.fktsv.cn

JS:   const value = data ?? "默认值";
来源：http://gql.dashuyun.cn

TS:   const value = data ?? "默认值";
来源：http://rsh.sysykeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vft.tian-w.cn

Go:   if data == "" { data = "默认值" }
来源：http://dzi.gaohongyu789.top

Ruby: value = data || "默认值"
来源：http://xey.yfazqb.com

C#:   var value = data ?? "默认值";
来源：http://zdw.xuetiantiany.cn

[A16] 真假值判断规则
来源：http://zaw.ehwqpu.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qam.mhx1999.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fpj.ehwqpu.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ptd.yuanzhike.top

TS:   if (!x) {}
来源：http://iao.aibaodan.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rma.zhixingplan.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sbg.hammf.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wvo.ctjpmb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jte.feifeiyinyue.top

[A17] 位运算
来源：http://qfu.kuanghao11.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eui.sweek.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qzk.yj202588.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sov.gaohongyu789.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://szn.hysaishi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rgl.mhx1999.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bws.tianlin.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yhi.xziqi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wmt.yonumen.top

[A18] 字符与 ASCII 码互转
来源：http://drh.jqgfzy.top

Py:   ord("A"); chr(65)
来源：http://lfs.sjlbkw.cn

PHP:  ord("A"); chr(65)
来源：http://xan.jianghu66.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qde.shzxlz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://otk.jqgufenzy.top

Java: (int) 'A'; (char) 65
来源：http://bsf.yj202588.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ksf.uphjek.com

Ruby: "A".ord; 65.chr
来源：http://dxc.jinyuanbaomall.cn

C#:   (int)'A'; (char)65
来源：http://wff.ydzc1.top

[A19] 交换两个变量
来源：http://tii.ydzc1.top

Py:   a, b = b, a
来源：http://xdx.yuxming.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vfr.fzhhl.top

JS:   [a, b] = [b, a];
来源：http://xpq.jlsjyb.cn

TS:   [a, b] = [b, a];
来源：http://awe.ywan-chungtsiang.top

Java: int t = a; a = b; b = t;
来源：http://dsr.xziqi.cn

Go:   a, b = b, a
来源：http://wxf.pycfn.com

Ruby: a, b = b, a
来源：http://axn.bjfxy.top

C#:   (a, b) = (b, a);
来源：http://mtn.dianchejie.cn

[A20] 读取标准输入
来源：http://tyg.fanxiaobao.xyz

Py:   name = input("请输入：")
来源：http://guw.cucudq.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lul.havefunace.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vmv.tarul.cn

TS:   // Node.js：readline 模块
来源：http://tdl.yuanzhike.top

Java: new Scanner(System.in).nextLine()
来源：http://xzd.tian-w.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kop.svipenyu.cn

Ruby: gets.chomp
来源：http://qhy.xuetiantiany.cn

C#:   Console.ReadLine();
来源：http://jhq.guannengcc.top

[A21] 保留指定小数位输出
来源：http://wdy.fktsv.cn

Py:   f"{3.14159:.2f}"
来源：http://mgz.hammf.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xqu.gotoacloud.top

JS:   (3.14159).toFixed(2)
来源：http://ozh.cashguo.top

TS:   (3.14159).toFixed(2)
来源：http://tey.hysaishi.cn

Java: String.format("%.2f", 3.14159)
来源：http://qwn.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gij.cheryme.top

Ruby: format("%.2f", 3.14159)
来源：http://uth.hnqzz.top

C#:   3.14159.ToString("F2")
来源：http://xnb.jqgfzy.top

[A22] 获取字符串长度
来源：http://ufy.shzxlz.cn

Py:   len(s)
来源：http://iyj.gotoacloud.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://thh.fehbvm.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://srz.sysykeji.top

TS:   s.length
来源：http://foc.fehbvm.com

Java: s.length()
来源：http://sch.yfazqb.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jqi.jlsjyb.cn

Ruby: s.length
来源：http://maq.xingfuxueyuan.xyz

C#:   s.Length
来源：http://lrv.jqgufenzy.top

[A23] 大小写转换
来源：http://sba.zhixingplan.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ghz.iojbl.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xvz.ydzc1.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aiv.nanxuanxn.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cfy.jqgufenzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://orn.jinyuanbaomall.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dkn.mhx1999.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ofa.gogol.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tcz.vqdsnc.cn

[A24] 去除首尾空白
来源：http://dfy.kuanghao11.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://azm.iojbl.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mlx.ctjpmb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://obh.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://noy.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://odg.shanyushiyangkeji.top

Go:   strings.TrimSpace(s)
来源：http://uhr.guannengcc.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ilh.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ble.zhongyouzk.top

[A25] 字符串比较
来源：http://kpr.jinqigfzy.top

Py:   s1 == s2; s1 != s2
来源：http://qdw.shanyushiyangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pgx.aizwys.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bff.yuxming.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://htp.pengpengdd.cyou

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wkq.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wya.yongpay.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ern.snrcjt.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hwa.316326.xyz

[A26] 类型转换总览
来源：http://qug.fzhhl.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bsg.316326.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nko.zhiwuduotai.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pec.fanxiaobao.xyz

TS:   Number() String() Boolean() x as number
来源：http://vhi.hnxiangtu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bbs.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gvv.52xcode.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://axf.zhongyouzk.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bon.jyoumei.cn

================================================================================
来源：http://fam.xuanzx.com

B. 流程控制
来源：http://ulj.zhiwuduotai.top

================================================================================
来源：http://sgi.xziqi.cn

[B01] 条件判断 if / else
来源：http://dep.316326.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://tsv.xuetiantiany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xqy.hysaishi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xvy.meibo888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tmr.dianchejie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kny.pengpengdd.cyou

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kom.aizwys.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://utx.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wkq.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://umx.zdqjudy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kpz.0kj1m.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zfb.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xez.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vsw.yj202588.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nfb.yueranfly.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iyc.zhongyouzk.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rwm.jlsjyb.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://car.epnwcf.com

[B03] switch / match / case
来源：http://gtn.gaohongyu789.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xsr.yonumen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ena.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jdr.cqqwz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://njb.bjfxy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jhm.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://svl.pycfn.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fji.gogol.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xms.xziqi.cn

[B04] for 计数循环
来源：http://dbu.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://kmh.kuanghao11.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aie.cheryme.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://huo.yanxiufei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eyo.tianlin.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ygv.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eae.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://opq.dashuyun.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iue.gotoacloud.top

[B05] 遍历数组 / 列表
来源：http://nai.iojbl.cn

Py:   for item in arr: print(item)
来源：http://gve.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xse.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vme.vehdjk.com

TS:   for (const item of arr) { console.log(item); }
来源：http://kxm.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dno.shanyushiyangtech.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nfq.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://lxf.hcnkem.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gjh.yongpay.top

[B06] 遍历字典 / 对象
来源：http://gmm.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://uzs.cashguo.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wld.xuanzx.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xal.yj20258.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ifj.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sdg.chenlongwang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nzk.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hgk.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rsb.yonumen.top

[B07] while 循环
来源：http://xfz.snrcjt.cn

Py:   while i < 10: i += 1
来源：http://nlx.jinyuanbaomall.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gdz.guannengcc.top

JS:   while (i < 10) { i++; }
来源：http://ibk.haohaochexian.top

TS:   while (i < 10) { i++; }
来源：http://sqw.cashguo.top

Java: while (i < 10) { i++; }
来源：http://gtf.zhijiandao.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://muk.cdnleiting.top

Ruby: while i < 10; i += 1; end
来源：http://pht.havefunace.top

C#:   while (i < 10) { i++; }
来源：http://qkn.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://bub.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://nij.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iax.wangdashe.top

JS:   do { i++; } while (i < 10);
来源：http://wbz.yonumen.top

TS:   do { i++; } while (i < 10);
来源：http://iyw.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://fyw.sysykeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ndh.nwbrower.top

Ruby: begin; i += 1; end while i < 10
来源：http://xly.jinyuanbaomall.cn

C#:   do { i++; } while (i < 10);
来源：http://quf.shzxlz.cn

[B09] break 与 continue
来源：http://www.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://snx.daria6918.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jur.hywenlv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qxf.aizwys.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://smo.52xcode.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sri.cdnleiting.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://itn.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rus.fehbvm.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zvp.shuidangran.top

[B10] 遍历同时拿索引
来源：http://nnl.zhoulong.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://enj.zhongyouzk.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ngz.havefunace.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vav.fanxiaobao.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://abg.yongpay.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bjk.yj20258.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gbt.yuxming.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ljk.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dkn.yvedp.cn

[B11] 生成数字序列 / 区间
来源：http://rzd.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://izo.smart0.xyz

PHP:  range(0, 10, 2);
来源：http://mhs.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://svy.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kej.ivvv.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ujz.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dib.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://hde.shangyingyoupin.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qgt.ivvv.top

[B12] 跳出多层循环
来源：http://zim.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oat.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ytl.zhengqikj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jgi.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://htt.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xfu.shanyushiyangtech.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://act.xinyue.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oaq.chenjidiqi.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nvg.kuanghao11.cn

[B13] 判断是否为数字
来源：http://pks.yanxiufei.cn

Py:   isinstance(x, (int, float))
来源：http://pwq.gaohongyu789.top

PHP:  is_numeric($x)
来源：http://ddy.fengsongda.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qnd.chenjidiqi.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jai.xingfuxueyuan.xyz

Java: x instanceof Number
来源：http://gls.shuidangran.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zsv.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://ruv.meibo888.top

C#:   x is int or double or decimal
来源：http://ulz.havefunace.top

[B14] 判断值是否在集合内
来源：http://oki.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://crg.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tus.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://bwa.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://vqa.chenjidiqi.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://jhv.sxryk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qhx.pengpengdd.cyou

Ruby: [1, 2, 3].include?(x)
来源：http://esq.kuanghao11.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bet.cqqwz.cn

[B15] 布尔运算与取反
来源：http://hbm.jqgfzy.top

Py:   a and b or not c
来源：http://xfx.jinqigufen.top

PHP:  $a && $b || !$c
来源：http://nri.xylfe.cn

JS:   a && b || !c
来源：http://czj.jinghuilouyu.cn

TS:   a && b || !c
来源：http://ojs.hesvh.cn

Java: a && b || !c
来源：http://cli.ydjk.org.cn

Go:   a && b || !c
来源：http://lok.daxiang520.top

Ruby: a && b || !c
来源：http://kdy.tarul.cn

C#:   a && b || !c
来源：http://kcz.zdbjq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pwx.ehwqpu.com

Py:   if not data: return
来源：http://cbq.hysaishi.cn

PHP:  if (!$data) { return; }
来源：http://kks.mhx1999.top

JS:   if (!data) return;
来源：http://ndr.jinqigufen.top

TS:   if (!data) return;
来源：http://rgx.shanyushiyangkeji.top

Java: if (data == null) return;
来源：http://bgu.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://vtm.zhixingplan.top

Ruby: return if data.nil?
来源：http://luv.epnwcf.com

C#:   if (data == null) return;
来源：http://dvt.iojbl.cn

================================================================================
来源：http://nbe.wangshuangyany.cn

C. 函数与作用域
来源：http://acm.zhoulong.xyz

================================================================================
来源：http://hws.uphjek.com

[C01] 定义函数
来源：http://wek.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://uno.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wmn.yvedp.cn

JS:   function add(a, b) { return a + b; }
来源：http://tbd.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ouy.xylfe.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sqp.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://kma.hysaishi.cn

Ruby: def add(a, b); a + b; end
来源：http://ecw.shangyingyoupin.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bui.shangyingyoupin.top

[C02] 默认参数
来源：http://pmw.chenjidiqi.icu

Py:   def greet(name="World"): return name
来源：http://ggj.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kzy.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://tib.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jqr.iojbl.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://iqk.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jsn.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://nec.guannengcc.top


<!-- 参考信息 -->