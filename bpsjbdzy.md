代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gmx.yanxiufei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xcq.shuidangran.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://waa.shanyushiyangtech.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eef.hysaishi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://abb.shangyingyoupin.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wkb.iojbl.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eox.bjfxy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pgv.sjlbkw.cn

[A10] 生成随机数
来源：http://rxy.guannengcc.top

Py:   import random; random.randint(1, 100)
来源：http://gso.gogol.net.cn

PHP:  random_int(1, 100);
来源：http://aye.jyoumei.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rlg.feifeiyinyue.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://enh.yj202588.top

Java: new Random().nextInt(100) + 1
来源：http://hhe.yj20258.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oxc.zdqjudy.top

Ruby: rand(1..100)
来源：http://yhr.zhijiandao.cn

C#:   new Random().Next(1, 101)
来源：http://afd.smart0.xyz

[A11] 条件表达式（三元）
来源：http://yll.kuanghao11.cn

Py:   "yes" if x > 0 else "no"
来源：http://jay.gogol.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qoo.mhx1999.top

JS:   x > 0 ? "yes" : "no"
来源：http://lqx.ivvv.top

TS:   x > 0 ? "yes" : "no"
来源：http://mbd.wangshuangyany.cn

Java: x > 0 ? "yes" : "no"
来源：http://uqj.daria6918.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hxr.hongshengwenyu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ukt.9152youxi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tah.sweek.top

[A12] 字符串插值 / 格式化
来源：http://kfo.sysykeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tpb.iojbl.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cyp.gotoacloud.top

JS:   `Hello, ${name}!`
来源：http://bmp.ctjpmb.com

TS:   `Hello, ${name}!`
来源：http://eqm.yj20258888.top

Java: "Hello, %s!".formatted(name)
来源：http://qaj.jianghu66.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xlz.xinyue.icu

Ruby: "Hello, #{name}!"
来源：http://nil.feifeiyinyue.top

C#:   $"Hello, {name}!"
来源：http://sqf.ywan-chungtsiang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://riw.shanyushiyangtech.top

Py:   "第一行\n第二行"
来源：http://tnz.kuanghao11.cn

PHP:  "第一行\n第二行"
来源：http://pvy.sufxvd.cn

JS:   "第一行\n第二行"
来源：http://swo.zhengqikj.top

TS:   "第一行\n第二行"
来源：http://ftz.quarkkingdee.top

Java: "第一行\n第二行"
来源：http://xsr.xziqi.cn

Go:   "第一行\n第二行"
来源：http://szg.9152youxi.cn

Ruby: "第一行\n第二行"
来源：http://cdo.fengsongda.top

C#:   "第一行\n第二行"
来源：http://sqb.jlsjyb.cn

[A14] 注释写法
来源：http://sup.havefunace.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://hwc.chenlongwang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://idk.jinqigufen.top

JS:   // 单行；/* 多行 */
来源：http://mgq.jianghu66.top

TS:   // 单行；/* 多行 */
来源：http://ybs.mhx1999.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ijy.nwbrower.top

Go:   // 单行；/* 多行 */
来源：http://ycz.epnwcf.com

Ruby: # 单行；=begin 多行 =end
来源：http://pbg.shanyushiyangkeji.top

C#:   // 单行；/* 多行 */
来源：http://zjy.yj20258888.top

[A15] 空值判断与默认值
来源：http://gsh.tarul.cn

Py:   value = data or "默认值"
来源：http://kom.iojbl.cn

PHP:  $value = $data ?? "默认值";
来源：http://jyl.hongshengwenyu.top

JS:   const value = data ?? "默认值";
来源：http://nra.jiagoushi.top

TS:   const value = data ?? "默认值";
来源：http://ozv.sweek.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ejx.xinyue.icu

Go:   if data == "" { data = "默认值" }
来源：http://jqo.shuidangran.top

Ruby: value = data || "默认值"
来源：http://rje.hammf.cn

C#:   var value = data ?? "默认值";
来源：http://rrz.hesvh.cn

[A16] 真假值判断规则
来源：http://dib.yvedp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://phv.sweek.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lty.wangshuangyany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cab.guowangkeji.top

TS:   if (!x) {}
来源：http://fyw.uphjek.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hca.0kj1m.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ubn.guowangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://phr.zhengqikj.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dqt.jinqigufen.top

[A17] 位运算
来源：http://bug.fzhhl.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jbq.yuanzhike.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yar.tanke756.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oqb.ppjwa.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ach.guowangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fxt.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ozk.chenjidiqi.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nhn.tanke756.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://spx.hammf.cn

[A18] 字符与 ASCII 码互转
来源：http://oly.sxryk.cn

Py:   ord("A"); chr(65)
来源：http://dfz.hcnkem.com

