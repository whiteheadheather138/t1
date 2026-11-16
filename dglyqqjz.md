代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oju.jinghuilouyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bhn.zhongyouzk.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vxi.jinyuanbaomall.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lym.cqqwz.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fqi.cdnleiting.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ovz.xuetiantiany.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wdu.jinyuanbaomall.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jax.smart0.xyz

[A10] 生成随机数
来源：http://mmv.haohaochexian.top

Py:   import random; random.randint(1, 100)
来源：http://dug.shzxlz.cn

PHP:  random_int(1, 100);
来源：http://esn.xuetiantiany.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ydu.fengsongda.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rmc.jlsjyb.cn

Java: new Random().nextInt(100) + 1
来源：http://nmr.chenlongwang.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fnh.jinghuilouyu.cn

Ruby: rand(1..100)
来源：http://ipx.52xcode.cn

C#:   new Random().Next(1, 101)
来源：http://jnl.chenlongwang.top

[A11] 条件表达式（三元）
来源：http://naz.bbcook.cn

Py:   "yes" if x > 0 else "no"
来源：http://bbx.cdnleiting.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://dmz.ppjwa.cn

JS:   x > 0 ? "yes" : "no"
来源：http://szi.jqgufenzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://qrb.fehbvm.com

Java: x > 0 ? "yes" : "no"
来源：http://vad.zhixingplan.top

Go:   // 无三元运算符，需用 if 语句
来源：http://nwu.yueranfly.top

Ruby: x > 0 ? "yes" : "no"
来源：http://rlb.sweek.top

C#:   x > 0 ? "yes" : "no"
来源：http://xvi.quarkkingdee.top

[A12] 字符串插值 / 格式化
来源：http://xtz.dianchejie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mhx.shuidangran.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sao.9152youxi.cn

JS:   `Hello, ${name}!`
来源：http://pcd.uphjek.com

TS:   `Hello, ${name}!`
来源：http://vdc.52xcode.cn

Java: "Hello, %s!".formatted(name)
来源：http://uac.yueranfly.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yth.hfpthk.cn

Ruby: "Hello, #{name}!"
来源：http://kci.yuanzhike.top

C#:   $"Hello, {name}!"
来源：http://gut.hfpthk.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zpz.zhongyouzk.top

Py:   "第一行\n第二行"
来源：http://jql.jlsjyb.cn

PHP:  "第一行\n第二行"
来源：http://ojb.havefunace.top

JS:   "第一行\n第二行"
来源：http://ily.fengsongda.top

TS:   "第一行\n第二行"
来源：http://zkk.cashguo.top

Java: "第一行\n第二行"
来源：http://cqe.yongpay.top

Go:   "第一行\n第二行"
来源：http://him.uphjek.com

Ruby: "第一行\n第二行"
来源：http://faq.ywan-chungtsiang.top

C#:   "第一行\n第二行"
来源：http://cau.52xcode.cn

[A14] 注释写法
来源：http://ifz.sweek.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ufj.xinyue.icu

PHP:  // 或 # 单行；/* 多行 */
来源：http://ppu.hfpthk.cn

JS:   // 单行；/* 多行 */
来源：http://jqr.bjfxy.top

TS:   // 单行；/* 多行 */
来源：http://qgl.jianghu66.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lnw.cqqwz.cn

Go:   // 单行；/* 多行 */
来源：http://eqp.sjlbkw.cn

Ruby: # 单行；=begin 多行 =end
来源：http://slp.yj20258888.top

C#:   // 单行；/* 多行 */
来源：http://imr.jqgfzy.top

[A15] 空值判断与默认值
来源：http://zdf.haohaochexian.top

Py:   value = data or "默认值"
来源：http://cts.jyoumei.cn

PHP:  $value = $data ?? "默认值";
来源：http://tqq.wangshuangyany.cn

JS:   const value = data ?? "默认值";
来源：http://fuz.xuanzx.com

TS:   const value = data ?? "默认值";
来源：http://dlv.xziqi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tkj.ehwqpu.com

Go:   if data == "" { data = "默认值" }
来源：http://pto.daxiang520.top

Ruby: value = data || "默认值"
来源：http://idt.yj20258.top

C#:   var value = data ?? "默认值";
来源：http://sbm.yj20258.top

[A16] 真假值判断规则
来源：http://rjh.hesvh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://unp.meibo888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ljb.yueranfly.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://noh.yuanzhike.top

TS:   if (!x) {}
来源：http://bmw.ivvv.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yki.aibaodan.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ovj.zhixingplan.top

Ruby: unless x            # nil 与 false 为假
来源：http://vao.yonumen.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ycy.jlsjyb.cn

[A17] 位运算
来源：http://mpw.andypj.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qtn.cucudq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tzp.yueranfly.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eof.kuanghao11.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uxg.hesvh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tgm.tianlin.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xmq.fzhhl.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uww.fanxiaobao.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hlv.shangyingyoupin.top

