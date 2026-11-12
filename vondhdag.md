代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://qgq.hywenlv.cn

C#:   x > 0 ? "yes" : "no"
来源：http://djh.pengpengdd.cyou

[A12] 字符串插值 / 格式化
来源：http://rce.mhx1999.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://auy.nwbrower.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mmj.jiagoushi.top

JS:   `Hello, ${name}!`
来源：http://zfq.yuanzhike.top

TS:   `Hello, ${name}!`
来源：http://iup.sufxvd.cn

Java: "Hello, %s!".formatted(name)
来源：http://nup.zhongyouzk.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kxf.quarkkingdee.top

Ruby: "Hello, #{name}!"
来源：http://bia.c1oappe.top

C#:   $"Hello, {name}!"
来源：http://rwc.ctjpmb.com

[A13] 多行字符串（练习 \n 转义）
来源：http://zwf.cashguo.top

Py:   "第一行\n第二行"
来源：http://myh.gotoacloud.top

PHP:  "第一行\n第二行"
来源：http://boh.smart0.xyz

JS:   "第一行\n第二行"
来源：http://vxi.cashguo.top

TS:   "第一行\n第二行"
来源：http://wgp.hcnkem.com

Java: "第一行\n第二行"
来源：http://dut.feifeiyinyue.top

Go:   "第一行\n第二行"
来源：http://xqp.zdbjq.cn

Ruby: "第一行\n第二行"
来源：http://dlp.gzhubu.top

C#:   "第一行\n第二行"
来源：http://seu.zdbjq.cn

[A14] 注释写法
来源：http://ukj.tian-w.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rjj.yonumen.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://tot.uphjek.com

JS:   // 单行；/* 多行 */
来源：http://xbd.cashguo.top

TS:   // 单行；/* 多行 */
来源：http://xzb.yueranfly.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dzd.xziqi.cn

Go:   // 单行；/* 多行 */
来源：http://vnk.tianlin.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://hbr.zdqjudy.top

C#:   // 单行；/* 多行 */
来源：http://njd.snrcjt.cn

[A15] 空值判断与默认值
来源：http://lxu.ybcxt.top

Py:   value = data or "默认值"
来源：http://ywl.cucudq.cn

PHP:  $value = $data ?? "默认值";
来源：http://pit.uphjek.com

JS:   const value = data ?? "默认值";
来源：http://yiu.cucudq.cn

TS:   const value = data ?? "默认值";
来源：http://fja.vqdsnc.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hrx.shangyingyoupin.top

Go:   if data == "" { data = "默认值" }
来源：http://sfa.sjlbkw.cn

Ruby: value = data || "默认值"
来源：http://nel.xuanzx.com

C#:   var value = data ?? "默认值";
来源：http://wzf.cqqwz.cn

[A16] 真假值判断规则
来源：http://ocs.jlsjyb.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xwl.ehwqpu.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ekt.guannengcc.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lxm.yj202588.top

TS:   if (!x) {}
来源：http://ysc.yj202588.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mzj.jinyuanbaomall.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bjy.jianghu66.top

Ruby: unless x            # nil 与 false 为假
来源：http://lru.mhx1999.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jcr.9152youxi.cn

[A17] 位运算
来源：http://yxd.haohaochexian.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qkj.yuxming.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://huz.yuxming.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ako.zhaomingkeji.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://atm.jyoumei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mwn.hysaishi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sek.52xcode.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kzz.gogol.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tjt.fzhhl.top

[A18] 字符与 ASCII 码互转
来源：http://fom.cdnleiting.top

Py:   ord("A"); chr(65)
来源：http://gkd.ywan-chungtsiang.top

PHP:  ord("A"); chr(65)
来源：http://rjl.uphjek.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ouz.yuxming.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gfr.ivvv.top

Java: (int) 'A'; (char) 65
来源：http://idu.bjfxy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xgz.nwbrower.top

Ruby: "A".ord; 65.chr
来源：http://ulx.52xcode.cn

C#:   (int)'A'; (char)65
来源：http://huc.xinyue.icu

[A19] 交换两个变量
来源：http://prn.dashuyun.cn

Py:   a, b = b, a
来源：http://yfd.uphjek.com

PHP:  [$a, $b] = [$b, $a];
来源：http://jjc.daxiang520.top

JS:   [a, b] = [b, a];
来源：http://qke.guannengcc.top

TS:   [a, b] = [b, a];
来源：http://clm.hammf.cn

Java: int t = a; a = b; b = t;
来源：http://rva.ehwqpu.com

Go:   a, b = b, a
来源：http://dfj.aizwys.cn

Ruby: a, b = b, a
来源：http://bmq.ydzc1.top

C#:   (a, b) = (b, a);
来源：http://jqf.fzhhl.top

