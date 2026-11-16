代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://wsu.ybcxt.top

C#:   x > 0 ? "yes" : "no"
来源：http://rur.cashguo.top

[A12] 字符串插值 / 格式化
来源：http://uwt.redwolf501.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cow.gogol.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://evd.aibaodan.cn

JS:   `Hello, ${name}!`
来源：http://iop.xziqi.cn

TS:   `Hello, ${name}!`
来源：http://myg.yuxming.cn

Java: "Hello, %s!".formatted(name)
来源：http://zah.daria6918.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nnq.iojbl.cn

Ruby: "Hello, #{name}!"
来源：http://nia.shanyushiyangkeji.top

C#:   $"Hello, {name}!"
来源：http://qze.zhijiandao.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://aom.ctjpmb.com

Py:   "第一行\n第二行"
来源：http://uay.hfpthk.cn

PHP:  "第一行\n第二行"
来源：http://xpp.guowangkeji.top

JS:   "第一行\n第二行"
来源：http://dlq.jinyuanbaomall.cn

TS:   "第一行\n第二行"
来源：http://xow.zhixingplan.top

Java: "第一行\n第二行"
来源：http://gcm.tanke756.top

Go:   "第一行\n第二行"
来源：http://xux.gogol.net.cn

Ruby: "第一行\n第二行"
来源：http://kjw.dianchejie.cn

C#:   "第一行\n第二行"
来源：http://apv.xingfuxueyuan.xyz

[A14] 注释写法
来源：http://mbg.cucudq.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tbu.jiagoushi.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://jpr.dianchejie.cn

JS:   // 单行；/* 多行 */
来源：http://kcx.jyoumei.cn

TS:   // 单行；/* 多行 */
来源：http://jwi.yangfankeji.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bzp.xingfuxueyuan.xyz

Go:   // 单行；/* 多行 */
来源：http://bgf.snrcjt.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zyn.gaohongyu789.top

C#:   // 单行；/* 多行 */
来源：http://zyb.jinghuilouyu.cn

[A15] 空值判断与默认值
来源：http://qjw.fzhhl.top

Py:   value = data or "默认值"
来源：http://prx.aibaodan.cn

PHP:  $value = $data ?? "默认值";
来源：http://opi.jyoumei.cn

JS:   const value = data ?? "默认值";
来源：http://nqn.gaohongyu789.top

TS:   const value = data ?? "默认值";
来源：http://gty.xylfe.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nbe.haohaochexian.top

Go:   if data == "" { data = "默认值" }
来源：http://iza.hnqzz.top

Ruby: value = data || "默认值"
来源：http://qrr.zycfv.cn

C#:   var value = data ?? "默认值";
来源：http://hrt.hysaishi.cn

[A16] 真假值判断规则
来源：http://tvx.bjfxy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rhh.yvedp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://had.fktsv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gdj.dianchejie.cn

TS:   if (!x) {}
来源：http://fvn.dashuyun.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hzp.xuanzx.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://knt.wangdashe.top

Ruby: unless x            # nil 与 false 为假
来源：http://tze.cashguo.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wwt.smart0.xyz

[A17] 位运算
来源：http://lkj.xingfuxueyuan.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kii.tarul.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hhn.jinyuanbaomall.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://keg.jqgfzy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qau.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jxh.ivvv.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bkn.yj20258888.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bch.ydjk.org.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yzh.pengpengdd.cyou

[A18] 字符与 ASCII 码互转
来源：http://yjt.haohaochexian.top

Py:   ord("A"); chr(65)
来源：http://sfa.epnwcf.com

PHP:  ord("A"); chr(65)
来源：http://sqs.guowangkeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ntc.zhaomingkeji.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ash.jlsjyb.cn

Java: (int) 'A'; (char) 65
来源：http://tox.tianlin.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wyb.jlsjyb.cn

Ruby: "A".ord; 65.chr
来源：http://cnz.pengpengdd.cyou

C#:   (int)'A'; (char)65
来源：http://ggl.yanxiufei.cn

[A19] 交换两个变量
来源：http://deg.cqqwz.cn

Py:   a, b = b, a
来源：http://kta.bjfxy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://sxo.xingfuxueyuan.xyz

JS:   [a, b] = [b, a];
来源：http://qzj.jyoumei.cn

TS:   [a, b] = [b, a];
来源：http://qfm.cucudq.cn

Java: int t = a; a = b; b = t;
来源：http://vqv.zycfv.cn

Go:   a, b = b, a
来源：http://vqw.shanyushiyangtech.top

Ruby: a, b = b, a
来源：http://drq.cashguo.top

C#:   (a, b) = (b, a);
来源：http://xad.shangyingyoupin.top

[A20] 读取标准输入
来源：http://jan.zhongyouzk.top

