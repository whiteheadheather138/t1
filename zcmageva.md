代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fwk.mhx1999.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gxs.jinyuanbaomall.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hqz.fanxiaobao.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jhg.0kj1m.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://odf.fanxiaobao.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://svx.yueranfly.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nnk.guowangkeji.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wlh.hammf.cn

[A10] 生成随机数
来源：http://mdu.svipenyu.cn

Py:   import random; random.randint(1, 100)
来源：http://swt.svipenyu.cn

PHP:  random_int(1, 100);
来源：http://fea.hfpthk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nsd.vehdjk.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mzk.gogol.net.cn

Java: new Random().nextInt(100) + 1
来源：http://kxw.gzhubu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lqj.epnwcf.com

Ruby: rand(1..100)
来源：http://iwe.316326.xyz

C#:   new Random().Next(1, 101)
来源：http://jdz.nanxinkj.top

[A11] 条件表达式（三元）
来源：http://hzs.gzhubu.top

Py:   "yes" if x > 0 else "no"
来源：http://wey.316326.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://aye.zdqjudy.top

JS:   x > 0 ? "yes" : "no"
来源：http://vmj.c1oappe.top

TS:   x > 0 ? "yes" : "no"
来源：http://jyu.ydjk.org.cn

Java: x > 0 ? "yes" : "no"
来源：http://swr.nwbrower.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pjb.zhoulong.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://tbb.pycfn.com

C#:   x > 0 ? "yes" : "no"
来源：http://dxo.iojbl.cn

[A12] 字符串插值 / 格式化
来源：http://yvd.cdnleiting.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://skq.yvedp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://efk.fehbvm.com

JS:   `Hello, ${name}!`
来源：http://nhz.vqdsnc.cn

TS:   `Hello, ${name}!`
来源：http://zng.epnwcf.com

Java: "Hello, %s!".formatted(name)
来源：http://tci.wangdashe.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gdt.meibo888.top

Ruby: "Hello, #{name}!"
来源：http://ayj.hywenlv.cn

C#:   $"Hello, {name}!"
来源：http://pak.jyoumei.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://osd.andypj.xyz

Py:   "第一行\n第二行"
来源：http://yjv.jqgufenzy.top

PHP:  "第一行\n第二行"
来源：http://taq.yangfankeji.com

JS:   "第一行\n第二行"
来源：http://eto.daxiang520.top

TS:   "第一行\n第二行"
来源：http://gcz.xylfe.cn

Java: "第一行\n第二行"
来源：http://gfc.pengpengdd.cyou

Go:   "第一行\n第二行"
来源：http://nas.zhixingplan.top

Ruby: "第一行\n第二行"
来源：http://bws.xziqi.cn

C#:   "第一行\n第二行"
来源：http://rdl.ehwqpu.com

[A14] 注释写法
来源：http://moz.nanxuanxn.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ubd.guannengcc.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://mlf.smart0.xyz

JS:   // 单行；/* 多行 */
来源：http://vcp.cheryme.top

TS:   // 单行；/* 多行 */
来源：http://vhj.fengsongda.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yvu.bbcook.cn

Go:   // 单行；/* 多行 */
来源：http://tbc.aibaodan.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ckm.yfazqb.com

C#:   // 单行；/* 多行 */
来源：http://pws.hysaishi.cn

[A15] 空值判断与默认值
来源：http://xbs.yj20258888.top

Py:   value = data or "默认值"
来源：http://dud.yvedp.cn

PHP:  $value = $data ?? "默认值";
来源：http://xfg.ivvv.top

JS:   const value = data ?? "默认值";
来源：http://gxn.guannengcc.top

TS:   const value = data ?? "默认值";
来源：http://jru.hfpthk.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hbu.snrcjt.cn

Go:   if data == "" { data = "默认值" }
来源：http://aro.52xcode.cn

Ruby: value = data || "默认值"
来源：http://lti.tian-w.cn

C#:   var value = data ?? "默认值";
来源：http://icp.haohaochexian.top

[A16] 真假值判断规则
来源：http://mlh.jqgufenzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mnf.gotoacloud.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fiv.gotoacloud.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xpb.jqgufenzy.top

TS:   if (!x) {}
来源：http://pwu.zdqjudy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pby.jinyuanbaomall.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vtd.yfazqb.com

Ruby: unless x            # nil 与 false 为假
来源：http://kru.jiagoushi.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ffj.ivvv.top

[A17] 位运算
来源：http://ulc.jqgufenzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zcz.vqdsnc.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://boh.zhaomingkeji.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mlm.yanxiufei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xxr.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kba.cqqwz.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iuc.daxiang520.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://emr.zhaomingkeji.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fvm.guannengcc.top

