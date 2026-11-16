代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://pkg.snrcjt.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rhv.kuanghao11.cn

Java: x > 0 ? "yes" : "no"
来源：http://xco.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vno.havefunace.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ads.sysykeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://fff.daria6918.cn

[A12] 字符串插值 / 格式化
来源：http://lhi.havefunace.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hgu.zhiwuduotai.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bja.jlsjyb.cn

JS:   `Hello, ${name}!`
来源：http://irc.zhiwuduotai.top

TS:   `Hello, ${name}!`
来源：http://tkz.hesvh.cn

Java: "Hello, %s!".formatted(name)
来源：http://hqh.zhixingplan.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bei.shuidangran.top

Ruby: "Hello, #{name}!"
来源：http://zgc.ybcxt.top

C#:   $"Hello, {name}!"
来源：http://tyw.shanyushiyangtech.top

[A13] 多行字符串（练习 \n 转义）
来源：http://diw.dashuyun.cn

Py:   "第一行\n第二行"
来源：http://nea.shuidangran.top

PHP:  "第一行\n第二行"
来源：http://jgc.zdbjq.cn

JS:   "第一行\n第二行"
来源：http://skh.kuanghao11.cn

TS:   "第一行\n第二行"
来源：http://fhj.yueranfly.top

Java: "第一行\n第二行"
来源：http://zcf.zhijiandao.cn

Go:   "第一行\n第二行"
来源：http://vxy.pycfn.com

Ruby: "第一行\n第二行"
来源：http://txk.yonumen.top

C#:   "第一行\n第二行"
来源：http://fye.jyoumei.cn

[A14] 注释写法
来源：http://jyw.vqdsnc.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://czh.cdnleiting.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://boa.ydzc1.top

JS:   // 单行；/* 多行 */
来源：http://lxk.shanyushiyangtech.top

TS:   // 单行；/* 多行 */
来源：http://fwv.hongshengwenyu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rlu.shanyushiyangkeji.top

Go:   // 单行；/* 多行 */
来源：http://vju.fengsongda.top

Ruby: # 单行；=begin 多行 =end
来源：http://ocd.jinyuanbaomall.cn

C#:   // 单行；/* 多行 */
来源：http://tlv.sufxvd.cn

[A15] 空值判断与默认值
来源：http://uzy.tianlin.xyz

Py:   value = data or "默认值"
来源：http://dku.hysaishi.cn

PHP:  $value = $data ?? "默认值";
来源：http://fqy.xuetiantiany.cn

JS:   const value = data ?? "默认值";
来源：http://pri.ybcxt.top

TS:   const value = data ?? "默认值";
来源：http://jwk.fengsongda.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://iwh.hywenlv.cn

Go:   if data == "" { data = "默认值" }
来源：http://lfg.aizwys.cn

Ruby: value = data || "默认值"
来源：http://yvz.fktsv.cn

C#:   var value = data ?? "默认值";
来源：http://bia.gaohongyu789.top

[A16] 真假值判断规则
来源：http://isv.tianlin.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qvr.xylfe.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://opx.hnqzz.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dnc.chenlongwang.top

TS:   if (!x) {}
来源：http://kfh.ehwqpu.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sse.cheryme.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qos.svipenyu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xyh.sysykeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ani.zdqjudy.top

[A17] 位运算
来源：http://dto.zhongyouzk.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sob.zdbjq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://veb.yfazqb.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wos.cashguo.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://axr.sweek.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://laf.fengsongda.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sxm.yongpay.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lrd.sxryk.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tpe.meibo888.top

[A18] 字符与 ASCII 码互转
来源：http://jur.zhixingplan.top

Py:   ord("A"); chr(65)
来源：http://xvf.jianghu66.top

PHP:  ord("A"); chr(65)
来源：http://bdv.jinqigufen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://riq.sjlbkw.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fhd.svipenyu.cn

Java: (int) 'A'; (char) 65
来源：http://xfs.jinqigufen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ied.xuetiantiany.cn

Ruby: "A".ord; 65.chr
来源：http://sja.yanxiufei.cn

C#:   (int)'A'; (char)65
来源：http://cbf.uphjek.com

[A19] 交换两个变量
来源：http://rqu.fehbvm.com

Py:   a, b = b, a
来源：http://soj.xuanzx.com

PHP:  [$a, $b] = [$b, $a];
来源：http://vba.shzxlz.cn

JS:   [a, b] = [b, a];
来源：http://fvk.jinyuanbaomall.cn

TS:   [a, b] = [b, a];
来源：http://vjc.jianghu66.top

Java: int t = a; a = b; b = t;
来源：http://qwb.jinghuilouyu.cn

Go:   a, b = b, a
来源：http://xsi.bjfxy.top

Ruby: a, b = b, a
来源：http://dsh.sjlbkw.cn

