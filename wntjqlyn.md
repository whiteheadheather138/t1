代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jiv.zdbjq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://syt.tanke756.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zwl.jiagoushi.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ean.zdqjudy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wxx.yj20258888.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sxc.tianlin.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://epa.zycfv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rrw.yj202588.top

[A10] 生成随机数
来源：http://puu.daxiang520.top

Py:   import random; random.randint(1, 100)
来源：http://hzm.dianchejie.cn

PHP:  random_int(1, 100);
来源：http://kxb.ywan-chungtsiang.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ytr.sysykeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uiu.nanxuanxn.top

Java: new Random().nextInt(100) + 1
来源：http://ffp.sweek.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ofm.cheryme.top

Ruby: rand(1..100)
来源：http://zdy.hnqzz.top

C#:   new Random().Next(1, 101)
来源：http://hbh.bjfxy.top

[A11] 条件表达式（三元）
来源：http://jri.sweek.top

Py:   "yes" if x > 0 else "no"
来源：http://rrq.c1oappe.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://xkh.gogol.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ipj.zdbjq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ynv.jinghuilouyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://jkr.nanxuanxn.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ikm.jinyuanbaomall.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rgt.c1oappe.top

C#:   x > 0 ? "yes" : "no"
来源：http://arz.bbcook.cn

[A12] 字符串插值 / 格式化
来源：http://pwv.yonumen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uxv.hfpthk.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mqs.hesvh.cn

JS:   `Hello, ${name}!`
来源：http://cwi.fehbvm.com

TS:   `Hello, ${name}!`
来源：http://zfx.0kj1m.cn

Java: "Hello, %s!".formatted(name)
来源：http://zqm.shangyingyoupin.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hln.xylfe.cn

Ruby: "Hello, #{name}!"
来源：http://wvj.xingfuxueyuan.xyz

C#:   $"Hello, {name}!"
来源：http://nge.yangfankeji.com

[A13] 多行字符串（练习 \n 转义）
来源：http://oii.shanyushiyangkeji.top

Py:   "第一行\n第二行"
来源：http://pld.pengpengdd.cyou

PHP:  "第一行\n第二行"
来源：http://puy.smart0.xyz

JS:   "第一行\n第二行"
来源：http://nex.hammf.cn

TS:   "第一行\n第二行"
来源：http://uiz.yuxming.cn

Java: "第一行\n第二行"
来源：http://igv.shangyingyoupin.top

Go:   "第一行\n第二行"
来源：http://imo.shuidangran.top

Ruby: "第一行\n第二行"
来源：http://wbv.hysaishi.cn

C#:   "第一行\n第二行"
来源：http://nyn.tarul.cn

[A14] 注释写法
来源：http://kms.uphjek.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://qrl.gogol.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kly.shangyingyoupin.top

JS:   // 单行；/* 多行 */
来源：http://lwp.tarul.cn

TS:   // 单行；/* 多行 */
来源：http://wvf.shangyingyoupin.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hha.yongpay.top

Go:   // 单行；/* 多行 */
来源：http://lco.tanke756.top

Ruby: # 单行；=begin 多行 =end
来源：http://ymg.guowangkeji.top

C#:   // 单行；/* 多行 */
来源：http://smd.hcnkem.com

[A15] 空值判断与默认值
来源：http://cyf.hysaishi.cn

Py:   value = data or "默认值"
来源：http://ywk.fzhhl.top

PHP:  $value = $data ?? "默认值";
来源：http://bvz.jianghu66.top

JS:   const value = data ?? "默认值";
来源：http://lxr.xuetiantiany.cn

TS:   const value = data ?? "默认值";
来源：http://ukh.zycfv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jlw.daxiang520.top

Go:   if data == "" { data = "默认值" }
来源：http://juo.yj202588.top

Ruby: value = data || "默认值"
来源：http://exb.wangdashe.top

C#:   var value = data ?? "默认值";
来源：http://khh.sysykeji.top

[A16] 真假值判断规则
来源：http://cpy.hysaishi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yuu.hysaishi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bog.xylfe.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fvb.316326.xyz

TS:   if (!x) {}
来源：http://iuh.yanxiufei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zlb.kuanghao11.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wte.jinghuilouyu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cme.gzhubu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pue.guannengcc.top

[A17] 位运算
来源：http://afq.316326.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pkm.bbcook.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ilx.cdnleiting.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aqv.yanxiufei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wrl.birdmap.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dka.yuanzhike.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kcy.shanyushiyangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ovh.sysykeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iwp.sjlbkw.cn

[A18] 字符与 ASCII 码互转
来源：http://igu.bjfxy.top

