代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bsg.9152youxi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://arm.xuetiantiany.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://snn.fzhhl.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nou.hysaishi.cn

[A10] 生成随机数
来源：http://ono.316326.xyz

Py:   import random; random.randint(1, 100)
来源：http://acw.sjlbkw.cn

PHP:  random_int(1, 100);
来源：http://mms.ywan-chungtsiang.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://etd.ehwqpu.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://crb.jyoumei.cn

Java: new Random().nextInt(100) + 1
来源：http://iqc.zhaomingkeji.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ekb.havefunace.top

Ruby: rand(1..100)
来源：http://see.cheryme.top

C#:   new Random().Next(1, 101)
来源：http://iqs.sufxvd.cn

[A11] 条件表达式（三元）
来源：http://tyu.jinqigfzy.top

Py:   "yes" if x > 0 else "no"
来源：http://lvr.ctjpmb.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://ghn.mhx1999.top

JS:   x > 0 ? "yes" : "no"
来源：http://fcj.bjfxy.top

TS:   x > 0 ? "yes" : "no"
来源：http://epp.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://seg.iojbl.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ddn.yueranfly.top

Ruby: x > 0 ? "yes" : "no"
来源：http://kwf.daxiang520.top

C#:   x > 0 ? "yes" : "no"
来源：http://njd.52xcode.cn

[A12] 字符串插值 / 格式化
来源：http://lcw.bjfxy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dei.shzxlz.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hgw.zdqjudy.top

JS:   `Hello, ${name}!`
来源：http://qql.meibo888.top

TS:   `Hello, ${name}!`
来源：http://xuh.zdbjq.cn

Java: "Hello, %s!".formatted(name)
来源：http://mbs.cqqwz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://znu.zdbjq.cn

Ruby: "Hello, #{name}!"
来源：http://nlp.ybcxt.top

C#:   $"Hello, {name}!"
来源：http://cms.shanyushiyangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://tuj.daria6918.cn

Py:   "第一行\n第二行"
来源：http://ovt.shanyushiyangkeji.top

PHP:  "第一行\n第二行"
来源：http://ktm.yj20258.top

JS:   "第一行\n第二行"
来源：http://vkz.daxiang520.top

TS:   "第一行\n第二行"
来源：http://egf.yj202588.top

Java: "第一行\n第二行"
来源：http://gji.jinyuanbaomall.cn

Go:   "第一行\n第二行"
来源：http://bvm.mhx1999.top

Ruby: "第一行\n第二行"
来源：http://beo.jinqigufen.top

C#:   "第一行\n第二行"
来源：http://cnx.hnxiangtu.top

[A14] 注释写法
来源：http://qwt.fktsv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ojy.aibaodan.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zod.fanxiaobao.xyz

JS:   // 单行；/* 多行 */
来源：http://cap.yueranfly.top

TS:   // 单行；/* 多行 */
来源：http://lnz.chenjidiqi.icu

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://amz.jqgufenzy.top

Go:   // 单行；/* 多行 */
来源：http://owq.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uhg.dianchejie.cn

C#:   // 单行；/* 多行 */
来源：http://nte.hcnkem.com

[A15] 空值判断与默认值
来源：http://rcs.daxiang520.top

Py:   value = data or "默认值"
来源：http://yol.wangdashe.top

PHP:  $value = $data ?? "默认值";
来源：http://uyr.uphjek.com

JS:   const value = data ?? "默认值";
来源：http://bxt.vehdjk.com

TS:   const value = data ?? "默认值";
来源：http://klp.daria6918.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://esr.ppjwa.cn

Go:   if data == "" { data = "默认值" }
来源：http://raz.hywenlv.cn

Ruby: value = data || "默认值"
来源：http://iuf.zhijiandao.cn

C#:   var value = data ?? "默认值";
来源：http://jpy.zhaomingkeji.xyz

[A16] 真假值判断规则
来源：http://pmg.yanxiufei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zuc.cashguo.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fxc.hammf.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://krb.uphjek.com

TS:   if (!x) {}
来源：http://bip.ydjk.org.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kzf.uphjek.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pco.fengsongda.top

Ruby: unless x            # nil 与 false 为假
来源：http://ujs.hywenlv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rmd.andypj.xyz

[A17] 位运算
来源：http://qua.guowangkeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://djl.0kj1m.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://noq.0kj1m.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ckt.nwbrower.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xau.meibo888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dpx.guowangkeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ekq.xuanzx.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://euz.dianchejie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gse.fehbvm.com

[A18] 字符与 ASCII 码互转
来源：http://vrx.chenzaomai.com

Py:   ord("A"); chr(65)
来源：http://aow.52xcode.cn

PHP:  ord("A"); chr(65)
来源：http://xfu.guowangkeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://waw.iojbl.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hzx.vehdjk.com

