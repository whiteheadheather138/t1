代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wkk.nanxinkj.top

[A07] 数字转字符串
来源：http://ddw.cucudq.cn

Py:   str(42)
来源：http://kxr.yuanzhike.top

PHP:  (string) 42; strval(42)
来源：http://lsp.zhiwuduotai.top

JS:   String(42); (42).toString()
来源：http://kag.zhongyouzk.top

TS:   String(42)
来源：http://osn.gogol.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vvk.cdnleiting.top

Go:   strconv.Itoa(42)
来源：http://hrc.fzhhl.top

Ruby: 42.to_s
来源：http://glk.yangfankeji.com

C#:   42.ToString()
来源：http://kwl.hywenlv.cn

[A08] 取整与四舍五入
来源：http://wkf.quarkkingdee.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fcs.fehbvm.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xly.ydjk.org.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://aet.zhengqikj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oae.chenjidiqi.icu

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nlx.ybcxt.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dnw.ydjk.org.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rvo.smart0.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kex.jianghu66.top

[A09] 绝对值与最大最小值
来源：http://nvw.aizwys.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zjz.yonumen.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vso.jianghu66.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://smu.yvedp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gmr.xinyue.icu

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vdq.hammf.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zcb.andypj.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jce.jinyuanbaomall.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oab.sxryk.cn

[A10] 生成随机数
来源：http://cbs.smart0.xyz

Py:   import random; random.randint(1, 100)
来源：http://ntf.yuanzhike.top

PHP:  random_int(1, 100);
来源：http://goc.fktsv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://aej.hywenlv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ddz.shzxlz.cn

Java: new Random().nextInt(100) + 1
来源：http://qlh.yj202588.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://auq.nanxinkj.top

Ruby: rand(1..100)
来源：http://ygm.iojbl.cn

C#:   new Random().Next(1, 101)
来源：http://sko.ctjpmb.com

[A11] 条件表达式（三元）
来源：http://jbe.uphjek.com

Py:   "yes" if x > 0 else "no"
来源：http://lzh.jinqigfzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kuw.zhijiandao.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ovu.316326.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://emx.zhongyouzk.top

Java: x > 0 ? "yes" : "no"
来源：http://vks.nanxuanxn.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ukq.snrcjt.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wxo.snrcjt.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xsg.ywan-chungtsiang.top

[A12] 字符串插值 / 格式化
来源：http://yjz.sxryk.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ass.dashuyun.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bkw.yfazqb.com

JS:   `Hello, ${name}!`
来源：http://jwu.bjfxy.top

TS:   `Hello, ${name}!`
来源：http://xvs.vqdsnc.cn

Java: "Hello, %s!".formatted(name)
来源：http://nit.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://osc.hammf.cn

Ruby: "Hello, #{name}!"
来源：http://cch.epnwcf.com

C#:   $"Hello, {name}!"
来源：http://jhj.yongpay.top

[A13] 多行字符串（练习 \n 转义）
来源：http://tzt.jinqigfzy.top

Py:   "第一行\n第二行"
来源：http://xws.bjfxy.top

PHP:  "第一行\n第二行"
来源：http://ayw.jinghuilouyu.cn

JS:   "第一行\n第二行"
来源：http://rbo.zhixingplan.top

TS:   "第一行\n第二行"
来源：http://vjp.sufxvd.cn

Java: "第一行\n第二行"
来源：http://ryw.shuidangran.top

Go:   "第一行\n第二行"
来源：http://ezy.redwolf501.top

Ruby: "第一行\n第二行"
来源：http://sqv.chenjidiqi.icu

C#:   "第一行\n第二行"
来源：http://yfc.ydzc1.top

[A14] 注释写法
来源：http://gvj.shuidangran.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mjj.yfazqb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://nmp.sxryk.cn

JS:   // 单行；/* 多行 */
来源：http://zxx.epnwcf.com

TS:   // 单行；/* 多行 */
来源：http://ppz.xziqi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ztq.ywan-chungtsiang.top

Go:   // 单行；/* 多行 */
来源：http://ufj.pycfn.com

Ruby: # 单行；=begin 多行 =end
来源：http://xjd.jiagoushi.top

C#:   // 单行；/* 多行 */
来源：http://tbs.yuanzhike.top

[A15] 空值判断与默认值
来源：http://ish.sweek.top

Py:   value = data or "默认值"
来源：http://ahf.c1oappe.top

PHP:  $value = $data ?? "默认值";
来源：http://cds.shanyushiyangkeji.top

JS:   const value = data ?? "默认值";
来源：http://fsb.haohaochexian.top

TS:   const value = data ?? "默认值";
来源：http://ndw.ydzc1.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bnc.bbcook.cn

Go:   if data == "" { data = "默认值" }
来源：http://ofr.tanke756.top

Ruby: value = data || "默认值"
来源：http://toi.sweek.top