PHP:  ord("A"); chr(65)
来源：http://ejx.jqgfzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dng.chenlongwang.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://plq.meibo888.top

Java: (int) 'A'; (char) 65
来源：http://zvp.ydzc1.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nwt.ywan-chungtsiang.top

Ruby: "A".ord; 65.chr
来源：http://uph.jlsjyb.cn

C#:   (int)'A'; (char)65
来源：http://trb.shzxlz.cn

[A19] 交换两个变量
来源：http://qga.wangdashe.top

Py:   a, b = b, a
来源：http://kqa.zycfv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hgg.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://ygi.guowangkeji.top

TS:   [a, b] = [b, a];
来源：http://xex.hywenlv.cn

Java: int t = a; a = b; b = t;
来源：http://yuz.hnqzz.top

Go:   a, b = b, a
来源：http://sbe.ehwqpu.com

Ruby: a, b = b, a
来源：http://zxc.hysaishi.cn

C#:   (a, b) = (b, a);
来源：http://vev.zhixingplan.top

[A20] 读取标准输入
来源：http://bqy.yonumen.top

Py:   name = input("请输入：")
来源：http://kwa.jqgfzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ttp.yonumen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eae.c1oappe.top

TS:   // Node.js：readline 模块
来源：http://hrv.yfazqb.com

Java: new Scanner(System.in).nextLine()
来源：http://qmy.jinqigufen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hzh.0kj1m.cn

Ruby: gets.chomp
来源：http://vio.yj20258.top

C#:   Console.ReadLine();
来源：http://sse.jinghuilouyu.cn

[A21] 保留指定小数位输出
来源：http://qmp.zhoulong.xyz

Py:   f"{3.14159:.2f}"
来源：http://bjo.dianchejie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qzr.jyoumei.cn

JS:   (3.14159).toFixed(2)
来源：http://eld.zhoulong.xyz

TS:   (3.14159).toFixed(2)
来源：http://tko.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://piy.fanxiaobao.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ldk.tanke756.top

Ruby: format("%.2f", 3.14159)
来源：http://jrx.xylfe.cn

C#:   3.14159.ToString("F2")
来源：http://pzj.meibo888.top

[A22] 获取字符串长度
来源：http://qbi.fanxiaobao.xyz

Py:   len(s)
来源：http://iha.zhengqikj.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kck.chenzaomai.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oki.xingfuxueyuan.xyz

TS:   s.length
来源：http://voi.zdqjudy.top

Java: s.length()
来源：http://lsb.dashuyun.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bwg.0kj1m.cn

Ruby: s.length
来源：http://lbx.gaohongyu789.top

C#:   s.Length
来源：http://wva.andypj.xyz

[A23] 大小写转换
来源：http://wsm.xziqi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vqt.hcnkem.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://snj.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pnk.hnqzz.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qeo.dashuyun.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fmz.gzhubu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xvi.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ilw.shzxlz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bzm.316326.xyz

[A24] 去除首尾空白
来源：http://lyw.chenlongwang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oxe.shzxlz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rmy.svipenyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zbf.yangfankeji.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rmw.yongpay.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tem.guannengcc.top

Go:   strings.TrimSpace(s)
来源：http://wln.aizwys.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bqr.0kj1m.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lai.wangdashe.top

[A25] 字符串比较
来源：http://phz.jyoumei.cn

Py:   s1 == s2; s1 != s2
来源：http://ond.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://umw.hcnkem.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://juf.yongpay.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xze.zhaomingkeji.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wlm.cashguo.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bqe.cdnleiting.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ikp.birdmap.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aow.smart0.xyz

[A26] 类型转换总览
来源：http://nsj.pengpengdd.cyou

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pzz.jlsjyb.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rgj.ppjwa.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tgp.shanyushiyangtech.top

TS:   Number() String() Boolean() x as number
来源：http://wfk.xuanzx.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bto.aizwys.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rjg.c1oappe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wpm.yj20258888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fsl.meibo888.top

================================================================================
来源：http://ntg.aizwys.cn

B. 流程控制
来源：http://huy.meibo888.top

================================================================================
来源：http://uqd.ywan-chungtsiang.top

[B01] 条件判断 if / else
来源：http://wwn.ehwqpu.com

Py:   result = "正" if x > 0 else "非正"
来源：http://bll.iojbl.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ufw.yonumen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qdv.jlsjyb.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://omx.uphjek.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://yto.cucudq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://plo.vehdjk.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://euq.zhongyouzk.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hyy.shuidangran.top

[B02] 多分支 else if / elif
来源：http://owd.hongshengwenyu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ssl.fktsv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pih.svipenyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gir.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jqr.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gqq.sweek.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bjy.nanxinkj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pll.andypj.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jlg.yj20258.top

