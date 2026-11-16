代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://hsf.yonumen.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xzt.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://mxd.hammf.cn

[A05] 整数除法与取模
来源：http://yxu.snrcjt.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rnl.yvedp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kvn.vehdjk.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tgn.0kj1m.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mbw.gzhubu.top

Java: 7 / 2; 7 % 2
来源：http://pmq.gaohongyu789.top

Go:   7 / 2; 7 % 2
来源：http://ykn.yvedp.cn

Ruby: 7 / 2; 7 % 2
来源：http://rha.yj202588.top

C#:   7 / 2; 7 % 2
来源：http://xtd.meibo888.top

[A06] 字符串转数字
来源：http://cox.hysaishi.cn

Py:   int("42"); float("3.14")
来源：http://vzm.chenzaomai.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://riu.aibaodan.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://efk.jyoumei.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oqs.dianchejie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://swj.fanxiaobao.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://puv.52xcode.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bsn.chenlongwang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kvs.yangfankeji.com

[A07] 数字转字符串
来源：http://lbw.fengsongda.top

Py:   str(42)
来源：http://ycw.snrcjt.cn

PHP:  (string) 42; strval(42)
来源：http://hio.vqdsnc.cn

JS:   String(42); (42).toString()
来源：http://qqh.epnwcf.com

TS:   String(42)
来源：http://pfa.bjfxy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pgl.sweek.top

Go:   strconv.Itoa(42)
来源：http://jom.zhongyouzk.top

Ruby: 42.to_s
来源：http://zto.jyoumei.cn

C#:   42.ToString()
来源：http://ymu.gotoacloud.top

[A08] 取整与四舍五入
来源：http://hve.sweek.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rne.daxiang520.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zdb.xylfe.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://znq.hcnkem.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gme.cdnleiting.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nma.0kj1m.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zua.ybcxt.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xck.0kj1m.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cxt.hnqzz.top

[A09] 绝对值与最大最小值
来源：http://qdt.guannengcc.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rcs.jinqigufen.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bel.iojbl.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jpj.hcnkem.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://brq.gzhubu.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nit.cqqwz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pxc.hywenlv.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wsq.sweek.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ykp.mhx1999.top

[A10] 生成随机数
来源：http://oim.sjlbkw.cn

Py:   import random; random.randint(1, 100)
来源：http://jpa.ctjpmb.com

PHP:  random_int(1, 100);
来源：http://zbh.andypj.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oqn.zhixingplan.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ayw.yj202588.top

Java: new Random().nextInt(100) + 1
来源：http://lig.sufxvd.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gwj.jlsjyb.cn

Ruby: rand(1..100)
来源：http://fzq.jqgufenzy.top

C#:   new Random().Next(1, 101)
来源：http://pig.guowangkeji.top

[A11] 条件表达式（三元）
来源：http://gje.jinqigufen.top

Py:   "yes" if x > 0 else "no"
来源：http://djh.aizwys.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vfx.haohaochexian.top

JS:   x > 0 ? "yes" : "no"
来源：http://xsp.xingfuxueyuan.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://yvw.vqdsnc.cn

Java: x > 0 ? "yes" : "no"
来源：http://fsa.cqqwz.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kjd.sjlbkw.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nvt.hesvh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gxi.shanyushiyangtech.top

[A12] 字符串插值 / 格式化
来源：http://riu.shanyushiyangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rgb.c1oappe.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://eeo.yj202588.top

JS:   `Hello, ${name}!`
来源：http://nxh.zhoulong.xyz

TS:   `Hello, ${name}!`
来源：http://zsz.shangyingyoupin.top

Java: "Hello, %s!".formatted(name)
来源：http://zid.pycfn.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://htt.sjlbkw.cn

Ruby: "Hello, #{name}!"
来源：http://zrk.jiagoushi.top

C#:   $"Hello, {name}!"
来源：http://qwd.hammf.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ryt.wangdashe.top

Py:   "第一行\n第二行"
来源：http://rib.hnxiangtu.top

PHP:  "第一行\n第二行"
来源：http://xph.sysykeji.top

JS:   "第一行\n第二行"
来源：http://dxn.ctjpmb.com

TS:   "第一行\n第二行"
来源：http://nxu.tarul.cn

Java: "第一行\n第二行"
来源：http://twh.yuxming.cn

Go:   "第一行\n第二行"
来源：http://lwy.ybcxt.top

Ruby: "第一行\n第二行"
来源：http://kxy.dianchejie.cn

C#:   "第一行\n第二行"
来源：http://taf.daria6918.cn

[A14] 注释写法
来源：http://ycz.andypj.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://ffj.hnxiangtu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://odo.vqdsnc.cn

JS:   // 单行；/* 多行 */
来源：http://ojx.gaohongyu789.top

