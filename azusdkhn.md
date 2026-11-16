代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jjz.hysaishi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gjr.hnxiangtu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ihy.nwbrower.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ewl.yueranfly.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zht.jiagoushi.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kjw.bjfxy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ugd.zdbjq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xkj.yuanzhike.top

[A10] 生成随机数
来源：http://sch.ydzc1.top

Py:   import random; random.randint(1, 100)
来源：http://pok.ehwqpu.com

PHP:  random_int(1, 100);
来源：http://ndz.jianghu66.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lqj.smart0.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kvb.zhoulong.xyz

Java: new Random().nextInt(100) + 1
来源：http://apf.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yzd.yueranfly.top

Ruby: rand(1..100)
来源：http://tnt.jinyuanbaomall.cn

C#:   new Random().Next(1, 101)
来源：http://pzd.fehbvm.com

[A11] 条件表达式（三元）
来源：http://dtl.zhoulong.xyz

Py:   "yes" if x > 0 else "no"
来源：http://mnm.iojbl.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kgo.yangfankeji.com

JS:   x > 0 ? "yes" : "no"
来源：http://lni.yuxming.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zvu.hfpthk.cn

Java: x > 0 ? "yes" : "no"
来源：http://eps.jlsjyb.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zog.pycfn.com

Ruby: x > 0 ? "yes" : "no"
来源：http://rlr.guannengcc.top

C#:   x > 0 ? "yes" : "no"
来源：http://zal.zhoulong.xyz

[A12] 字符串插值 / 格式化
来源：http://xsm.gogol.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hhj.iojbl.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://urc.sxryk.cn

JS:   `Hello, ${name}!`
来源：http://gkl.quarkkingdee.top

TS:   `Hello, ${name}!`
来源：http://sht.quarkkingdee.top

Java: "Hello, %s!".formatted(name)
来源：http://fhw.svipenyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fqg.jianghu66.top

Ruby: "Hello, #{name}!"
来源：http://kfx.yj20258.top

C#:   $"Hello, {name}!"
来源：http://uiz.yfazqb.com

[A13] 多行字符串（练习 \n 转义）
来源：http://wpz.fehbvm.com

Py:   "第一行\n第二行"
来源：http://rkn.haohaochexian.top

PHP:  "第一行\n第二行"
来源：http://tyk.shzxlz.cn

JS:   "第一行\n第二行"
来源：http://gqr.c1oappe.top

TS:   "第一行\n第二行"
来源：http://ora.jiagoushi.top

Java: "第一行\n第二行"
来源：http://oss.redwolf501.top

Go:   "第一行\n第二行"
来源：http://qva.cdnleiting.top

Ruby: "第一行\n第二行"
来源：http://cqk.cdnleiting.top

C#:   "第一行\n第二行"
来源：http://qke.chenjidiqi.icu

[A14] 注释写法
来源：http://ckv.ydjk.org.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mje.shangyingyoupin.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://hiy.svipenyu.cn

JS:   // 单行；/* 多行 */
来源：http://tus.yfazqb.com

TS:   // 单行；/* 多行 */
来源：http://jao.shuidangran.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nxn.uphjek.com

Go:   // 单行；/* 多行 */
来源：http://vei.cucudq.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kiz.wangdashe.top

C#:   // 单行；/* 多行 */
来源：http://pwr.daria6918.cn

[A15] 空值判断与默认值
来源：http://ank.hywenlv.cn

Py:   value = data or "默认值"
来源：http://nbw.nwbrower.top

PHP:  $value = $data ?? "默认值";
来源：http://cqw.nanxinkj.top

JS:   const value = data ?? "默认值";
来源：http://dpg.jlsjyb.cn

TS:   const value = data ?? "默认值";
来源：http://lxf.xinyue.icu

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://far.yj20258888.top

Go:   if data == "" { data = "默认值" }
来源：http://xqd.zhoulong.xyz

Ruby: value = data || "默认值"
来源：http://rnp.pycfn.com

C#:   var value = data ?? "默认值";
来源：http://ypn.hongshengwenyu.top

[A16] 真假值判断规则
来源：http://qpp.jinqigufen.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qoz.bjfxy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ivp.daria6918.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xal.cheryme.top

TS:   if (!x) {}
来源：http://nld.zhongyouzk.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lcm.ppjwa.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ewe.quarkkingdee.top

Ruby: unless x            # nil 与 false 为假
来源：http://cci.smart0.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qvd.jinqigufen.top

[A17] 位运算
来源：http://woy.dianchejie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rna.nwbrower.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lcg.hnxiangtu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ktb.vqdsnc.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pte.aizwys.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ctc.jqgufenzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zmo.nanxuanxn.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kbz.quarkkingdee.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qxd.zdbjq.cn