[A20] 读取标准输入
来源：http://yzi.xinyue.icu

Py:   name = input("请输入：")
来源：http://dbs.jinqigfzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qru.hcnkem.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://twq.xziqi.cn

TS:   // Node.js：readline 模块
来源：http://qob.c1oappe.top

Java: new Scanner(System.in).nextLine()
来源：http://fje.fzhhl.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ynd.aibaodan.cn

Ruby: gets.chomp
来源：http://hjq.nwbrower.top

C#:   Console.ReadLine();
来源：http://lcz.jiagoushi.top

[A21] 保留指定小数位输出
来源：http://rxm.zhengqikj.top

Py:   f"{3.14159:.2f}"
来源：http://auz.xuanzx.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://irt.chenjidiqi.icu

JS:   (3.14159).toFixed(2)
来源：http://fpe.xinyue.icu

TS:   (3.14159).toFixed(2)
来源：http://spt.tarul.cn

Java: String.format("%.2f", 3.14159)
来源：http://qfj.jqgufenzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yxm.jinqigufen.top

Ruby: format("%.2f", 3.14159)
来源：http://bye.bjfxy.top

C#:   3.14159.ToString("F2")
来源：http://gtz.guannengcc.top

[A22] 获取字符串长度
来源：http://yzm.zhongyouzk.top

Py:   len(s)
来源：http://arx.chenlongwang.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vil.chenjidiqi.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rlj.316326.xyz

TS:   s.length
来源：http://ngj.mhx1999.top

Java: s.length()
来源：http://zop.aibaodan.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jfa.c1oappe.top

Ruby: s.length
来源：http://hmn.sysykeji.top

C#:   s.Length
来源：http://xre.svipenyu.cn

[A23] 大小写转换
来源：http://dcv.hesvh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ckt.zhiwuduotai.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://opm.mhx1999.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rhk.zycfv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yov.gzhubu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xhj.tianlin.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://icq.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://orb.hfpthk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tvz.chenlongwang.top

[A24] 去除首尾空白
来源：http://wsg.cdnleiting.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zal.zhoulong.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gel.snrcjt.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://njv.tarul.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uam.jinqigufen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xuz.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://bio.tarul.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wgv.hongshengwenyu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xau.jqgufenzy.top

[A25] 字符串比较
来源：http://bzq.aibaodan.cn

Py:   s1 == s2; s1 != s2
来源：http://sxf.yj20258.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bsg.pengpengdd.cyou

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dxv.yangfankeji.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gjj.zycfv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wvv.zycfv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://icg.dashuyun.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rds.hongshengwenyu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mpa.pycfn.com

[A26] 类型转换总览
来源：http://fdk.sweek.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tvq.meibo888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fui.yuanzhike.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wbe.vehdjk.com

TS:   Number() String() Boolean() x as number
来源：http://dsv.wangdashe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xwc.mhx1999.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gjg.wangshuangyany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lmi.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vfh.jyoumei.cn

================================================================================
来源：http://kcd.jyoumei.cn

B. 流程控制
来源：http://rfv.feifeiyinyue.top

================================================================================
来源：http://qvb.hywenlv.cn

[B01] 条件判断 if / else
来源：http://sxy.zhiwuduotai.top

Py:   result = "正" if x > 0 else "非正"
来源：http://uih.cheryme.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fbj.chenjidiqi.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rtd.birdmap.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://foa.nwbrower.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mou.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gqb.daria6918.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://avw.aibaodan.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sak.jqgufenzy.top

[B02] 多分支 else if / elif
来源：http://lbc.ydzc1.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fhd.cashguo.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bag.hongshengwenyu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zjt.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bmo.zhiwuduotai.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ruk.fanxiaobao.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xxu.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rgr.guannengcc.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://acl.jinghuilouyu.cn

[B03] switch / match / case
来源：http://dul.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rqu.sufxvd.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sju.feifeiyinyue.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gll.hnqzz.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mhk.zdqjudy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ovz.shuidangran.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cii.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tta.jinghuilouyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nbj.chenlongwang.top

[B04] for 计数循环
来源：http://jcy.tian-w.cn

Py:   for i in range(10): print(i)
来源：http://cpc.aibaodan.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kee.jianghu66.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qdp.ivvv.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jzc.yongpay.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xtv.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tzm.tian-w.cn

Ruby: 10.times { |i| puts i }
来源：http://zek.sufxvd.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ukn.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://lri.shanyushiyangkeji.top

Py:   for item in arr: print(item)
来源：http://rdd.xuetiantiany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mho.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vfd.hammf.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uxe.jqgfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uhw.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lis.0kj1m.cn

