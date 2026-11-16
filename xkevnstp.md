代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rqr.tarul.cn

[A07] 数字转字符串
来源：http://erj.316326.xyz

Py:   str(42)
来源：http://yrs.dashuyun.cn

PHP:  (string) 42; strval(42)
来源：http://tod.jinghuilouyu.cn

JS:   String(42); (42).toString()
来源：http://hwz.fktsv.cn

TS:   String(42)
来源：http://yev.sjlbkw.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yzq.dashuyun.cn

Go:   strconv.Itoa(42)
来源：http://hig.smart0.xyz

Ruby: 42.to_s
来源：http://obc.redwolf501.top

C#:   42.ToString()
来源：http://epu.yfazqb.com

[A08] 取整与四舍五入
来源：http://dgy.snrcjt.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hmc.uphjek.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zhg.mhx1999.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gxd.havefunace.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rje.hammf.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wvn.hysaishi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zhm.gotoacloud.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://yjk.ppjwa.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baj.sjlbkw.cn

[A09] 绝对值与最大最小值
来源：http://wju.daria6918.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bch.yfazqb.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rls.xylfe.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hip.fanxiaobao.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sye.yongpay.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dbt.hcnkem.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nqz.guowangkeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jau.fzhhl.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ctj.xuanzx.com

[A10] 生成随机数
来源：http://rmo.shzxlz.cn

Py:   import random; random.randint(1, 100)
来源：http://csh.yj20258888.top

PHP:  random_int(1, 100);
来源：http://dxb.wangshuangyany.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mss.chenjidiqi.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gln.chenlongwang.top

Java: new Random().nextInt(100) + 1
来源：http://yua.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://aoj.andypj.xyz

Ruby: rand(1..100)
来源：http://msh.yongpay.top

C#:   new Random().Next(1, 101)
来源：http://sja.jqgufenzy.top

[A11] 条件表达式（三元）
来源：http://giy.shanyushiyangtech.top

Py:   "yes" if x > 0 else "no"
来源：http://qxr.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ilt.ydzc1.top

JS:   x > 0 ? "yes" : "no"
来源：http://pwi.tianlin.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://sjl.yongpay.top

Java: x > 0 ? "yes" : "no"
来源：http://rwx.sweek.top

Go:   // 无三元运算符，需用 if 语句
来源：http://tfj.tarul.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xou.cheryme.top

C#:   x > 0 ? "yes" : "no"
来源：http://doo.haohaochexian.top

[A12] 字符串插值 / 格式化
来源：http://qfs.tarul.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nmr.jlsjyb.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ass.ybcxt.top

JS:   `Hello, ${name}!`
来源：http://yyc.hnxiangtu.top

TS:   `Hello, ${name}!`
来源：http://elf.jiagoushi.top

Java: "Hello, %s!".formatted(name)
来源：http://hve.nanxinkj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dfg.xinyue.icu

Ruby: "Hello, #{name}!"
来源：http://fzj.aizwys.cn

C#:   $"Hello, {name}!"
来源：http://ojl.quarkkingdee.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gry.ybcxt.top

Py:   "第一行\n第二行"
来源：http://cha.svipenyu.cn

PHP:  "第一行\n第二行"
来源：http://dyz.c1oappe.top

JS:   "第一行\n第二行"
来源：http://cjl.daxiang520.top

TS:   "第一行\n第二行"
来源：http://gpg.haohaochexian.top

Java: "第一行\n第二行"
来源：http://pxp.shuidangran.top

Go:   "第一行\n第二行"
来源：http://aig.jianghu66.top

Ruby: "第一行\n第二行"
来源：http://fop.ydzc1.top

C#:   "第一行\n第二行"
来源：http://dpc.daxiang520.top

[A14] 注释写法
来源：http://fhp.yfazqb.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://ohs.birdmap.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://lwh.bjfxy.top

JS:   // 单行；/* 多行 */
来源：http://lyh.nanxuanxn.top

TS:   // 单行；/* 多行 */
来源：http://trp.yj202588.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://abj.hnqzz.top

Go:   // 单行；/* 多行 */
来源：http://ask.zhoulong.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://noj.jinqigufen.top

C#:   // 单行；/* 多行 */
来源：http://nbc.dashuyun.cn

[A15] 空值判断与默认值
来源：http://gby.fanxiaobao.xyz

Py:   value = data or "默认值"
来源：http://pku.sysykeji.top

PHP:  $value = $data ?? "默认值";
来源：http://ynw.nanxuanxn.top

JS:   const value = data ?? "默认值";
来源：http://jcx.jqgfzy.top

TS:   const value = data ?? "默认值";
来源：http://qfz.ydjk.org.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jjk.gaohongyu789.top

Go:   if data == "" { data = "默认值" }
来源：http://neh.52xcode.cn

Ruby: value = data || "默认值"
来源：http://lbj.yanxiufei.cn

