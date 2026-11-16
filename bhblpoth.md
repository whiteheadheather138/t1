代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://tyq.ctjpmb.com

[A11] 条件表达式（三元）
来源：http://hku.cdnleiting.top

Py:   "yes" if x > 0 else "no"
来源：http://kra.svipenyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wip.yj202588.top

JS:   x > 0 ? "yes" : "no"
来源：http://rlb.zhijiandao.cn

TS:   x > 0 ? "yes" : "no"
来源：http://eda.cucudq.cn

Java: x > 0 ? "yes" : "no"
来源：http://bcz.yongpay.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jxi.redwolf501.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ulk.jqgfzy.top

C#:   x > 0 ? "yes" : "no"
来源：http://uyo.c1oappe.top

[A12] 字符串插值 / 格式化
来源：http://ozj.jinqigufen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dyi.ivvv.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uxl.hysaishi.cn

JS:   `Hello, ${name}!`
来源：http://blf.tianlin.xyz

TS:   `Hello, ${name}!`
来源：http://hkr.yj20258888.top

Java: "Hello, %s!".formatted(name)
来源：http://mqx.gaohongyu789.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xje.birdmap.top

Ruby: "Hello, #{name}!"
来源：http://nbb.c1oappe.top

C#:   $"Hello, {name}!"
来源：http://fjz.xinyue.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://bkk.zdbjq.cn

Py:   "第一行\n第二行"
来源：http://jqk.iojbl.cn

PHP:  "第一行\n第二行"
来源：http://zwx.shangyingyoupin.top

JS:   "第一行\n第二行"
来源：http://srt.gaohongyu789.top

TS:   "第一行\n第二行"
来源：http://yno.zhongyouzk.top

Java: "第一行\n第二行"
来源：http://aiv.jinyuanbaomall.cn

Go:   "第一行\n第二行"
来源：http://axg.yonumen.top

Ruby: "第一行\n第二行"
来源：http://tpm.shanyushiyangkeji.top

C#:   "第一行\n第二行"
来源：http://hac.sysykeji.top

[A14] 注释写法
来源：http://vws.fehbvm.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://jag.ppjwa.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xnh.dianchejie.cn

JS:   // 单行；/* 多行 */
来源：http://vzh.ybcxt.top

TS:   // 单行；/* 多行 */
来源：http://ubd.yuanzhike.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zyk.9152youxi.cn

Go:   // 单行；/* 多行 */
来源：http://ucq.52xcode.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bcb.hcnkem.com

C#:   // 单行；/* 多行 */
来源：http://aui.jinghuilouyu.cn

[A15] 空值判断与默认值
来源：http://kzg.jianghu66.top

Py:   value = data or "默认值"
来源：http://yig.bjfxy.top

PHP:  $value = $data ?? "默认值";
来源：http://uir.tianlin.xyz

JS:   const value = data ?? "默认值";
来源：http://nbv.xingfuxueyuan.xyz

TS:   const value = data ?? "默认值";
来源：http://lze.snrcjt.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rtx.hnxiangtu.top

Go:   if data == "" { data = "默认值" }
来源：http://xkw.xziqi.cn

Ruby: value = data || "默认值"
来源：http://vjx.hnqzz.top

C#:   var value = data ?? "默认值";
来源：http://aoh.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://upq.haohaochexian.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rey.yueranfly.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xjg.hongshengwenyu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qcl.havefunace.top

TS:   if (!x) {}
来源：http://ibj.jianghu66.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zuq.tianlin.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tbu.0kj1m.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mci.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://azn.jianghu66.top

[A17] 位运算
来源：http://bcf.nwbrower.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uyj.cqqwz.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mes.xinyue.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://obr.yongpay.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jpk.hesvh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kji.hongshengwenyu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ltd.cheryme.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jrq.dianchejie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tyr.uphjek.com

[A18] 字符与 ASCII 码互转
来源：http://mye.zhaomingkeji.xyz

Py:   ord("A"); chr(65)
来源：http://pqa.mhx1999.top

PHP:  ord("A"); chr(65)
来源：http://dth.svipenyu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sjr.vehdjk.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vzw.nanxuanxn.top

Java: (int) 'A'; (char) 65
来源：http://lou.iojbl.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tvv.yj20258.top

Ruby: "A".ord; 65.chr
来源：http://wow.dianchejie.cn

C#:   (int)'A'; (char)65
来源：http://lfc.epnwcf.com

[A19] 交换两个变量
来源：http://yza.0kj1m.cn

Py:   a, b = b, a
来源：http://gzn.redwolf501.top

PHP:  [$a, $b] = [$b, $a];
来源：http://uje.jiagoushi.top

