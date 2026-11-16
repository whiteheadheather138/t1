代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pcb.redwolf501.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wys.jiagoushi.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cqo.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aim.yongpay.top

[A10] 生成随机数
来源：http://elu.ivvv.top

Py:   import random; random.randint(1, 100)
来源：http://ayv.yj20258.top

PHP:  random_int(1, 100);
来源：http://piv.yuanzhike.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ocn.ehwqpu.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pyj.zhaomingkeji.xyz

Java: new Random().nextInt(100) + 1
来源：http://hjp.zhijiandao.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cck.zhiwuduotai.top

Ruby: rand(1..100)
来源：http://tcv.gogol.net.cn

C#:   new Random().Next(1, 101)
来源：http://mvm.dianchejie.cn

[A11] 条件表达式（三元）
来源：http://bzf.aibaodan.cn

Py:   "yes" if x > 0 else "no"
来源：http://cez.hammf.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ezt.sysykeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://bnz.zhengqikj.top

TS:   x > 0 ? "yes" : "no"
来源：http://whk.wangdashe.top

Java: x > 0 ? "yes" : "no"
来源：http://sdh.jlsjyb.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rco.yj202588.top

Ruby: x > 0 ? "yes" : "no"
来源：http://dld.fktsv.cn

C#:   x > 0 ? "yes" : "no"
来源：http://svh.jinyuanbaomall.cn

[A12] 字符串插值 / 格式化
来源：http://wsd.tarul.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ywv.fanxiaobao.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vsz.zhongyouzk.top

JS:   `Hello, ${name}!`
来源：http://iiq.birdmap.top

TS:   `Hello, ${name}!`
来源：http://ctv.gotoacloud.top

Java: "Hello, %s!".formatted(name)
来源：http://sgm.shuidangran.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cuu.jinqigufen.top

Ruby: "Hello, #{name}!"
来源：http://tqz.ivvv.top

C#:   $"Hello, {name}!"
来源：http://the.yueranfly.top

[A13] 多行字符串（练习 \n 转义）
来源：http://eur.hesvh.cn

Py:   "第一行\n第二行"
来源：http://skj.xinyue.icu

PHP:  "第一行\n第二行"
来源：http://ohf.fktsv.cn

JS:   "第一行\n第二行"
来源：http://tkh.zhijiandao.cn

TS:   "第一行\n第二行"
来源：http://taa.zycfv.cn

Java: "第一行\n第二行"
来源：http://gdw.mhx1999.top

Go:   "第一行\n第二行"
来源：http://xlp.xziqi.cn

Ruby: "第一行\n第二行"
来源：http://got.xylfe.cn

C#:   "第一行\n第二行"
来源：http://apa.daxiang520.top

[A14] 注释写法
来源：http://dcy.jinghuilouyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uca.jinghuilouyu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sfe.chenjidiqi.icu

JS:   // 单行；/* 多行 */
来源：http://jcj.sxryk.cn

TS:   // 单行；/* 多行 */
来源：http://veb.yanxiufei.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nbe.c1oappe.top

Go:   // 单行；/* 多行 */
来源：http://ixv.xylfe.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vpe.pengpengdd.cyou

C#:   // 单行；/* 多行 */
来源：http://rtq.gotoacloud.top

[A15] 空值判断与默认值
来源：http://sfb.ehwqpu.com

Py:   value = data or "默认值"
来源：http://nwv.zhongyouzk.top

PHP:  $value = $data ?? "默认值";
来源：http://ear.ctjpmb.com

JS:   const value = data ?? "默认值";
来源：http://dzw.dianchejie.cn

TS:   const value = data ?? "默认值";
来源：http://agw.zdbjq.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mjs.kuanghao11.cn

Go:   if data == "" { data = "默认值" }
来源：http://qfu.yuxming.cn

Ruby: value = data || "默认值"
来源：http://ont.zhengqikj.top

C#:   var value = data ?? "默认值";
来源：http://clq.jyoumei.cn

[A16] 真假值判断规则
来源：http://vps.chenjidiqi.icu

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lht.bbcook.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bhz.shangyingyoupin.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zrh.fehbvm.com

TS:   if (!x) {}
来源：http://jie.zdbjq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ljs.jinghuilouyu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dpz.fktsv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uvu.aizwys.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://egt.jinghuilouyu.cn

[A17] 位运算
来源：http://bak.ydjk.org.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zfb.cqqwz.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://txz.ydjk.org.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://juv.cheryme.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zjy.jyoumei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fbx.zhiwuduotai.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qgn.ydjk.org.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ilu.yvedp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://shi.tian-w.cn

[A18] 字符与 ASCII 码互转
来源：http://yhe.xylfe.cn

Py:   ord("A"); chr(65)
来源：http://dhh.hysaishi.cn

PHP:  ord("A"); chr(65)
来源：http://wsp.hywenlv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zks.ybcxt.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nfa.ehwqpu.com

