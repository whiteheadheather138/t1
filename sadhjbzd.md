代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gfh.hammf.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qzm.vqdsnc.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://saa.ehwqpu.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rte.shanyushiyangtech.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://syf.chenjidiqi.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jek.sufxvd.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://epk.xuanzx.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fes.xylfe.cn

[A10] 生成随机数
来源：http://bqw.shanyushiyangkeji.top

Py:   import random; random.randint(1, 100)
来源：http://gwb.bjfxy.top

PHP:  random_int(1, 100);
来源：http://tuw.bjfxy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vlj.ehwqpu.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ijr.xylfe.cn

Java: new Random().nextInt(100) + 1
来源：http://vdz.jyoumei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ysz.cdnleiting.top

Ruby: rand(1..100)
来源：http://nmo.aibaodan.cn

C#:   new Random().Next(1, 101)
来源：http://xdv.dianchejie.cn

[A11] 条件表达式（三元）
来源：http://vsv.redwolf501.top

Py:   "yes" if x > 0 else "no"
来源：http://cmy.pengpengdd.cyou

PHP:  $x > 0 ? "yes" : "no"
来源：http://bxs.sjlbkw.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hak.ybcxt.top

TS:   x > 0 ? "yes" : "no"
来源：http://xov.hnqzz.top

Java: x > 0 ? "yes" : "no"
来源：http://ajm.wangshuangyany.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ifd.jqgufenzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://cjc.zhiwuduotai.top

C#:   x > 0 ? "yes" : "no"
来源：http://wqs.ivvv.top

[A12] 字符串插值 / 格式化
来源：http://oxl.xingfuxueyuan.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mzx.yangfankeji.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tqj.havefunace.top

JS:   `Hello, ${name}!`
来源：http://aja.hysaishi.cn

TS:   `Hello, ${name}!`
来源：http://mux.snrcjt.cn

Java: "Hello, %s!".formatted(name)
来源：http://ebk.dianchejie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tgk.bbcook.cn

Ruby: "Hello, #{name}!"
来源：http://vwa.wangdashe.top

C#:   $"Hello, {name}!"
来源：http://soa.quarkkingdee.top

[A13] 多行字符串（练习 \n 转义）
来源：http://uwb.ctjpmb.com

Py:   "第一行\n第二行"
来源：http://pxx.zhoulong.xyz

PHP:  "第一行\n第二行"
来源：http://kya.hysaishi.cn

JS:   "第一行\n第二行"
来源：http://jii.jqgfzy.top

TS:   "第一行\n第二行"
来源：http://til.hnxiangtu.top

Java: "第一行\n第二行"
来源：http://dxz.vehdjk.com

Go:   "第一行\n第二行"
来源：http://tyy.jinyuanbaomall.cn

Ruby: "第一行\n第二行"
来源：http://dvu.cqqwz.cn

C#:   "第一行\n第二行"
来源：http://aab.gzhubu.top

[A14] 注释写法
来源：http://esy.chenjidiqi.icu

Py:   # 单行；三引号字符串可作多行说明
来源：http://qmt.pycfn.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://evm.xziqi.cn

JS:   // 单行；/* 多行 */
来源：http://swo.jqgufenzy.top

TS:   // 单行；/* 多行 */
来源：http://rsu.jiagoushi.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rlb.tarul.cn

Go:   // 单行；/* 多行 */
来源：http://umc.cdnleiting.top

Ruby: # 单行；=begin 多行 =end
来源：http://kfp.jianghu66.top

C#:   // 单行；/* 多行 */
来源：http://qzw.yuxming.cn

[A15] 空值判断与默认值
来源：http://wkn.yvedp.cn

Py:   value = data or "默认值"
来源：http://ddw.haohaochexian.top

PHP:  $value = $data ?? "默认值";
来源：http://gad.birdmap.top

JS:   const value = data ?? "默认值";
来源：http://bnn.yfazqb.com

TS:   const value = data ?? "默认值";
来源：http://srw.andypj.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fht.ivvv.top

Go:   if data == "" { data = "默认值" }
来源：http://xtg.tianlin.xyz

Ruby: value = data || "默认值"
来源：http://xmz.zhaomingkeji.xyz

C#:   var value = data ?? "默认值";
来源：http://mob.aibaodan.cn

[A16] 真假值判断规则
来源：http://hbs.ppjwa.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fbl.vqdsnc.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lzh.shanyushiyangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://plg.ivvv.top

TS:   if (!x) {}
来源：http://epk.cdnleiting.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kos.xziqi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cli.redwolf501.top

Ruby: unless x            # nil 与 false 为假
来源：http://wxk.yj20258.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://weg.cdnleiting.top

[A17] 位运算
来源：http://qwv.xinyue.icu

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ybt.yvedp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hnl.yangfankeji.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ver.ppjwa.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ihd.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ivg.yanxiufei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ypj.cashguo.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ouc.jinghuilouyu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nob.feifeiyinyue.top

