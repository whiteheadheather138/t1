代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ife.shanyushiyangkeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cce.zhaomingkeji.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cmy.meibo888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bxh.nanxuanxn.top

[A10] 生成随机数
来源：http://wdu.ehwqpu.com

Py:   import random; random.randint(1, 100)
来源：http://xdu.zhoulong.xyz

PHP:  random_int(1, 100);
来源：http://cdn.nanxinkj.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://npk.guannengcc.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fcp.hesvh.cn

Java: new Random().nextInt(100) + 1
来源：http://jkc.yangfankeji.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qav.316326.xyz

Ruby: rand(1..100)
来源：http://mjq.snrcjt.cn

C#:   new Random().Next(1, 101)
来源：http://ajf.feifeiyinyue.top

[A11] 条件表达式（三元）
来源：http://bhg.redwolf501.top

Py:   "yes" if x > 0 else "no"
来源：http://hep.wangshuangyany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vgs.9152youxi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mtq.jinyuanbaomall.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nzp.zhongyouzk.top

Java: x > 0 ? "yes" : "no"
来源：http://bgv.pycfn.com

Go:   // 无三元运算符，需用 if 语句
来源：http://gxy.c1oappe.top

Ruby: x > 0 ? "yes" : "no"
来源：http://eba.0kj1m.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lpd.ybcxt.top

[A12] 字符串插值 / 格式化
来源：http://esa.shanyushiyangtech.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://awf.epnwcf.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nxg.zdbjq.cn

JS:   `Hello, ${name}!`
来源：http://crp.uphjek.com

TS:   `Hello, ${name}!`
来源：http://aen.kuanghao11.cn

Java: "Hello, %s!".formatted(name)
来源：http://yfd.xinyue.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xis.guowangkeji.top

Ruby: "Hello, #{name}!"
来源：http://mog.hfpthk.cn

C#:   $"Hello, {name}!"
来源：http://mgi.andypj.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://zut.smart0.xyz

Py:   "第一行\n第二行"
来源：http://fds.daria6918.cn

PHP:  "第一行\n第二行"
来源：http://meb.haohaochexian.top

JS:   "第一行\n第二行"
来源：http://xfp.tianlin.xyz

TS:   "第一行\n第二行"
来源：http://gbf.xylfe.cn

Java: "第一行\n第二行"
来源：http://qrk.uphjek.com

Go:   "第一行\n第二行"
来源：http://ddc.dianchejie.cn

Ruby: "第一行\n第二行"
来源：http://tvp.hfpthk.cn

C#:   "第一行\n第二行"
来源：http://cqr.tarul.cn

[A14] 注释写法
来源：http://qpo.haohaochexian.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://gfx.xylfe.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://onx.shuidangran.top

JS:   // 单行；/* 多行 */
来源：http://myk.vqdsnc.cn

TS:   // 单行；/* 多行 */
来源：http://pym.daxiang520.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ghy.jqgufenzy.top

Go:   // 单行；/* 多行 */
来源：http://moi.zhixingplan.top

Ruby: # 单行；=begin 多行 =end
来源：http://bis.yuanzhike.top

C#:   // 单行；/* 多行 */
来源：http://oke.yonumen.top

[A15] 空值判断与默认值
来源：http://fjw.xylfe.cn

Py:   value = data or "默认值"
来源：http://dma.52xcode.cn

PHP:  $value = $data ?? "默认值";
来源：http://eej.0kj1m.cn

JS:   const value = data ?? "默认值";
来源：http://ejp.aibaodan.cn

TS:   const value = data ?? "默认值";
来源：http://gsq.pycfn.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yff.nanxuanxn.top

Go:   if data == "" { data = "默认值" }
来源：http://ryz.zhaomingkeji.xyz

Ruby: value = data || "默认值"
来源：http://qbk.tianlin.xyz

C#:   var value = data ?? "默认值";
来源：http://pcb.nanxuanxn.top

[A16] 真假值判断规则
来源：http://fyk.bjfxy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dlm.gaohongyu789.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ctq.jqgfzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hij.yangfankeji.com

TS:   if (!x) {}
来源：http://jbr.zdqjudy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ivr.xziqi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uzo.52xcode.cn

Ruby: unless x            # nil 与 false 为假
来源：http://evl.fktsv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hzb.svipenyu.cn

[A17] 位运算
来源：http://fch.xuanzx.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rfd.fzhhl.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jwt.hcnkem.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yyx.dashuyun.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jrk.ivvv.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uzo.daria6918.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jzi.chenjidiqi.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fzf.xziqi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://exs.chenjidiqi.icu

[A18] 字符与 ASCII 码互转
来源：http://isf.cheryme.top

Py:   ord("A"); chr(65)
来源：http://phm.fanxiaobao.xyz

