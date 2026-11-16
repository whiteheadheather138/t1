代发 wailian999

[A10] 生成随机数
来源：http://fyb.shangyingyoupin.top

Py:   import random; random.randint(1, 100)
来源：http://xrg.hesvh.cn

PHP:  random_int(1, 100);
来源：http://zno.zhixingplan.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zrs.zhengqikj.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xtl.zycfv.cn

Java: new Random().nextInt(100) + 1
来源：http://jla.yj20258.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rvr.tian-w.cn

Ruby: rand(1..100)
来源：http://tbh.xuetiantiany.cn

C#:   new Random().Next(1, 101)
来源：http://bqt.gzhubu.top

[A11] 条件表达式（三元）
来源：http://oqx.shanyushiyangkeji.top

Py:   "yes" if x > 0 else "no"
来源：http://anf.dashuyun.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://voq.hongshengwenyu.top

JS:   x > 0 ? "yes" : "no"
来源：http://yte.smart0.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://gmr.xylfe.cn

Java: x > 0 ? "yes" : "no"
来源：http://mfj.xylfe.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wlz.fehbvm.com

Ruby: x > 0 ? "yes" : "no"
来源：http://zhw.jinghuilouyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ffo.shuidangran.top

[A12] 字符串插值 / 格式化
来源：http://yac.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jmt.meibo888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ugf.zycfv.cn

JS:   `Hello, ${name}!`
来源：http://sbd.yj20258.top

TS:   `Hello, ${name}!`
来源：http://gth.shanyushiyangtech.top

Java: "Hello, %s!".formatted(name)
来源：http://kwf.hesvh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gek.jlsjyb.cn

Ruby: "Hello, #{name}!"
来源：http://dhf.zdbjq.cn

C#:   $"Hello, {name}!"
来源：http://gsi.sxryk.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yrf.chenlongwang.top

Py:   "第一行\n第二行"
来源：http://eca.shzxlz.cn

PHP:  "第一行\n第二行"
来源：http://sxq.haohaochexian.top

JS:   "第一行\n第二行"
来源：http://rvn.cashguo.top

TS:   "第一行\n第二行"
来源：http://jyv.wangdashe.top

Java: "第一行\n第二行"
来源：http://ylr.yvedp.cn

Go:   "第一行\n第二行"
来源：http://aga.nwbrower.top

Ruby: "第一行\n第二行"
来源：http://gra.c1oappe.top

C#:   "第一行\n第二行"
来源：http://usu.redwolf501.top

[A14] 注释写法
来源：http://ghf.gogol.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jcq.gzhubu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ppn.tarul.cn

JS:   // 单行；/* 多行 */
来源：http://mzz.jlsjyb.cn

TS:   // 单行；/* 多行 */
来源：http://fyi.tian-w.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kdv.daria6918.cn

Go:   // 单行；/* 多行 */
来源：http://iik.yvedp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nfs.zdbjq.cn

C#:   // 单行；/* 多行 */
来源：http://egc.52xcode.cn

[A15] 空值判断与默认值
来源：http://yzl.shangyingyoupin.top

Py:   value = data or "默认值"
来源：http://pml.andypj.xyz

PHP:  $value = $data ?? "默认值";
来源：http://yox.yongpay.top

JS:   const value = data ?? "默认值";
来源：http://zzz.birdmap.top

TS:   const value = data ?? "默认值";
来源：http://lei.sjlbkw.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mae.hnqzz.top

Go:   if data == "" { data = "默认值" }
来源：http://plr.vehdjk.com

Ruby: value = data || "默认值"
来源：http://igq.hnqzz.top

C#:   var value = data ?? "默认值";
来源：http://iag.hongshengwenyu.top

[A16] 真假值判断规则
来源：http://azd.chenzaomai.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://chd.sysykeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xii.fehbvm.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xin.yvedp.cn

TS:   if (!x) {}
来源：http://cfe.vehdjk.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vfo.haohaochexian.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hjz.sweek.top

Ruby: unless x            # nil 与 false 为假
来源：http://fsl.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://syv.jinqigufen.top

[A17] 位运算
来源：http://hrj.bbcook.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://txk.chenjidiqi.icu

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nfw.gotoacloud.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gnj.yongpay.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qka.zdqjudy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://afh.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zvx.ybcxt.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jqk.yonumen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gfl.redwolf501.top

[A18] 字符与 ASCII 码互转
来源：http://rre.hammf.cn

Py:   ord("A"); chr(65)
来源：http://ryj.9152youxi.cn

PHP:  ord("A"); chr(65)
来源：http://pld.cqqwz.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kfh.zycfv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xgz.tianlin.xyz

