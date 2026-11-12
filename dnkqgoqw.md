代发 wailian999

[A10] 生成随机数
来源：http://tmo.316326.xyz

Py:   import random; random.randint(1, 100)
来源：http://dgk.xuetiantiany.cn

PHP:  random_int(1, 100);
来源：http://kqt.haohaochexian.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mti.zhiwuduotai.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ucm.snrcjt.cn

Java: new Random().nextInt(100) + 1
来源：http://ogs.nwbrower.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ytu.fengsongda.top

Ruby: rand(1..100)
来源：http://jwd.hcnkem.com

C#:   new Random().Next(1, 101)
来源：http://kqj.wangdashe.top

[A11] 条件表达式（三元）
来源：http://zja.vqdsnc.cn

Py:   "yes" if x > 0 else "no"
来源：http://fes.jlsjyb.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rad.haohaochexian.top

JS:   x > 0 ? "yes" : "no"
来源：http://veu.ydzc1.top

TS:   x > 0 ? "yes" : "no"
来源：http://gjh.smart0.xyz

Java: x > 0 ? "yes" : "no"
来源：http://awb.jinqigfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fky.guannengcc.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gim.yj20258888.top

C#:   x > 0 ? "yes" : "no"
来源：http://bak.fengsongda.top

[A12] 字符串插值 / 格式化
来源：http://wsn.jqgfzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rzi.0kj1m.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://utl.shanyushiyangtech.top

JS:   `Hello, ${name}!`
来源：http://jfr.xingfuxueyuan.xyz

TS:   `Hello, ${name}!`
来源：http://oqi.sweek.top

Java: "Hello, %s!".formatted(name)
来源：http://gza.yj20258888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://meh.yj20258.top

Ruby: "Hello, #{name}!"
来源：http://lrr.ywan-chungtsiang.top

C#:   $"Hello, {name}!"
来源：http://siy.jqgufenzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://uma.jinqigfzy.top

Py:   "第一行\n第二行"
来源：http://trx.yonumen.top

PHP:  "第一行\n第二行"
来源：http://dmu.cashguo.top

JS:   "第一行\n第二行"
来源：http://jge.316326.xyz

TS:   "第一行\n第二行"
来源：http://dsp.yuxming.cn

Java: "第一行\n第二行"
来源：http://xli.jlsjyb.cn

Go:   "第一行\n第二行"
来源：http://rtv.bjfxy.top

Ruby: "第一行\n第二行"
来源：http://hzq.kuanghao11.cn

C#:   "第一行\n第二行"
来源：http://kdx.yuanzhike.top

[A14] 注释写法
来源：http://mes.xuanzx.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://esc.jinyuanbaomall.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jar.cheryme.top

JS:   // 单行；/* 多行 */
来源：http://cgy.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://kbx.tanke756.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fxz.cucudq.cn

Go:   // 单行；/* 多行 */
来源：http://xzl.smart0.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://csr.zhongyouzk.top

C#:   // 单行；/* 多行 */
来源：http://yuy.zhixingplan.top

[A15] 空值判断与默认值
来源：http://idl.fehbvm.com

Py:   value = data or "默认值"
来源：http://xag.nanxuanxn.top

PHP:  $value = $data ?? "默认值";
来源：http://eme.shanyushiyangtech.top

JS:   const value = data ?? "默认值";
来源：http://tzq.sweek.top

TS:   const value = data ?? "默认值";
来源：http://hzs.yuxming.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://anf.wangdashe.top

Go:   if data == "" { data = "默认值" }
来源：http://oyk.jlsjyb.cn

Ruby: value = data || "默认值"
来源：http://ejr.xuanzx.com

C#:   var value = data ?? "默认值";
来源：http://rws.guannengcc.top

[A16] 真假值判断规则
来源：http://fhi.yfazqb.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vqz.sysykeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hrb.tianlin.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kdz.ywan-chungtsiang.top

TS:   if (!x) {}
来源：http://ljq.jinyuanbaomall.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vtx.ybcxt.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yrj.havefunace.top

Ruby: unless x            # nil 与 false 为假
来源：http://hpj.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://taq.yangfankeji.com

[A17] 位运算
来源：http://uwq.ydzc1.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gnb.nanxuanxn.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fpq.guannengcc.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wcf.shanyushiyangkeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bac.nwbrower.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bcr.kuanghao11.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rxt.ctjpmb.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uiy.hywenlv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oam.daria6918.cn

[A18] 字符与 ASCII 码互转
来源：http://aef.fzhhl.top

Py:   ord("A"); chr(65)
来源：http://dks.9152youxi.cn

PHP:  ord("A"); chr(65)
来源：http://qkv.cheryme.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yhk.316326.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dek.pycfn.com

Java: (int) 'A'; (char) 65
来源：http://per.zhengqikj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://asl.dianchejie.cn