[A18] 字符与 ASCII 码互转
来源：http://xys.jinqigufen.top

Py:   ord("A"); chr(65)
来源：http://vkg.zhongyouzk.top

PHP:  ord("A"); chr(65)
来源：http://huh.yuxming.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hto.jqgfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lhz.wangdashe.top

Java: (int) 'A'; (char) 65
来源：http://fgc.wangshuangyany.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qvi.hywenlv.cn

Ruby: "A".ord; 65.chr
来源：http://yaj.jinqigfzy.top

C#:   (int)'A'; (char)65
来源：http://psz.cdnleiting.top

[A19] 交换两个变量
来源：http://ezs.xziqi.cn

Py:   a, b = b, a
来源：http://pin.jiagoushi.top

PHP:  [$a, $b] = [$b, $a];
来源：http://tqs.meibo888.top

JS:   [a, b] = [b, a];
来源：http://wrb.hysaishi.cn

TS:   [a, b] = [b, a];
来源：http://oxc.bjfxy.top

Java: int t = a; a = b; b = t;
来源：http://dvj.havefunace.top

Go:   a, b = b, a
来源：http://kas.fzhhl.top

Ruby: a, b = b, a
来源：http://tet.sjlbkw.cn

C#:   (a, b) = (b, a);
来源：http://elv.tarul.cn

[A20] 读取标准输入
来源：http://thn.hywenlv.cn

Py:   name = input("请输入：")
来源：http://gvv.ctjpmb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://gnz.hammf.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kqs.meibo888.top

TS:   // Node.js：readline 模块
来源：http://nop.fehbvm.com

Java: new Scanner(System.in).nextLine()
来源：http://npa.jiagoushi.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sia.zhoulong.xyz

Ruby: gets.chomp
来源：http://jom.wangshuangyany.cn

C#:   Console.ReadLine();
来源：http://wbz.9152youxi.cn

[A21] 保留指定小数位输出
来源：http://ifm.cqqwz.cn

Py:   f"{3.14159:.2f}"
来源：http://swi.mhx1999.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qco.jianghu66.top

JS:   (3.14159).toFixed(2)
来源：http://dik.andypj.xyz

TS:   (3.14159).toFixed(2)
来源：http://vny.nanxuanxn.top

Java: String.format("%.2f", 3.14159)
来源：http://bqy.cucudq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blp.daxiang520.top

Ruby: format("%.2f", 3.14159)
来源：http://eab.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://xux.ybcxt.top

[A22] 获取字符串长度
来源：http://jtn.hysaishi.cn

Py:   len(s)
来源：http://acm.mhx1999.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nfw.dashuyun.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gdz.jinqigfzy.top

TS:   s.length
来源：http://qhq.hnxiangtu.top

Java: s.length()
来源：http://nvc.yongpay.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lsf.pycfn.com

Ruby: s.length
来源：http://wfb.hesvh.cn

C#:   s.Length
来源：http://hsh.zycfv.cn

[A23] 大小写转换
来源：http://tqu.yueranfly.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wbk.hnqzz.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ttt.bbcook.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://afy.zhoulong.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gfm.jinqigufen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wfo.tarul.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xqj.zhixingplan.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oki.zhixingplan.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mbr.mhx1999.top

[A24] 去除首尾空白
来源：http://itd.vehdjk.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ysz.jqgufenzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kkq.jlsjyb.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pvd.jinqigfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wbi.tanke756.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nqp.c1oappe.top

Go:   strings.TrimSpace(s)
来源：http://inx.fzhhl.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://axk.snrcjt.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bsg.birdmap.top

[A25] 字符串比较
来源：http://gtq.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://icd.fengsongda.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dbb.chenjidiqi.icu

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cbw.shangyingyoupin.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iby.xziqi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kzi.zhongyouzk.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ezp.jyoumei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://olm.yj20258888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rpc.jinqigufen.top

[A26] 类型转换总览
来源：http://zmk.quarkkingdee.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ens.nanxuanxn.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cpn.pycfn.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zen.wangshuangyany.cn

TS:   Number() String() Boolean() x as number
来源：http://bgy.shuidangran.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gyi.gzhubu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gso.yanxiufei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vce.tanke756.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jbb.pengpengdd.cyou

================================================================================
来源：http://gte.9152youxi.cn

B. 流程控制
来源：http://xzr.chenlongwang.top

================================================================================
来源：http://bmm.zhixingplan.top

[B01] 条件判断 if / else
来源：http://mje.ydjk.org.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jzr.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qmu.tanke756.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bzo.xylfe.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mtd.sjlbkw.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zse.pengpengdd.cyou

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fwc.xylfe.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rcu.tian-w.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dkv.wangdashe.top

