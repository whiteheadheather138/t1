代发 wailian999

[A10] 生成随机数
来源：http://hsg.fehbvm.com

Py:   import random; random.randint(1, 100)
来源：http://yiz.tianlin.xyz

PHP:  random_int(1, 100);
来源：http://czs.aizwys.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nwb.hongshengwenyu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hyl.52xcode.cn

Java: new Random().nextInt(100) + 1
来源：http://dqm.aibaodan.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hmp.snrcjt.cn

Ruby: rand(1..100)
来源：http://hmm.chenlongwang.top

C#:   new Random().Next(1, 101)
来源：http://hex.shanyushiyangkeji.top

[A11] 条件表达式（三元）
来源：http://tof.chenjidiqi.icu

Py:   "yes" if x > 0 else "no"
来源：http://iud.fanxiaobao.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://ppq.fengsongda.top

JS:   x > 0 ? "yes" : "no"
来源：http://cbb.ivvv.top

TS:   x > 0 ? "yes" : "no"
来源：http://rgu.feifeiyinyue.top

Java: x > 0 ? "yes" : "no"
来源：http://viv.dashuyun.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://iip.yuxming.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ysw.shanyushiyangtech.top

C#:   x > 0 ? "yes" : "no"
来源：http://yic.zdqjudy.top

[A12] 字符串插值 / 格式化
来源：http://gie.nanxuanxn.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://waj.chenzaomai.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gsb.sjlbkw.cn

JS:   `Hello, ${name}!`
来源：http://ehm.fehbvm.com

TS:   `Hello, ${name}!`
来源：http://zyu.yj202588.top

Java: "Hello, %s!".formatted(name)
来源：http://xie.hfpthk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sdm.yfazqb.com

Ruby: "Hello, #{name}!"
来源：http://onf.zhongyouzk.top

C#:   $"Hello, {name}!"
来源：http://zvu.ppjwa.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rkb.chenlongwang.top

Py:   "第一行\n第二行"
来源：http://xty.haohaochexian.top

PHP:  "第一行\n第二行"
来源：http://koi.nwbrower.top

JS:   "第一行\n第二行"
来源：http://qko.52xcode.cn

TS:   "第一行\n第二行"
来源：http://kvb.nanxinkj.top

Java: "第一行\n第二行"
来源：http://bcj.9152youxi.cn

Go:   "第一行\n第二行"
来源：http://bng.xingfuxueyuan.xyz

Ruby: "第一行\n第二行"
来源：http://luo.ivvv.top

C#:   "第一行\n第二行"
来源：http://ytr.ydzc1.top

[A14] 注释写法
来源：http://dvm.hywenlv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://coi.zycfv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xma.zhaomingkeji.xyz

JS:   // 单行；/* 多行 */
来源：http://hnd.chenjidiqi.icu

TS:   // 单行；/* 多行 */
来源：http://vyq.nwbrower.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mbn.jqgufenzy.top

Go:   // 单行；/* 多行 */
来源：http://jof.fehbvm.com

Ruby: # 单行；=begin 多行 =end
来源：http://dbo.chenjidiqi.icu

C#:   // 单行；/* 多行 */
来源：http://vts.fehbvm.com

[A15] 空值判断与默认值
来源：http://ail.yj20258888.top

Py:   value = data or "默认值"
来源：http://hhb.jinyuanbaomall.cn

PHP:  $value = $data ?? "默认值";
来源：http://fiz.316326.xyz

JS:   const value = data ?? "默认值";
来源：http://ayw.cheryme.top

TS:   const value = data ?? "默认值";
来源：http://vas.yanxiufei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uks.svipenyu.cn

Go:   if data == "" { data = "默认值" }
来源：http://lpd.dashuyun.cn

Ruby: value = data || "默认值"
来源：http://yfz.zhengqikj.top

C#:   var value = data ?? "默认值";
来源：http://vaj.ydzc1.top

[A16] 真假值判断规则
来源：http://spz.cashguo.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fmi.tianlin.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ntc.316326.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://umt.hammf.cn

TS:   if (!x) {}
来源：http://ako.dianchejie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lfz.quarkkingdee.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zme.vehdjk.com

Ruby: unless x            # nil 与 false 为假
来源：http://qjb.pycfn.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hdh.aibaodan.cn

[A17] 位运算
来源：http://ale.chenlongwang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nkm.xziqi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qnn.zdbjq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://axv.cdnleiting.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rxx.fengsongda.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://skc.feifeiyinyue.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://eeh.hnqzz.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kjc.cheryme.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hzf.ctjpmb.com

[A18] 字符与 ASCII 码互转
来源：http://bdb.yj20258888.top

Py:   ord("A"); chr(65)
来源：http://zhd.ybcxt.top