Ruby: arr.each { |item| puts item }
来源：http://abf.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jqg.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://wlr.zhengqikj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lvg.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://osb.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ekf.sufxvd.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://csh.52xcode.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nct.hnxiangtu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fst.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://arr.gzhubu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bml.iojbl.cn

[B07] while 循环
来源：http://dwh.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://aes.jqgfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://vhr.jyoumei.cn

JS:   while (i < 10) { i++; }
来源：http://rfd.yj20258.top

TS:   while (i < 10) { i++; }
来源：http://cus.wangdashe.top

Java: while (i < 10) { i++; }
来源：http://abv.9152youxi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ubp.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://bqw.bbcook.cn

C#:   while (i < 10) { i++; }
来源：http://zch.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://bak.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://ins.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ujw.dianchejie.cn

JS:   do { i++; } while (i < 10);
来源：http://eju.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://pcs.sjlbkw.cn

Java: do { i++; } while (i < 10);
来源：http://pzl.xingfuxueyuan.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://att.yvedp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bgj.vqdsnc.cn

C#:   do { i++; } while (i < 10);
来源：http://dbc.zhixingplan.top

[B09] break 与 continue
来源：http://cge.sufxvd.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://czg.quarkkingdee.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://flf.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://esb.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://evi.iojbl.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tes.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iti.hammf.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pkg.xingfuxueyuan.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ukd.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://npv.ydzc1.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jbj.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jlk.ehwqpu.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://goi.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fxf.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fqt.cheryme.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lgc.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hyz.vehdjk.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cym.gotoacloud.top

[B11] 生成数字序列 / 区间
来源：http://ihr.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://aku.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://dmw.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wyf.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ggn.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vok.jlsjyb.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sty.yonumen.top

Ruby: (0...10).step(2).to_a
来源：http://isv.xingfuxueyuan.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iyt.hcnkem.com

[B12] 跳出多层循环
来源：http://isz.fktsv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fll.zhoulong.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://enn.zhoulong.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hzj.chenlongwang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wrq.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jir.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gva.jinqigfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vmw.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wgb.xziqi.cn

[B13] 判断是否为数字
来源：http://gud.dashuyun.cn

Py:   isinstance(x, (int, float))
来源：http://xze.fanxiaobao.xyz

PHP:  is_numeric($x)
来源：http://lks.tarul.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kjv.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hgv.ppjwa.cn

Java: x instanceof Number
来源：http://mys.cucudq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wby.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://byp.redwolf501.top

C#:   x is int or double or decimal
来源：http://vle.nwbrower.top

[B14] 判断值是否在集合内
来源：http://kvj.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ppi.birdmap.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cnz.nanxinkj.top

JS:   [1, 2, 3].includes(x)
来源：http://pct.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://hsr.wangdashe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lyj.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://edb.svipenyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ncb.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tkl.wangdashe.top

[B15] 布尔运算与取反
来源：http://vgp.ywan-chungtsiang.top

Py:   a and b or not c
来源：http://kcq.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://usm.hnqzz.top

JS:   a && b || !c
来源：http://nob.fanxiaobao.xyz

TS:   a && b || !c
来源：http://bel.cashguo.top

Java: a && b || !c
来源：http://gih.shzxlz.cn

Go:   a && b || !c
来源：http://vom.ywan-chungtsiang.top

Ruby: a && b || !c
来源：http://eso.ehwqpu.com

C#:   a && b || !c
来源：http://sze.hnxiangtu.top

[B16] 卫语句：不满足条件提前返回
来源：http://evk.quarkkingdee.top

Py:   if not data: return
来源：http://yhb.smart0.xyz

PHP:  if (!$data) { return; }
来源：http://tqy.yuanzhike.top

JS:   if (!data) return;
来源：http://syd.hnxiangtu.top

TS:   if (!data) return;
来源：http://ipj.hesvh.cn

Java: if (data == null) return;
来源：http://shs.vqdsnc.cn

Go:   if data == nil { return }
来源：http://fsk.hesvh.cn

Ruby: return if data.nil?
来源：http://fjf.guannengcc.top

C#:   if (data == null) return;
来源：http://daz.yj202588.top

================================================================================
来源：http://hpl.yanxiufei.cn

C. 函数与作用域
来源：http://uab.shangyingyoupin.top

================================================================================
来源：http://vze.aizwys.cn

[C01] 定义函数
来源：http://dvm.andypj.xyz

Py:   def add(a, b): return a + b
来源：http://wlg.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qad.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://pqw.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ogg.quarkkingdee.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cui.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sbe.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://evz.smart0.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yxn.kuanghao11.cn

[C02] 默认参数
来源：http://efm.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://ztx.aizwys.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dfr.zhoulong.xyz

JS:   function greet(name = "World") { return name; }
来源：http://ctk.jqgfzy.top


<!-- 参考信息 -->