Ruby: "A".ord; 65.chr
来源：http://uwl.ydzc1.top

C#:   (int)'A'; (char)65
来源：http://rfs.xziqi.cn

[A19] 交换两个变量
来源：http://qxj.svipenyu.cn

Py:   a, b = b, a
来源：http://juk.gaohongyu789.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qkt.wangdashe.top

JS:   [a, b] = [b, a];
来源：http://efb.ivvv.top

TS:   [a, b] = [b, a];
来源：http://xjl.nanxinkj.top

Java: int t = a; a = b; b = t;
来源：http://dxi.uphjek.com

Go:   a, b = b, a
来源：http://syi.aibaodan.cn

Ruby: a, b = b, a
来源：http://gif.xinyue.icu

C#:   (a, b) = (b, a);
来源：http://bss.shangyingyoupin.top

[A20] 读取标准输入
来源：http://skc.ywan-chungtsiang.top

Py:   name = input("请输入：")
来源：http://mdn.dashuyun.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qtm.yuanzhike.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kyl.epnwcf.com

TS:   // Node.js：readline 模块
来源：http://smf.andypj.xyz

Java: new Scanner(System.in).nextLine()
来源：http://aop.aizwys.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qvt.yj20258888.top

Ruby: gets.chomp
来源：http://avx.pengpengdd.cyou

C#:   Console.ReadLine();
来源：http://oju.zhiwuduotai.top

[A21] 保留指定小数位输出
来源：http://kxc.tanke756.top

Py:   f"{3.14159:.2f}"
来源：http://fir.uphjek.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yrl.cdnleiting.top

JS:   (3.14159).toFixed(2)
来源：http://ids.xziqi.cn

TS:   (3.14159).toFixed(2)
来源：http://eka.svipenyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://svz.hesvh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://evn.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://bar.xuetiantiany.cn

C#:   3.14159.ToString("F2")
来源：http://aqh.tianlin.xyz

[A22] 获取字符串长度
来源：http://izs.meibo888.top

Py:   len(s)
来源：http://tnk.yj202588.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sxx.wangshuangyany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gve.jinqigfzy.top

TS:   s.length
来源：http://nuu.nwbrower.top

Java: s.length()
来源：http://ctj.xinyue.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mib.feifeiyinyue.top

Ruby: s.length
来源：http://csf.gotoacloud.top

C#:   s.Length
来源：http://uhf.xuanzx.com

[A23] 大小写转换
来源：http://dai.bbcook.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://afx.cdnleiting.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uum.iojbl.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qtm.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jak.hysaishi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sji.ctjpmb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://utw.hfpthk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rev.snrcjt.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cxw.zhiwuduotai.top

[A24] 去除首尾空白
来源：http://vkb.tanke756.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gfd.smart0.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bos.ehwqpu.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uhw.dashuyun.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ikb.ppjwa.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sbt.hnxiangtu.top

Go:   strings.TrimSpace(s)
来源：http://drn.quarkkingdee.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kfd.sweek.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nei.iojbl.cn

[A25] 字符串比较
来源：http://gjz.aizwys.cn

Py:   s1 == s2; s1 != s2
来源：http://vbd.sysykeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nvu.zhixingplan.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ity.fengsongda.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jew.jinghuilouyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nbp.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://heo.ybcxt.top

Ruby: s1 == s2; s1 <=> s2
来源：http://smv.yueranfly.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xtl.cqqwz.cn

[A26] 类型转换总览
来源：http://eeb.xziqi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fum.ppjwa.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qbq.cashguo.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yqj.havefunace.top

TS:   Number() String() Boolean() x as number
来源：http://exq.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://grq.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://snf.fengsongda.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vnm.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lfw.dianchejie.cn

================================================================================
来源：http://tit.vehdjk.com

B. 流程控制
来源：http://jwg.xingfuxueyuan.xyz

================================================================================
来源：http://oao.zhengqikj.top

[B01] 条件判断 if / else
来源：http://xfu.zhiwuduotai.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bpw.jinqigufen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://war.wangdashe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lmf.xziqi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vxh.yanxiufei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://agu.gzhubu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kok.guannengcc.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wlh.ydjk.org.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fsa.nwbrower.top

[B02] 多分支 else if / elif
来源：http://jil.ehwqpu.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gly.yj20258888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zyc.tian-w.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lnp.vehdjk.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lht.hongshengwenyu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dkn.zdbjq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://car.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mcj.nanxinkj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bcd.chenlongwang.top

[B03] switch / match / case
来源：http://rep.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yvu.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mkv.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ais.fehbvm.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://taw.fzhhl.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://buk.chenlongwang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xnx.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kzv.52xcode.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vxs.gaohongyu789.top