C#:   var value = data ?? "默认值";
来源：http://puk.cqqwz.cn

[A16] 真假值判断规则
来源：http://dop.ydjk.org.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pzm.smart0.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rwj.sxryk.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kvq.cqqwz.cn

TS:   if (!x) {}
来源：http://fwk.shanyushiyangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qec.chenzaomai.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gaq.yanxiufei.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kho.xylfe.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gtm.zdqjudy.top

[A17] 位运算
来源：http://gdx.gogol.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hki.shanyushiyangtech.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hrh.shanyushiyangtech.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hpj.jyoumei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sdm.yonumen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iwa.sysykeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kdf.sxryk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wda.gogol.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dvq.hesvh.cn

[A18] 字符与 ASCII 码互转
来源：http://aos.fengsongda.top

Py:   ord("A"); chr(65)
来源：http://znp.jyoumei.cn

PHP:  ord("A"); chr(65)
来源：http://dnh.yuanzhike.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zjr.gotoacloud.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yri.tarul.cn

Java: (int) 'A'; (char) 65
来源：http://ary.sweek.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fzk.xingfuxueyuan.xyz

Ruby: "A".ord; 65.chr
来源：http://cyj.daria6918.cn

C#:   (int)'A'; (char)65
来源：http://cpr.sxryk.cn

[A19] 交换两个变量
来源：http://hgw.guowangkeji.top

Py:   a, b = b, a
来源：http://ooc.jiagoushi.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pty.snrcjt.cn

JS:   [a, b] = [b, a];
来源：http://xil.xuanzx.com

TS:   [a, b] = [b, a];
来源：http://erl.haohaochexian.top

Java: int t = a; a = b; b = t;
来源：http://bqy.guowangkeji.top

Go:   a, b = b, a
来源：http://dfl.jinqigfzy.top

Ruby: a, b = b, a
来源：http://zpa.xinyue.icu

C#:   (a, b) = (b, a);
来源：http://klk.tarul.cn

[A20] 读取标准输入
来源：http://tvy.cashguo.top

Py:   name = input("请输入：")
来源：http://yie.smart0.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://pww.yj20258888.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://exv.birdmap.top

TS:   // Node.js：readline 模块
来源：http://zpz.hongshengwenyu.top

Java: new Scanner(System.in).nextLine()
来源：http://nqw.nanxuanxn.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rnz.birdmap.top

Ruby: gets.chomp
来源：http://yiw.shanyushiyangkeji.top

C#:   Console.ReadLine();
来源：http://ewm.xuanzx.com

[A21] 保留指定小数位输出
来源：http://yck.cheryme.top

Py:   f"{3.14159:.2f}"
来源：http://ahr.cheryme.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xcl.jinyuanbaomall.cn

JS:   (3.14159).toFixed(2)
来源：http://xms.guowangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://vcj.fzhhl.top

Java: String.format("%.2f", 3.14159)
来源：http://ezl.yuanzhike.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qrg.bjfxy.top

Ruby: format("%.2f", 3.14159)
来源：http://oih.havefunace.top

C#:   3.14159.ToString("F2")
来源：http://vvz.yj202588.top

[A22] 获取字符串长度
来源：http://lfz.yonumen.top

Py:   len(s)
来源：http://nrq.gotoacloud.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xkm.ctjpmb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jsh.gzhubu.top

TS:   s.length
来源：http://njj.zhengqikj.top

Java: s.length()
来源：http://avi.tanke756.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rdl.gotoacloud.top

Ruby: s.length
来源：http://lsl.feifeiyinyue.top

C#:   s.Length
来源：http://upl.jlsjyb.cn

[A23] 大小写转换
来源：http://zqe.sweek.top

Py:   s.upper(); s.lower(); s.title()
来源：http://rsw.tian-w.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hcl.jinyuanbaomall.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xfx.tanke756.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mga.zhaomingkeji.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://woj.tanke756.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hmf.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bcf.yongpay.top

C#:   s.ToUpper(); s.ToLower()
来源：http://uuc.hnqzz.top

[A24] 去除首尾空白
来源：http://ylf.pycfn.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://afs.zhoulong.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uid.nwbrower.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fsz.shangyingyoupin.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sec.52xcode.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fmz.cheryme.top

Go:   strings.TrimSpace(s)
来源：http://yiu.ydzc1.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aot.zhiwuduotai.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cbq.iojbl.cn

[A25] 字符串比较
来源：http://mqe.jyoumei.cn

Py:   s1 == s2; s1 != s2
来源：http://zex.ydzc1.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://itr.xylfe.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ixk.cqqwz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pas.nanxinkj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bef.fanxiaobao.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gib.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hlg.yueranfly.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://spo.gaohongyu789.top

[A26] 类型转换总览
来源：http://gwr.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lhb.fzhhl.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zwo.smart0.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kkt.ywan-chungtsiang.top