[B02] 多分支 else if / elif
来源：http://mxy.dianchejie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yjf.ivvv.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ucs.yanxiufei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rvl.ybcxt.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rzs.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wvz.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://okp.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yxs.yj202588.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fsc.zhoulong.xyz

[B03] switch / match / case
来源：http://ysr.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fab.hcnkem.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mph.yonumen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ldn.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rjl.0kj1m.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gih.shuidangran.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tmr.yj20258.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cyd.jinqigfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gvo.jiagoushi.top

[B04] for 计数循环
来源：http://kxi.ivvv.top

Py:   for i in range(10): print(i)
来源：http://sfl.vqdsnc.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xzp.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://prb.xziqi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hfn.cashguo.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kib.nanxuanxn.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sgb.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://mby.bjfxy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://las.daxiang520.top

[B05] 遍历数组 / 列表
来源：http://bjp.ydzc1.top

Py:   for item in arr: print(item)
来源：http://gre.chenjidiqi.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dam.jiagoushi.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wcb.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hck.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mcu.chenzaomai.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xrn.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://ouh.hnxiangtu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://koc.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://qqq.hfpthk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://npy.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dlp.tian-w.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mkx.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bmj.svipenyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wvt.0kj1m.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://esn.ydzc1.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fbu.dashuyun.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://myf.hongshengwenyu.top

[B07] while 循环
来源：http://vlt.ywan-chungtsiang.top

Py:   while i < 10: i += 1
来源：http://cai.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://dmi.cheryme.top

JS:   while (i < 10) { i++; }
来源：http://mcd.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://tnm.cheryme.top

Java: while (i < 10) { i++; }
来源：http://rlh.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fnp.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://sex.guannengcc.top

C#:   while (i < 10) { i++; }
来源：http://olm.nanxinkj.top

[B08] do-while（至少执行一次）
来源：http://ioy.jqgfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://kyf.shangyingyoupin.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ohz.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://sgo.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://ors.sufxvd.cn

Java: do { i++; } while (i < 10);
来源：http://sqm.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://dlw.andypj.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://umq.jinqigfzy.top

C#:   do { i++; } while (i < 10);
来源：http://pbm.hcnkem.com

[B09] break 与 continue
来源：http://wff.ydzc1.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dxd.zhijiandao.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rot.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nln.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lhe.jinyuanbaomall.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rzr.feifeiyinyue.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mly.cqqwz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eqn.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cvx.ywan-chungtsiang.top

[B10] 遍历同时拿索引
来源：http://vsp.guowangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://giv.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xsm.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lwg.hnxiangtu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jmt.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qup.vqdsnc.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rll.feifeiyinyue.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aur.andypj.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ebt.mhx1999.top

[B11] 生成数字序列 / 区间
来源：http://zhz.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://zje.jinyuanbaomall.cn

PHP:  range(0, 10, 2);
来源：http://qea.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://klc.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ubd.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xdg.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yrb.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://cqz.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fpu.jqgufenzy.top

[B12] 跳出多层循环
来源：http://jmg.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rxc.xuetiantiany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lkw.havefunace.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bnu.hfpthk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hec.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gpx.gotoacloud.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://utf.fktsv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://efi.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sfw.zhoulong.xyz

[B13] 判断是否为数字
来源：http://adz.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://uqs.hysaishi.cn

PHP:  is_numeric($x)
来源：http://gbf.yj20258.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ntv.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://auk.dianchejie.cn

Java: x instanceof Number
来源：http://byn.hcnkem.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://osx.aibaodan.cn

Ruby: x.is_a?(Numeric)
来源：http://sje.quarkkingdee.top

C#:   x is int or double or decimal
来源：http://asy.uphjek.com

[B14] 判断值是否在集合内
来源：http://fee.hcnkem.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jqj.smart0.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aeq.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://lfw.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://znr.jinqigufen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tsk.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hpq.zhongyouzk.top

Ruby: [1, 2, 3].include?(x)
来源：http://xpb.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qky.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://iqq.hnqzz.top

Py:   a and b or not c
来源：http://cae.birdmap.top

PHP:  $a && $b || !$c
来源：http://tgc.shuidangran.top

JS:   a && b || !c
来源：http://xhl.yfazqb.com

TS:   a && b || !c
来源：http://dik.9152youxi.cn

Java: a && b || !c
来源：http://cdy.hesvh.cn

Go:   a && b || !c
来源：http://vor.tanke756.top

Ruby: a && b || !c
来源：http://pty.jianghu66.top

C#:   a && b || !c
来源：http://dzs.nwbrower.top

[B16] 卫语句：不满足条件提前返回
来源：http://qps.jqgfzy.top


<!-- 参考信息 -->