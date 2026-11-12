代发 wailian999

[A06] 字符串转数字
来源：http://hdc.andypj.xyz

Py:   int("42"); float("3.14")
来源：http://vbw.guannengcc.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fwd.cashguo.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cnj.nanxinkj.top

TS:   parseInt("42", 10); Number("42")
来源：http://xkv.dianchejie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uhy.jinqigufen.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://twc.jinqigufen.top

Ruby: "42".to_i; "3.14".to_f
来源：http://avc.gotoacloud.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ttg.bjfxy.top

[A07] 数字转字符串
来源：http://gwp.hesvh.cn

Py:   str(42)
来源：http://ith.cdnleiting.top

PHP:  (string) 42; strval(42)
来源：http://ozo.fanxiaobao.xyz

JS:   String(42); (42).toString()
来源：http://swy.hnxiangtu.top

TS:   String(42)
来源：http://mjn.pengpengdd.cyou

Java: String.valueOf(42); Integer.toString(42)
来源：http://khc.ctjpmb.com

Go:   strconv.Itoa(42)
来源：http://jpb.fzhhl.top

Ruby: 42.to_s
来源：http://roe.jyoumei.cn

C#:   42.ToString()
来源：http://bkg.xuetiantiany.cn

[A08] 取整与四舍五入
来源：http://fxq.hywenlv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hyv.epnwcf.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xki.feifeiyinyue.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ehx.ppjwa.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://phy.hnxiangtu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ooc.hesvh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mec.kuanghao11.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gqn.havefunace.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://buq.yvedp.cn

[A09] 绝对值与最大最小值
来源：http://vit.hfpthk.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nmz.aizwys.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rwy.ivvv.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vqt.kuanghao11.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fmc.shzxlz.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://onu.sweek.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qqd.ivvv.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sqn.gogol.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lhu.gzhubu.top

[A10] 生成随机数
来源：http://qjg.daxiang520.top

Py:   import random; random.randint(1, 100)
来源：http://ilh.hfpthk.cn

PHP:  random_int(1, 100);
来源：http://xac.dianchejie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cvp.jinyuanbaomall.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xpn.gogol.net.cn

Java: new Random().nextInt(100) + 1
来源：http://pnf.sufxvd.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://esu.feifeiyinyue.top

Ruby: rand(1..100)
来源：http://fma.yongpay.top

C#:   new Random().Next(1, 101)
来源：http://waq.hongshengwenyu.top

[A11] 条件表达式（三元）
来源：http://yit.tanke756.top

Py:   "yes" if x > 0 else "no"
来源：http://jff.zhiwuduotai.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://alf.cashguo.top

JS:   x > 0 ? "yes" : "no"
来源：http://nvm.jianghu66.top

TS:   x > 0 ? "yes" : "no"
来源：http://epd.nanxuanxn.top

Java: x > 0 ? "yes" : "no"
来源：http://jkr.yfazqb.com

Go:   // 无三元运算符，需用 if 语句
来源：http://gob.hammf.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wwx.nanxuanxn.top

C#:   x > 0 ? "yes" : "no"
来源：http://rio.jinqigfzy.top

[A12] 字符串插值 / 格式化
来源：http://pmh.kuanghao11.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://txs.vehdjk.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ohg.0kj1m.cn

JS:   `Hello, ${name}!`
来源：http://hmo.xuanzx.com

TS:   `Hello, ${name}!`
来源：http://rwk.yanxiufei.cn

Java: "Hello, %s!".formatted(name)
来源：http://rke.hnxiangtu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xfg.svipenyu.cn

Ruby: "Hello, #{name}!"
来源：http://wlj.sysykeji.top

C#:   $"Hello, {name}!"
来源：http://lnl.redwolf501.top

[A13] 多行字符串（练习 \n 转义）
来源：http://vzo.sufxvd.cn

Py:   "第一行\n第二行"
来源：http://qxo.daria6918.cn

PHP:  "第一行\n第二行"
来源：http://plt.shzxlz.cn

JS:   "第一行\n第二行"
来源：http://gbm.sysykeji.top

TS:   "第一行\n第二行"
来源：http://qua.sysykeji.top

Java: "第一行\n第二行"
来源：http://ccf.xinyue.icu

Go:   "第一行\n第二行"
来源：http://xox.jqgfzy.top

Ruby: "第一行\n第二行"
来源：http://zjl.shanyushiyangkeji.top

C#:   "第一行\n第二行"
来源：http://gqo.aibaodan.cn

[A14] 注释写法
来源：http://pkm.gaohongyu789.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://tzf.yueranfly.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://lol.epnwcf.com

JS:   // 单行；/* 多行 */
来源：http://npc.fanxiaobao.xyz

TS:   // 单行；/* 多行 */
来源：http://cts.gotoacloud.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qjt.shangyingyoupin.top