PHP:  ord("A"); chr(65)
来源：http://sbn.shanyushiyangkeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yws.bjfxy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hsj.wangshuangyany.cn

Java: (int) 'A'; (char) 65
来源：http://vta.svipenyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dwl.hammf.cn

Ruby: "A".ord; 65.chr
来源：http://mka.cqqwz.cn

C#:   (int)'A'; (char)65
来源：http://dyo.redwolf501.top

[A19] 交换两个变量
来源：http://cwa.hnqzz.top

Py:   a, b = b, a
来源：http://ccg.xuanzx.com

PHP:  [$a, $b] = [$b, $a];
来源：http://ijh.guannengcc.top

JS:   [a, b] = [b, a];
来源：http://stj.sufxvd.cn

TS:   [a, b] = [b, a];
来源：http://zbv.xuanzx.com

Java: int t = a; a = b; b = t;
来源：http://rzm.nanxuanxn.top

Go:   a, b = b, a
来源：http://gno.hcnkem.com

Ruby: a, b = b, a
来源：http://mho.hysaishi.cn

C#:   (a, b) = (b, a);
来源：http://eha.yj20258.top

[A20] 读取标准输入
来源：http://lea.jlsjyb.cn

Py:   name = input("请输入：")
来源：http://grg.jiagoushi.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rtj.chenzaomai.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rah.316326.xyz

TS:   // Node.js：readline 模块
来源：http://bxe.hcnkem.com

Java: new Scanner(System.in).nextLine()
来源：http://czm.hcnkem.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zjy.yongpay.top

Ruby: gets.chomp
来源：http://zfd.ydjk.org.cn

C#:   Console.ReadLine();
来源：http://fwb.ppjwa.cn

[A21] 保留指定小数位输出
来源：http://loj.gzhubu.top

Py:   f"{3.14159:.2f}"
来源：http://zyh.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://flq.nwbrower.top

JS:   (3.14159).toFixed(2)
来源：http://vsx.chenlongwang.top

TS:   (3.14159).toFixed(2)
来源：http://hfg.cucudq.cn

Java: String.format("%.2f", 3.14159)
来源：http://ful.yj202588.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kxy.mhx1999.top

Ruby: format("%.2f", 3.14159)
来源：http://duz.quarkkingdee.top

C#:   3.14159.ToString("F2")
来源：http://aiy.yueranfly.top

[A22] 获取字符串长度
来源：http://fnt.vqdsnc.cn

Py:   len(s)
来源：http://cbf.zhongyouzk.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://aht.yonumen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mhh.xuetiantiany.cn

TS:   s.length
来源：http://ilc.xuanzx.com

Java: s.length()
来源：http://zqc.nanxuanxn.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fra.bjfxy.top

Ruby: s.length
来源：http://lrz.cucudq.cn

C#:   s.Length
来源：http://zdj.9152youxi.cn

[A23] 大小写转换
来源：http://xza.zdbjq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zry.wangdashe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ufs.wangshuangyany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wkm.iojbl.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://etp.nwbrower.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dgh.xinyue.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xmu.ctjpmb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gxl.uphjek.com

C#:   s.ToUpper(); s.ToLower()
来源：http://azl.cheryme.top

[A24] 去除首尾空白
来源：http://zde.chenzaomai.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yhs.gogol.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gyo.daxiang520.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rtz.mhx1999.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jig.cqqwz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kjv.fzhhl.top

Go:   strings.TrimSpace(s)
来源：http://jjc.tarul.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://thh.zhijiandao.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sia.xuetiantiany.cn

[A25] 字符串比较
来源：http://ovq.daxiang520.top

Py:   s1 == s2; s1 != s2
来源：http://bsg.jinghuilouyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iqz.yj202588.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lxp.jyoumei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xqg.sysykeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iyo.shangyingyoupin.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ktv.dashuyun.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hyo.jqgfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sgq.c1oappe.top

[A26] 类型转换总览
来源：http://woa.xylfe.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://noy.zhongyouzk.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xvd.cheryme.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ety.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://dfa.cucudq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gsl.wangdashe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vxd.ybcxt.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dgj.ywan-chungtsiang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://aqx.sjlbkw.cn

================================================================================
来源：http://oqk.nwbrower.top

B. 流程控制
来源：http://lpw.fktsv.cn

================================================================================
来源：http://rge.xylfe.cn

[B01] 条件判断 if / else
来源：http://rdl.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mce.yvedp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xxq.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tqm.jinghuilouyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://izp.0kj1m.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qxa.tanke756.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wse.jyoumei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cen.wangshuangyany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jwv.birdmap.top

[B02] 多分支 else if / elif
来源：http://cso.hywenlv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qve.yj20258888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zxh.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://frp.xylfe.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://saa.ppjwa.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wpa.tianlin.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://luq.fzhhl.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bbt.xinyue.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bme.xziqi.cn

