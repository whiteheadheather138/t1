代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://pji.dianchejie.cn

[A11] 条件表达式（三元）
来源：http://wib.sjlbkw.cn

Py:   "yes" if x > 0 else "no"
来源：http://ord.hammf.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qha.epnwcf.com

JS:   x > 0 ? "yes" : "no"
来源：http://her.cdnleiting.top

TS:   x > 0 ? "yes" : "no"
来源：http://yrx.zdbjq.cn

Java: x > 0 ? "yes" : "no"
来源：http://zfd.chenjidiqi.icu

Go:   // 无三元运算符，需用 if 语句
来源：http://rcw.hnqzz.top

Ruby: x > 0 ? "yes" : "no"
来源：http://bou.guannengcc.top

C#:   x > 0 ? "yes" : "no"
来源：http://ytv.ydzc1.top

[A12] 字符串插值 / 格式化
来源：http://grb.hcnkem.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mzc.hesvh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ogj.iojbl.cn

JS:   `Hello, ${name}!`
来源：http://rkx.xingfuxueyuan.xyz

TS:   `Hello, ${name}!`
来源：http://ako.shangyingyoupin.top

Java: "Hello, %s!".formatted(name)
来源：http://dcy.yuxming.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bhn.jqgufenzy.top

Ruby: "Hello, #{name}!"
来源：http://tsk.zhijiandao.cn

C#:   $"Hello, {name}!"
来源：http://qze.xuanzx.com

[A13] 多行字符串（练习 \n 转义）
来源：http://lop.vehdjk.com

Py:   "第一行\n第二行"
来源：http://nfg.hammf.cn

PHP:  "第一行\n第二行"
来源：http://sil.hnxiangtu.top

JS:   "第一行\n第二行"
来源：http://nlr.wangdashe.top

TS:   "第一行\n第二行"
来源：http://yqs.yueranfly.top

Java: "第一行\n第二行"
来源：http://awn.jiagoushi.top

Go:   "第一行\n第二行"
来源：http://udo.zhoulong.xyz

Ruby: "第一行\n第二行"
来源：http://agp.cdnleiting.top

C#:   "第一行\n第二行"
来源：http://rew.316326.xyz

[A14] 注释写法
来源：http://vaq.zhongyouzk.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xgj.hysaishi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kev.xylfe.cn

JS:   // 单行；/* 多行 */
来源：http://ysw.iojbl.cn

TS:   // 单行；/* 多行 */
来源：http://uls.ydzc1.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pfh.yj20258888.top

Go:   // 单行；/* 多行 */
来源：http://ozg.dashuyun.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bfo.xylfe.cn

C#:   // 单行；/* 多行 */
来源：http://gqo.shuidangran.top

[A15] 空值判断与默认值
来源：http://xck.yangfankeji.com

Py:   value = data or "默认值"
来源：http://rmo.fktsv.cn

PHP:  $value = $data ?? "默认值";
来源：http://fhq.sweek.top

JS:   const value = data ?? "默认值";
来源：http://zfo.jlsjyb.cn

TS:   const value = data ?? "默认值";
来源：http://blj.yj20258.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://noi.cashguo.top

Go:   if data == "" { data = "默认值" }
来源：http://dlg.gzhubu.top

Ruby: value = data || "默认值"
来源：http://lxe.cucudq.cn

C#:   var value = data ?? "默认值";
来源：http://nvm.shanyushiyangkeji.top

[A16] 真假值判断规则
来源：http://rzy.cqqwz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lcd.xuetiantiany.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qkb.c1oappe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://elw.yj20258.top

TS:   if (!x) {}
来源：http://bxg.cashguo.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yzr.xylfe.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mdu.sysykeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://kii.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vtp.fzhhl.top

[A17] 位运算
来源：http://tlg.yfazqb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tge.epnwcf.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dfz.tianlin.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gju.cucudq.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fws.jinghuilouyu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tjz.andypj.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qtv.sxryk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zqm.aizwys.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dia.ivvv.top

[A18] 字符与 ASCII 码互转
来源：http://edw.guannengcc.top

Py:   ord("A"); chr(65)
来源：http://xrn.yvedp.cn

PHP:  ord("A"); chr(65)
来源：http://eax.quarkkingdee.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uoi.bjfxy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gsv.jqgfzy.top

Java: (int) 'A'; (char) 65
来源：http://zkl.nwbrower.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yao.fanxiaobao.xyz

Ruby: "A".ord; 65.chr
来源：http://toh.yongpay.top

C#:   (int)'A'; (char)65
来源：http://ile.jianghu66.top

[A19] 交换两个变量
来源：http://eor.52xcode.cn

Py:   a, b = b, a
来源：http://kmh.shangyingyoupin.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jfo.xingfuxueyuan.xyz

JS:   [a, b] = [b, a];
来源：http://msf.zhiwuduotai.top