Java: (int) 'A'; (char) 65
来源：http://mis.zycfv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zxb.zycfv.cn

Ruby: "A".ord; 65.chr
来源：http://vxi.c1oappe.top

C#:   (int)'A'; (char)65
来源：http://gpo.haohaochexian.top

[A19] 交换两个变量
来源：http://liy.guannengcc.top

Py:   a, b = b, a
来源：http://mjp.zhongyouzk.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kwz.tian-w.cn

JS:   [a, b] = [b, a];
来源：http://asm.haohaochexian.top

TS:   [a, b] = [b, a];
来源：http://gvd.hywenlv.cn

Java: int t = a; a = b; b = t;
来源：http://feb.snrcjt.cn

Go:   a, b = b, a
来源：http://pta.gaohongyu789.top

Ruby: a, b = b, a
来源：http://hll.52xcode.cn

C#:   (a, b) = (b, a);
来源：http://xqh.birdmap.top

[A20] 读取标准输入
来源：http://ngm.sxryk.cn

Py:   name = input("请输入：")
来源：http://gpb.9152youxi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qii.yangfankeji.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qje.pengpengdd.cyou

TS:   // Node.js：readline 模块
来源：http://byj.tianlin.xyz

Java: new Scanner(System.in).nextLine()
来源：http://dlr.shanyushiyangtech.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yno.nanxinkj.top

Ruby: gets.chomp
来源：http://gwp.zdbjq.cn

C#:   Console.ReadLine();
来源：http://mfd.nanxuanxn.top

[A21] 保留指定小数位输出
来源：http://ciw.fanxiaobao.xyz

Py:   f"{3.14159:.2f}"
来源：http://ntp.nwbrower.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://aad.yanxiufei.cn

JS:   (3.14159).toFixed(2)
来源：http://ioo.quarkkingdee.top

TS:   (3.14159).toFixed(2)
来源：http://cah.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://ebq.dashuyun.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xwh.xziqi.cn

Ruby: format("%.2f", 3.14159)
来源：http://uyz.quarkkingdee.top

C#:   3.14159.ToString("F2")
来源：http://jvv.mhx1999.top

[A22] 获取字符串长度
来源：http://qwt.fzhhl.top

Py:   len(s)
来源：http://exj.zhoulong.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cxi.pengpengdd.cyou

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gai.daria6918.cn

TS:   s.length
来源：http://dbz.sufxvd.cn

Java: s.length()
来源：http://pml.fanxiaobao.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ruh.zhengqikj.top

Ruby: s.length
来源：http://nax.mhx1999.top

C#:   s.Length
来源：http://dep.feifeiyinyue.top

[A23] 大小写转换
来源：http://ahg.meibo888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ecu.xinyue.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nqk.jinyuanbaomall.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://keo.cheryme.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lwf.fanxiaobao.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gmk.jiagoushi.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pam.yj20258888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cgq.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lef.fengsongda.top

[A24] 去除首尾空白
来源：http://dpn.quarkkingdee.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xrn.fehbvm.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xun.52xcode.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uzn.bbcook.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://joh.dianchejie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://spt.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://arl.guowangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wwt.gogol.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pzx.haohaochexian.top

[A25] 字符串比较
来源：http://lfs.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://get.bbcook.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ldv.yj20258888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qwm.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uja.fehbvm.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ymd.shanyushiyangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://alr.xuanzx.com

Ruby: s1 == s2; s1 <=> s2
来源：http://yye.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qev.zdqjudy.top

[A26] 类型转换总览
来源：http://ntr.iojbl.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ffk.xziqi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hdg.ppjwa.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cxe.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://twf.meibo888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nhx.ybcxt.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vgm.hnqzz.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://czs.yfazqb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rel.sufxvd.cn

================================================================================
来源：http://hqb.jlsjyb.cn

B. 流程控制
来源：http://xxq.jqgfzy.top

================================================================================
来源：http://ieu.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://ynz.bbcook.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fwy.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uua.hysaishi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ihc.sysykeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mvt.sweek.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vik.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tql.cdnleiting.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wwy.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qql.pycfn.com

[B02] 多分支 else if / elif
来源：http://ygv.fktsv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://isw.gzhubu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qav.tian-w.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://snf.kuanghao11.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yev.shzxlz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zdm.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vqv.sjlbkw.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gml.fengsongda.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jjb.shzxlz.cn

[B03] switch / match / case
来源：http://aqx.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qlg.yonumen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oqv.guowangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://faj.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jum.yvedp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pzn.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://anm.nanxinkj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vun.ehwqpu.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hty.bbcook.cn

[B04] for 计数循环
来源：http://tfp.sweek.top