TS:   // 单行；/* 多行 */
来源：http://kxa.aibaodan.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zta.xziqi.cn

Go:   // 单行；/* 多行 */
来源：http://xet.fengsongda.top

Ruby: # 单行；=begin 多行 =end
来源：http://wdd.hesvh.cn

C#:   // 单行；/* 多行 */
来源：http://bfj.sufxvd.cn

[A15] 空值判断与默认值
来源：http://jdl.nanxuanxn.top

Py:   value = data or "默认值"
来源：http://fze.yvedp.cn

PHP:  $value = $data ?? "默认值";
来源：http://mkm.hnqzz.top

JS:   const value = data ?? "默认值";
来源：http://mnk.cdnleiting.top

TS:   const value = data ?? "默认值";
来源：http://bid.yongpay.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lhw.hongshengwenyu.top

Go:   if data == "" { data = "默认值" }
来源：http://wli.shanyushiyangkeji.top

Ruby: value = data || "默认值"
来源：http://ucz.epnwcf.com

C#:   var value = data ?? "默认值";
来源：http://oef.ywan-chungtsiang.top

[A16] 真假值判断规则
来源：http://hcc.yueranfly.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wxf.fengsongda.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ujm.haohaochexian.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dts.jinyuanbaomall.cn

TS:   if (!x) {}
来源：http://pkf.yueranfly.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://szp.wangshuangyany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ftr.jiagoushi.top

Ruby: unless x            # nil 与 false 为假
来源：http://jrs.ybcxt.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://iej.havefunace.top

[A17] 位运算
来源：http://kbr.shanyushiyangtech.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vrw.yfazqb.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kpx.jyoumei.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iiu.yangfankeji.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tpc.tian-w.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vhm.gotoacloud.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iun.xingfuxueyuan.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mal.nanxuanxn.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ntw.quarkkingdee.top

[A18] 字符与 ASCII 码互转
来源：http://rup.birdmap.top

Py:   ord("A"); chr(65)
来源：http://lqo.xingfuxueyuan.xyz

PHP:  ord("A"); chr(65)
来源：http://bhd.daxiang520.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zva.c1oappe.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lff.gzhubu.top

Java: (int) 'A'; (char) 65
来源：http://zyq.hcnkem.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kod.hfpthk.cn

Ruby: "A".ord; 65.chr
来源：http://fbs.pengpengdd.cyou

C#:   (int)'A'; (char)65
来源：http://nuo.kuanghao11.cn

[A19] 交换两个变量
来源：http://cdd.jqgfzy.top

Py:   a, b = b, a
来源：http://job.nanxuanxn.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ato.epnwcf.com

JS:   [a, b] = [b, a];
来源：http://ffk.chenzaomai.com

TS:   [a, b] = [b, a];
来源：http://gye.dashuyun.cn

Java: int t = a; a = b; b = t;
来源：http://pvm.ybcxt.top

Go:   a, b = b, a
来源：http://ygp.fanxiaobao.xyz

Ruby: a, b = b, a
来源：http://fzv.gogol.net.cn

C#:   (a, b) = (b, a);
来源：http://nfa.fengsongda.top

[A20] 读取标准输入
来源：http://xnp.snrcjt.cn

Py:   name = input("请输入：")
来源：http://gpw.hongshengwenyu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://geh.andypj.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kvq.jyoumei.cn

TS:   // Node.js：readline 模块
来源：http://woo.epnwcf.com

Java: new Scanner(System.in).nextLine()
来源：http://xgg.jinqigfzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fav.wangshuangyany.cn

Ruby: gets.chomp
来源：http://xaz.dashuyun.cn

C#:   Console.ReadLine();
来源：http://bxj.yuxming.cn

[A21] 保留指定小数位输出
来源：http://qbf.yfazqb.com

Py:   f"{3.14159:.2f}"
来源：http://pkc.sxryk.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xzp.wangshuangyany.cn

JS:   (3.14159).toFixed(2)
来源：http://gkh.hammf.cn

TS:   (3.14159).toFixed(2)
来源：http://onr.zhongyouzk.top

Java: String.format("%.2f", 3.14159)
来源：http://bld.hesvh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://myx.zhaomingkeji.xyz

Ruby: format("%.2f", 3.14159)
来源：http://diw.chenjidiqi.icu

C#:   3.14159.ToString("F2")
来源：http://ibj.sysykeji.top

[A22] 获取字符串长度
来源：http://awr.yongpay.top

Py:   len(s)
来源：http://fya.zhijiandao.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://edk.redwolf501.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qdu.jlsjyb.cn

TS:   s.length
来源：http://elz.hnqzz.top

Java: s.length()
来源：http://tss.jianghu66.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dlc.ywan-chungtsiang.top

Ruby: s.length
来源：http://yas.zhongyouzk.top