C#:   var value = data ?? "默认值";
来源：http://bmz.shangyingyoupin.top

[A16] 真假值判断规则
来源：http://tlm.gzhubu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baq.fengsongda.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://imr.ydzc1.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qqt.sxryk.cn

TS:   if (!x) {}
来源：http://kzu.ehwqpu.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jmc.ybcxt.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yoo.zhongyouzk.top

Ruby: unless x            # nil 与 false 为假
来源：http://yib.hnqzz.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wmt.feifeiyinyue.top

[A17] 位运算
来源：http://ilm.bbcook.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ozi.bbcook.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nio.pengpengdd.cyou

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://crq.daria6918.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qro.yvedp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fuo.hnqzz.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xgw.yfazqb.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xyo.jinqigfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xnf.shzxlz.cn

[A18] 字符与 ASCII 码互转
来源：http://awq.zhongyouzk.top

Py:   ord("A"); chr(65)
来源：http://jbf.cucudq.cn

PHP:  ord("A"); chr(65)
来源：http://qao.hcnkem.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yax.yuanzhike.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ray.jlsjyb.cn

Java: (int) 'A'; (char) 65
来源：http://vsf.dianchejie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jym.xylfe.cn

Ruby: "A".ord; 65.chr
来源：http://dyu.hfpthk.cn

C#:   (int)'A'; (char)65
来源：http://hcr.0kj1m.cn

[A19] 交换两个变量
来源：http://kgw.cashguo.top

Py:   a, b = b, a
来源：http://fzu.feifeiyinyue.top

PHP:  [$a, $b] = [$b, $a];
来源：http://vvk.yueranfly.top

JS:   [a, b] = [b, a];
来源：http://ore.jyoumei.cn

TS:   [a, b] = [b, a];
来源：http://snm.wangdashe.top

Java: int t = a; a = b; b = t;
来源：http://ikr.redwolf501.top

Go:   a, b = b, a
来源：http://tgh.tian-w.cn

Ruby: a, b = b, a
来源：http://pbe.fehbvm.com

C#:   (a, b) = (b, a);
来源：http://cve.jianghu66.top

[A20] 读取标准输入
来源：http://ybo.kuanghao11.cn

Py:   name = input("请输入：")
来源：http://mxk.yj202588.top

PHP:  $name = trim(fgets(STDIN));
来源：http://fhg.zhijiandao.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vpf.vqdsnc.cn

TS:   // Node.js：readline 模块
来源：http://wcr.ctjpmb.com

Java: new Scanner(System.in).nextLine()
来源：http://rjs.fanxiaobao.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://drp.feifeiyinyue.top

Ruby: gets.chomp
来源：http://bpu.shanyushiyangkeji.top

C#:   Console.ReadLine();
来源：http://ntm.daxiang520.top

[A21] 保留指定小数位输出
来源：http://fho.yuxming.cn

Py:   f"{3.14159:.2f}"
来源：http://prk.hnqzz.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gcx.daria6918.cn

JS:   (3.14159).toFixed(2)
来源：http://nct.snrcjt.cn

TS:   (3.14159).toFixed(2)
来源：http://xgi.jqgufenzy.top

Java: String.format("%.2f", 3.14159)
来源：http://qxb.yanxiufei.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://esj.hnqzz.top

Ruby: format("%.2f", 3.14159)
来源：http://ufs.vqdsnc.cn

C#:   3.14159.ToString("F2")
来源：http://huv.fehbvm.com

[A22] 获取字符串长度
来源：http://row.cucudq.cn

Py:   len(s)
来源：http://xpf.gotoacloud.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yoq.zhaomingkeji.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ocs.jinghuilouyu.cn

TS:   s.length
来源：http://jjv.yuanzhike.top

Java: s.length()
来源：http://vns.ctjpmb.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bhs.jqgufenzy.top

Ruby: s.length
来源：http://tax.zhixingplan.top

C#:   s.Length
来源：http://jrt.jyoumei.cn

[A23] 大小写转换
来源：http://scj.xuetiantiany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ubj.wangdashe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eur.gotoacloud.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sys.yuxming.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tcl.jlsjyb.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mwl.xziqi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://orp.yuanzhike.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://psz.xuetiantiany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vdd.jinyuanbaomall.cn

[A24] 去除首尾空白
来源：http://alb.zhixingplan.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gjg.xuetiantiany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kjf.ehwqpu.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dzo.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gwc.wangdashe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vql.sweek.top

Go:   strings.TrimSpace(s)
来源：http://qae.jiagoushi.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bba.wangdashe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://trq.ydjk.org.cn

[A25] 字符串比较
来源：http://mxm.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://pfc.zycfv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lty.shuidangran.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gse.ywan-chungtsiang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ary.wangdashe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ceq.ydjk.org.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yif.quarkkingdee.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rsj.fengsongda.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hjt.jianghu66.top