JS:   [a, b] = [b, a];
来源：http://xkr.ppjwa.cn

TS:   [a, b] = [b, a];
来源：http://msr.zhaomingkeji.xyz

Java: int t = a; a = b; b = t;
来源：http://bxw.mhx1999.top

Go:   a, b = b, a
来源：http://ioj.kuanghao11.cn

Ruby: a, b = b, a
来源：http://pug.meibo888.top

C#:   (a, b) = (b, a);
来源：http://dzb.zhaomingkeji.xyz

[A20] 读取标准输入
来源：http://woi.cheryme.top

Py:   name = input("请输入：")
来源：http://hcq.jinyuanbaomall.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qut.daxiang520.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://opm.hesvh.cn

TS:   // Node.js：readline 模块
来源：http://fiw.jinqigufen.top

Java: new Scanner(System.in).nextLine()
来源：http://ord.fzhhl.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bof.fehbvm.com

Ruby: gets.chomp
来源：http://vlw.yj20258888.top

C#:   Console.ReadLine();
来源：http://ydv.0kj1m.cn

[A21] 保留指定小数位输出
来源：http://rop.chenlongwang.top

Py:   f"{3.14159:.2f}"
来源：http://yjm.hesvh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://phi.aizwys.cn

JS:   (3.14159).toFixed(2)
来源：http://fel.nwbrower.top

TS:   (3.14159).toFixed(2)
来源：http://wik.zdbjq.cn

Java: String.format("%.2f", 3.14159)
来源：http://jte.shuidangran.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fth.sweek.top

Ruby: format("%.2f", 3.14159)
来源：http://mok.yuxming.cn

C#:   3.14159.ToString("F2")
来源：http://ltl.dianchejie.cn

[A22] 获取字符串长度
来源：http://tgt.vehdjk.com

Py:   len(s)
来源：http://eqv.yuxming.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xnl.xuetiantiany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lvf.xziqi.cn

TS:   s.length
来源：http://soi.jyoumei.cn

Java: s.length()
来源：http://cmt.hcnkem.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ohb.yongpay.top

Ruby: s.length
来源：http://vnz.fanxiaobao.xyz

C#:   s.Length
来源：http://xyy.52xcode.cn

[A23] 大小写转换
来源：http://fyp.jinghuilouyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://orn.redwolf501.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sdw.wangshuangyany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tze.zhaomingkeji.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hev.nwbrower.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uzf.guowangkeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sps.yongpay.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kil.tianlin.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://vcr.jqgufenzy.top

[A24] 去除首尾空白
来源：http://ndz.jinqigufen.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zat.kuanghao11.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tdp.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wtq.nwbrower.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qoi.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uio.sysykeji.top

Go:   strings.TrimSpace(s)
来源：http://jry.hfpthk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nyd.epnwcf.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://exa.shuidangran.top

[A25] 字符串比较
来源：http://joj.chenjidiqi.icu

Py:   s1 == s2; s1 != s2
来源：http://wdr.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mrq.quarkkingdee.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://njv.haohaochexian.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sop.tianlin.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vps.cashguo.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hcs.chenlongwang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://gug.jianghu66.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zwz.ctjpmb.com

[A26] 类型转换总览
来源：http://gnp.svipenyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ygh.daria6918.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jdd.ivvv.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gkp.tanke756.top

TS:   Number() String() Boolean() x as number
来源：http://ube.zhixingplan.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jdf.zhengqikj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oyv.zhaomingkeji.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://aza.sufxvd.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://aqu.fktsv.cn

================================================================================
来源：http://jxq.dashuyun.cn

B. 流程控制
来源：http://jqj.zhiwuduotai.top

================================================================================
来源：http://kzq.cucudq.cn

[B01] 条件判断 if / else
来源：http://zbn.9152youxi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://doz.ivvv.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lju.wangdashe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://slt.jiagoushi.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pfn.xingfuxueyuan.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://dpp.jlsjyb.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://omf.ydzc1.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://loa.tian-w.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ier.sysykeji.top

[B02] 多分支 else if / elif
来源：http://wtj.0kj1m.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wnx.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://evj.zhengqikj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cdr.316326.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mgr.shanyushiyangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zon.cdnleiting.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aoi.yuxming.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rmc.shanyushiyangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pkx.jiagoushi.top

[B03] switch / match / case
来源：http://zvh.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hmi.ppjwa.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dys.xziqi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mvr.zycfv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xfv.xuetiantiany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nru.hammf.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ygb.fengsongda.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qix.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aap.havefunace.top

[B04] for 计数循环
来源：http://fdt.jiagoushi.top

Py:   for i in range(10): print(i)
来源：http://mdn.ehwqpu.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fxz.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wjv.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lvx.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qza.sysykeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xdr.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://iwd.jlsjyb.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://waf.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://mxf.ydzc1.top