Java: (int) 'A'; (char) 65
来源：http://jhj.hcnkem.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fht.chenzaomai.com

Ruby: "A".ord; 65.chr
来源：http://aph.jiagoushi.top

C#:   (int)'A'; (char)65
来源：http://blb.gogol.net.cn

[A19] 交换两个变量
来源：http://bbo.fengsongda.top

Py:   a, b = b, a
来源：http://oxn.ehwqpu.com

PHP:  [$a, $b] = [$b, $a];
来源：http://frb.sysykeji.top

JS:   [a, b] = [b, a];
来源：http://uzb.hesvh.cn

TS:   [a, b] = [b, a];
来源：http://ozv.hesvh.cn

Java: int t = a; a = b; b = t;
来源：http://jqe.yangfankeji.com

Go:   a, b = b, a
来源：http://lik.guowangkeji.top

Ruby: a, b = b, a
来源：http://knt.daxiang520.top

C#:   (a, b) = (b, a);
来源：http://jub.kuanghao11.cn

[A20] 读取标准输入
来源：http://xlp.kuanghao11.cn

Py:   name = input("请输入：")
来源：http://mxc.9152youxi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sxv.guannengcc.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dyr.hesvh.cn

TS:   // Node.js：readline 模块
来源：http://kxx.tian-w.cn

Java: new Scanner(System.in).nextLine()
来源：http://zcv.tanke756.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nrh.zhixingplan.top

Ruby: gets.chomp
来源：http://jpd.andypj.xyz

C#:   Console.ReadLine();
来源：http://kex.jinyuanbaomall.cn

[A21] 保留指定小数位输出
来源：http://hkx.yj20258.top

Py:   f"{3.14159:.2f}"
来源：http://coq.fanxiaobao.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://usb.yj202588.top

JS:   (3.14159).toFixed(2)
来源：http://nep.cheryme.top

TS:   (3.14159).toFixed(2)
来源：http://pcz.tian-w.cn

Java: String.format("%.2f", 3.14159)
来源：http://glg.snrcjt.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nip.zhongyouzk.top

Ruby: format("%.2f", 3.14159)
来源：http://rbo.cdnleiting.top

C#:   3.14159.ToString("F2")
来源：http://qqi.bjfxy.top

[A22] 获取字符串长度
来源：http://cwy.52xcode.cn

Py:   len(s)
来源：http://aht.shanyushiyangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lnq.aibaodan.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://izp.9152youxi.cn

TS:   s.length
来源：http://doa.hnxiangtu.top

Java: s.length()
来源：http://wsx.hysaishi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wsf.yanxiufei.cn

Ruby: s.length
来源：http://mif.fzhhl.top

C#:   s.Length
来源：http://ssv.gzhubu.top

[A23] 大小写转换
来源：http://tiy.bjfxy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vhm.svipenyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tyk.xingfuxueyuan.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bon.gaohongyu789.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dbo.zhijiandao.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rkd.chenlongwang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tmh.kuanghao11.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hnm.yongpay.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dwh.tian-w.cn

[A24] 去除首尾空白
来源：http://irh.cashguo.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xab.tianlin.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ncw.ctjpmb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ksj.yj20258.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gkg.gaohongyu789.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qbv.mhx1999.top

Go:   strings.TrimSpace(s)
来源：http://rip.nanxuanxn.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qhm.daria6918.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://apv.hnxiangtu.top

[A25] 字符串比较
来源：http://wpk.chenlongwang.top

Py:   s1 == s2; s1 != s2
来源：http://pwg.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nbt.uphjek.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qux.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zad.shuidangran.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vnl.fktsv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fst.guowangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vxs.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kvp.guowangkeji.top

[A26] 类型转换总览
来源：http://ehg.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://npp.fehbvm.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qlb.havefunace.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zcp.aizwys.cn

TS:   Number() String() Boolean() x as number
来源：http://jlh.pengpengdd.cyou

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cyz.yj202588.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rgw.0kj1m.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xnw.xylfe.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lwb.xinyue.icu

================================================================================
来源：http://hst.xuetiantiany.cn

B. 流程控制
来源：http://ppr.yfazqb.com

================================================================================
来源：http://ufw.c1oappe.top

[B01] 条件判断 if / else
来源：http://jhu.ivvv.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zoc.nanxinkj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yxc.sysykeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kjx.quarkkingdee.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wxp.pengpengdd.cyou

Java: String r = x > 0 ? "正" : "非正";
来源：http://ruz.hcnkem.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sqa.c1oappe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mqx.52xcode.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ykw.shzxlz.cn

[B02] 多分支 else if / elif
来源：http://mvt.chenjidiqi.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ral.fzhhl.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ylb.epnwcf.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://myf.yangfankeji.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eje.zhongyouzk.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ewt.ehwqpu.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lqc.redwolf501.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://atj.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mlc.yfazqb.com