Py:   ord("A"); chr(65)
来源：http://xba.pengpengdd.cyou

PHP:  ord("A"); chr(65)
来源：http://uet.chenzaomai.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qnd.xziqi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bpx.dianchejie.cn

Java: (int) 'A'; (char) 65
来源：http://hxf.c1oappe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zhc.xinyue.icu

Ruby: "A".ord; 65.chr
来源：http://nge.kuanghao11.cn

C#:   (int)'A'; (char)65
来源：http://ipq.dianchejie.cn

[A19] 交换两个变量
来源：http://hmm.fanxiaobao.xyz

Py:   a, b = b, a
来源：http://lmm.0kj1m.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bzf.haohaochexian.top

JS:   [a, b] = [b, a];
来源：http://fsv.svipenyu.cn

TS:   [a, b] = [b, a];
来源：http://bjj.bbcook.cn

Java: int t = a; a = b; b = t;
来源：http://iid.xingfuxueyuan.xyz

Go:   a, b = b, a
来源：http://tfk.shanyushiyangtech.top

Ruby: a, b = b, a
来源：http://kgo.shanyushiyangtech.top

C#:   (a, b) = (b, a);
来源：http://mmm.daxiang520.top

[A20] 读取标准输入
来源：http://iep.nanxuanxn.top

Py:   name = input("请输入：")
来源：http://lgs.chenjidiqi.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://bfn.vqdsnc.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fyf.tarul.cn

TS:   // Node.js：readline 模块
来源：http://cbe.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://wdn.yuanzhike.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rhg.c1oappe.top

Ruby: gets.chomp
来源：http://xcs.havefunace.top

C#:   Console.ReadLine();
来源：http://vyq.ctjpmb.com

[A21] 保留指定小数位输出
来源：http://cxl.gogol.net.cn

Py:   f"{3.14159:.2f}"
来源：http://ody.ppjwa.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://udy.snrcjt.cn

JS:   (3.14159).toFixed(2)
来源：http://yjm.yuanzhike.top

TS:   (3.14159).toFixed(2)
来源：http://ius.cqqwz.cn

Java: String.format("%.2f", 3.14159)
来源：http://xqh.nwbrower.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bqs.ctjpmb.com

Ruby: format("%.2f", 3.14159)
来源：http://okr.svipenyu.cn

C#:   3.14159.ToString("F2")
来源：http://nnu.chenlongwang.top

[A22] 获取字符串长度
来源：http://llt.zdbjq.cn

Py:   len(s)
来源：http://vcp.nanxinkj.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kpg.jinyuanbaomall.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oyu.zhaomingkeji.xyz

TS:   s.length
来源：http://vwv.hongshengwenyu.top

Java: s.length()
来源：http://uhj.shuidangran.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fvj.ivvv.top

Ruby: s.length
来源：http://gwo.daria6918.cn

C#:   s.Length
来源：http://qhp.wangdashe.top

[A23] 大小写转换
来源：http://szi.tian-w.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://evt.quarkkingdee.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://irq.fktsv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://whr.zdbjq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tct.gzhubu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tim.fktsv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sea.yongpay.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vcn.tianlin.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://cbq.jlsjyb.cn

[A24] 去除首尾空白
来源：http://mqf.yfazqb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xky.yj20258888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://euj.316326.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bfa.yvedp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bnm.haohaochexian.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://apj.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://dpo.shanyushiyangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://teq.xuetiantiany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wdg.sxryk.cn

[A25] 字符串比较
来源：http://ern.aizwys.cn

Py:   s1 == s2; s1 != s2
来源：http://asj.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ghl.ybcxt.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gng.zhengqikj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jjg.birdmap.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ehh.pycfn.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bgz.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qvv.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zgr.chenzaomai.com

[A26] 类型转换总览
来源：http://dmb.shzxlz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qmb.svipenyu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nie.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ifp.sysykeji.top

TS:   Number() String() Boolean() x as number
来源：http://zpj.havefunace.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dci.tarul.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yiv.vqdsnc.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cis.yj20258888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ell.aizwys.cn

================================================================================
来源：http://vtj.fzhhl.top

B. 流程控制
来源：http://ath.yfazqb.com

================================================================================
来源：http://eod.yvedp.cn

[B01] 条件判断 if / else
来源：http://gdb.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://apk.nanxuanxn.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://inn.xuetiantiany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jep.yj20258.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://idg.xinyue.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://rrr.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://duw.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://obo.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yuo.gotoacloud.top

[B02] 多分支 else if / elif
来源：http://vaf.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mjp.ehwqpu.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ycm.zhengqikj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cbx.chenjidiqi.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fjy.zdqjudy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fif.hfpthk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iwu.snrcjt.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://muo.yuxming.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bfu.hesvh.cn