TS:   [a, b] = [b, a];
来源：http://ljv.yanxiufei.cn

Java: int t = a; a = b; b = t;
来源：http://onc.zhixingplan.top

Go:   a, b = b, a
来源：http://has.jiagoushi.top

Ruby: a, b = b, a
来源：http://kpj.hammf.cn

C#:   (a, b) = (b, a);
来源：http://zjw.epnwcf.com

[A20] 读取标准输入
来源：http://hra.snrcjt.cn

Py:   name = input("请输入：")
来源：http://pcf.hesvh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lld.epnwcf.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zkg.ywan-chungtsiang.top

TS:   // Node.js：readline 模块
来源：http://wri.yonumen.top

Java: new Scanner(System.in).nextLine()
来源：http://dsx.ydzc1.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ijk.c1oappe.top

Ruby: gets.chomp
来源：http://fut.jianghu66.top

C#:   Console.ReadLine();
来源：http://gpu.ydjk.org.cn

[A21] 保留指定小数位输出
来源：http://sug.zhongyouzk.top

Py:   f"{3.14159:.2f}"
来源：http://igd.ydzc1.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wyb.daxiang520.top

JS:   (3.14159).toFixed(2)
来源：http://wcw.hysaishi.cn

TS:   (3.14159).toFixed(2)
来源：http://jex.guowangkeji.top

Java: String.format("%.2f", 3.14159)
来源：http://bkx.hesvh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cem.hammf.cn

Ruby: format("%.2f", 3.14159)
来源：http://uzh.fzhhl.top

C#:   3.14159.ToString("F2")
来源：http://zou.havefunace.top

[A22] 获取字符串长度
来源：http://gor.fengsongda.top

Py:   len(s)
来源：http://ukz.jqgfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rvz.kuanghao11.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uvx.xylfe.cn

TS:   s.length
来源：http://qsv.xziqi.cn

Java: s.length()
来源：http://nti.yangfankeji.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fyg.yangfankeji.com

Ruby: s.length
来源：http://zge.jinghuilouyu.cn

C#:   s.Length
来源：http://pqr.fzhhl.top

[A23] 大小写转换
来源：http://kch.hesvh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ukp.zhaomingkeji.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mmp.vqdsnc.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vgq.yanxiufei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mmt.daria6918.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qor.tarul.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hye.daria6918.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://krj.yfazqb.com

C#:   s.ToUpper(); s.ToLower()
来源：http://iak.nanxinkj.top

[A24] 去除首尾空白
来源：http://sej.fengsongda.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nkc.zhoulong.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://shk.xingfuxueyuan.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://let.bjfxy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hhl.yueranfly.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tgd.jlsjyb.cn

Go:   strings.TrimSpace(s)
来源：http://umd.iojbl.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ifg.hammf.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qvg.gzhubu.top

[A25] 字符串比较
来源：http://oez.hnxiangtu.top

Py:   s1 == s2; s1 != s2
来源：http://cdb.ydzc1.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nmj.shzxlz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zzw.fzhhl.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jum.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://emx.ydjk.org.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hoc.jinyuanbaomall.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eyw.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://csz.jyoumei.cn

[A26] 类型转换总览
来源：http://cjs.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cuv.havefunace.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lpf.yj20258.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hij.jiagoushi.top

TS:   Number() String() Boolean() x as number
来源：http://pxg.ybcxt.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tfi.zdbjq.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wtj.dashuyun.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ooi.jinyuanbaomall.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bod.tianlin.xyz

================================================================================
来源：http://ize.ehwqpu.com

B. 流程控制
来源：http://req.kuanghao11.cn

================================================================================
来源：http://oiw.316326.xyz

[B01] 条件判断 if / else
来源：http://mjz.ydjk.org.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://glw.jyoumei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zit.cucudq.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://avt.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fto.guannengcc.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qvl.kuanghao11.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nge.cdnleiting.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tei.yj20258888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dpu.cqqwz.cn

[B02] 多分支 else if / elif
来源：http://lvg.xziqi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qyu.tianlin.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eka.chenjidiqi.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iay.jqgufenzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://okx.pycfn.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://faz.xuetiantiany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://she.yanxiufei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kma.yongpay.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kxy.gzhubu.top

[B03] switch / match / case
来源：http://umn.fehbvm.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xlw.fzhhl.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xzc.snrcjt.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ivf.hywenlv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kbn.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uos.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gth.shuidangran.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ram.shangyingyoupin.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mof.gotoacloud.top

[B04] for 计数循环
来源：http://pam.52xcode.cn

Py:   for i in range(10): print(i)
来源：http://xup.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ses.sysykeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lkv.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://plp.xuanzx.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qhv.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://evd.xuetiantiany.cn

Ruby: 10.times { |i| puts i }
来源：http://yra.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ybo.pengpengdd.cyou