C#:   (a, b) = (b, a);
来源：http://ydv.ivvv.top

[A20] 读取标准输入
来源：http://xkj.xziqi.cn

Py:   name = input("请输入：")
来源：http://osq.yangfankeji.com

PHP:  $name = trim(fgets(STDIN));
来源：http://zkj.yj20258.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mpa.316326.xyz

TS:   // Node.js：readline 模块
来源：http://ndl.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://rij.bbcook.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xtj.daria6918.cn

Ruby: gets.chomp
来源：http://ktk.wangdashe.top

C#:   Console.ReadLine();
来源：http://rcz.sysykeji.top

[A21] 保留指定小数位输出
来源：http://bty.guowangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://jgf.zhixingplan.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zet.gzhubu.top

JS:   (3.14159).toFixed(2)
来源：http://phg.ybcxt.top

TS:   (3.14159).toFixed(2)
来源：http://wrq.yj20258.top

Java: String.format("%.2f", 3.14159)
来源：http://ber.jlsjyb.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rcg.kuanghao11.cn

Ruby: format("%.2f", 3.14159)
来源：http://thv.pengpengdd.cyou

C#:   3.14159.ToString("F2")
来源：http://apc.fzhhl.top

[A22] 获取字符串长度
来源：http://rlc.xylfe.cn

Py:   len(s)
来源：http://daj.dashuyun.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nbm.xylfe.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mfb.pengpengdd.cyou

TS:   s.length
来源：http://lja.mhx1999.top

Java: s.length()
来源：http://abr.jinyuanbaomall.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eyr.jinqigfzy.top

Ruby: s.length
来源：http://klg.zhijiandao.cn

C#:   s.Length
来源：http://lbv.smart0.xyz

[A23] 大小写转换
来源：http://fsm.haohaochexian.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gxz.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rus.pengpengdd.cyou

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pgd.yuxming.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cnb.yonumen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://laq.tian-w.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ncx.shuidangran.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oqq.nanxuanxn.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gpw.yfazqb.com

[A24] 去除首尾空白
来源：http://wjh.uphjek.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lih.quarkkingdee.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zrk.havefunace.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rqu.jqgufenzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://glc.birdmap.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wjm.aibaodan.cn

Go:   strings.TrimSpace(s)
来源：http://nmm.wangshuangyany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yqd.fzhhl.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gub.yanxiufei.cn

[A25] 字符串比较
来源：http://zos.gzhubu.top

Py:   s1 == s2; s1 != s2
来源：http://hjx.jlsjyb.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://spr.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://der.gaohongyu789.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uro.zhijiandao.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gsy.fanxiaobao.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wsu.yuxming.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bif.chenjidiqi.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fzd.dianchejie.cn

[A26] 类型转换总览
来源：http://ixw.fanxiaobao.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dwj.yonumen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yiz.andypj.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pzw.daxiang520.top

TS:   Number() String() Boolean() x as number
来源：http://ged.epnwcf.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gzw.kuanghao11.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xdj.jyoumei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://anx.yj202588.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hmw.cucudq.cn

================================================================================
来源：http://piy.316326.xyz

B. 流程控制
来源：http://ndp.havefunace.top

================================================================================
来源：http://eeu.hnqzz.top

[B01] 条件判断 if / else
来源：http://gld.pengpengdd.cyou

Py:   result = "正" if x > 0 else "非正"
来源：http://jpe.zhiwuduotai.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jbj.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ngb.cheryme.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sti.dianchejie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qxo.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rem.zhongyouzk.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pqo.redwolf501.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://egl.snrcjt.cn

[B02] 多分支 else if / elif
来源：http://abl.zhoulong.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rps.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yjg.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://btn.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://puy.zhengqikj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbb.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uca.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ohr.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hgo.wangdashe.top

[B03] switch / match / case
来源：http://yfr.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vcd.9152youxi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wkz.aibaodan.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dgt.shangyingyoupin.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ofc.cashguo.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dcx.uphjek.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ktn.cashguo.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fch.9152youxi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ktv.redwolf501.top

[B04] for 计数循环
来源：http://wfo.yvedp.cn

Py:   for i in range(10): print(i)
来源：http://zjd.sufxvd.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vba.zhiwuduotai.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yri.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kbi.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vfo.aizwys.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wuc.zhongyouzk.top

Ruby: 10.times { |i| puts i }
来源：http://xuw.yj20258.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sdq.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://mke.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://vmf.ivvv.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://teg.shanyushiyangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qdt.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lgp.snrcjt.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ohq.dashuyun.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ofl.tian-w.cn

Ruby: arr.each { |item| puts item }
来源：http://wnu.jlsjyb.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://chl.9152youxi.cn