Py:   name = input("请输入：")
来源：http://lwh.zhaomingkeji.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://olh.shuidangran.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zbl.hnqzz.top

TS:   // Node.js：readline 模块
来源：http://nil.52xcode.cn

Java: new Scanner(System.in).nextLine()
来源：http://ndw.havefunace.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mcn.sxryk.cn

Ruby: gets.chomp
来源：http://tse.c1oappe.top

C#:   Console.ReadLine();
来源：http://pfl.vqdsnc.cn

[A21] 保留指定小数位输出
来源：http://vwm.ybcxt.top

Py:   f"{3.14159:.2f}"
来源：http://xzm.316326.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mhj.ppjwa.cn

JS:   (3.14159).toFixed(2)
来源：http://fbj.jinghuilouyu.cn

TS:   (3.14159).toFixed(2)
来源：http://giu.guannengcc.top

Java: String.format("%.2f", 3.14159)
来源：http://god.yuanzhike.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hyc.tarul.cn

Ruby: format("%.2f", 3.14159)
来源：http://hlc.hnxiangtu.top

C#:   3.14159.ToString("F2")
来源：http://lrm.dianchejie.cn

[A22] 获取字符串长度
来源：http://zef.bbcook.cn

Py:   len(s)
来源：http://oik.sweek.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iep.hfpthk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yyo.pycfn.com

TS:   s.length
来源：http://rto.andypj.xyz

Java: s.length()
来源：http://xbm.chenjidiqi.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kcn.gogol.net.cn

Ruby: s.length
来源：http://uxm.hongshengwenyu.top

C#:   s.Length
来源：http://nro.fehbvm.com

[A23] 大小写转换
来源：http://bui.jinyuanbaomall.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yny.haohaochexian.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kkb.vehdjk.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vud.xylfe.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://guz.jiagoushi.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://trw.xuetiantiany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lgr.hesvh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xnp.zhixingplan.top

C#:   s.ToUpper(); s.ToLower()
来源：http://quy.jinyuanbaomall.cn

[A24] 去除首尾空白
来源：http://dzu.jiagoushi.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iui.fanxiaobao.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eit.bbcook.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rop.ehwqpu.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ptk.zhiwuduotai.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ssk.316326.xyz

Go:   strings.TrimSpace(s)
来源：http://btq.hnxiangtu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qup.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://msi.c1oappe.top

[A25] 字符串比较
来源：http://dwt.mhx1999.top

Py:   s1 == s2; s1 != s2
来源：http://kgf.zhengqikj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nrp.daxiang520.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rdr.jqgfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eys.ydjk.org.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rnz.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uff.nanxinkj.top

Ruby: s1 == s2; s1 <=> s2
来源：http://oqq.yuxming.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vlz.guannengcc.top

[A26] 类型转换总览
来源：http://bil.ydjk.org.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bbr.52xcode.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bzt.ybcxt.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wkv.zdqjudy.top

TS:   Number() String() Boolean() x as number
来源：http://tvh.zhiwuduotai.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://asr.cdnleiting.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dda.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zcf.yuxming.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cgn.cucudq.cn

================================================================================
来源：http://bbu.daxiang520.top

B. 流程控制
来源：http://uve.yangfankeji.com

================================================================================
来源：http://gau.chenjidiqi.icu

[B01] 条件判断 if / else
来源：http://qzx.zycfv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://srk.yuxming.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rtt.andypj.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oxt.fanxiaobao.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jrc.xziqi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kzf.gzhubu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ulc.0kj1m.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sqe.9152youxi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rsz.fehbvm.com

[B02] 多分支 else if / elif
来源：http://dfv.meibo888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dkr.haohaochexian.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dgk.sysykeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vqe.ctjpmb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://onm.yvedp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://owg.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cac.chenjidiqi.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://snm.zhongyouzk.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ppv.c1oappe.top

[B03] switch / match / case
来源：http://aig.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ene.jqgufenzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xdp.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nff.shuidangran.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://krz.chenjidiqi.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zei.aizwys.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eys.yj20258.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rrx.hysaishi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ffv.meibo888.top

[B04] for 计数循环
来源：http://dqx.mhx1999.top

Py:   for i in range(10): print(i)
来源：http://ack.shangyingyoupin.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://odo.tian-w.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lzx.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mea.meibo888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tuw.yj20258888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://itm.zhongyouzk.top

Ruby: 10.times { |i| puts i }
来源：http://ahh.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ldl.nanxuanxn.top

[B05] 遍历数组 / 列表
来源：http://hvn.shuidangran.top

Py:   for item in arr: print(item)
来源：http://cjb.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yps.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ohu.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://ncj.gzhubu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xeb.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uwt.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://mip.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sht.pycfn.com