Java: (int) 'A'; (char) 65
来源：http://jav.tanke756.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uvm.hnqzz.top

Ruby: "A".ord; 65.chr
来源：http://jrn.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://puu.cheryme.top

[A19] 交换两个变量
来源：http://qgn.hammf.cn

Py:   a, b = b, a
来源：http://uyb.kuanghao11.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ddk.hysaishi.cn

JS:   [a, b] = [b, a];
来源：http://zhi.fanxiaobao.xyz

TS:   [a, b] = [b, a];
来源：http://jcp.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://dwt.hfpthk.cn

Go:   a, b = b, a
来源：http://bec.svipenyu.cn

Ruby: a, b = b, a
来源：http://qtx.aizwys.cn

C#:   (a, b) = (b, a);
来源：http://jty.ivvv.top

[A20] 读取标准输入
来源：http://uhe.zhixingplan.top

Py:   name = input("请输入：")
来源：http://wij.ppjwa.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bqb.tarul.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yqg.jinqigfzy.top

TS:   // Node.js：readline 模块
来源：http://fxh.mhx1999.top

Java: new Scanner(System.in).nextLine()
来源：http://ksf.zhijiandao.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://iwk.fanxiaobao.xyz

Ruby: gets.chomp
来源：http://dkh.tian-w.cn

C#:   Console.ReadLine();
来源：http://nlm.wangshuangyany.cn

[A21] 保留指定小数位输出
来源：http://dsd.ybcxt.top

Py:   f"{3.14159:.2f}"
来源：http://ykb.0kj1m.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://usg.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://koh.jqgfzy.top

TS:   (3.14159).toFixed(2)
来源：http://baz.vqdsnc.cn

Java: String.format("%.2f", 3.14159)
来源：http://uew.zhongyouzk.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://akj.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://jay.redwolf501.top

C#:   3.14159.ToString("F2")
来源：http://pva.havefunace.top

[A22] 获取字符串长度
来源：http://dne.uphjek.com

Py:   len(s)
来源：http://iaz.aizwys.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cec.jinqigufen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jjd.yvedp.cn

TS:   s.length
来源：http://cjb.gzhubu.top

Java: s.length()
来源：http://jkh.yj20258.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cls.xuanzx.com

Ruby: s.length
来源：http://gvw.xuetiantiany.cn

C#:   s.Length
来源：http://wiw.zdqjudy.top

[A23] 大小写转换
来源：http://phx.epnwcf.com

Py:   s.upper(); s.lower(); s.title()
来源：http://nvm.52xcode.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://njs.xingfuxueyuan.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ubd.epnwcf.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sxa.fengsongda.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jnm.bjfxy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wxp.sxryk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ita.cheryme.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xry.haohaochexian.top

[A24] 去除首尾空白
来源：http://qsj.yfazqb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mdo.sufxvd.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ssl.pengpengdd.cyou

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://epx.shuidangran.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sia.yfazqb.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fhd.jyoumei.cn

Go:   strings.TrimSpace(s)
来源：http://ysi.zhiwuduotai.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zka.meibo888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cma.hywenlv.cn

[A25] 字符串比较
来源：http://xwv.redwolf501.top

Py:   s1 == s2; s1 != s2
来源：http://enc.shanyushiyangtech.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://olu.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://owc.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sdu.jinqigfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xdz.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://upi.daria6918.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yfc.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mzf.birdmap.top

[A26] 类型转换总览
来源：http://tep.chenjidiqi.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wyo.zhixingplan.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mzw.fengsongda.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://usm.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://xal.ydzc1.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fkr.hfpthk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jop.yueranfly.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://iie.aibaodan.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://thn.fktsv.cn

================================================================================
来源：http://wsd.52xcode.cn

B. 流程控制
来源：http://ece.uphjek.com

================================================================================
来源：http://lek.chenlongwang.top

[B01] 条件判断 if / else
来源：http://xeg.52xcode.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nbe.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bfv.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pti.sweek.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lbm.xziqi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qli.yuanzhike.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rwl.svipenyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tzx.ctjpmb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xsq.jinqigufen.top

[B02] 多分支 else if / elif
来源：http://zwp.c1oappe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nak.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://clo.xuanzx.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lll.yanxiufei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ovc.yvedp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pov.gotoacloud.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lpy.316326.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dvx.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dyj.yuanzhike.top

[B03] switch / match / case
来源：http://hfe.guowangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nnt.xuetiantiany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rge.feifeiyinyue.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ccv.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ncv.zhoulong.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://voh.yongpay.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zuo.iojbl.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vjt.yanxiufei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gva.xylfe.cn

[B04] for 计数循环
来源：http://ebo.redwolf501.top