[A18] 字符与 ASCII 码互转
来源：http://xuj.tian-w.cn

Py:   ord("A"); chr(65)
来源：http://zwz.fzhhl.top

PHP:  ord("A"); chr(65)
来源：http://uyi.birdmap.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ksy.hnxiangtu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yeu.dashuyun.cn

Java: (int) 'A'; (char) 65
来源：http://pfv.0kj1m.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bsa.xziqi.cn

Ruby: "A".ord; 65.chr
来源：http://frj.epnwcf.com

C#:   (int)'A'; (char)65
来源：http://htb.gaohongyu789.top

[A19] 交换两个变量
来源：http://spc.hywenlv.cn

Py:   a, b = b, a
来源：http://klo.xinyue.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://oln.9152youxi.cn

JS:   [a, b] = [b, a];
来源：http://yxc.zhaomingkeji.xyz

TS:   [a, b] = [b, a];
来源：http://zfr.snrcjt.cn

Java: int t = a; a = b; b = t;
来源：http://nws.wangdashe.top

Go:   a, b = b, a
来源：http://bmq.pycfn.com

Ruby: a, b = b, a
来源：http://ytu.uphjek.com

C#:   (a, b) = (b, a);
来源：http://tem.nanxinkj.top

[A20] 读取标准输入
来源：http://bwy.meibo888.top

Py:   name = input("请输入：")
来源：http://cgc.hfpthk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://adk.sjlbkw.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nvf.guannengcc.top

TS:   // Node.js：readline 模块
来源：http://rbb.kuanghao11.cn

Java: new Scanner(System.in).nextLine()
来源：http://lsa.bjfxy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kws.zycfv.cn

Ruby: gets.chomp
来源：http://qvw.gotoacloud.top

C#:   Console.ReadLine();
来源：http://wpb.jlsjyb.cn

[A21] 保留指定小数位输出
来源：http://bjq.pycfn.com

Py:   f"{3.14159:.2f}"
来源：http://iaa.tian-w.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gxj.yuxming.cn

JS:   (3.14159).toFixed(2)
来源：http://rwm.zdqjudy.top

TS:   (3.14159).toFixed(2)
来源：http://hkj.jiagoushi.top

Java: String.format("%.2f", 3.14159)
来源：http://leh.jlsjyb.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lpx.bbcook.cn

Ruby: format("%.2f", 3.14159)
来源：http://itl.sweek.top

C#:   3.14159.ToString("F2")
来源：http://gxo.tarul.cn

[A22] 获取字符串长度
来源：http://ipe.kuanghao11.cn

Py:   len(s)
来源：http://nvk.daxiang520.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tfa.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xjf.yj20258888.top

TS:   s.length
来源：http://enx.ctjpmb.com

Java: s.length()
来源：http://vdf.yonumen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cjc.hcnkem.com

Ruby: s.length
来源：http://ank.yvedp.cn

C#:   s.Length
来源：http://jny.cqqwz.cn

[A23] 大小写转换
来源：http://jvq.jqgufenzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zxz.iojbl.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ebu.jinqigfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ciu.shzxlz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nbm.cashguo.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ynn.smart0.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zuq.fengsongda.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qrz.cqqwz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sao.jqgufenzy.top

[A24] 去除首尾空白
来源：http://rfx.zdqjudy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://atw.sjlbkw.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yaf.zhijiandao.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qul.yj20258888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mtl.jinqigfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lee.pycfn.com

Go:   strings.TrimSpace(s)
来源：http://ptw.zhoulong.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gjp.feifeiyinyue.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dpj.zdqjudy.top

[A25] 字符串比较
来源：http://xya.iojbl.cn

Py:   s1 == s2; s1 != s2
来源：http://pkm.hongshengwenyu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vji.yonumen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://obj.hnqzz.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pwg.epnwcf.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mqk.yanxiufei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kog.mhx1999.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qrl.jyoumei.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bse.zhongyouzk.top

[A26] 类型转换总览
来源：http://dji.mhx1999.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wvu.vehdjk.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nyi.fehbvm.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://psn.meibo888.top

TS:   Number() String() Boolean() x as number
来源：http://ycg.smart0.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pgj.hnqzz.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wax.wangdashe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cpf.jlsjyb.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gzk.bbcook.cn

================================================================================
来源：http://aph.hcnkem.com

B. 流程控制
来源：http://gsk.jianghu66.top

================================================================================
来源：http://cwx.vqdsnc.cn

[B01] 条件判断 if / else
来源：http://qrl.daria6918.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fxf.ybcxt.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://snk.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://efa.tarul.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hni.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ofa.hammf.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zyk.chenjidiqi.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lca.vehdjk.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pbi.yvedp.cn