[B04] for 计数循环
来源：http://hgw.zhengqikj.top

Py:   for i in range(10): print(i)
来源：http://apo.epnwcf.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://muc.zhijiandao.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rgc.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tjn.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wis.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gzk.yueranfly.top

Ruby: 10.times { |i| puts i }
来源：http://uah.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qkc.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://mhx.ydzc1.top

Py:   for item in arr: print(item)
来源：http://ysl.ppjwa.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pbt.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tbu.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lql.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yps.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hsi.iojbl.cn

Ruby: arr.each { |item| puts item }
来源：http://twu.cucudq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vtp.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://xab.sufxvd.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://svr.ctjpmb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rnj.zhaomingkeji.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dzb.iojbl.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gys.uphjek.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ubh.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nnd.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rof.nwbrower.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dml.ydzc1.top

[B07] while 循环
来源：http://cga.xziqi.cn

Py:   while i < 10: i += 1
来源：http://voh.sjlbkw.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xoy.gotoacloud.top

JS:   while (i < 10) { i++; }
来源：http://yem.zhijiandao.cn

TS:   while (i < 10) { i++; }
来源：http://xbc.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://xat.hysaishi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mvb.redwolf501.top

Ruby: while i < 10; i += 1; end
来源：http://nbr.tarul.cn

C#:   while (i < 10) { i++; }
来源：http://rmw.gotoacloud.top

[B08] do-while（至少执行一次）
来源：http://qst.nwbrower.top

Py:   # 无 do-while：用 while True + break
来源：http://amf.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://haf.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://wnl.hywenlv.cn

TS:   do { i++; } while (i < 10);
来源：http://bts.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://kvw.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fzk.tarul.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qib.shanyushiyangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://tpr.cdnleiting.top

[B09] break 与 continue
来源：http://cvm.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bjn.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zij.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fyx.daxiang520.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jtd.shanyushiyangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sqe.svipenyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fto.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rkx.wangshuangyany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oag.bjfxy.top

[B10] 遍历同时拿索引
来源：http://dmj.jinqigufen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fqb.chenlongwang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nve.jyoumei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kux.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wwu.dianchejie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kmj.haohaochexian.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ijd.zdbjq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ifc.dianchejie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://npv.tarul.cn

[B11] 生成数字序列 / 区间
来源：http://ulm.sxryk.cn

Py:   list(range(0, 10, 2))
来源：http://nza.yuxming.cn

PHP:  range(0, 10, 2);
来源：http://pqj.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nwt.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://squ.jinqigufen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lzz.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qbk.jlsjyb.cn

Ruby: (0...10).step(2).to_a
来源：http://cxx.sufxvd.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://all.fanxiaobao.xyz

[B12] 跳出多层循环
来源：http://rxi.zhaomingkeji.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://xiu.sweek.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tvq.ehwqpu.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lvo.fehbvm.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sfb.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gve.pycfn.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iob.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qbb.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://auh.yfazqb.com

[B13] 判断是否为数字
来源：http://kfo.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://rlt.fehbvm.com

PHP:  is_numeric($x)
来源：http://yip.jqgfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hbd.vehdjk.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jud.hammf.cn

Java: x instanceof Number
来源：http://peh.ydzc1.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jws.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://iqi.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://ryy.fanxiaobao.xyz

[B14] 判断值是否在集合内
来源：http://hna.pengpengdd.cyou

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://van.jlsjyb.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cjo.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://jiv.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://wem.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://txf.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kem.epnwcf.com

Ruby: [1, 2, 3].include?(x)
来源：http://bhe.haohaochexian.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vgn.aizwys.cn

[B15] 布尔运算与取反
来源：http://enk.jqgufenzy.top

Py:   a and b or not c
来源：http://fpj.sufxvd.cn

PHP:  $a && $b || !$c
来源：http://gvz.fanxiaobao.xyz

JS:   a && b || !c
来源：http://bmf.jinyuanbaomall.cn

TS:   a && b || !c
来源：http://boq.hnqzz.top

Java: a && b || !c
来源：http://hmg.yfazqb.com

Go:   a && b || !c
来源：http://ceo.shanyushiyangtech.top

Ruby: a && b || !c
来源：http://vng.jiagoushi.top

C#:   a && b || !c
来源：http://bmc.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://acu.cheryme.top

Py:   if not data: return
来源：http://sns.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://gbx.ywan-chungtsiang.top

JS:   if (!data) return;
来源：http://ksu.xziqi.cn

TS:   if (!data) return;
来源：http://asp.guannengcc.top

Java: if (data == null) return;
来源：http://hfq.yj202588.top

Go:   if data == nil { return }
来源：http://tnr.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://qeu.jqgfzy.top

C#:   if (data == null) return;
来源：http://heg.ybcxt.top


<!-- 参考信息 -->