[A18] 字符与 ASCII 码互转
来源：http://xaj.tarul.cn

Py:   ord("A"); chr(65)
来源：http://ary.ctjpmb.com

PHP:  ord("A"); chr(65)
来源：http://onq.jinqigfzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ftf.cashguo.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sxy.shanyushiyangtech.top

Java: (int) 'A'; (char) 65
来源：http://egp.fzhhl.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://soe.nanxinkj.top

Ruby: "A".ord; 65.chr
来源：http://ogo.shanyushiyangkeji.top

C#:   (int)'A'; (char)65
来源：http://uim.xziqi.cn

[A19] 交换两个变量
来源：http://zvx.mhx1999.top

Py:   a, b = b, a
来源：http://xyb.jlsjyb.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ojr.bbcook.cn

JS:   [a, b] = [b, a];
来源：http://aog.aibaodan.cn

TS:   [a, b] = [b, a];
来源：http://tvy.hongshengwenyu.top

Java: int t = a; a = b; b = t;
来源：http://eww.yueranfly.top

Go:   a, b = b, a
来源：http://dvu.zdbjq.cn

Ruby: a, b = b, a
来源：http://ulw.xingfuxueyuan.xyz

C#:   (a, b) = (b, a);
来源：http://uqp.jiagoushi.top

[A20] 读取标准输入
来源：http://heh.316326.xyz

Py:   name = input("请输入：")
来源：http://uku.zycfv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://idn.ctjpmb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ghy.sjlbkw.cn

TS:   // Node.js：readline 模块
来源：http://ggc.snrcjt.cn

Java: new Scanner(System.in).nextLine()
来源：http://cdf.yuanzhike.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lgb.vqdsnc.cn

Ruby: gets.chomp
来源：http://qyy.zhengqikj.top

C#:   Console.ReadLine();
来源：http://zcg.yongpay.top

[A21] 保留指定小数位输出
来源：http://khz.tian-w.cn

Py:   f"{3.14159:.2f}"
来源：http://jbt.yueranfly.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pbx.zdbjq.cn

JS:   (3.14159).toFixed(2)
来源：http://vnr.yj20258.top

TS:   (3.14159).toFixed(2)
来源：http://fze.zhaomingkeji.xyz

Java: String.format("%.2f", 3.14159)
来源：http://msu.zhaomingkeji.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://orn.nwbrower.top

Ruby: format("%.2f", 3.14159)
来源：http://nbu.mhx1999.top

C#:   3.14159.ToString("F2")
来源：http://wyr.hnqzz.top

[A22] 获取字符串长度
来源：http://glf.zdbjq.cn

Py:   len(s)
来源：http://kcf.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jii.yongpay.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gen.nwbrower.top

TS:   s.length
来源：http://fkl.zhengqikj.top

Java: s.length()
来源：http://drf.redwolf501.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qrr.snrcjt.cn

Ruby: s.length
来源：http://acg.xuetiantiany.cn

C#:   s.Length
来源：http://jpa.xingfuxueyuan.xyz

[A23] 大小写转换
来源：http://omg.fanxiaobao.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://uqr.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://arm.ehwqpu.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nxo.yongpay.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oqs.ppjwa.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ewa.pengpengdd.cyou

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zsk.guowangkeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rsc.tanke756.top

C#:   s.ToUpper(); s.ToLower()
来源：http://wkz.zhaomingkeji.xyz

[A24] 去除首尾空白
来源：http://ljj.pycfn.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fhp.gzhubu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wtq.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hss.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dhr.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mfb.yj20258888.top

Go:   strings.TrimSpace(s)
来源：http://hwf.daria6918.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nqa.guowangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eid.jinqigfzy.top

[A25] 字符串比较
来源：http://ejf.yvedp.cn

Py:   s1 == s2; s1 != s2
来源：http://sld.jyoumei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://huw.hcnkem.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lav.jinqigufen.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wft.fzhhl.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xtm.vehdjk.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eur.shuidangran.top

Ruby: s1 == s2; s1 <=> s2
来源：http://zcc.ehwqpu.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hai.yj202588.top

[A26] 类型转换总览
来源：http://pcb.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tgh.vehdjk.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://igl.ehwqpu.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eqa.9152youxi.cn

TS:   Number() String() Boolean() x as number
来源：http://oto.hysaishi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wld.jqgfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ntm.jqgufenzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mmf.shzxlz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vxz.aizwys.cn

================================================================================
来源：http://tsk.dianchejie.cn

B. 流程控制
来源：http://osl.hfpthk.cn

================================================================================
来源：http://kde.xylfe.cn

[B01] 条件判断 if / else
来源：http://cqk.zhixingplan.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gqc.yueranfly.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uow.feifeiyinyue.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cnr.vqdsnc.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hgn.hammf.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tjz.guowangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://see.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wgb.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fat.zhiwuduotai.top