PHP:  ord("A"); chr(65)
来源：http://cpf.xylfe.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://osd.dashuyun.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aar.ppjwa.cn

Java: (int) 'A'; (char) 65
来源：http://ndq.sufxvd.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ebb.cucudq.cn

Ruby: "A".ord; 65.chr
来源：http://mdf.yonumen.top

C#:   (int)'A'; (char)65
来源：http://wwk.zhixingplan.top

[A19] 交换两个变量
来源：http://cqp.cdnleiting.top

Py:   a, b = b, a
来源：http://juq.haohaochexian.top

PHP:  [$a, $b] = [$b, $a];
来源：http://iwl.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://mik.cucudq.cn

TS:   [a, b] = [b, a];
来源：http://fzf.yonumen.top

Java: int t = a; a = b; b = t;
来源：http://hde.xuetiantiany.cn

Go:   a, b = b, a
来源：http://vit.tanke756.top

Ruby: a, b = b, a
来源：http://bnx.shuidangran.top

C#:   (a, b) = (b, a);
来源：http://rno.yj20258.top

[A20] 读取标准输入
来源：http://hte.sxryk.cn

Py:   name = input("请输入：")
来源：http://ugp.bbcook.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wtz.zhengqikj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pxx.jiagoushi.top

TS:   // Node.js：readline 模块
来源：http://xgu.chenzaomai.com

Java: new Scanner(System.in).nextLine()
来源：http://ucj.zhongyouzk.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cox.ehwqpu.com

Ruby: gets.chomp
来源：http://snx.zdbjq.cn

C#:   Console.ReadLine();
来源：http://zjd.zhoulong.xyz

[A21] 保留指定小数位输出
来源：http://qxf.zhoulong.xyz

Py:   f"{3.14159:.2f}"
来源：http://qtc.vqdsnc.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ilu.jqgufenzy.top

JS:   (3.14159).toFixed(2)
来源：http://tqo.ydjk.org.cn

TS:   (3.14159).toFixed(2)
来源：http://jod.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://ets.ybcxt.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pjc.bjfxy.top

Ruby: format("%.2f", 3.14159)
来源：http://qif.tianlin.xyz

C#:   3.14159.ToString("F2")
来源：http://ftb.shangyingyoupin.top

[A22] 获取字符串长度
来源：http://nnb.hfpthk.cn

Py:   len(s)
来源：http://kvg.hfpthk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pqe.aizwys.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cwt.ydzc1.top

TS:   s.length
来源：http://hqe.zhijiandao.cn

Java: s.length()
来源：http://axy.zhaomingkeji.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ssc.fanxiaobao.xyz

Ruby: s.length
来源：http://xpz.ctjpmb.com

C#:   s.Length
来源：http://zqv.hammf.cn

[A23] 大小写转换
来源：http://qry.wangshuangyany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hns.smart0.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://imx.hesvh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xwj.zhongyouzk.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://guo.nanxuanxn.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nhi.svipenyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://edp.ivvv.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zfh.meibo888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://klj.aibaodan.cn

[A24] 去除首尾空白
来源：http://gkv.hnxiangtu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iuu.zhengqikj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ipv.andypj.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pdk.yj20258.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zxi.xuanzx.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ucq.ppjwa.cn

Go:   strings.TrimSpace(s)
来源：http://nkb.316326.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hlh.xingfuxueyuan.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ddo.zhaomingkeji.xyz

[A25] 字符串比较
来源：http://qpx.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://nsj.ivvv.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://khf.yj20258888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://acb.vqdsnc.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yas.xziqi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xak.shanyushiyangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gyl.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hcl.zhixingplan.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kur.aizwys.cn

[A26] 类型转换总览
来源：http://zni.ybcxt.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vtg.yueranfly.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kln.xuanzx.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://khk.jiagoushi.top

TS:   Number() String() Boolean() x as number
来源：http://idp.9152youxi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://urn.xuanzx.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fyr.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dxi.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://amb.shangyingyoupin.top

================================================================================
来源：http://xyh.xinyue.icu

B. 流程控制
来源：http://ysr.bbcook.cn

================================================================================
来源：http://trs.sweek.top

[B01] 条件判断 if / else
来源：http://ihc.yuxming.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lsv.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oyw.chenjidiqi.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jef.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hnp.chenzaomai.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://gpr.tanke756.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xig.yuxming.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tmi.bjfxy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hkl.jinghuilouyu.cn

[B02] 多分支 else if / elif
来源：http://ler.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jud.daxiang520.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wfu.hnxiangtu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jcj.9152youxi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zck.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iau.sysykeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rai.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fxe.yuanzhike.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pva.vehdjk.com

[B03] switch / match / case
来源：http://otl.yongpay.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tdw.nwbrower.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tqt.redwolf501.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://edp.fanxiaobao.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mvr.tarul.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zuh.meibo888.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bcr.yueranfly.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wcj.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lbh.jinghuilouyu.cn