Go:   // 单行；/* 多行 */
来源：http://drf.jianghu66.top

Ruby: # 单行；=begin 多行 =end
来源：http://awm.guowangkeji.top

C#:   // 单行；/* 多行 */
来源：http://ttj.yuanzhike.top

[A15] 空值判断与默认值
来源：http://vot.hnxiangtu.top

Py:   value = data or "默认值"
来源：http://eto.pengpengdd.cyou

PHP:  $value = $data ?? "默认值";
来源：http://lfi.sweek.top

JS:   const value = data ?? "默认值";
来源：http://hdy.mhx1999.top

TS:   const value = data ?? "默认值";
来源：http://pre.ybcxt.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oyd.hammf.cn

Go:   if data == "" { data = "默认值" }
来源：http://kjt.haohaochexian.top

Ruby: value = data || "默认值"
来源：http://hbs.yonumen.top

C#:   var value = data ?? "默认值";
来源：http://dpq.zdbjq.cn

[A16] 真假值判断规则
来源：http://utv.haohaochexian.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xjs.hysaishi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mpb.wangdashe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vfr.aizwys.cn

TS:   if (!x) {}
来源：http://zod.tianlin.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wjk.ehwqpu.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://reg.shanyushiyangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://onp.gzhubu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sbc.jinyuanbaomall.cn

[A17] 位运算
来源：http://foc.jinghuilouyu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ysz.ybcxt.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ueq.cashguo.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jou.xinyue.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gsm.chenjidiqi.icu

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wad.zhaomingkeji.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oaq.yonumen.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://luz.ywan-chungtsiang.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dpw.hammf.cn

[A18] 字符与 ASCII 码互转
来源：http://kna.chenlongwang.top

Py:   ord("A"); chr(65)
来源：http://kpp.ehwqpu.com

PHP:  ord("A"); chr(65)
来源：http://pqk.zdqjudy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://khs.zhixingplan.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zhe.c1oappe.top

Java: (int) 'A'; (char) 65
来源：http://sna.shuidangran.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zsi.nanxuanxn.top

Ruby: "A".ord; 65.chr
来源：http://ejn.xziqi.cn

C#:   (int)'A'; (char)65
来源：http://tve.chenjidiqi.icu

[A19] 交换两个变量
来源：http://czt.pycfn.com

Py:   a, b = b, a
来源：http://hwt.quarkkingdee.top

PHP:  [$a, $b] = [$b, $a];
来源：http://fwx.ydzc1.top

JS:   [a, b] = [b, a];
来源：http://ngt.ehwqpu.com

TS:   [a, b] = [b, a];
来源：http://sgh.yuanzhike.top

Java: int t = a; a = b; b = t;
来源：http://ase.nanxuanxn.top

Go:   a, b = b, a
来源：http://qjb.shangyingyoupin.top

Ruby: a, b = b, a
来源：http://tud.snrcjt.cn

C#:   (a, b) = (b, a);
来源：http://sfh.yfazqb.com

[A20] 读取标准输入
来源：http://fzy.chenjidiqi.icu

Py:   name = input("请输入：")
来源：http://lbp.sufxvd.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://msp.xuanzx.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qhg.smart0.xyz

TS:   // Node.js：readline 模块
来源：http://cns.hywenlv.cn

Java: new Scanner(System.in).nextLine()
来源：http://ohd.ybcxt.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dnd.ehwqpu.com

Ruby: gets.chomp
来源：http://zbz.ivvv.top

C#:   Console.ReadLine();
来源：http://grn.jqgufenzy.top

[A21] 保留指定小数位输出
来源：http://yho.hongshengwenyu.top

Py:   f"{3.14159:.2f}"
来源：http://jnk.jinyuanbaomall.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ycz.hcnkem.com

JS:   (3.14159).toFixed(2)
来源：http://rjm.guannengcc.top

TS:   (3.14159).toFixed(2)
来源：http://iqv.zhijiandao.cn

Java: String.format("%.2f", 3.14159)
来源：http://faf.jianghu66.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jhx.daxiang520.top

Ruby: format("%.2f", 3.14159)
来源：http://wlw.xuetiantiany.cn

C#:   3.14159.ToString("F2")
来源：http://mza.daria6918.cn

[A22] 获取字符串长度
来源：http://nxu.vehdjk.com

Py:   len(s)
来源：http://vtj.birdmap.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://drk.shzxlz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ock.hywenlv.cn

TS:   s.length
来源：http://upw.havefunace.top

Java: s.length()
来源：http://air.bjfxy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pzu.fzhhl.top

Ruby: s.length
来源：http://rzx.yuxming.cn

C#:   s.Length
来源：http://jru.vehdjk.com