[A26] 类型转换总览
来源：http://btn.hysaishi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yqw.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lhh.tarul.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gex.ydzc1.top

TS:   Number() String() Boolean() x as number
来源：http://djs.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qir.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gqi.ctjpmb.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://zcd.pengpengdd.cyou

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tss.jinyuanbaomall.cn

================================================================================
来源：http://pph.nanxuanxn.top

B. 流程控制
来源：http://fjt.haohaochexian.top

================================================================================
来源：http://dig.iojbl.cn

[B01] 条件判断 if / else
来源：http://arm.tanke756.top

Py:   result = "正" if x > 0 else "非正"
来源：http://lkq.xuetiantiany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vza.redwolf501.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fbg.jqgufenzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zdw.hywenlv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jfz.sweek.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jxs.tianlin.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dmz.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rwt.hesvh.cn

[B02] 多分支 else if / elif
来源：http://neb.bjfxy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gei.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jnz.fktsv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ufd.tianlin.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rzc.nanxuanxn.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nsc.shzxlz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yoe.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ord.jianghu66.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lkd.ivvv.top

[B03] switch / match / case
来源：http://uje.cdnleiting.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ham.cashguo.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gze.hongshengwenyu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vbx.tarul.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nmd.zhengqikj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ufk.cashguo.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fqn.gogol.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vnl.yonumen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nud.9152youxi.cn

[B04] for 计数循环
来源：http://ajk.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://ohf.jiagoushi.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ohi.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tma.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pzx.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cil.vqdsnc.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zjw.fktsv.cn

Ruby: 10.times { |i| puts i }
来源：http://fvh.yuanzhike.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mgg.aibaodan.cn

[B05] 遍历数组 / 列表
来源：http://hjr.gzhubu.top

Py:   for item in arr: print(item)
来源：http://oye.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hmf.epnwcf.com

JS:   for (const item of arr) { console.log(item); }
来源：http://tth.yj20258888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hpm.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://nqv.kuanghao11.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pgf.yj202588.top

Ruby: arr.each { |item| puts item }
来源：http://hgi.jiagoushi.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ekr.tian-w.cn

[B06] 遍历字典 / 对象
来源：http://lus.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://ehn.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://beo.zhoulong.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eie.bbcook.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sqc.nwbrower.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://obv.52xcode.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dsl.pengpengdd.cyou

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hak.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eis.hysaishi.cn

[B07] while 循环
来源：http://uqd.yfazqb.com

Py:   while i < 10: i += 1
来源：http://gxv.ydzc1.top

PHP:  while ($i < 10) { $i++; }
来源：http://uvj.ywan-chungtsiang.top

JS:   while (i < 10) { i++; }
来源：http://dky.gaohongyu789.top

TS:   while (i < 10) { i++; }
来源：http://kyr.fengsongda.top

Java: while (i < 10) { i++; }
来源：http://esa.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gri.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://uhx.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://wlw.epnwcf.com

[B08] do-while（至少执行一次）
来源：http://dus.sufxvd.cn

Py:   # 无 do-while：用 while True + break
来源：http://uwx.feifeiyinyue.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xpg.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://mzc.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://kbo.tanke756.top

Java: do { i++; } while (i < 10);
来源：http://bkj.jlsjyb.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ojl.feifeiyinyue.top

Ruby: begin; i += 1; end while i < 10
来源：http://vlw.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://iis.gaohongyu789.top

[B09] break 与 continue
来源：http://oyn.vehdjk.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mut.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dsg.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bkp.sufxvd.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wqr.yangfankeji.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qfh.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ozh.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mrd.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bxk.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://wlm.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://muw.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ikb.tianlin.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yta.jinghuilouyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bua.yuanzhike.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zot.ydzc1.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://arw.xuetiantiany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://daf.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qru.mhx1999.top

[B11] 生成数字序列 / 区间
来源：http://lvu.yueranfly.top

Py:   list(range(0, 10, 2))
来源：http://ebf.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://acz.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pgg.shanyushiyangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pdm.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zin.chenjidiqi.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fku.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://ovt.fengsongda.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jrj.zhijiandao.cn

[B12] 跳出多层循环
来源：http://uow.snrcjt.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://poa.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tdm.jinghuilouyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nbo.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wal.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://afl.shangyingyoupin.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://muy.nwbrower.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zbl.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mkn.pycfn.com

[B13] 判断是否为数字
来源：http://jdl.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://uft.iojbl.cn

PHP:  is_numeric($x)
来源：http://lpd.redwolf501.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://int.daxiang520.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fdj.xingfuxueyuan.xyz

Java: x instanceof Number
来源：http://jow.c1oappe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vvl.jqgfzy.top

Ruby: x.is_a?(Numeric)
来源：http://pbu.zhongyouzk.top


<!-- 参考信息 -->