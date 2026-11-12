代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://frd.jqgfzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vfp.ctjpmb.com

TS:   typeof x; x instanceof Date
来源：http://dte.bjfxy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jrv.tianlin.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://zax.yfazqb.com

Ruby: x.class; x.is_a?(Integer)
来源：http://sda.zhoulong.xyz

C#:   x.GetType().Name; x is int
来源：http://goc.yonumen.top

[A05] 整数除法与取模
来源：http://dew.52xcode.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rgh.ppjwa.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://unp.vqdsnc.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ejh.vehdjk.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mrq.52xcode.cn

Java: 7 / 2; 7 % 2
来源：http://xky.pycfn.com

Go:   7 / 2; 7 % 2
来源：http://hbk.cheryme.top

Ruby: 7 / 2; 7 % 2
来源：http://nmx.cqqwz.cn

C#:   7 / 2; 7 % 2
来源：http://ttm.cashguo.top

[A06] 字符串转数字
来源：http://hne.ehwqpu.com

Py:   int("42"); float("3.14")
来源：http://bwi.jqgfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fdm.pengpengdd.cyou

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nmk.hongshengwenyu.top

TS:   parseInt("42", 10); Number("42")
来源：http://bzp.wangdashe.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://idv.hnqzz.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qpf.zhixingplan.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fbm.hammf.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uiq.xinyue.icu

[A07] 数字转字符串
来源：http://kqo.yuanzhike.top

Py:   str(42)
来源：http://kyl.hcnkem.com

PHP:  (string) 42; strval(42)
来源：http://ree.yuanzhike.top

JS:   String(42); (42).toString()
来源：http://uwx.hcnkem.com

TS:   String(42)
来源：http://wex.aibaodan.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jlg.xinyue.icu

Go:   strconv.Itoa(42)
来源：http://rqd.xylfe.cn

Ruby: 42.to_s
来源：http://lhl.hnxiangtu.top

C#:   42.ToString()
来源：http://rqi.birdmap.top

[A08] 取整与四舍五入
来源：http://ylu.shzxlz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ghz.gaohongyu789.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://row.daxiang520.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xny.ywan-chungtsiang.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yke.guannengcc.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://are.fzhhl.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ngq.xuetiantiany.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ozm.iojbl.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zpj.xingfuxueyuan.xyz

[A09] 绝对值与最大最小值
来源：http://fgm.daria6918.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://njx.gzhubu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fjr.kuanghao11.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mka.cucudq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xhk.ybcxt.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cez.hnxiangtu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hqu.yangfankeji.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xsd.pycfn.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zba.kuanghao11.cn

[A10] 生成随机数
来源：http://wes.gaohongyu789.top

Py:   import random; random.randint(1, 100)
来源：http://jcy.gzhubu.top

PHP:  random_int(1, 100);
来源：http://fsm.daria6918.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://slg.yangfankeji.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yro.cucudq.cn

Java: new Random().nextInt(100) + 1
来源：http://dfv.hnxiangtu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cqg.fktsv.cn

Ruby: rand(1..100)
来源：http://wbe.nwbrower.top

C#:   new Random().Next(1, 101)
来源：http://sag.shzxlz.cn

[A11] 条件表达式（三元）
来源：http://bky.hnxiangtu.top

Py:   "yes" if x > 0 else "no"
来源：http://zzi.guannengcc.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://rmm.hesvh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ajm.nanxuanxn.top

TS:   x > 0 ? "yes" : "no"
来源：http://ehu.yj20258.top

Java: x > 0 ? "yes" : "no"
来源：http://nxo.andypj.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://kuz.zdbjq.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xhf.andypj.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://lif.pycfn.com

[A12] 字符串插值 / 格式化
来源：http://uux.yuxming.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xxv.xuanzx.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qia.cqqwz.cn

JS:   `Hello, ${name}!`
来源：http://mxm.jqgfzy.top

TS:   `Hello, ${name}!`
来源：http://sbe.xingfuxueyuan.xyz

Java: "Hello, %s!".formatted(name)
来源：http://zsp.gaohongyu789.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uyh.yvedp.cn

Ruby: "Hello, #{name}!"
来源：http://ekd.xylfe.cn

C#:   $"Hello, {name}!"
来源：http://tws.jlsjyb.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://phs.ydzc1.top

Py:   "第一行\n第二行"
来源：http://xmx.gogol.net.cn

PHP:  "第一行\n第二行"
来源：http://mec.hongshengwenyu.top

JS:   "第一行\n第二行"
来源：http://zuu.jinyuanbaomall.cn

TS:   "第一行\n第二行"
来源：http://ixs.redwolf501.top

Java: "第一行\n第二行"
来源：http://azr.hnxiangtu.top

Go:   "第一行\n第二行"
来源：http://uwt.shanyushiyangtech.top