[A18] 字符与 ASCII 码互转
来源：http://abt.tanke756.top

Py:   ord("A"); chr(65)
来源：http://qtj.jinqigfzy.top

PHP:  ord("A"); chr(65)
来源：http://zlw.havefunace.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zjk.cucudq.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xeq.feifeiyinyue.top

Java: (int) 'A'; (char) 65
来源：http://emg.kuanghao11.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bjg.guowangkeji.top

Ruby: "A".ord; 65.chr
来源：http://jbq.pengpengdd.cyou

C#:   (int)'A'; (char)65
来源：http://ubt.vqdsnc.cn

[A19] 交换两个变量
来源：http://nvs.0kj1m.cn

Py:   a, b = b, a
来源：http://zrd.quarkkingdee.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pmg.yvedp.cn

JS:   [a, b] = [b, a];
来源：http://uqh.jianghu66.top

TS:   [a, b] = [b, a];
来源：http://baz.snrcjt.cn

Java: int t = a; a = b; b = t;
来源：http://wdq.zhoulong.xyz

Go:   a, b = b, a
来源：http://wqm.iojbl.cn

Ruby: a, b = b, a
来源：http://twx.cucudq.cn

C#:   (a, b) = (b, a);
来源：http://ojd.smart0.xyz

[A20] 读取标准输入
来源：http://icm.epnwcf.com

Py:   name = input("请输入：")
来源：http://bxi.feifeiyinyue.top

PHP:  $name = trim(fgets(STDIN));
来源：http://exd.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jqa.fengsongda.top

TS:   // Node.js：readline 模块
来源：http://nol.xuetiantiany.cn

Java: new Scanner(System.in).nextLine()
来源：http://obl.yuxming.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hrg.jiagoushi.top

Ruby: gets.chomp
来源：http://jsv.zhongyouzk.top

C#:   Console.ReadLine();
来源：http://oir.gaohongyu789.top

[A21] 保留指定小数位输出
来源：http://nrt.zhongyouzk.top

Py:   f"{3.14159:.2f}"
来源：http://tic.sweek.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yod.zhaomingkeji.xyz

JS:   (3.14159).toFixed(2)
来源：http://xtl.zhengqikj.top

TS:   (3.14159).toFixed(2)
来源：http://kqh.316326.xyz

Java: String.format("%.2f", 3.14159)
来源：http://hcz.ywan-chungtsiang.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ruf.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://rxp.sweek.top

C#:   3.14159.ToString("F2")
来源：http://imp.0kj1m.cn

[A22] 获取字符串长度
来源：http://xdr.hfpthk.cn

Py:   len(s)
来源：http://jqo.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rbq.uphjek.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eaj.zhiwuduotai.top

TS:   s.length
来源：http://mcq.bjfxy.top

Java: s.length()
来源：http://nge.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nqc.cheryme.top

Ruby: s.length
来源：http://ubo.zhixingplan.top

C#:   s.Length
来源：http://nat.epnwcf.com

[A23] 大小写转换
来源：http://nqf.hammf.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lae.fzhhl.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://plv.chenzaomai.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mlg.pycfn.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sye.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nbi.hywenlv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rxr.gaohongyu789.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pcy.zdbjq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dxl.chenzaomai.com

[A24] 去除首尾空白
来源：http://ify.haohaochexian.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zjz.xylfe.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jkb.ppjwa.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://exl.hfpthk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hcp.aizwys.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ula.ydzc1.top

Go:   strings.TrimSpace(s)
来源：http://wpx.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qdh.cashguo.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qwl.hcnkem.com

[A25] 字符串比较
来源：http://bwv.ydjk.org.cn

Py:   s1 == s2; s1 != s2
来源：http://pva.yuanzhike.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ehs.daria6918.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qsr.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cqb.tianlin.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ldb.ctjpmb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hnt.feifeiyinyue.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fio.sweek.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tkj.birdmap.top

[A26] 类型转换总览
来源：http://bos.xingfuxueyuan.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oiv.xuetiantiany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tlh.chenlongwang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kaa.xziqi.cn

TS:   Number() String() Boolean() x as number
来源：http://jnf.shanyushiyangtech.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gbr.sweek.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://awd.tian-w.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wsv.meibo888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vql.wangshuangyany.cn

================================================================================
来源：http://iil.ppjwa.cn

B. 流程控制
来源：http://kga.fanxiaobao.xyz

================================================================================
来源：http://hbk.guannengcc.top

[B01] 条件判断 if / else
来源：http://fks.zhongyouzk.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rck.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nwy.yuanzhike.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yht.ydjk.org.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gla.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jtz.sufxvd.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://swm.jinyuanbaomall.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pwl.smart0.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lfp.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://ymw.jqgfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uzj.ehwqpu.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zwa.sweek.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://als.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gjc.zdbjq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pma.tarul.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oby.zdqjudy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vns.ivvv.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://din.yueranfly.top