Py:   for i in range(10): print(i)
来源：http://tbt.jinyuanbaomall.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dko.snrcjt.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xzm.meibo888.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bii.daxiang520.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ety.daria6918.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xfx.fktsv.cn

Ruby: 10.times { |i| puts i }
来源：http://cup.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vkc.tanke756.top

[B05] 遍历数组 / 列表
来源：http://oks.pengpengdd.cyou

Py:   for item in arr: print(item)
来源：http://joa.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hsk.jianghu66.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ijx.bbcook.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yie.fengsongda.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://brk.tanke756.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cny.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://poq.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ygn.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://mnd.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://amj.tanke756.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tpf.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://exp.chenzaomai.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qmd.hammf.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xmo.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rci.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vyj.hesvh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wqu.jiagoushi.top

[B07] while 循环
来源：http://qru.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://nuk.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://bso.jinqigufen.top

JS:   while (i < 10) { i++; }
来源：http://ltw.pengpengdd.cyou

TS:   while (i < 10) { i++; }
来源：http://shh.ehwqpu.com

Java: while (i < 10) { i++; }
来源：http://hhc.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sge.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://mew.9152youxi.cn

C#:   while (i < 10) { i++; }
来源：http://qcf.shzxlz.cn

[B08] do-while（至少执行一次）
来源：http://jck.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://hln.andypj.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://eah.uphjek.com

JS:   do { i++; } while (i < 10);
来源：http://vyj.hywenlv.cn

TS:   do { i++; } while (i < 10);
来源：http://quc.zhoulong.xyz

Java: do { i++; } while (i < 10);
来源：http://amc.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://kcm.nanxuanxn.top

Ruby: begin; i += 1; end while i < 10
来源：http://nfx.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://pjm.yonumen.top

[B09] break 与 continue
来源：http://vla.yvedp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://djl.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dtu.dashuyun.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ply.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hlv.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://slf.hfpthk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sgs.wangdashe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zee.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ard.svipenyu.cn

[B10] 遍历同时拿索引
来源：http://zgu.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xzy.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ckg.gogol.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kof.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xil.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://czf.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jra.fengsongda.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://abz.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sta.ppjwa.cn

[B11] 生成数字序列 / 区间
来源：http://mol.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://fjf.feifeiyinyue.top

PHP:  range(0, 10, 2);
来源：http://oim.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rkz.wangshuangyany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lld.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ntn.hammf.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wzj.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://vcl.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oxz.zdqjudy.top

[B12] 跳出多层循环
来源：http://rag.yuxming.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mpu.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nqn.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kvo.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fik.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ubu.shuidangran.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gqx.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dcm.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yqp.yanxiufei.cn

[B13] 判断是否为数字
来源：http://cte.yuxming.cn

Py:   isinstance(x, (int, float))
来源：http://mte.chenlongwang.top

PHP:  is_numeric($x)
来源：http://cyu.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sru.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://djq.nanxinkj.top

Java: x instanceof Number
来源：http://hxl.chenzaomai.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kiu.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://mdi.guannengcc.top

C#:   x is int or double or decimal
来源：http://vjs.xuanzx.com

[B14] 判断值是否在集合内
来源：http://fup.andypj.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ceu.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nsy.jinqigufen.top

JS:   [1, 2, 3].includes(x)
来源：http://aww.zhixingplan.top

TS:   [1, 2, 3].includes(x)
来源：http://gzs.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nqi.iojbl.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qlu.jqgfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://lyp.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vbt.shzxlz.cn

[B15] 布尔运算与取反
来源：http://tyf.nanxuanxn.top

Py:   a and b or not c
来源：http://hnh.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://mvz.ehwqpu.com

JS:   a && b || !c
来源：http://qwh.yonumen.top

TS:   a && b || !c
来源：http://lrj.yvedp.cn

Java: a && b || !c
来源：http://csr.jqgufenzy.top

Go:   a && b || !c
来源：http://ake.uphjek.com

Ruby: a && b || !c
来源：http://tnq.yvedp.cn

C#:   a && b || !c
来源：http://ktm.jinghuilouyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gcq.feifeiyinyue.top

Py:   if not data: return
来源：http://ckf.ivvv.top

PHP:  if (!$data) { return; }
来源：http://ubo.zhengqikj.top

JS:   if (!data) return;
来源：http://xeu.xylfe.cn

TS:   if (!data) return;
来源：http://ucl.kuanghao11.cn

Java: if (data == null) return;
来源：http://fav.xuanzx.com

Go:   if data == nil { return }
来源：http://crm.hfpthk.cn

Ruby: return if data.nil?
来源：http://ynu.ydjk.org.cn

C#:   if (data == null) return;
来源：http://rcs.nanxuanxn.top


<!-- 参考信息 -->