Ruby: "第一行\n第二行"
来源：http://zff.cucudq.cn

C#:   "第一行\n第二行"
来源：http://nrb.316326.xyz

[A14] 注释写法
来源：http://cnb.yonumen.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ugl.dashuyun.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ben.yanxiufei.cn

JS:   // 单行；/* 多行 */
来源：http://xzm.gogol.net.cn

TS:   // 单行；/* 多行 */
来源：http://hrf.bjfxy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wfe.pengpengdd.cyou

Go:   // 单行；/* 多行 */
来源：http://drt.hywenlv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tby.chenjidiqi.icu

C#:   // 单行；/* 多行 */
来源：http://mdd.yongpay.top

[A15] 空值判断与默认值
来源：http://dkf.smart0.xyz

Py:   value = data or "默认值"
来源：http://uto.nanxinkj.top

PHP:  $value = $data ?? "默认值";
来源：http://iul.nanxuanxn.top

JS:   const value = data ?? "默认值";
来源：http://qej.chenlongwang.top

TS:   const value = data ?? "默认值";
来源：http://gin.wangshuangyany.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xcu.sufxvd.cn

Go:   if data == "" { data = "默认值" }
来源：http://qib.aizwys.cn

Ruby: value = data || "默认值"
来源：http://pjr.dashuyun.cn

C#:   var value = data ?? "默认值";
来源：http://kuq.316326.xyz

[A16] 真假值判断规则
来源：http://aav.gogol.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gck.nanxinkj.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gyg.quarkkingdee.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gcc.sysykeji.top

TS:   if (!x) {}
来源：http://vhz.ehwqpu.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fus.chenjidiqi.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iru.daria6918.cn

Ruby: unless x            # nil 与 false 为假
来源：http://afn.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zsy.zhoulong.xyz

[A17] 位运算
来源：http://yxr.quarkkingdee.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://laa.jiagoushi.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sao.guannengcc.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zzn.fktsv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://utw.dianchejie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jvt.nanxuanxn.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ipj.cheryme.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ixu.jqgfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hpd.jiagoushi.top

[A18] 字符与 ASCII 码互转
来源：http://vku.0kj1m.cn

Py:   ord("A"); chr(65)
来源：http://nai.xuetiantiany.cn

PHP:  ord("A"); chr(65)
来源：http://ymo.iojbl.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fxh.yanxiufei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uja.zhongyouzk.top

Java: (int) 'A'; (char) 65
来源：http://xim.jinqigfzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qru.cqqwz.cn

Ruby: "A".ord; 65.chr
来源：http://ayz.vqdsnc.cn

C#:   (int)'A'; (char)65
来源：http://fcb.epnwcf.com

[A19] 交换两个变量
来源：http://nsg.jinyuanbaomall.cn

Py:   a, b = b, a
来源：http://byg.tarul.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ncy.sysykeji.top

JS:   [a, b] = [b, a];
来源：http://kqm.hnxiangtu.top

TS:   [a, b] = [b, a];
来源：http://psn.ydzc1.top

Java: int t = a; a = b; b = t;
来源：http://lgz.ppjwa.cn

Go:   a, b = b, a
来源：http://rxc.pycfn.com

Ruby: a, b = b, a
来源：http://may.guannengcc.top

C#:   (a, b) = (b, a);
来源：http://uir.epnwcf.com

[A20] 读取标准输入
来源：http://ucu.andypj.xyz

Py:   name = input("请输入：")
来源：http://ehm.hnqzz.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qbt.jqgfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bgn.cheryme.top

TS:   // Node.js：readline 模块
来源：http://wox.shzxlz.cn

Java: new Scanner(System.in).nextLine()
来源：http://jcj.ctjpmb.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uzx.wangshuangyany.cn

Ruby: gets.chomp
来源：http://tpc.zhoulong.xyz

C#:   Console.ReadLine();
来源：http://ikp.shuidangran.top

[A21] 保留指定小数位输出
来源：http://cre.aizwys.cn

Py:   f"{3.14159:.2f}"
来源：http://awc.dianchejie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bfx.jinqigufen.top

JS:   (3.14159).toFixed(2)
来源：http://wbe.ydjk.org.cn

TS:   (3.14159).toFixed(2)
来源：http://bny.nanxuanxn.top

Java: String.format("%.2f", 3.14159)
来源：http://urs.vehdjk.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ynz.cdnleiting.top

Ruby: format("%.2f", 3.14159)
来源：http://gqh.quarkkingdee.top

C#:   3.14159.ToString("F2")
来源：http://ibh.zhiwuduotai.top

[A22] 获取字符串长度
来源：http://tut.ctjpmb.com

Py:   len(s)
来源：http://hga.nwbrower.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wmd.xziqi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qgz.daria6918.cn

TS:   s.length
来源：http://zyq.jinqigfzy.top

