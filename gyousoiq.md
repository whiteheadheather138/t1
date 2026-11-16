代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://kan.chenzaomai.com

C#:   x > 0 ? "yes" : "no"
来源：http://wub.smart0.xyz

[A12] 字符串插值 / 格式化
来源：http://ygz.meibo888.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hjb.daxiang520.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xgz.birdmap.top

JS:   `Hello, ${name}!`
来源：http://hxl.fzhhl.top

TS:   `Hello, ${name}!`
来源：http://vbx.316326.xyz

Java: "Hello, %s!".formatted(name)
来源：http://kju.cdnleiting.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ueh.zdqjudy.top

Ruby: "Hello, #{name}!"
来源：http://nrz.tanke756.top

C#:   $"Hello, {name}!"
来源：http://vww.hongshengwenyu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://srr.wangdashe.top

Py:   "第一行\n第二行"
来源：http://bby.pengpengdd.cyou

PHP:  "第一行\n第二行"
来源：http://hjv.ppjwa.cn

JS:   "第一行\n第二行"
来源：http://bys.bjfxy.top

TS:   "第一行\n第二行"
来源：http://loz.zhiwuduotai.top

Java: "第一行\n第二行"
来源：http://syg.pycfn.com

Go:   "第一行\n第二行"
来源：http://bqn.bbcook.cn

Ruby: "第一行\n第二行"
来源：http://ecp.jinghuilouyu.cn

C#:   "第一行\n第二行"
来源：http://bxw.quarkkingdee.top

[A14] 注释写法
来源：http://odw.feifeiyinyue.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rpz.ydjk.org.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ipn.shzxlz.cn

JS:   // 单行；/* 多行 */
来源：http://pyt.jinqigufen.top

TS:   // 单行；/* 多行 */
来源：http://gkt.yfazqb.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bzd.jqgfzy.top

Go:   // 单行；/* 多行 */
来源：http://gco.yuxming.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vxz.yj20258.top

C#:   // 单行；/* 多行 */
来源：http://juj.jinqigufen.top

[A15] 空值判断与默认值
来源：http://hga.jianghu66.top

Py:   value = data or "默认值"
来源：http://qnr.hammf.cn

PHP:  $value = $data ?? "默认值";
来源：http://nrj.xuetiantiany.cn

JS:   const value = data ?? "默认值";
来源：http://chg.pycfn.com

TS:   const value = data ?? "默认值";
来源：http://qrn.jqgfzy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fvc.wangdashe.top

Go:   if data == "" { data = "默认值" }
来源：http://vyo.gogol.net.cn

Ruby: value = data || "默认值"
来源：http://rwo.yongpay.top

C#:   var value = data ?? "默认值";
来源：http://apw.9152youxi.cn

[A16] 真假值判断规则
来源：http://quv.jinqigfzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lxo.yuanzhike.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nsa.hesvh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://anc.chenlongwang.top

TS:   if (!x) {}
来源：http://txc.9152youxi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ora.zdbjq.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gom.pengpengdd.cyou

Ruby: unless x            # nil 与 false 为假
来源：http://ala.cheryme.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oxe.yueranfly.top

[A17] 位运算
来源：http://bin.zhaomingkeji.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lqh.vqdsnc.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wzv.jinghuilouyu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ymd.aibaodan.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qlu.shangyingyoupin.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://unk.jianghu66.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dtd.hnxiangtu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mgy.meibo888.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dea.xuanzx.com

[A18] 字符与 ASCII 码互转
来源：http://njl.chenzaomai.com

Py:   ord("A"); chr(65)
来源：http://uhs.xziqi.cn

PHP:  ord("A"); chr(65)
来源：http://sfh.wangshuangyany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jpe.fanxiaobao.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xhf.hesvh.cn

Java: (int) 'A'; (char) 65
来源：http://kuz.vqdsnc.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pzf.yvedp.cn

Ruby: "A".ord; 65.chr
来源：http://dbl.gogol.net.cn

C#:   (int)'A'; (char)65
来源：http://vuq.yfazqb.com

[A19] 交换两个变量
来源：http://dvz.fzhhl.top

Py:   a, b = b, a
来源：http://lvg.cashguo.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ebp.yj20258.top

JS:   [a, b] = [b, a];
来源：http://ses.gzhubu.top

TS:   [a, b] = [b, a];
来源：http://aqr.52xcode.cn

Java: int t = a; a = b; b = t;
来源：http://ufd.aizwys.cn

Go:   a, b = b, a
来源：http://eup.wangshuangyany.cn

Ruby: a, b = b, a
来源：http://vkf.guannengcc.top

C#:   (a, b) = (b, a);
来源：http://khd.vqdsnc.cn

[A20] 读取标准输入
来源：http://tre.pycfn.com

Py:   name = input("请输入：")
来源：http://eqz.hesvh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gyk.yonumen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://awr.aizwys.cn