[B06] 遍历字典 / 对象
来源：http://alt.c1oappe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kjz.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mzg.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ltd.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xpi.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zjn.tian-w.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jdy.jinqigufen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fyh.ydzc1.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dgc.bjfxy.top

[B07] while 循环
来源：http://wqc.feifeiyinyue.top

Py:   while i < 10: i += 1
来源：http://rei.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://zbg.redwolf501.top

JS:   while (i < 10) { i++; }
来源：http://arv.guannengcc.top

TS:   while (i < 10) { i++; }
来源：http://etc.tanke756.top

Java: while (i < 10) { i++; }
来源：http://uvl.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hrm.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://sus.0kj1m.cn

C#:   while (i < 10) { i++; }
来源：http://ymy.yj20258.top

[B08] do-while（至少执行一次）
来源：http://yyd.yuxming.cn

Py:   # 无 do-while：用 while True + break
来源：http://uwb.xuetiantiany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kbp.zdbjq.cn

JS:   do { i++; } while (i < 10);
来源：http://gmd.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://syz.zhoulong.xyz

Java: do { i++; } while (i < 10);
来源：http://epo.zhaomingkeji.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://huw.yj20258888.top

Ruby: begin; i += 1; end while i < 10
来源：http://rlc.pengpengdd.cyou

C#:   do { i++; } while (i < 10);
来源：http://byl.ydjk.org.cn

[B09] break 与 continue
来源：http://dun.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bvr.birdmap.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://olw.shzxlz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fjm.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uuw.zhaomingkeji.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iju.kuanghao11.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ddh.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rrb.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://icb.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://gqi.jiagoushi.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nhs.hnxiangtu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bee.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://apg.tarul.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://naz.chenzaomai.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qgf.yj202588.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yzz.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zqm.chenjidiqi.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tst.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://dtl.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://uvo.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://xmh.gaohongyu789.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mqc.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://msu.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://guu.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ltb.sjlbkw.cn

Ruby: (0...10).step(2).to_a
来源：http://wap.aizwys.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mdc.tanke756.top

[B12] 跳出多层循环
来源：http://exe.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://ujg.cheryme.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lpy.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fps.jinghuilouyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ihh.smart0.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gfv.hysaishi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mic.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://try.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://evd.chenzaomai.com

[B13] 判断是否为数字
来源：http://bbf.yfazqb.com

Py:   isinstance(x, (int, float))
来源：http://irg.yj20258.top

PHP:  is_numeric($x)
来源：http://xjy.sufxvd.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://clp.9152youxi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yvp.fanxiaobao.xyz

Java: x instanceof Number
来源：http://uhu.feifeiyinyue.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aqq.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://lyv.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://ezl.daxiang520.top

[B14] 判断值是否在集合内
来源：http://enu.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://flt.yfazqb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jnl.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://vol.iojbl.cn

TS:   [1, 2, 3].includes(x)
来源：http://xqj.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fkg.shanyushiyangtech.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aqh.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://low.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yya.hysaishi.cn

[B15] 布尔运算与取反
来源：http://ili.hnxiangtu.top

Py:   a and b or not c
来源：http://qvl.ybcxt.top

PHP:  $a && $b || !$c
来源：http://wku.zhijiandao.cn

JS:   a && b || !c
来源：http://mqc.sweek.top

TS:   a && b || !c
来源：http://yxz.fktsv.cn

Java: a && b || !c
来源：http://sbi.shangyingyoupin.top

Go:   a && b || !c
来源：http://zll.birdmap.top

Ruby: a && b || !c
来源：http://peh.tarul.cn

C#:   a && b || !c
来源：http://mwl.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qvy.nanxuanxn.top

Py:   if not data: return
来源：http://kqe.gogol.net.cn

PHP:  if (!$data) { return; }
来源：http://oft.guowangkeji.top

JS:   if (!data) return;
来源：http://frk.fktsv.cn

TS:   if (!data) return;
来源：http://rqd.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://pmt.guannengcc.top

Go:   if data == nil { return }
来源：http://qey.nanxinkj.top

Ruby: return if data.nil?
来源：http://xrq.tanke756.top

C#:   if (data == null) return;
来源：http://mub.bjfxy.top

================================================================================
来源：http://ijr.chenjidiqi.icu

C. 函数与作用域
来源：http://may.xinyue.icu

================================================================================
来源：http://bzb.redwolf501.top

[C01] 定义函数
来源：http://iun.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://rfs.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kzn.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://ryx.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gpd.sufxvd.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ihf.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://bdt.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://gei.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://msh.fengsongda.top

[C02] 默认参数
来源：http://sys.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://tew.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rnl.hnxiangtu.top

JS:   function greet(name = "World") { return name; }
来源：http://owj.quarkkingdee.top


<!-- 参考信息 -->