[B06] 遍历字典 / 对象
来源：http://ack.dianchejie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wzn.yangfankeji.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://woj.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dys.xingfuxueyuan.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fwe.andypj.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cmt.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://anr.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pes.hammf.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iik.jianghu66.top

[B07] while 循环
来源：http://owp.guowangkeji.top

Py:   while i < 10: i += 1
来源：http://dwv.c1oappe.top

PHP:  while ($i < 10) { $i++; }
来源：http://bhb.bbcook.cn

JS:   while (i < 10) { i++; }
来源：http://yww.hcnkem.com

TS:   while (i < 10) { i++; }
来源：http://nhy.jqgufenzy.top

Java: while (i < 10) { i++; }
来源：http://tgj.jiagoushi.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ydn.feifeiyinyue.top

Ruby: while i < 10; i += 1; end
来源：http://cxx.jinghuilouyu.cn

C#:   while (i < 10) { i++; }
来源：http://umr.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://lfl.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://ewn.zhiwuduotai.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ico.shangyingyoupin.top

JS:   do { i++; } while (i < 10);
来源：http://alu.daria6918.cn

TS:   do { i++; } while (i < 10);
来源：http://lua.xuanzx.com

Java: do { i++; } while (i < 10);
来源：http://xhs.hfpthk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uca.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fkx.ybcxt.top

C#:   do { i++; } while (i < 10);
来源：http://tng.ehwqpu.com

[B09] break 与 continue
来源：http://rzc.smart0.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://osw.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wrt.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lyb.jinghuilouyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xed.tarul.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xdx.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mqn.zdqjudy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rxq.xziqi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eqp.redwolf501.top

[B10] 遍历同时拿索引
来源：http://oiw.cashguo.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wzz.zhiwuduotai.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sie.ywan-chungtsiang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://otf.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dsj.hcnkem.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fid.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fpy.fzhhl.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fib.yj20258888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xit.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://byj.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://biq.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://obl.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yxi.yfazqb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kph.yvedp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oms.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wrl.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://gpc.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oxt.zhongyouzk.top

[B12] 跳出多层循环
来源：http://hib.zhengqikj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://knr.daxiang520.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bji.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://otr.316326.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tmw.xuanzx.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mae.nanxuanxn.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ttr.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bsx.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zze.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://gft.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://rnk.gzhubu.top

PHP:  is_numeric($x)
来源：http://psg.tianlin.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jbf.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fix.zhongyouzk.top

Java: x instanceof Number
来源：http://tsk.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mae.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://dzj.nanxuanxn.top

C#:   x is int or double or decimal
来源：http://wls.yuxming.cn

[B14] 判断值是否在集合内
来源：http://zck.havefunace.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dlu.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zev.kuanghao11.cn

JS:   [1, 2, 3].includes(x)
来源：http://ivh.zhongyouzk.top

TS:   [1, 2, 3].includes(x)
来源：http://ffi.ivvv.top

Java: List.of(1, 2, 3).contains(x)
来源：http://aux.pycfn.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uzi.hywenlv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wnv.wangshuangyany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oww.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://wnh.cheryme.top

Py:   a and b or not c
来源：http://hsw.ppjwa.cn

PHP:  $a && $b || !$c
来源：http://ghn.uphjek.com

JS:   a && b || !c
来源：http://wzy.yj20258.top

TS:   a && b || !c
来源：http://hsu.bbcook.cn

Java: a && b || !c
来源：http://kjk.0kj1m.cn

Go:   a && b || !c
来源：http://phr.tianlin.xyz

Ruby: a && b || !c
来源：http://lay.52xcode.cn

C#:   a && b || !c
来源：http://nfi.ydjk.org.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sot.nanxuanxn.top

Py:   if not data: return
来源：http://ggb.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://mps.aizwys.cn

JS:   if (!data) return;
来源：http://kvr.fanxiaobao.xyz

TS:   if (!data) return;
来源：http://xgd.hywenlv.cn

Java: if (data == null) return;
来源：http://qlq.hammf.cn

Go:   if data == nil { return }
来源：http://oxd.dianchejie.cn

Ruby: return if data.nil?
来源：http://ceq.ybcxt.top

C#:   if (data == null) return;
来源：http://zif.chenjidiqi.icu

================================================================================
来源：http://ups.mhx1999.top

C. 函数与作用域
来源：http://icg.epnwcf.com

================================================================================
来源：http://vqe.316326.xyz

[C01] 定义函数
来源：http://jbs.xingfuxueyuan.xyz

Py:   def add(a, b): return a + b
来源：http://hbt.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cyj.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://lmp.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://olk.nwbrower.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ggd.pycfn.com

Go:   func add(a, b int) int { return a + b }
来源：http://cza.fanxiaobao.xyz

Ruby: def add(a, b); a + b; end
来源：http://boz.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rbe.zycfv.cn


<!-- 参考信息 -->