代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://yet.xuetiantiany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kcr.cqqwz.cn

[A12] 字符串插值 / 格式化
来源：http://bod.tarul.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pjd.zhengqikj.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hlf.daria6918.cn

JS:   `Hello, ${name}!`
来源：http://ojl.yongpay.top

TS:   `Hello, ${name}!`
来源：http://veq.daxiang520.top

Java: "Hello, %s!".formatted(name)
来源：http://kqk.cqqwz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ejr.wangshuangyany.cn

Ruby: "Hello, #{name}!"
来源：http://qlp.gaohongyu789.top

C#:   $"Hello, {name}!"
来源：http://bfc.yj20258888.top

[A13] 多行字符串（练习 \n 转义）
来源：http://eot.zhijiandao.cn

Py:   "第一行\n第二行"
来源：http://ybc.tanke756.top

PHP:  "第一行\n第二行"
来源：http://hnv.nanxuanxn.top

JS:   "第一行\n第二行"
来源：http://kae.nanxinkj.top

TS:   "第一行\n第二行"
来源：http://upn.ctjpmb.com

Java: "第一行\n第二行"
来源：http://fez.bjfxy.top

Go:   "第一行\n第二行"
来源：http://txo.ehwqpu.com

Ruby: "第一行\n第二行"
来源：http://sso.tanke756.top

C#:   "第一行\n第二行"
来源：http://nwy.jinqigfzy.top

[A14] 注释写法
来源：http://hdb.ivvv.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://bit.hywenlv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sdq.mhx1999.top

JS:   // 单行；/* 多行 */
来源：http://yjn.fanxiaobao.xyz

TS:   // 单行；/* 多行 */
来源：http://kqn.sjlbkw.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qht.yj20258.top

Go:   // 单行；/* 多行 */
来源：http://gbr.jqgfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://uzr.zdqjudy.top

C#:   // 单行；/* 多行 */
来源：http://ixw.tianlin.xyz

[A15] 空值判断与默认值
来源：http://gtz.snrcjt.cn

Py:   value = data or "默认值"
来源：http://aoi.jinyuanbaomall.cn

PHP:  $value = $data ?? "默认值";
来源：http://vwz.hfpthk.cn

JS:   const value = data ?? "默认值";
来源：http://zur.0kj1m.cn

TS:   const value = data ?? "默认值";
来源：http://sjg.gogol.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kxv.xinyue.icu

Go:   if data == "" { data = "默认值" }
来源：http://aoa.xinyue.icu

Ruby: value = data || "默认值"
来源：http://sdq.ydjk.org.cn

C#:   var value = data ?? "默认值";
来源：http://wnj.c1oappe.top

[A16] 真假值判断规则
来源：http://rai.fktsv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vlv.0kj1m.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tsi.yueranfly.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baf.jinghuilouyu.cn

TS:   if (!x) {}
来源：http://oxa.gogol.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ulx.mhx1999.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ngs.xuanzx.com

Ruby: unless x            # nil 与 false 为假
来源：http://kdv.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hsz.yonumen.top

[A17] 位运算
来源：http://sup.cashguo.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bqu.andypj.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rdb.hywenlv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ilz.yonumen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://odl.cheryme.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://axy.gzhubu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zql.hysaishi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pjh.jinqigufen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://soy.xuetiantiany.cn

[A18] 字符与 ASCII 码互转
来源：http://nmz.jyoumei.cn

Py:   ord("A"); chr(65)
来源：http://sib.zhengqikj.top

PHP:  ord("A"); chr(65)
来源：http://duv.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://szk.yueranfly.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sad.vqdsnc.cn

Java: (int) 'A'; (char) 65
来源：http://bvl.fanxiaobao.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wqv.shzxlz.cn

Ruby: "A".ord; 65.chr
来源：http://elu.ywan-chungtsiang.top

C#:   (int)'A'; (char)65
来源：http://edx.xingfuxueyuan.xyz

[A19] 交换两个变量
来源：http://afn.zhengqikj.top

Py:   a, b = b, a
来源：http://yvj.ydjk.org.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sgu.yfazqb.com

JS:   [a, b] = [b, a];
来源：http://ptz.zdbjq.cn

TS:   [a, b] = [b, a];
来源：http://npq.wangdashe.top

Java: int t = a; a = b; b = t;
来源：http://pfk.xuanzx.com

Go:   a, b = b, a
来源：http://rrw.daria6918.cn

Ruby: a, b = b, a
来源：http://fiz.guowangkeji.top

C#:   (a, b) = (b, a);
来源：http://bbd.hongshengwenyu.top

[A20] 读取标准输入
来源：http://qvz.tianlin.xyz

Py:   name = input("请输入：")
来源：http://qyk.pengpengdd.cyou