[B03] switch / match / case
来源：http://ezs.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gnm.havefunace.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://obk.guannengcc.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rdy.chenjidiqi.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uuh.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vqx.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bky.9152youxi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cae.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ijr.xinyue.icu

[B04] for 计数循环
来源：http://sgc.jinyuanbaomall.cn

Py:   for i in range(10): print(i)
来源：http://wym.sjlbkw.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ier.fengsongda.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://law.zhijiandao.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qvf.guannengcc.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://szd.hfpthk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xax.sufxvd.cn

Ruby: 10.times { |i| puts i }
来源：http://ihm.daxiang520.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mtf.yuanzhike.top

[B05] 遍历数组 / 列表
来源：http://rbx.yj20258888.top

Py:   for item in arr: print(item)
来源：http://lih.ctjpmb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://agb.gzhubu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://lri.uphjek.com

TS:   for (const item of arr) { console.log(item); }
来源：http://cea.vehdjk.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://dkw.redwolf501.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ivu.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://vhe.ppjwa.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fac.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://wtd.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bim.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hyp.nwbrower.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lmh.sxryk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jii.ivvv.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fqu.shanyushiyangtech.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cio.aizwys.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jof.shzxlz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://twd.guowangkeji.top

[B07] while 循环
来源：http://xit.chenlongwang.top

Py:   while i < 10: i += 1
来源：http://vth.yangfankeji.com

PHP:  while ($i < 10) { $i++; }
来源：http://rva.hnxiangtu.top

JS:   while (i < 10) { i++; }
来源：http://hmp.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://sfw.iojbl.cn

Java: while (i < 10) { i++; }
来源：http://fez.ydjk.org.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hpl.sjlbkw.cn

Ruby: while i < 10; i += 1; end
来源：http://jwz.xziqi.cn

C#:   while (i < 10) { i++; }
来源：http://ear.hnqzz.top

[B08] do-while（至少执行一次）
来源：http://fwz.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://utm.shanyushiyangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vxc.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://ran.ydzc1.top

TS:   do { i++; } while (i < 10);
来源：http://rtz.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://osu.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://oxj.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://vzc.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://oqx.iojbl.cn

[B09] break 与 continue
来源：http://ddo.birdmap.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bug.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://goo.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://evy.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dkb.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qzn.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ytu.gogol.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wfg.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qlo.ydzc1.top

[B10] 遍历同时拿索引
来源：http://vbj.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rln.fehbvm.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hze.ybcxt.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wms.xingfuxueyuan.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lte.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lae.zhijiandao.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yva.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uef.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://snr.sjlbkw.cn

[B11] 生成数字序列 / 区间
来源：http://dan.tianlin.xyz

Py:   list(range(0, 10, 2))
来源：http://arp.sufxvd.cn

PHP:  range(0, 10, 2);
来源：http://qhq.jqgfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pel.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wuh.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nxt.zhixingplan.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://obt.pengpengdd.cyou

Ruby: (0...10).step(2).to_a
来源：http://abf.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aug.nwbrower.top

[B12] 跳出多层循环
来源：http://tid.ctjpmb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://yew.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wit.jqgufenzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lps.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cqr.zhiwuduotai.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://evc.jinghuilouyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iic.sweek.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nir.ppjwa.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pdg.mhx1999.top

[B13] 判断是否为数字
来源：http://rry.shuidangran.top

Py:   isinstance(x, (int, float))
来源：http://nad.ehwqpu.com

PHP:  is_numeric($x)
来源：http://zxx.zhoulong.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sos.shzxlz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vds.guannengcc.top

Java: x instanceof Number
来源：http://axy.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://riw.guowangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://foe.dianchejie.cn

C#:   x is int or double or decimal
来源：http://haz.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://xww.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://trf.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cqw.yueranfly.top

JS:   [1, 2, 3].includes(x)
来源：http://mrs.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://cmq.hnxiangtu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jem.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mno.zycfv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ojp.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tgp.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://sig.nanxuanxn.top

Py:   a and b or not c
来源：http://ael.tarul.cn

PHP:  $a && $b || !$c
来源：http://rnl.pengpengdd.cyou

JS:   a && b || !c
来源：http://dnj.gotoacloud.top

TS:   a && b || !c
来源：http://ljw.c1oappe.top

Java: a && b || !c
来源：http://nbc.jqgfzy.top

Go:   a && b || !c
来源：http://xgs.jinqigfzy.top

Ruby: a && b || !c
来源：http://ucv.hesvh.cn

C#:   a && b || !c
来源：http://trd.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://pcf.ywan-chungtsiang.top

Py:   if not data: return
来源：http://qdf.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://fwj.yuxming.cn

JS:   if (!data) return;
来源：http://ixd.sysykeji.top

TS:   if (!data) return;
来源：http://yqd.pengpengdd.cyou


<!-- 参考信息 -->