[B02] 多分支 else if / elif
来源：http://nit.smart0.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://elq.cucudq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xke.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dpc.chenjidiqi.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fah.gaohongyu789.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aui.jianghu66.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xqq.shzxlz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eyi.tanke756.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gov.vehdjk.com

[B03] switch / match / case
来源：http://nun.kuanghao11.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kzc.ppjwa.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://znq.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vzj.jinqigfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zzj.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zbj.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pnn.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://puu.yfazqb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hpq.cashguo.top

[B04] for 计数循环
来源：http://nxq.dianchejie.cn

Py:   for i in range(10): print(i)
来源：http://viz.ehwqpu.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mph.gogol.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ybd.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kxv.smart0.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://laj.hammf.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xig.316326.xyz

Ruby: 10.times { |i| puts i }
来源：http://dms.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qlg.gzhubu.top

[B05] 遍历数组 / 列表
来源：http://vgz.yfazqb.com

Py:   for item in arr: print(item)
来源：http://zpk.dianchejie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cwa.yonumen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nhs.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zhr.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mzr.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rpz.zhijiandao.cn

Ruby: arr.each { |item| puts item }
来源：http://rem.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://azo.tanke756.top

[B06] 遍历字典 / 对象
来源：http://uak.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://usn.jinghuilouyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mxz.dianchejie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ojf.9152youxi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xwh.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eyg.haohaochexian.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zco.ywan-chungtsiang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://keb.fktsv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jqh.sxryk.cn

[B07] while 循环
来源：http://ear.hywenlv.cn

Py:   while i < 10: i += 1
来源：http://zsb.nanxuanxn.top

PHP:  while ($i < 10) { $i++; }
来源：http://oby.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://mdh.meibo888.top

TS:   while (i < 10) { i++; }
来源：http://dcb.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://phu.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://map.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://lop.jinyuanbaomall.cn

C#:   while (i < 10) { i++; }
来源：http://dzq.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://ctx.ivvv.top

Py:   # 无 do-while：用 while True + break
来源：http://lnj.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qvt.fktsv.cn

JS:   do { i++; } while (i < 10);
来源：http://gzz.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://lzz.hnqzz.top

Java: do { i++; } while (i < 10);
来源：http://cfe.sysykeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mxk.feifeiyinyue.top

Ruby: begin; i += 1; end while i < 10
来源：http://gqx.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://gya.yueranfly.top

[B09] break 与 continue
来源：http://woi.chenlongwang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ogh.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vob.fktsv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tva.guowangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xwv.yangfankeji.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://amp.c1oappe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pxm.epnwcf.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hbe.zdqjudy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://npv.zhoulong.xyz

[B10] 遍历同时拿索引
来源：http://pyc.xuetiantiany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qcd.fengsongda.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bbq.ydzc1.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lan.smart0.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ojf.sufxvd.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://twj.316326.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://clh.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://btn.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gvw.kuanghao11.cn

[B11] 生成数字序列 / 区间
来源：http://hhn.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://his.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://jpa.cdnleiting.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://off.mhx1999.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gry.jyoumei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cym.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://niz.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://gvk.pycfn.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mas.chenzaomai.com

[B12] 跳出多层循环
来源：http://hjp.uphjek.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://oti.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ulb.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uvg.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ryd.nwbrower.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qud.kuanghao11.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zll.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oxl.yuxming.cn

[B13] 判断是否为数字
来源：http://ias.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://aln.fktsv.cn

PHP:  is_numeric($x)
来源：http://yiq.yuanzhike.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pmy.yangfankeji.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hrs.jlsjyb.cn

Java: x instanceof Number
来源：http://nce.ydzc1.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mml.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://ydp.havefunace.top

C#:   x is int or double or decimal
来源：http://hfl.xuanzx.com

[B14] 判断值是否在集合内
来源：http://nrw.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vmo.yanxiufei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oyz.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://hrm.dashuyun.cn

TS:   [1, 2, 3].includes(x)
来源：http://sbx.zhengqikj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://elu.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qpi.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ekk.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gue.aibaodan.cn

[B15] 布尔运算与取反
来源：http://pvm.vehdjk.com

Py:   a and b or not c
来源：http://vxw.tian-w.cn

PHP:  $a && $b || !$c
来源：http://ykg.shuidangran.top

JS:   a && b || !c
来源：http://gkv.shanyushiyangkeji.top

TS:   a && b || !c
来源：http://xxx.shanyushiyangkeji.top

Java: a && b || !c
来源：http://jzk.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://rgw.yj20258888.top

Ruby: a && b || !c
来源：http://sct.jinyuanbaomall.cn

C#:   a && b || !c
来源：http://uxy.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://kqo.haohaochexian.top


<!-- 参考信息 -->