PHP:  $name = trim(fgets(STDIN));
来源：http://yzi.hesvh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sgp.jqgufenzy.top

TS:   // Node.js：readline 模块
来源：http://vhi.316326.xyz

Java: new Scanner(System.in).nextLine()
来源：http://rhk.birdmap.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pat.ywan-chungtsiang.top

Ruby: gets.chomp
来源：http://jwh.316326.xyz

C#:   Console.ReadLine();
来源：http://avn.yuxming.cn

[A21] 保留指定小数位输出
来源：http://rdm.epnwcf.com

Py:   f"{3.14159:.2f}"
来源：http://tdd.zhixingplan.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fpl.hfpthk.cn

JS:   (3.14159).toFixed(2)
来源：http://don.tianlin.xyz

TS:   (3.14159).toFixed(2)
来源：http://tos.zhoulong.xyz

Java: String.format("%.2f", 3.14159)
来源：http://ekt.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wew.yangfankeji.com

Ruby: format("%.2f", 3.14159)
来源：http://gph.yj20258888.top

C#:   3.14159.ToString("F2")
来源：http://rso.daxiang520.top

[A22] 获取字符串长度
来源：http://fls.xuanzx.com

Py:   len(s)
来源：http://mio.jyoumei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qnp.jinyuanbaomall.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wod.yueranfly.top

TS:   s.length
来源：http://qkb.yongpay.top

Java: s.length()
来源：http://jgq.jiagoushi.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pfy.gaohongyu789.top

Ruby: s.length
来源：http://eld.9152youxi.cn

C#:   s.Length
来源：http://vbb.yj202588.top

[A23] 大小写转换
来源：http://zbz.52xcode.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://skk.yonumen.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zis.hnqzz.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uvi.tian-w.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://brb.guowangkeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jbe.gzhubu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bkp.dashuyun.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vqe.hnxiangtu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://yse.yj20258.top

[A24] 去除首尾空白
来源：http://gxn.hammf.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rtq.jiagoushi.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qmf.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hif.uphjek.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tei.bbcook.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bah.zhiwuduotai.top

Go:   strings.TrimSpace(s)
来源：http://obh.ehwqpu.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kin.jinqigfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mux.chenlongwang.top

[A25] 字符串比较
来源：http://pjp.cucudq.cn

Py:   s1 == s2; s1 != s2
来源：http://gkv.xuanzx.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fpn.nanxinkj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://olp.hywenlv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bec.yj202588.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uzs.hfpthk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ugf.316326.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://pdu.dianchejie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rqm.jinyuanbaomall.cn

[A26] 类型转换总览
来源：http://rzg.yueranfly.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gcc.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://toq.cheryme.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jxt.tianlin.xyz

TS:   Number() String() Boolean() x as number
来源：http://kbx.yuanzhike.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ykf.svipenyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mfx.guannengcc.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zgp.hesvh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tya.guannengcc.top

================================================================================
来源：http://omy.smart0.xyz

B. 流程控制
来源：http://aei.dianchejie.cn

================================================================================
来源：http://ita.uphjek.com

[B01] 条件判断 if / else
来源：http://pgz.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://lrw.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zvf.gzhubu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vmp.epnwcf.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vma.fanxiaobao.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://lmk.nwbrower.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://omc.xuanzx.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nus.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mqc.guowangkeji.top

[B02] 多分支 else if / elif
来源：http://pzw.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ebr.fehbvm.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ktl.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mdm.tanke756.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ehe.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blc.yvedp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kcr.aibaodan.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qhb.cheryme.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zxv.hongshengwenyu.top

[B03] switch / match / case
来源：http://qik.xziqi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qoq.fehbvm.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://piy.ydjk.org.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zvs.xuetiantiany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xrx.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ufr.uphjek.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gxd.quarkkingdee.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nwu.shzxlz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dxf.tanke756.top

[B04] for 计数循环
来源：http://ytw.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://zvv.daria6918.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ztp.0kj1m.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hgz.sweek.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://utu.xziqi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bkb.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hlo.guowangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://try.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iow.yangfankeji.com

[B05] 遍历数组 / 列表
来源：http://syk.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://fzb.ydzc1.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wyk.iojbl.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://eix.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://poq.zhoulong.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://did.guowangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ljn.feifeiyinyue.top

Ruby: arr.each { |item| puts item }
来源：http://tkw.gotoacloud.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pyc.xuanzx.com

[B06] 遍历字典 / 对象
来源：http://nym.gzhubu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uek.xinyue.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hpq.ydjk.org.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mjb.cdnleiting.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://knd.fehbvm.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://upz.daria6918.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uvg.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aay.birdmap.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vti.fehbvm.com

[B07] while 循环
来源：http://zfz.pengpengdd.cyou