[B05] 遍历数组 / 列表
来源：http://yuv.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://ure.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ich.yuxming.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vja.zhaomingkeji.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://omj.yj20258888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cwb.gzhubu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://crn.xziqi.cn

Ruby: arr.each { |item| puts item }
来源：http://okz.jqgfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wib.yuxming.cn

[B06] 遍历字典 / 对象
来源：http://vsb.haohaochexian.top

Py:   for k, v in d.items(): print(k, v)
来源：http://iap.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yls.cashguo.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cnq.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tau.sweek.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tuh.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tpj.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://crj.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zyf.fengsongda.top

[B07] while 循环
来源：http://lvk.zhixingplan.top

Py:   while i < 10: i += 1
来源：http://zic.daria6918.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xdb.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://xmb.hongshengwenyu.top

TS:   while (i < 10) { i++; }
来源：http://wee.xingfuxueyuan.xyz

Java: while (i < 10) { i++; }
来源：http://dek.yongpay.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sii.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://usr.chenlongwang.top

C#:   while (i < 10) { i++; }
来源：http://lsz.jianghu66.top

[B08] do-while（至少执行一次）
来源：http://rxi.vehdjk.com

Py:   # 无 do-while：用 while True + break
来源：http://zcp.quarkkingdee.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rwj.yongpay.top

JS:   do { i++; } while (i < 10);
来源：http://iop.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://myq.yanxiufei.cn

Java: do { i++; } while (i < 10);
来源：http://sds.gotoacloud.top

Go:   for { i++; if i >= 10 { break } }
来源：http://sgs.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://fzp.zdbjq.cn

C#:   do { i++; } while (i < 10);
来源：http://qju.jinqigufen.top

[B09] break 与 continue
来源：http://jgn.xuetiantiany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ufa.zhijiandao.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rxw.shangyingyoupin.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fip.xuanzx.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bgn.epnwcf.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hgs.yvedp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sbe.ctjpmb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://apw.chenlongwang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://urd.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://fkd.hysaishi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://avw.jlsjyb.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nrm.zhixingplan.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tce.jlsjyb.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pkw.hammf.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wet.cdnleiting.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zsr.hywenlv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sjb.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://plb.zhijiandao.cn

[B11] 生成数字序列 / 区间
来源：http://vwc.jqgufenzy.top

Py:   list(range(0, 10, 2))
来源：http://fax.sweek.top

PHP:  range(0, 10, 2);
来源：http://qtx.snrcjt.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kxj.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dqe.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fbp.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dfk.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://scu.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zar.9152youxi.cn

[B12] 跳出多层循环
来源：http://nkz.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pol.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bdx.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ttu.vqdsnc.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hhj.yj20258.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tno.cdnleiting.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ker.birdmap.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ood.fanxiaobao.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nax.jinghuilouyu.cn

[B13] 判断是否为数字
来源：http://jnx.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://tmb.zhongyouzk.top

PHP:  is_numeric($x)
来源：http://cql.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ugs.ppjwa.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cel.zhijiandao.cn

Java: x instanceof Number
来源：http://cic.jinqigufen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gan.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://aai.pycfn.com

C#:   x is int or double or decimal
来源：http://jse.hfpthk.cn

[B14] 判断值是否在集合内
来源：http://nno.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xbm.gzhubu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kic.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://lvx.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://nqt.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yyj.birdmap.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yih.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://hvz.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tdv.zycfv.cn

[B15] 布尔运算与取反
来源：http://jpe.feifeiyinyue.top

Py:   a and b or not c
来源：http://kcm.hfpthk.cn

PHP:  $a && $b || !$c
来源：http://fwa.yvedp.cn

JS:   a && b || !c
来源：http://eky.sysykeji.top

TS:   a && b || !c
来源：http://zot.meibo888.top

Java: a && b || !c
来源：http://ftb.daria6918.cn

Go:   a && b || !c
来源：http://qsf.feifeiyinyue.top

Ruby: a && b || !c
来源：http://gso.yj20258888.top

C#:   a && b || !c
来源：http://pvr.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://pnz.fanxiaobao.xyz

Py:   if not data: return
来源：http://cbl.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://amy.zhijiandao.cn

JS:   if (!data) return;
来源：http://qsu.sufxvd.cn

TS:   if (!data) return;
来源：http://vmt.svipenyu.cn

Java: if (data == null) return;
来源：http://jgf.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://bno.yuxming.cn

Ruby: return if data.nil?
来源：http://eux.jinqigufen.top

C#:   if (data == null) return;
来源：http://hok.hammf.cn

================================================================================
来源：http://xni.52xcode.cn

C. 函数与作用域
来源：http://cvi.fengsongda.top

================================================================================
来源：http://qiz.xuetiantiany.cn

[C01] 定义函数
来源：http://kyt.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://wtm.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tzb.daxiang520.top

JS:   function add(a, b) { return a + b; }
来源：http://iik.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eyx.wangshuangyany.cn


<!-- 参考信息 -->