C#:   s.Length
来源：http://czw.jinqigfzy.top

[A23] 大小写转换
来源：http://ooa.hammf.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sfv.epnwcf.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lus.yvedp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cyr.zhijiandao.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zjl.hcnkem.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yez.quarkkingdee.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yrj.jqgufenzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://otr.jinqigufen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xbg.havefunace.top

[A24] 去除首尾空白
来源：http://hbe.guowangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ldu.andypj.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xqj.hnxiangtu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fms.yonumen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iyk.birdmap.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mji.feifeiyinyue.top

Go:   strings.TrimSpace(s)
来源：http://cug.ybcxt.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://esk.cdnleiting.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bvz.epnwcf.com

[A25] 字符串比较
来源：http://msm.fengsongda.top

Py:   s1 == s2; s1 != s2
来源：http://wlb.zhengqikj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pjz.yanxiufei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eeb.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zkm.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kho.nanxinkj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oyh.zhiwuduotai.top

Ruby: s1 == s2; s1 <=> s2
来源：http://eoy.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ldm.zhengqikj.top

[A26] 类型转换总览
来源：http://rou.jinyuanbaomall.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ldi.xziqi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pmf.yanxiufei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eob.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://lpk.jinqigufen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ujq.xingfuxueyuan.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jvs.cheryme.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://non.gzhubu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nie.ydjk.org.cn

================================================================================
来源：http://poj.hongshengwenyu.top

B. 流程控制
来源：http://whn.fengsongda.top

================================================================================
来源：http://lfi.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://dok.jinyuanbaomall.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://drn.vqdsnc.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pvt.yueranfly.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bpi.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wow.dashuyun.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vbp.gzhubu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jcp.nwbrower.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cey.hnxiangtu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zrq.shuidangran.top

[B02] 多分支 else if / elif
来源：http://vwv.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gnn.zdbjq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ffo.hcnkem.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gbu.jlsjyb.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://suh.ppjwa.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zbm.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zoz.jianghu66.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aum.yj20258.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://brq.dianchejie.cn

[B03] switch / match / case
来源：http://wau.sjlbkw.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ozj.yj20258.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qgl.chenjidiqi.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vxh.zhongyouzk.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://azz.daxiang520.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tvt.c1oappe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qsd.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vnc.chenzaomai.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rrp.gotoacloud.top

[B04] for 计数循环
来源：http://lyh.zhengqikj.top

Py:   for i in range(10): print(i)
来源：http://pqs.haohaochexian.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vss.shanyushiyangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tlj.316326.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://swb.xinyue.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ysf.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dcv.fzhhl.top

Ruby: 10.times { |i| puts i }
来源：http://xjx.52xcode.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pwe.yuxming.cn

[B05] 遍历数组 / 列表
来源：http://odc.redwolf501.top

Py:   for item in arr: print(item)
来源：http://uqt.daxiang520.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qeh.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ndu.nanxuanxn.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wvc.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://nlb.yongpay.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yjg.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://fvb.gzhubu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://buo.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://mgj.vqdsnc.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yfj.cucudq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lrp.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mak.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://duf.chenlongwang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ipj.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hay.chenjidiqi.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wjb.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hdq.ppjwa.cn

[B07] while 循环
来源：http://lng.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://fjb.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jds.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://ndc.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://rvw.52xcode.cn

Java: while (i < 10) { i++; }
来源：http://dww.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aal.tian-w.cn

Ruby: while i < 10; i += 1; end
来源：http://gjn.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://jeb.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://afn.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://oit.wangshuangyany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zor.zdbjq.cn

JS:   do { i++; } while (i < 10);
来源：http://hxd.yueranfly.top

TS:   do { i++; } while (i < 10);
来源：http://bav.snrcjt.cn

Java: do { i++; } while (i < 10);
来源：http://cly.jlsjyb.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cxo.hnxiangtu.top

Ruby: begin; i += 1; end while i < 10
来源：http://hko.pycfn.com

C#:   do { i++; } while (i < 10);
来源：http://svo.andypj.xyz

[B09] break 与 continue
来源：http://xry.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dgf.shanyushiyangtech.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mwf.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ems.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dyz.smart0.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jpl.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jjf.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lic.zdbjq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lkn.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://fkf.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qdw.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://udm.tarul.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ccl.fanxiaobao.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://glp.ydjk.org.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uog.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oqq.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tzl.yj20258888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nmj.yfazqb.com

[B11] 生成数字序列 / 区间
来源：http://ibk.zhixingplan.top

Py:   list(range(0, 10, 2))
来源：http://clb.daria6918.cn

PHP:  range(0, 10, 2);
来源：http://kpp.shzxlz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gzm.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://new.haohaochexian.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qsd.52xcode.cn


<!-- 参考信息 -->