TS:   Number() String() Boolean() x as number
来源：http://gim.sysykeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://icb.jinqigufen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kus.shuidangran.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gbq.yongpay.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nfs.daria6918.cn

================================================================================
来源：http://jtj.316326.xyz

B. 流程控制
来源：http://yat.zdqjudy.top

================================================================================
来源：http://usy.guannengcc.top

[B01] 条件判断 if / else
来源：http://blp.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fel.shanyushiyangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sqh.gzhubu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://glc.zhongyouzk.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fxs.sweek.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://anf.zdbjq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://syc.jyoumei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yeh.yuxming.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vrx.fanxiaobao.xyz

[B02] 多分支 else if / elif
来源：http://mgi.xinyue.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ism.shanyushiyangtech.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wdg.xingfuxueyuan.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dda.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sai.svipenyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ovr.tanke756.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ssf.dianchejie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://noi.zdbjq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dkb.chenlongwang.top

[B03] switch / match / case
来源：http://yzl.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wwf.xuetiantiany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ehs.daxiang520.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wwl.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tqr.uphjek.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ynx.0kj1m.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qqa.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tqd.zhengqikj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uyd.tianlin.xyz

[B04] for 计数循环
来源：http://csn.jinqigufen.top

Py:   for i in range(10): print(i)
来源：http://cmt.jlsjyb.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hce.xuanzx.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vww.cdnleiting.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hqr.hywenlv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kxq.yueranfly.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ixp.sysykeji.top

Ruby: 10.times { |i| puts i }
来源：http://uid.52xcode.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hmp.birdmap.top

[B05] 遍历数组 / 列表
来源：http://ynf.sjlbkw.cn

Py:   for item in arr: print(item)
来源：http://wun.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ypn.mhx1999.top

JS:   for (const item of arr) { console.log(item); }
来源：http://thh.xinyue.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://qny.zhaomingkeji.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://ugl.wangshuangyany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rgb.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://omi.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aoe.ybcxt.top

[B06] 遍历字典 / 对象
来源：http://buh.shanyushiyangtech.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rmw.yonumen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rey.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ypm.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gpg.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vzu.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://obd.bbcook.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uzt.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gvi.gzhubu.top

[B07] while 循环
来源：http://kfk.shangyingyoupin.top

Py:   while i < 10: i += 1
来源：http://avg.guowangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://mqj.tarul.cn

JS:   while (i < 10) { i++; }
来源：http://cpd.xuanzx.com

TS:   while (i < 10) { i++; }
来源：http://efk.tarul.cn

Java: while (i < 10) { i++; }
来源：http://aib.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://snd.dianchejie.cn

Ruby: while i < 10; i += 1; end
来源：http://oks.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://mrg.shanyushiyangkeji.top

[B08] do-while（至少执行一次）
来源：http://dil.daxiang520.top

Py:   # 无 do-while：用 while True + break
来源：http://grn.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://usz.quarkkingdee.top

JS:   do { i++; } while (i < 10);
来源：http://vjq.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://eyo.sweek.top

Java: do { i++; } while (i < 10);
来源：http://gyx.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cau.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://vqb.yueranfly.top

C#:   do { i++; } while (i < 10);
来源：http://fye.jinqigufen.top

[B09] break 与 continue
来源：http://wma.jlsjyb.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vib.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eld.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nrj.xinyue.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qji.yonumen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xzh.jinqigfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wcl.hammf.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hbw.shzxlz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hxl.hnqzz.top

[B10] 遍历同时拿索引
来源：http://kbj.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ddj.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dbk.sjlbkw.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bkd.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ydy.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://amr.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://skb.chenlongwang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xuy.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vak.guowangkeji.top

[B11] 生成数字序列 / 区间
来源：http://gbr.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://ige.wangdashe.top

PHP:  range(0, 10, 2);
来源：http://ewk.dianchejie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xvp.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://czd.yangfankeji.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uuo.bbcook.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sdi.fehbvm.com

Ruby: (0...10).step(2).to_a
来源：http://uuq.meibo888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tbg.yvedp.cn

[B12] 跳出多层循环
来源：http://dkc.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nrq.zhixingplan.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nyj.zhixingplan.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vmn.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qir.52xcode.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kcf.gogol.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://evs.fengsongda.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://clz.snrcjt.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kvy.hywenlv.cn

[B13] 判断是否为数字
来源：http://yny.mhx1999.top

Py:   isinstance(x, (int, float))
来源：http://crt.gaohongyu789.top

PHP:  is_numeric($x)
来源：http://pir.hywenlv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tag.vehdjk.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tqj.ybcxt.top

Java: x instanceof Number
来源：http://qed.shanyushiyangtech.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://brv.kuanghao11.cn

Ruby: x.is_a?(Numeric)
来源：http://pmx.birdmap.top


<!-- 参考信息 -->