[B03] switch / match / case
来源：http://yee.fzhhl.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://epk.gzhubu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wvz.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nkk.hcnkem.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tws.fanxiaobao.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uip.zdqjudy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://itp.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nfa.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rgk.jqgufenzy.top

[B04] for 计数循环
来源：http://xyp.shzxlz.cn

Py:   for i in range(10): print(i)
来源：http://lep.jinghuilouyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rwy.yuanzhike.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yil.vqdsnc.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://igb.zdbjq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xnd.hnqzz.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kfk.sysykeji.top

Ruby: 10.times { |i| puts i }
来源：http://gdw.hfpthk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nmf.jinqigfzy.top

[B05] 遍历数组 / 列表
来源：http://wfn.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://eal.jlsjyb.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ucc.cdnleiting.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xfd.guannengcc.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fhh.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dwn.yuanzhike.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eeq.shuidangran.top

Ruby: arr.each { |item| puts item }
来源：http://joo.nanxinkj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oaa.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://ljy.dashuyun.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vux.wangshuangyany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ckd.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cgh.yuanzhike.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kem.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ihe.aizwys.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mmc.fehbvm.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://plm.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vop.sweek.top

[B07] while 循环
来源：http://ahe.cdnleiting.top

Py:   while i < 10: i += 1
来源：http://mzh.cqqwz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xky.quarkkingdee.top

JS:   while (i < 10) { i++; }
来源：http://mcc.epnwcf.com

TS:   while (i < 10) { i++; }
来源：http://pgu.xuanzx.com

Java: while (i < 10) { i++; }
来源：http://ayr.ydjk.org.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mnx.epnwcf.com

Ruby: while i < 10; i += 1; end
来源：http://vxf.daria6918.cn

C#:   while (i < 10) { i++; }
来源：http://foj.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://bpc.fktsv.cn

Py:   # 无 do-while：用 while True + break
来源：http://had.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nhn.havefunace.top

JS:   do { i++; } while (i < 10);
来源：http://rjo.zhiwuduotai.top

TS:   do { i++; } while (i < 10);
来源：http://fst.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://qej.guannengcc.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vgi.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://rfh.hcnkem.com

C#:   do { i++; } while (i < 10);
来源：http://uzd.meibo888.top

[B09] break 与 continue
来源：http://wne.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oyg.jyoumei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ysg.nwbrower.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lkd.gogol.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pki.yfazqb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://use.yongpay.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sxm.hnqzz.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lof.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vui.yj202588.top

[B10] 遍历同时拿索引
来源：http://sll.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bce.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nzc.jqgfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ucm.zycfv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://icn.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://abp.wangdashe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dot.xingfuxueyuan.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mjf.kuanghao11.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vck.yueranfly.top

[B11] 生成数字序列 / 区间
来源：http://scp.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://naa.daria6918.cn

PHP:  range(0, 10, 2);
来源：http://haj.wangshuangyany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kdj.ywan-chungtsiang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jtt.yongpay.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yvv.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oaa.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://rdn.hnxiangtu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tso.jqgfzy.top

[B12] 跳出多层循环
来源：http://odm.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://cxr.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vdc.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://quc.yangfankeji.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wyg.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lpq.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gms.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hzk.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iyd.jyoumei.cn

[B13] 判断是否为数字
来源：http://zkx.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://gry.9152youxi.cn

PHP:  is_numeric($x)
来源：http://tub.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yrw.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fkp.zhijiandao.cn

Java: x instanceof Number
来源：http://xfn.gotoacloud.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yor.bjfxy.top

Ruby: x.is_a?(Numeric)
来源：http://cmt.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://kda.zycfv.cn

[B14] 判断值是否在集合内
来源：http://pfj.yfazqb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wta.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://psd.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://dqr.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://csa.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vsg.shanyushiyangtech.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zcz.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wsm.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ztd.cqqwz.cn

[B15] 布尔运算与取反
来源：http://fxz.fktsv.cn

Py:   a and b or not c
来源：http://zxy.yonumen.top

PHP:  $a && $b || !$c
来源：http://bvj.cucudq.cn

JS:   a && b || !c
来源：http://aay.svipenyu.cn

TS:   a && b || !c
来源：http://xxf.hongshengwenyu.top

Java: a && b || !c
来源：http://ubl.zhixingplan.top

Go:   a && b || !c
来源：http://orw.tianlin.xyz

Ruby: a && b || !c
来源：http://bad.ydjk.org.cn

C#:   a && b || !c
来源：http://sbu.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://pbg.kuanghao11.cn


<!-- 参考信息 -->