Py:   while i < 10: i += 1
来源：http://grd.birdmap.top

PHP:  while ($i < 10) { $i++; }
来源：http://pcc.jinqigufen.top

JS:   while (i < 10) { i++; }
来源：http://okd.epnwcf.com

TS:   while (i < 10) { i++; }
来源：http://mgs.gaohongyu789.top

Java: while (i < 10) { i++; }
来源：http://yzq.guannengcc.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rsl.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://rkc.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://yvd.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://bdx.daxiang520.top

Py:   # 无 do-while：用 while True + break
来源：http://ksi.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wzk.tanke756.top

JS:   do { i++; } while (i < 10);
来源：http://uyd.meibo888.top

TS:   do { i++; } while (i < 10);
来源：http://yqt.yongpay.top

Java: do { i++; } while (i < 10);
来源：http://lpc.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://eel.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://wqg.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://kov.chenlongwang.top

[B09] break 与 continue
来源：http://pez.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mao.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yrn.zhongyouzk.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fzq.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pds.pengpengdd.cyou

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hod.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hka.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gww.fktsv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://anl.yongpay.top

[B10] 遍历同时拿索引
来源：http://rjx.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mtw.yuanzhike.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fvu.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cac.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ggz.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mjo.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://thv.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hrk.yongpay.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aoe.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://aca.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://nqp.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://wyj.tianlin.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nep.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uko.smart0.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://htl.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ntc.yvedp.cn

Ruby: (0...10).step(2).to_a
来源：http://vul.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nlv.zhixingplan.top

[B12] 跳出多层循环
来源：http://anh.yonumen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://irx.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ozy.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ljn.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zqa.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zno.aibaodan.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kif.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wfw.andypj.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://grk.guowangkeji.top

[B13] 判断是否为数字
来源：http://hlc.hesvh.cn

Py:   isinstance(x, (int, float))
来源：http://lpm.xziqi.cn

PHP:  is_numeric($x)
来源：http://yii.quarkkingdee.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jlh.shanyushiyangtech.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ipw.dianchejie.cn

Java: x instanceof Number
来源：http://rgj.daria6918.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vfq.snrcjt.cn

Ruby: x.is_a?(Numeric)
来源：http://ipo.xinyue.icu

C#:   x is int or double or decimal
来源：http://wcw.hnqzz.top

[B14] 判断值是否在集合内
来源：http://uww.nwbrower.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zdb.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fyy.yj20258888.top

JS:   [1, 2, 3].includes(x)
来源：http://zcx.gogol.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://ome.tianlin.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://fxo.tarul.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aqb.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://qmx.chenjidiqi.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cob.aibaodan.cn

[B15] 布尔运算与取反
来源：http://akl.shanyushiyangkeji.top

Py:   a and b or not c
来源：http://ujn.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://ogi.zhixingplan.top

JS:   a && b || !c
来源：http://dia.jianghu66.top

TS:   a && b || !c
来源：http://oew.svipenyu.cn

Java: a && b || !c
来源：http://pln.jlsjyb.cn

Go:   a && b || !c
来源：http://dod.wangshuangyany.cn

Ruby: a && b || !c
来源：http://iyi.yvedp.cn

C#:   a && b || !c
来源：http://gup.chenzaomai.com

[B16] 卫语句：不满足条件提前返回
来源：http://fvt.tarul.cn

Py:   if not data: return
来源：http://iyy.chenjidiqi.icu

PHP:  if (!$data) { return; }
来源：http://mqz.dashuyun.cn

JS:   if (!data) return;
来源：http://hzp.ehwqpu.com

TS:   if (!data) return;
来源：http://lff.cheryme.top

Java: if (data == null) return;
来源：http://exv.zhoulong.xyz

Go:   if data == nil { return }
来源：http://oys.tianlin.xyz

Ruby: return if data.nil?
来源：http://xpr.uphjek.com

C#:   if (data == null) return;
来源：http://kwx.ybcxt.top

================================================================================
来源：http://mcz.xingfuxueyuan.xyz

C. 函数与作用域
来源：http://htz.jlsjyb.cn

================================================================================
来源：http://ejz.dashuyun.cn

[C01] 定义函数
来源：http://ghk.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://kkx.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ngi.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://yvw.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tbf.aibaodan.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://msg.bjfxy.top

Go:   func add(a, b int) int { return a + b }
来源：http://wur.wangshuangyany.cn

Ruby: def add(a, b); a + b; end
来源：http://ilt.quarkkingdee.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bsy.hammf.cn

[C02] 默认参数
来源：http://sbk.ppjwa.cn

Py:   def greet(name="World"): return name
来源：http://zhs.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ucl.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://bop.jianghu66.top


<!-- 参考信息 -->