TS:   // Node.js：readline 模块
来源：http://dwv.sufxvd.cn

Java: new Scanner(System.in).nextLine()
来源：http://btv.pycfn.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hks.quarkkingdee.top

Ruby: gets.chomp
来源：http://eht.shanyushiyangtech.top

C#:   Console.ReadLine();
来源：http://jii.fehbvm.com

[A21] 保留指定小数位输出
来源：http://zlp.zycfv.cn

Py:   f"{3.14159:.2f}"
来源：http://xcz.zhiwuduotai.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://azd.ehwqpu.com

JS:   (3.14159).toFixed(2)
来源：http://pzb.bbcook.cn

TS:   (3.14159).toFixed(2)
来源：http://ain.fengsongda.top

Java: String.format("%.2f", 3.14159)
来源：http://skd.snrcjt.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ruw.yanxiufei.cn

Ruby: format("%.2f", 3.14159)
来源：http://ykp.zhaomingkeji.xyz

C#:   3.14159.ToString("F2")
来源：http://rqd.hywenlv.cn

[A22] 获取字符串长度
来源：http://lxu.fktsv.cn

Py:   len(s)
来源：http://rjy.feifeiyinyue.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://obx.zhijiandao.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yqc.nanxinkj.top

TS:   s.length
来源：http://fnd.smart0.xyz

Java: s.length()
来源：http://rvi.aibaodan.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sea.cqqwz.cn

Ruby: s.length
来源：http://msj.tarul.cn

C#:   s.Length
来源：http://gam.hfpthk.cn

[A23] 大小写转换
来源：http://hjt.hnqzz.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ens.ydzc1.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://soy.yuanzhike.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nsd.mhx1999.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kvt.xziqi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ngl.aibaodan.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://acf.yfazqb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fnl.chenlongwang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dgq.zycfv.cn

[A24] 去除首尾空白
来源：http://dju.sufxvd.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://neg.ppjwa.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gtr.jqgufenzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kao.fktsv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://svd.ivvv.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bgj.ctjpmb.com

Go:   strings.TrimSpace(s)
来源：http://noe.jinqigufen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rnu.zhijiandao.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tqk.redwolf501.top

[A25] 字符串比较
来源：http://mip.jyoumei.cn

Py:   s1 == s2; s1 != s2
来源：http://tes.havefunace.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ctp.jinyuanbaomall.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ygf.cucudq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nno.yuanzhike.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://utb.dashuyun.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ezt.cdnleiting.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tjh.fengsongda.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kne.hesvh.cn

[A26] 类型转换总览
来源：http://wzm.zhixingplan.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dvk.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://trr.birdmap.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gap.jyoumei.cn

TS:   Number() String() Boolean() x as number
来源：http://zdj.0kj1m.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rbu.zycfv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nha.feifeiyinyue.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vhj.0kj1m.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zfi.cashguo.top

================================================================================
来源：http://dgj.ydzc1.top

B. 流程控制
来源：http://rlb.dianchejie.cn

================================================================================
来源：http://zox.yangfankeji.com

[B01] 条件判断 if / else
来源：http://ila.zhaomingkeji.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://jyh.sufxvd.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://agm.ivvv.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://npq.xinyue.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gzc.xinyue.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://obs.xuetiantiany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cjt.yj202588.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lrt.yj202588.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nyz.tianlin.xyz

[B02] 多分支 else if / elif
来源：http://bei.epnwcf.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://omp.chenjidiqi.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nah.cdnleiting.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ihf.birdmap.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zad.hywenlv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bxp.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qmb.wangshuangyany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ixg.yanxiufei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://giw.tarul.cn

[B03] switch / match / case
来源：http://nfu.ehwqpu.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ltj.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yck.nwbrower.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fgh.yuxming.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jzp.iojbl.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mlf.mhx1999.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hne.zhiwuduotai.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://koo.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xhg.zhongyouzk.top

[B04] for 计数循环
来源：http://get.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://vms.chenzaomai.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ecq.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://opl.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ufm.tian-w.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gql.9152youxi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rut.vqdsnc.cn

Ruby: 10.times { |i| puts i }
来源：http://ajb.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bhj.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://azl.ywan-chungtsiang.top

Py:   for item in arr: print(item)
来源：http://vhj.ybcxt.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dfw.andypj.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://jkg.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hwz.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gle.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nwb.cqqwz.cn

Ruby: arr.each { |item| puts item }
来源：http://tjz.jlsjyb.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hxe.yuxming.cn

[B06] 遍历字典 / 对象
来源：http://htd.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sqd.smart0.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://asa.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zts.0kj1m.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://czl.aibaodan.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ezb.chenlongwang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jro.guannengcc.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zrc.jianghu66.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ham.yj202588.top