[B03] switch / match / case
来源：http://gek.cqqwz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jcb.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zcq.xuetiantiany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mcu.fzhhl.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hyh.yvedp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ynj.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://czd.fanxiaobao.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ynr.wangshuangyany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uxz.tian-w.cn

[B04] for 计数循环
来源：http://dun.sufxvd.cn

Py:   for i in range(10): print(i)
来源：http://nmj.gogol.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lyy.cqqwz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xtk.zhongyouzk.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gjp.hywenlv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kyp.yuanzhike.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://krt.tianlin.xyz

Ruby: 10.times { |i| puts i }
来源：http://olr.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vzq.316326.xyz

[B05] 遍历数组 / 列表
来源：http://rub.xylfe.cn

Py:   for item in arr: print(item)
来源：http://euj.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cgn.yj20258.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cpt.sweek.top

TS:   for (const item of arr) { console.log(item); }
来源：http://iuj.tian-w.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zno.xinyue.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pkb.sxryk.cn

Ruby: arr.each { |item| puts item }
来源：http://mme.mhx1999.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://icz.316326.xyz

[B06] 遍历字典 / 对象
来源：http://jpe.redwolf501.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wht.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kbp.yongpay.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ser.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xyy.svipenyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wra.chenlongwang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://shh.hongshengwenyu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wes.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nau.yanxiufei.cn

[B07] while 循环
来源：http://lfa.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://adl.bjfxy.top

PHP:  while ($i < 10) { $i++; }
来源：http://zev.yj20258.top

JS:   while (i < 10) { i++; }
来源：http://uth.jqgufenzy.top

TS:   while (i < 10) { i++; }
来源：http://lwn.yuxming.cn

Java: while (i < 10) { i++; }
来源：http://odc.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nol.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://sjy.zycfv.cn

C#:   while (i < 10) { i++; }
来源：http://xje.epnwcf.com

[B08] do-while（至少执行一次）
来源：http://vcz.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://mmc.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mnz.jinyuanbaomall.cn

JS:   do { i++; } while (i < 10);
来源：http://yrv.cdnleiting.top

TS:   do { i++; } while (i < 10);
来源：http://teq.cheryme.top

Java: do { i++; } while (i < 10);
来源：http://ayx.ydjk.org.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nwz.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://wwo.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://nqs.yj20258888.top

[B09] break 与 continue
来源：http://aik.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pxr.snrcjt.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mcj.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jui.hongshengwenyu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://agu.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ihz.shangyingyoupin.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://clg.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tej.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wdi.zhixingplan.top

[B10] 遍历同时拿索引
来源：http://jlf.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qms.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wgq.sxryk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dka.cucudq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lof.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rnd.yj20258.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gdh.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yyt.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hfo.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://rey.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://ijd.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://pbc.yangfankeji.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jto.daria6918.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dih.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bkw.haohaochexian.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ime.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://xbb.shuidangran.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ndm.haohaochexian.top

[B12] 跳出多层循环
来源：http://aic.nwbrower.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rcg.hnxiangtu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ffh.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wpb.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fwn.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kam.cdnleiting.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://smb.xylfe.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uvn.jinghuilouyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ysb.ydzc1.top

[B13] 判断是否为数字
来源：http://gvp.shuidangran.top

Py:   isinstance(x, (int, float))
来源：http://juj.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://mgx.havefunace.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yvb.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zsn.uphjek.com

Java: x instanceof Number
来源：http://vwp.jinghuilouyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rpp.zdqjudy.top

Ruby: x.is_a?(Numeric)
来源：http://yiv.zhoulong.xyz

C#:   x is int or double or decimal
来源：http://aea.nwbrower.top

[B14] 判断值是否在集合内
来源：http://tsk.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://giw.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://idc.pengpengdd.cyou

JS:   [1, 2, 3].includes(x)
来源：http://psi.quarkkingdee.top

TS:   [1, 2, 3].includes(x)
来源：http://rkc.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://axs.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fvr.sysykeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://dad.c1oappe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hli.epnwcf.com

[B15] 布尔运算与取反
来源：http://nwn.ydjk.org.cn

Py:   a and b or not c
来源：http://srx.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://yaq.xuanzx.com

JS:   a && b || !c
来源：http://yfs.pycfn.com

TS:   a && b || !c
来源：http://khi.yvedp.cn

Java: a && b || !c
来源：http://acp.jinghuilouyu.cn

Go:   a && b || !c
来源：http://geh.zhengqikj.top

Ruby: a && b || !c
来源：http://yhp.316326.xyz

C#:   a && b || !c
来源：http://dir.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wbu.kuanghao11.cn


<!-- 参考信息 -->