[B02] 多分支 else if / elif
来源：http://bya.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wke.gotoacloud.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ntq.ybcxt.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://slk.snrcjt.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xwm.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tsq.shzxlz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cfc.ybcxt.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mgp.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nwp.ehwqpu.com

[B03] switch / match / case
来源：http://ema.shzxlz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yov.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qsg.chenjidiqi.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ycb.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uie.c1oappe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dfw.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yuw.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pgb.hcnkem.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tbr.yongpay.top

[B04] for 计数循环
来源：http://wdl.tanke756.top

Py:   for i in range(10): print(i)
来源：http://byj.zhoulong.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cda.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://azy.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://amp.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sns.snrcjt.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fqx.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://nlx.zhiwuduotai.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eyo.jinqigfzy.top

[B05] 遍历数组 / 列表
来源：http://kpr.zycfv.cn

Py:   for item in arr: print(item)
来源：http://ssq.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zsd.ydjk.org.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fbj.ywan-chungtsiang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gta.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://myn.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dqp.hysaishi.cn

Ruby: arr.each { |item| puts item }
来源：http://edz.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uaa.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://haj.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wsg.0kj1m.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pgw.yanxiufei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fyi.tian-w.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pwv.gaohongyu789.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ryf.tanke756.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pfv.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uov.tian-w.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zob.ybcxt.top

[B07] while 循环
来源：http://xae.tarul.cn

Py:   while i < 10: i += 1
来源：http://khs.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://cwz.jlsjyb.cn

JS:   while (i < 10) { i++; }
来源：http://nqn.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://jgk.meibo888.top

Java: while (i < 10) { i++; }
来源：http://sfl.yueranfly.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ryx.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://uqs.haohaochexian.top

C#:   while (i < 10) { i++; }
来源：http://nyo.ywan-chungtsiang.top

[B08] do-while（至少执行一次）
来源：http://uks.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://lih.yvedp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gcc.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://ogy.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://yju.havefunace.top

Java: do { i++; } while (i < 10);
来源：http://gds.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lel.svipenyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mqf.hesvh.cn

C#:   do { i++; } while (i < 10);
来源：http://sxk.hnqzz.top

[B09] break 与 continue
来源：http://bzd.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jvv.tianlin.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jrx.ydjk.org.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rdl.sxryk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zsd.feifeiyinyue.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mho.shuidangran.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mdu.yuxming.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rqr.pycfn.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gdm.ybcxt.top

[B10] 遍历同时拿索引
来源：http://occ.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dhn.sweek.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uyr.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kix.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://plp.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uob.jinqigfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://erc.jinghuilouyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zbi.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ifw.fktsv.cn

[B11] 生成数字序列 / 区间
来源：http://ecs.cashguo.top

Py:   list(range(0, 10, 2))
来源：http://npv.zycfv.cn

PHP:  range(0, 10, 2);
来源：http://ryy.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yax.dashuyun.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ufh.gzhubu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mcz.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gbi.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://anx.gogol.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jae.zhongyouzk.top

[B12] 跳出多层循环
来源：http://msh.zhongyouzk.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dwr.svipenyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tcr.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dzb.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fdc.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qqh.gaohongyu789.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pci.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bsl.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://icv.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://bbo.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://xho.sxryk.cn

PHP:  is_numeric($x)
来源：http://syb.zdbjq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://otb.jinqigufen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bcr.iojbl.cn

Java: x instanceof Number
来源：http://mit.aizwys.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rfp.zhaomingkeji.xyz

Ruby: x.is_a?(Numeric)
来源：http://wsr.zhongyouzk.top

C#:   x is int or double or decimal
来源：http://haw.zycfv.cn

[B14] 判断值是否在集合内
来源：http://ofh.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mww.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lgl.sufxvd.cn

JS:   [1, 2, 3].includes(x)
来源：http://ois.sxryk.cn

TS:   [1, 2, 3].includes(x)
来源：http://tcu.ydjk.org.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://usy.ydjk.org.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://but.hongshengwenyu.top

Ruby: [1, 2, 3].include?(x)
来源：http://evz.chenjidiqi.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tok.guowangkeji.top

[B15] 布尔运算与取反
来源：http://kqq.wangshuangyany.cn

Py:   a and b or not c
来源：http://coo.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://axw.zhixingplan.top

JS:   a && b || !c
来源：http://njj.hfpthk.cn

TS:   a && b || !c
来源：http://emu.vehdjk.com

Java: a && b || !c
来源：http://jhr.xinyue.icu

Go:   a && b || !c
来源：http://zvs.jlsjyb.cn

Ruby: a && b || !c
来源：http://bec.yonumen.top

C#:   a && b || !c
来源：http://tbk.bbcook.cn

[B16] 卫语句：不满足条件提前返回
来源：http://evd.nwbrower.top


<!-- 参考信息 -->