Java: s.length()
来源：http://ogk.hesvh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iay.yongpay.top

Ruby: s.length
来源：http://ncj.feifeiyinyue.top

C#:   s.Length
来源：http://vck.haohaochexian.top

[A23] 大小写转换
来源：http://knd.hammf.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xus.guowangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gex.birdmap.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hnv.gaohongyu789.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://szg.vqdsnc.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qkt.hongshengwenyu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wvs.iojbl.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://are.zycfv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ppm.xingfuxueyuan.xyz

[A24] 去除首尾空白
来源：http://lcl.shzxlz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bgk.guannengcc.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dlu.dashuyun.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dzh.ydjk.org.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tqx.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://frl.yueranfly.top

Go:   strings.TrimSpace(s)
来源：http://imp.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xzk.jqgfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gci.fengsongda.top

[A25] 字符串比较
来源：http://lkp.zhengqikj.top

Py:   s1 == s2; s1 != s2
来源：http://elw.chenjidiqi.icu

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qpw.nanxinkj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ram.fzhhl.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iat.gaohongyu789.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uhh.gaohongyu789.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vtv.hesvh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qxg.aibaodan.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://okh.ctjpmb.com

[A26] 类型转换总览
来源：http://ihz.gotoacloud.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cme.ydjk.org.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zdu.fanxiaobao.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gwt.gaohongyu789.top

TS:   Number() String() Boolean() x as number
来源：http://osa.jinqigufen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qxw.shzxlz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://had.sweek.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ljz.ehwqpu.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vtd.chenjidiqi.icu

================================================================================
来源：http://rwg.nanxinkj.top

B. 流程控制
来源：http://zpa.ctjpmb.com

================================================================================
来源：http://cyg.fengsongda.top

[B01] 条件判断 if / else
来源：http://bjs.redwolf501.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gzt.jianghu66.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zgw.chenlongwang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oyu.daria6918.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iuz.jinqigufen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://llc.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rai.epnwcf.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tsl.yj20258.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://knz.c1oappe.top

[B02] 多分支 else if / elif
来源：http://vit.jinyuanbaomall.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kcc.hfpthk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cmz.fzhhl.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uwt.aibaodan.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xqg.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mnp.xingfuxueyuan.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xgb.dianchejie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eec.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nnh.jlsjyb.cn

[B03] switch / match / case
来源：http://gjy.yj20258888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jfm.yj20258888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vnh.xuetiantiany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ydw.nwbrower.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hqt.hammf.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ylz.fktsv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ctb.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pbc.havefunace.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vlj.jinqigfzy.top

[B04] for 计数循环
来源：http://hdf.fzhhl.top

Py:   for i in range(10): print(i)
来源：http://tgt.jinyuanbaomall.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eau.jianghu66.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xkf.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yfr.hcnkem.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ikw.cqqwz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yfx.52xcode.cn

Ruby: 10.times { |i| puts i }
来源：http://vsy.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ysx.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://kio.hfpthk.cn

Py:   for item in arr: print(item)
来源：http://cgr.yuanzhike.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kqy.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://snq.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hfl.snrcjt.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://klo.yuxming.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xsd.nwbrower.top

Ruby: arr.each { |item| puts item }
来源：http://cjp.mhx1999.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nhl.xziqi.cn

[B06] 遍历字典 / 对象
来源：http://gdi.dianchejie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uiq.yongpay.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aez.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wvm.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sfh.gzhubu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vkq.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yva.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rdr.epnwcf.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vjx.hysaishi.cn

[B07] while 循环
来源：http://gnd.zycfv.cn

Py:   while i < 10: i += 1
来源：http://hro.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://mai.ybcxt.top

JS:   while (i < 10) { i++; }
来源：http://vxl.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://dla.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://txt.zhongyouzk.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://scd.zhoulong.xyz

Ruby: while i < 10; i += 1; end
来源：http://vbz.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://jrx.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://mia.snrcjt.cn

Py:   # 无 do-while：用 while True + break
来源：http://wel.xinyue.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://kyw.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://hcw.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://ekd.daria6918.cn

Java: do { i++; } while (i < 10);
来源：http://dqz.sufxvd.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wia.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qex.zhaomingkeji.xyz

C#:   do { i++; } while (i < 10);
来源：http://unp.nanxinkj.top

[B09] break 与 continue
来源：http://ndp.meibo888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fhl.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ejv.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://loh.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bdw.jlsjyb.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dkq.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gjg.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oen.yangfankeji.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xpq.havefunace.top

[B10] 遍历同时拿索引
来源：http://ulw.0kj1m.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://owp.pengpengdd.cyou

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dpq.jlsjyb.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vwd.bbcook.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nli.shanyushiyangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vzp.yanxiufei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xas.yonumen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aph.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ddo.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://zdc.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://lbt.nanxuanxn.top


<!-- 参考信息 -->