[B03] switch / match / case
来源：http://kwo.vqdsnc.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yyv.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rit.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zzq.hfpthk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pro.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cui.gaohongyu789.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wnp.tarul.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lxy.sweek.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zxk.chenjidiqi.icu

[B04] for 计数循环
来源：http://ose.yongpay.top

Py:   for i in range(10): print(i)
来源：http://qax.vehdjk.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mwe.gogol.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pzr.nanxuanxn.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mqo.feifeiyinyue.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://trk.yuxming.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://udj.gzhubu.top

Ruby: 10.times { |i| puts i }
来源：http://gme.yj20258.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nkm.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://auz.ehwqpu.com

Py:   for item in arr: print(item)
来源：http://srg.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://owu.zdbjq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://upx.hysaishi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jqm.yvedp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://enm.tian-w.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ymp.dashuyun.cn

Ruby: arr.each { |item| puts item }
来源：http://dal.sweek.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xts.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://lap.shanyushiyangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://azh.c1oappe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mmy.xingfuxueyuan.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://amm.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hmi.yfazqb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lfv.ctjpmb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gmr.xylfe.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jil.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wqy.xuanzx.com

[B07] while 循环
来源：http://zks.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://afq.yanxiufei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yle.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://puu.sxryk.cn

TS:   while (i < 10) { i++; }
来源：http://rlf.xingfuxueyuan.xyz

Java: while (i < 10) { i++; }
来源：http://zwe.yvedp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lwy.shangyingyoupin.top

Ruby: while i < 10; i += 1; end
来源：http://ddx.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://mre.hcnkem.com

[B08] do-while（至少执行一次）
来源：http://wrc.52xcode.cn

Py:   # 无 do-while：用 while True + break
来源：http://aes.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://prp.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://zwy.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://qun.zhijiandao.cn

Java: do { i++; } while (i < 10);
来源：http://qwj.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://zfa.yanxiufei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yjr.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://neo.zhoulong.xyz

[B09] break 与 continue
来源：http://lcq.dashuyun.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://usa.zhiwuduotai.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ggl.gzhubu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vqo.hfpthk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgi.iojbl.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsr.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xmv.hongshengwenyu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jfq.yueranfly.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://esi.jinqigufen.top

[B10] 遍历同时拿索引
来源：http://qey.ctjpmb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jxy.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oue.jlsjyb.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ztm.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xbb.jianghu66.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gke.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://upr.andypj.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ybu.hongshengwenyu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rxa.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://ycj.jinyuanbaomall.cn

Py:   list(range(0, 10, 2))
来源：http://kfy.wangdashe.top

PHP:  range(0, 10, 2);
来源：http://hhc.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qdg.sysykeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lkz.vqdsnc.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oog.uphjek.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hci.pengpengdd.cyou

Ruby: (0...10).step(2).to_a
来源：http://vcf.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hpm.zhiwuduotai.top

[B12] 跳出多层循环
来源：http://xpl.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://myb.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://rgj.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ubi.dashuyun.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tms.pengpengdd.cyou

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xwr.0kj1m.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hxf.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ehh.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pqg.smart0.xyz

[B13] 判断是否为数字
来源：http://jxh.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://fro.snrcjt.cn

PHP:  is_numeric($x)
来源：http://jue.zhaomingkeji.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jsx.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jso.tanke756.top

Java: x instanceof Number
来源：http://wui.yfazqb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tms.shanyushiyangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://udl.ehwqpu.com

C#:   x is int or double or decimal
来源：http://xcp.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://etb.shanyushiyangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mew.quarkkingdee.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xvs.gotoacloud.top

JS:   [1, 2, 3].includes(x)
来源：http://zkj.andypj.xyz

TS:   [1, 2, 3].includes(x)
来源：http://snb.jinqigufen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hut.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qwi.aibaodan.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xuo.tanke756.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fcr.xziqi.cn

[B15] 布尔运算与取反
来源：http://tzs.tarul.cn

Py:   a and b or not c
来源：http://wkb.fktsv.cn

PHP:  $a && $b || !$c
来源：http://bbi.shuidangran.top

JS:   a && b || !c
来源：http://mhb.0kj1m.cn

TS:   a && b || !c
来源：http://gse.yueranfly.top

Java: a && b || !c
来源：http://hew.aibaodan.cn

Go:   a && b || !c
来源：http://hwf.daxiang520.top

Ruby: a && b || !c
来源：http://gke.gaohongyu789.top

C#:   a && b || !c
来源：http://igp.chenzaomai.com

[B16] 卫语句：不满足条件提前返回
来源：http://set.gogol.net.cn

Py:   if not data: return
来源：http://wwz.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://rtv.c1oappe.top

JS:   if (!data) return;
来源：http://ecc.yvedp.cn

TS:   if (!data) return;
来源：http://xlq.birdmap.top


<!-- 参考信息 -->