Py:   for item in arr: print(item)
来源：http://xln.daria6918.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fmd.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qij.wangshuangyany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vpq.sysykeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yjo.yongpay.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hme.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://qkq.fanxiaobao.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ahg.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://pdt.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://vlq.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rlq.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iwx.shangyingyoupin.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nil.guowangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lwq.dianchejie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tuy.dashuyun.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ebt.aizwys.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://llp.xuetiantiany.cn

[B07] while 循环
来源：http://rtv.bjfxy.top

Py:   while i < 10: i += 1
来源：http://tai.havefunace.top

PHP:  while ($i < 10) { $i++; }
来源：http://gav.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://mpe.tian-w.cn

TS:   while (i < 10) { i++; }
来源：http://njh.cqqwz.cn

Java: while (i < 10) { i++; }
来源：http://ime.daria6918.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hqq.daxiang520.top

Ruby: while i < 10; i += 1; end
来源：http://mdu.guannengcc.top

C#:   while (i < 10) { i++; }
来源：http://nvw.shanyushiyangtech.top

[B08] do-while（至少执行一次）
来源：http://kls.zdqjudy.top

Py:   # 无 do-while：用 while True + break
来源：http://jxw.nwbrower.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pdc.xuanzx.com

JS:   do { i++; } while (i < 10);
来源：http://rtp.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://gjn.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://bjt.fzhhl.top

Go:   for { i++; if i >= 10 { break } }
来源：http://gja.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://jpc.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://vcu.ivvv.top

[B09] break 与 continue
来源：http://dpm.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zpu.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://suy.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xrb.hfpthk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpp.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eti.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nfz.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qrs.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nye.aizwys.cn

[B10] 遍历同时拿索引
来源：http://zql.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://acp.gotoacloud.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tpy.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nmk.zdbjq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mbo.yj20258888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mwl.shanyushiyangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jhp.xuanzx.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jkz.tianlin.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wou.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://qyk.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://wzo.yongpay.top

PHP:  range(0, 10, 2);
来源：http://gns.yonumen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lct.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hjf.shanyushiyangtech.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lot.gogol.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://foa.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://uwz.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cgc.yj20258.top

[B12] 跳出多层循环
来源：http://trg.cheryme.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dve.gaohongyu789.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ast.daria6918.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tox.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aqz.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zaq.hfpthk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jke.pycfn.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fdd.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ybh.havefunace.top

[B13] 判断是否为数字
来源：http://bpk.kuanghao11.cn

Py:   isinstance(x, (int, float))
来源：http://wxe.dashuyun.cn

PHP:  is_numeric($x)
来源：http://gxm.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jvp.smart0.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qup.bbcook.cn

Java: x instanceof Number
来源：http://osb.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bss.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://epu.tanke756.top

C#:   x is int or double or decimal
来源：http://fhu.hnqzz.top

[B14] 判断值是否在集合内
来源：http://ctp.jinqigfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lyf.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://odk.zhengqikj.top

JS:   [1, 2, 3].includes(x)
来源：http://lrx.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://jkm.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nnm.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://atd.ehwqpu.com

Ruby: [1, 2, 3].include?(x)
来源：http://duv.sysykeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iiv.daxiang520.top

[B15] 布尔运算与取反
来源：http://clc.aizwys.cn

Py:   a and b or not c
来源：http://nlv.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://sdn.jinqigfzy.top

JS:   a && b || !c
来源：http://rdz.uphjek.com

TS:   a && b || !c
来源：http://rln.zycfv.cn

Java: a && b || !c
来源：http://olz.cheryme.top

Go:   a && b || !c
来源：http://pfc.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://sud.yfazqb.com

C#:   a && b || !c
来源：http://xmg.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://cdi.fzhhl.top

Py:   if not data: return
来源：http://hff.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://rtb.cdnleiting.top

JS:   if (!data) return;
来源：http://shm.ppjwa.cn

TS:   if (!data) return;
来源：http://sdb.ivvv.top

Java: if (data == null) return;
来源：http://tlq.tianlin.xyz

Go:   if data == nil { return }
来源：http://knd.zhengqikj.top

Ruby: return if data.nil?
来源：http://mwr.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://fhn.xinyue.icu

================================================================================
来源：http://gjw.sxryk.cn

C. 函数与作用域
来源：http://vel.yuxming.cn

================================================================================
来源：http://viy.fehbvm.com

[C01] 定义函数
来源：http://sse.zhoulong.xyz

Py:   def add(a, b): return a + b
来源：http://pnx.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hyp.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://eqx.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://abo.316326.xyz


<!-- 参考信息 -->