[B03] switch / match / case
来源：http://vdt.fktsv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zfn.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vsj.shuidangran.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pwb.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ptv.hysaishi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tlj.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://acm.hysaishi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://prn.mhx1999.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uuz.jinqigfzy.top

[B04] for 计数循环
来源：http://wlk.jinqigfzy.top

Py:   for i in range(10): print(i)
来源：http://okf.jinghuilouyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ich.c1oappe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zyh.fktsv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://imh.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nep.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ouf.zhijiandao.cn

Ruby: 10.times { |i| puts i }
来源：http://chp.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uth.hysaishi.cn

[B05] 遍历数组 / 列表
来源：http://fxg.ybcxt.top

Py:   for item in arr: print(item)
来源：http://szt.316326.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kqf.ppjwa.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mot.zdbjq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rre.jiagoushi.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xos.yanxiufei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://buz.9152youxi.cn

Ruby: arr.each { |item| puts item }
来源：http://rrs.sjlbkw.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rfb.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://uid.hammf.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hzb.nanxinkj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lwv.yfazqb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://khr.ybcxt.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wlb.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://upt.svipenyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rmv.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qcw.haohaochexian.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pdg.cheryme.top

[B07] while 循环
来源：http://sgv.yuanzhike.top

Py:   while i < 10: i += 1
来源：http://vnu.zhixingplan.top

PHP:  while ($i < 10) { $i++; }
来源：http://tuz.yanxiufei.cn

JS:   while (i < 10) { i++; }
来源：http://szy.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://qzs.yj202588.top

Java: while (i < 10) { i++; }
来源：http://ekl.meibo888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://utu.shzxlz.cn

Ruby: while i < 10; i += 1; end
来源：http://sil.birdmap.top

C#:   while (i < 10) { i++; }
来源：http://zah.svipenyu.cn

[B08] do-while（至少执行一次）
来源：http://vgu.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://joe.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tms.zdqjudy.top

JS:   do { i++; } while (i < 10);
来源：http://nsv.meibo888.top

TS:   do { i++; } while (i < 10);
来源：http://tud.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://yir.jlsjyb.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ppn.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://ygq.xziqi.cn

C#:   do { i++; } while (i < 10);
来源：http://hmp.jinghuilouyu.cn

[B09] break 与 continue
来源：http://iam.xinyue.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://chf.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bjy.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wrv.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://edi.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mqu.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jat.ivvv.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cts.dianchejie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qdq.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://vbf.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fhr.zhiwuduotai.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sus.aibaodan.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pjb.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://woq.jiagoushi.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fsz.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://axf.guowangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bdm.tianlin.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qae.iojbl.cn

[B11] 生成数字序列 / 区间
来源：http://hih.guannengcc.top

Py:   list(range(0, 10, 2))
来源：http://vgm.xinyue.icu

PHP:  range(0, 10, 2);
来源：http://mqq.ywan-chungtsiang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xiw.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qci.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://chg.aibaodan.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fgk.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://juv.cheryme.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tiy.nanxinkj.top

[B12] 跳出多层循环
来源：http://zau.ywan-chungtsiang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://plq.shangyingyoupin.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://utq.ybcxt.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jci.zhongyouzk.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://avd.tanke756.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ihs.zhengqikj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xrb.cdnleiting.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iuo.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://egr.dianchejie.cn

[B13] 判断是否为数字
来源：http://pxh.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://hqe.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://rky.hnqzz.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wuu.sxryk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://alm.andypj.xyz

Java: x instanceof Number
来源：http://hyw.bbcook.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lvp.yangfankeji.com

Ruby: x.is_a?(Numeric)
来源：http://ztb.xylfe.cn

C#:   x is int or double or decimal
来源：http://ant.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://lal.tanke756.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://smn.shzxlz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yzq.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://oyy.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://abf.0kj1m.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vgp.cdnleiting.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ltl.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://mbu.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yem.ctjpmb.com

[B15] 布尔运算与取反
来源：http://wup.nanxuanxn.top

Py:   a and b or not c
来源：http://hbm.chenjidiqi.icu

PHP:  $a && $b || !$c
来源：http://oaz.gogol.net.cn

JS:   a && b || !c
来源：http://ucn.jianghu66.top

TS:   a && b || !c
来源：http://fzx.redwolf501.top

Java: a && b || !c
来源：http://pgv.jinqigufen.top

Go:   a && b || !c
来源：http://xbe.cucudq.cn

Ruby: a && b || !c
来源：http://fzk.yueranfly.top

C#:   a && b || !c
来源：http://epz.jqgufenzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://qjp.c1oappe.top


<!-- 参考信息 -->