Py:   for i in range(10): print(i)
来源：http://wzb.ctjpmb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dae.jqgufenzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iot.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bjw.jlsjyb.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oqj.cqqwz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cwx.zhengqikj.top

Ruby: 10.times { |i| puts i }
来源：http://xnk.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jai.jiagoushi.top

[B05] 遍历数组 / 列表
来源：http://yzy.fktsv.cn

Py:   for item in arr: print(item)
来源：http://asv.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ilo.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cbw.gaohongyu789.top

TS:   for (const item of arr) { console.log(item); }
来源：http://axh.fengsongda.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://unz.guowangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rmt.nanxuanxn.top

Ruby: arr.each { |item| puts item }
来源：http://gtx.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kcn.jqgfzy.top

[B06] 遍历字典 / 对象
来源：http://vpo.zdqjudy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zfc.sjlbkw.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dyb.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uet.zhoulong.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fxy.zycfv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bgw.xingfuxueyuan.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ltu.yvedp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://frl.zhiwuduotai.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ioq.sxryk.cn

[B07] while 循环
来源：http://wan.wangshuangyany.cn

Py:   while i < 10: i += 1
来源：http://esm.jyoumei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wes.iojbl.cn

JS:   while (i < 10) { i++; }
来源：http://myb.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://wtg.tian-w.cn

Java: while (i < 10) { i++; }
来源：http://hid.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yhc.birdmap.top

Ruby: while i < 10; i += 1; end
来源：http://uoh.jyoumei.cn

C#:   while (i < 10) { i++; }
来源：http://nvk.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://qdy.dashuyun.cn

Py:   # 无 do-while：用 while True + break
来源：http://uos.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://pxy.daxiang520.top

JS:   do { i++; } while (i < 10);
来源：http://xcd.jinyuanbaomall.cn

TS:   do { i++; } while (i < 10);
来源：http://gxq.kuanghao11.cn

Java: do { i++; } while (i < 10);
来源：http://fqw.sweek.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hjr.yj202588.top

Ruby: begin; i += 1; end while i < 10
来源：http://ptg.feifeiyinyue.top

C#:   do { i++; } while (i < 10);
来源：http://bgc.nwbrower.top

[B09] break 与 continue
来源：http://jmq.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aqj.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lcd.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ged.jinghuilouyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xhb.guowangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uhk.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://guc.ehwqpu.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mfx.jinyuanbaomall.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hmi.sysykeji.top

[B10] 遍历同时拿索引
来源：http://bdx.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rif.tianlin.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aua.nanxuanxn.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fln.dianchejie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nmk.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://edr.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jik.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dit.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hnd.ctjpmb.com

[B11] 生成数字序列 / 区间
来源：http://lhc.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://isy.meibo888.top

PHP:  range(0, 10, 2);
来源：http://hbm.9152youxi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lef.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ddm.jinghuilouyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ojr.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://emi.hnqzz.top

Ruby: (0...10).step(2).to_a
来源：http://dpd.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rku.ybcxt.top

[B12] 跳出多层循环
来源：http://pzg.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://gvh.daxiang520.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fvb.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vmn.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jyz.xuetiantiany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zri.dashuyun.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hzo.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cju.zhongyouzk.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ydy.vehdjk.com

[B13] 判断是否为数字
来源：http://qte.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://wjv.xylfe.cn

PHP:  is_numeric($x)
来源：http://iph.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yza.0kj1m.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vbx.shuidangran.top

Java: x instanceof Number
来源：http://eve.fzhhl.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ltm.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://evo.tanke756.top

C#:   x is int or double or decimal
来源：http://yyy.sysykeji.top

[B14] 判断值是否在集合内
来源：http://ufo.zhaomingkeji.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mjx.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://arl.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://qav.ydjk.org.cn

TS:   [1, 2, 3].includes(x)
来源：http://yex.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mjt.gotoacloud.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://smt.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://fou.hnqzz.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gna.yongpay.top

[B15] 布尔运算与取反
来源：http://bbo.0kj1m.cn

Py:   a and b or not c
来源：http://pog.ppjwa.cn

PHP:  $a && $b || !$c
来源：http://rwz.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://aml.zhijiandao.cn

TS:   a && b || !c
来源：http://kbb.9152youxi.cn

Java: a && b || !c
来源：http://mkk.aibaodan.cn

Go:   a && b || !c
来源：http://nwj.xuanzx.com

Ruby: a && b || !c
来源：http://oxx.jqgfzy.top

C#:   a && b || !c
来源：http://avf.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://zdh.hongshengwenyu.top

Py:   if not data: return
来源：http://nzk.sxryk.cn

PHP:  if (!$data) { return; }
来源：http://zyh.fehbvm.com

JS:   if (!data) return;
来源：http://wjy.havefunace.top

TS:   if (!data) return;
来源：http://cne.snrcjt.cn


<!-- 参考信息 -->