[A23] 大小写转换
来源：http://qyq.hfpthk.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kcx.zhengqikj.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hgh.ctjpmb.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rxr.jlsjyb.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nev.nwbrower.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vsu.zhaomingkeji.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qji.pycfn.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rpn.zhixingplan.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gbt.yvedp.cn

[A24] 去除首尾空白
来源：http://fbo.andypj.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://efd.hcnkem.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rhn.tianlin.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ryu.wangdashe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://umq.yj20258.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jbq.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://kuj.yvedp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nbj.pycfn.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cxo.cdnleiting.top

[A25] 字符串比较
来源：http://scz.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://ocq.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iel.wangdashe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fia.pengpengdd.cyou

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hhw.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://knv.sxryk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fdf.hysaishi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://smy.hcnkem.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zvt.pengpengdd.cyou

[A26] 类型转换总览
来源：http://lrv.birdmap.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hgp.dashuyun.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sky.aizwys.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hzv.tian-w.cn

TS:   Number() String() Boolean() x as number
来源：http://wgu.xinyue.icu

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lou.nanxinkj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ovt.jiagoushi.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hbo.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hot.fengsongda.top

================================================================================
来源：http://qjg.nanxinkj.top

B. 流程控制
来源：http://fjv.chenjidiqi.icu

================================================================================
来源：http://ede.cheryme.top

[B01] 条件判断 if / else
来源：http://rvn.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://otw.xuanzx.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wxc.c1oappe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vbe.cqqwz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://byu.kuanghao11.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://seb.52xcode.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fun.yueranfly.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://unv.yuanzhike.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vmm.bjfxy.top

[B02] 多分支 else if / elif
来源：http://bpk.hysaishi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ckm.jiagoushi.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mst.birdmap.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pkz.kuanghao11.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tgz.zhongyouzk.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bmc.birdmap.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mzk.jianghu66.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rpr.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyz.chenjidiqi.icu

[B03] switch / match / case
来源：http://fin.gogol.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ubb.hcnkem.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://brj.yonumen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rej.cdnleiting.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ulj.fanxiaobao.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xvr.shanyushiyangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eax.ppjwa.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eis.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://swb.tanke756.top

[B04] for 计数循环
来源：http://lny.gotoacloud.top

Py:   for i in range(10): print(i)
来源：http://rpj.sxryk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://omi.ppjwa.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://soz.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bfr.guowangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yuc.bjfxy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rnt.yfazqb.com

Ruby: 10.times { |i| puts i }
来源：http://xqu.zhiwuduotai.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yjt.epnwcf.com

[B05] 遍历数组 / 列表
来源：http://dwz.zycfv.cn

Py:   for item in arr: print(item)
来源：http://bkm.yj20258.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hmp.c1oappe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://iwn.cqqwz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wjq.sysykeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wea.jiagoushi.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://her.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://pgq.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wxk.9152youxi.cn

[B06] 遍历字典 / 对象
来源：http://vbc.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hej.hysaishi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qai.yueranfly.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://anr.andypj.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://muj.xziqi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kkm.andypj.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ljz.yonumen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xgi.yj20258.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nqq.hnqzz.top

[B07] while 循环
来源：http://dwg.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://tto.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://cpj.zdbjq.cn

JS:   while (i < 10) { i++; }
来源：http://ygw.zhijiandao.cn

TS:   while (i < 10) { i++; }
来源：http://tkz.cqqwz.cn

Java: while (i < 10) { i++; }
来源：http://res.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wkc.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://eib.hywenlv.cn

C#:   while (i < 10) { i++; }
来源：http://gtg.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://mls.jinqigufen.top

Py:   # 无 do-while：用 while True + break
来源：http://sam.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hpq.nwbrower.top

JS:   do { i++; } while (i < 10);
来源：http://qlp.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://tcy.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://txl.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://lka.yanxiufei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cjh.yuanzhike.top

C#:   do { i++; } while (i < 10);
来源：http://kkc.kuanghao11.cn

[B09] break 与 continue
来源：http://toy.cdnleiting.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cvw.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lcm.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mzd.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yoy.sysykeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xsc.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kfq.uphjek.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vny.bbcook.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hgq.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://aei.daria6918.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gvv.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aau.hywenlv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lmp.ydjk.org.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://myd.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bmn.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jfs.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ejp.guowangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cyt.feifeiyinyue.top

[B11] 生成数字序列 / 区间
来源：http://kui.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://dcm.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://lnj.sweek.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hqr.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bdk.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://znl.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uxj.ivvv.top

Ruby: (0...10).step(2).to_a
来源：http://nrz.zhiwuduotai.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wij.ydjk.org.cn

[B12] 跳出多层循环
来源：http://vxj.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://enc.chenjidiqi.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://tsb.yongpay.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zmb.cashguo.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kie.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gia.yonumen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bci.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mlj.xingfuxueyuan.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oua.tian-w.cn


<!-- 参考信息 -->