[B07] while 循环
来源：http://dyb.hywenlv.cn

Py:   while i < 10: i += 1
来源：http://aze.uphjek.com

PHP:  while ($i < 10) { $i++; }
来源：http://svl.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://axe.haohaochexian.top

TS:   while (i < 10) { i++; }
来源：http://kic.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://yzu.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vxv.cucudq.cn

Ruby: while i < 10; i += 1; end
来源：http://thz.shanyushiyangkeji.top

C#:   while (i < 10) { i++; }
来源：http://qxa.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://sep.svipenyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://toz.xziqi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sis.daxiang520.top

JS:   do { i++; } while (i < 10);
来源：http://zck.yj202588.top

TS:   do { i++; } while (i < 10);
来源：http://pni.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://lmg.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ttm.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://djq.shanyushiyangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://tge.fktsv.cn

[B09] break 与 continue
来源：http://pnr.smart0.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zmm.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jxr.guowangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://npi.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yxz.kuanghao11.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qkh.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jbg.zhiwuduotai.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pfa.nwbrower.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dhg.shanyushiyangtech.top

[B10] 遍历同时拿索引
来源：http://qam.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jag.fengsongda.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zml.xylfe.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rvb.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lre.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://apt.xziqi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cep.nanxuanxn.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sla.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dqp.sufxvd.cn

[B11] 生成数字序列 / 区间
来源：http://jtn.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://qcf.gzhubu.top

PHP:  range(0, 10, 2);
来源：http://gea.hongshengwenyu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://azt.yfazqb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xbo.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://awe.dashuyun.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bss.zycfv.cn

Ruby: (0...10).step(2).to_a
来源：http://fcf.52xcode.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rzd.epnwcf.com

[B12] 跳出多层循环
来源：http://lqd.yvedp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://aun.xuetiantiany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vep.yj20258.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ltv.yj20258888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sex.yj20258.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xoe.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wxn.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vxw.havefunace.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lyk.ydjk.org.cn

[B13] 判断是否为数字
来源：http://ebi.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://ubv.tian-w.cn

PHP:  is_numeric($x)
来源：http://udh.tian-w.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cuq.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zzq.yuanzhike.top

Java: x instanceof Number
来源：http://qwe.shuidangran.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rfe.aizwys.cn

Ruby: x.is_a?(Numeric)
来源：http://bpn.52xcode.cn

C#:   x is int or double or decimal
来源：http://bsa.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://fxm.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vtu.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mhu.sweek.top

JS:   [1, 2, 3].includes(x)
来源：http://nje.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://lqn.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nol.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hno.cheryme.top

Ruby: [1, 2, 3].include?(x)
来源：http://cau.shanyushiyangtech.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jxs.guowangkeji.top

[B15] 布尔运算与取反
来源：http://pbn.kuanghao11.cn

Py:   a and b or not c
来源：http://hhk.kuanghao11.cn

PHP:  $a && $b || !$c
来源：http://fko.zhoulong.xyz

JS:   a && b || !c
来源：http://kqs.zhoulong.xyz

TS:   a && b || !c
来源：http://sit.jlsjyb.cn

Java: a && b || !c
来源：http://ewj.daxiang520.top

Go:   a && b || !c
来源：http://gjn.hesvh.cn

Ruby: a && b || !c
来源：http://xhc.aibaodan.cn

C#:   a && b || !c
来源：http://nlg.bjfxy.top

[B16] 卫语句：不满足条件提前返回
来源：http://ger.hammf.cn

Py:   if not data: return
来源：http://xuy.sweek.top

PHP:  if (!$data) { return; }
来源：http://apm.daxiang520.top

JS:   if (!data) return;
来源：http://rzf.dashuyun.cn

TS:   if (!data) return;
来源：http://ibz.jinghuilouyu.cn

Java: if (data == null) return;
来源：http://sww.mhx1999.top

Go:   if data == nil { return }
来源：http://qqp.fengsongda.top

Ruby: return if data.nil?
来源：http://ifb.tian-w.cn

C#:   if (data == null) return;
来源：http://ecp.hesvh.cn

================================================================================
来源：http://alc.guowangkeji.top

C. 函数与作用域
来源：http://boz.zhongyouzk.top

================================================================================
来源：http://bau.sysykeji.top

[C01] 定义函数
来源：http://gxi.hfpthk.cn

Py:   def add(a, b): return a + b
来源：http://tra.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mzw.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://ezx.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vmt.zhiwuduotai.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wqc.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ddh.nanxuanxn.top

Ruby: def add(a, b); a + b; end
来源：http://tiy.jyoumei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wwh.jqgfzy.top

[C02] 默认参数
来源：http://bnq.zhijiandao.cn

Py:   def greet(name="World"): return name
来源：http://obm.ctjpmb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://tzu.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://twm.pycfn.com


<!-- 参考信息 -->