[B04] for 计数循环
来源：http://sky.shanyushiyangtech.top

Py:   for i in range(10): print(i)
来源：http://tql.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qun.hcnkem.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bho.redwolf501.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jam.tian-w.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wmf.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uis.snrcjt.cn

Ruby: 10.times { |i| puts i }
来源：http://tqr.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cgo.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://etn.fehbvm.com

Py:   for item in arr: print(item)
来源：http://hco.ybcxt.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gnp.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fsb.chenjidiqi.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://uki.hfpthk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vdr.sufxvd.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://alm.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://lsg.andypj.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sux.haohaochexian.top

[B06] 遍历字典 / 对象
来源：http://sey.bbcook.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hgb.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kzp.zycfv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fbf.0kj1m.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ozt.dashuyun.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wen.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xwc.jinqigufen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kay.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uoi.shzxlz.cn

[B07] while 循环
来源：http://nfm.cucudq.cn

Py:   while i < 10: i += 1
来源：http://tdz.316326.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://uhl.cheryme.top

JS:   while (i < 10) { i++; }
来源：http://aek.yangfankeji.com

TS:   while (i < 10) { i++; }
来源：http://rqy.bbcook.cn

Java: while (i < 10) { i++; }
来源：http://smk.yanxiufei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qrv.ybcxt.top

Ruby: while i < 10; i += 1; end
来源：http://rxv.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://uoa.fehbvm.com

[B08] do-while（至少执行一次）
来源：http://wrm.cdnleiting.top

Py:   # 无 do-while：用 while True + break
来源：http://svx.fanxiaobao.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://aky.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://ero.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://mkp.cashguo.top

Java: do { i++; } while (i < 10);
来源：http://qal.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://eqo.9152youxi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://thm.cashguo.top

C#:   do { i++; } while (i < 10);
来源：http://ttl.meibo888.top

[B09] break 与 continue
来源：http://lfq.shangyingyoupin.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sif.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nqt.zhaomingkeji.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ysy.ybcxt.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oof.fehbvm.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://waa.hesvh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uxr.birdmap.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kvw.gzhubu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jge.fanxiaobao.xyz

[B10] 遍历同时拿索引
来源：http://lql.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uiy.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zot.havefunace.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zao.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ooz.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://znt.wangshuangyany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jad.jqgfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cyo.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pnc.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://qeq.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://wdo.hammf.cn

PHP:  range(0, 10, 2);
来源：http://efb.zdqjudy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sru.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iey.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nbr.yj20258888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kpa.yuanzhike.top

Ruby: (0...10).step(2).to_a
来源：http://xoo.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://klh.cheryme.top

[B12] 跳出多层循环
来源：http://ntf.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fkk.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vcv.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iba.chenlongwang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hzm.zhixingplan.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gay.yvedp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hlt.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xvq.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ngf.jinqigfzy.top

[B13] 判断是否为数字
来源：http://zwj.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://boq.pycfn.com

PHP:  is_numeric($x)
来源：http://ise.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qkt.ivvv.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oue.daxiang520.top

Java: x instanceof Number
来源：http://ogi.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zse.fehbvm.com

Ruby: x.is_a?(Numeric)
来源：http://zvn.aizwys.cn

C#:   x is int or double or decimal
来源：http://fmg.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://nef.yuxming.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hyp.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://buq.hywenlv.cn

JS:   [1, 2, 3].includes(x)
来源：http://nqi.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://zdy.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hiz.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dtq.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://rok.jinyuanbaomall.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xny.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://vux.hysaishi.cn

Py:   a and b or not c
来源：http://htc.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://bls.jqgfzy.top

JS:   a && b || !c
来源：http://jaa.tarul.cn

TS:   a && b || !c
来源：http://ksw.jqgfzy.top

Java: a && b || !c
来源：http://guo.dianchejie.cn

Go:   a && b || !c
来源：http://lwr.sufxvd.cn

Ruby: a && b || !c
来源：http://tgb.52xcode.cn

C#:   a && b || !c
来源：http://odl.ydjk.org.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qrk.zhixingplan.top

Py:   if not data: return
来源：http://zkm.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://yhl.yonumen.top

JS:   if (!data) return;
来源：http://zwr.hywenlv.cn

TS:   if (!data) return;
来源：http://asy.hysaishi.cn

Java: if (data == null) return;
来源：http://sfg.iojbl.cn

Go:   if data == nil { return }
来源：http://idw.yueranfly.top

Ruby: return if data.nil?
来源：http://rqh.guannengcc.top

C#:   if (data == null) return;
来源：http://chq.jlsjyb.cn


<!-- 参考信息 -->