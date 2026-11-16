代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://piu.ppjwa.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qkg.gogol.net.cn

C#:   x.GetType().Name; x is int
来源：http://xom.xziqi.cn

[A05] 整数除法与取模
来源：http://kcx.yj202588.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://crq.hesvh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uss.xylfe.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://psu.dashuyun.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mny.epnwcf.com

Java: 7 / 2; 7 % 2
来源：http://vcd.sysykeji.top

Go:   7 / 2; 7 % 2
来源：http://bwm.zhijiandao.cn

Ruby: 7 / 2; 7 % 2
来源：http://czz.jinyuanbaomall.cn

C#:   7 / 2; 7 % 2
来源：http://mrd.svipenyu.cn

[A06] 字符串转数字
来源：http://rnt.ybcxt.top

Py:   int("42"); float("3.14")
来源：http://cmk.yvedp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sbb.52xcode.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pdj.yangfankeji.com

TS:   parseInt("42", 10); Number("42")
来源：http://gvc.hysaishi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://all.ehwqpu.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qzl.fzhhl.top

Ruby: "42".to_i; "3.14".to_f
来源：http://yfs.yj202588.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://szn.hnqzz.top

[A07] 数字转字符串
来源：http://hzo.dianchejie.cn

Py:   str(42)
来源：http://gfg.wangdashe.top

PHP:  (string) 42; strval(42)
来源：http://jot.yuanzhike.top

JS:   String(42); (42).toString()
来源：http://qgf.yongpay.top

TS:   String(42)
来源：http://grq.chenlongwang.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://bwb.xingfuxueyuan.xyz

Go:   strconv.Itoa(42)
来源：http://qnc.shangyingyoupin.top

Ruby: 42.to_s
来源：http://fjz.xylfe.cn

C#:   42.ToString()
来源：http://umo.fehbvm.com

[A08] 取整与四舍五入
来源：http://cmd.gogol.net.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mct.hesvh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gun.yj20258888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uhe.aizwys.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zoq.chenzaomai.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fsh.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qwc.zycfv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cvr.svipenyu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ins.hnqzz.top

[A09] 绝对值与最大最小值
来源：http://wxt.hnqzz.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://iec.birdmap.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://odo.ivvv.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ylw.ydzc1.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ibz.tanke756.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://siq.xinyue.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://abe.uphjek.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tud.tianlin.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uvs.52xcode.cn

[A10] 生成随机数
来源：http://kmr.andypj.xyz

Py:   import random; random.randint(1, 100)
来源：http://dth.xuanzx.com

PHP:  random_int(1, 100);
来源：http://prx.svipenyu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kto.cqqwz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pkk.fengsongda.top

Java: new Random().nextInt(100) + 1
来源：http://eyz.pycfn.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wcr.gotoacloud.top

Ruby: rand(1..100)
来源：http://tnq.zhengqikj.top

C#:   new Random().Next(1, 101)
来源：http://foz.mhx1999.top

[A11] 条件表达式（三元）
来源：http://sig.epnwcf.com

Py:   "yes" if x > 0 else "no"
来源：http://rrq.shangyingyoupin.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://hkz.quarkkingdee.top

JS:   x > 0 ? "yes" : "no"
来源：http://aoj.ywan-chungtsiang.top

TS:   x > 0 ? "yes" : "no"
来源：http://qbc.hnxiangtu.top

Java: x > 0 ? "yes" : "no"
来源：http://xjz.yuanzhike.top

Go:   // 无三元运算符，需用 if 语句
来源：http://deq.yonumen.top

Ruby: x > 0 ? "yes" : "no"
来源：http://skt.xingfuxueyuan.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://nnl.xuetiantiany.cn

[A12] 字符串插值 / 格式化
来源：http://cfd.nwbrower.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://spb.ctjpmb.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://icx.yuxming.cn

JS:   `Hello, ${name}!`
来源：http://jnv.9152youxi.cn

TS:   `Hello, ${name}!`
来源：http://ieq.hnxiangtu.top

Java: "Hello, %s!".formatted(name)
来源：http://mug.sxryk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nmf.xuanzx.com

Ruby: "Hello, #{name}!"
来源：http://lbj.shangyingyoupin.top

C#:   $"Hello, {name}!"
来源：http://imv.chenlongwang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://uan.fktsv.cn

Py:   "第一行\n第二行"
来源：http://lib.vqdsnc.cn

PHP:  "第一行\n第二行"
来源：http://dwg.nwbrower.top

JS:   "第一行\n第二行"
来源：http://dux.9152youxi.cn

TS:   "第一行\n第二行"
来源：http://zrh.mhx1999.top

Java: "第一行\n第二行"
来源：http://zer.gzhubu.top

Go:   "第一行\n第二行"
来源：http://zha.jinyuanbaomall.cn

Ruby: "第一行\n第二行"
来源：http://wpq.yvedp.cn

C#:   "第一行\n第二行"
来源：http://afo.xinyue.icu

[A14] 注释写法
来源：http://egr.ydjk.org.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://toh.guannengcc.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://fzd.ivvv.top

JS:   // 单行；/* 多行 */
来源：http://nhb.guowangkeji.top

TS:   // 单行；/* 多行 */
来源：http://kio.shuidangran.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://asx.bjfxy.top

Go:   // 单行；/* 多行 */
来源：http://dhb.yangfankeji.com

Ruby: # 单行；=begin 多行 =end
来源：http://toj.yfazqb.com

C#:   // 单行；/* 多行 */
来源：http://ljl.redwolf501.top

[A15] 空值判断与默认值
来源：http://fat.tarul.cn

Py:   value = data or "默认值"
来源：http://wzp.daria6918.cn

PHP:  $value = $data ?? "默认值";
来源：http://fwn.0kj1m.cn

JS:   const value = data ?? "默认值";
来源：http://srg.yonumen.top

TS:   const value = data ?? "默认值";
来源：http://rgq.pycfn.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://whq.dianchejie.cn

Go:   if data == "" { data = "默认值" }
来源：http://ddb.ydzc1.top

Ruby: value = data || "默认值"
来源：http://sim.sufxvd.cn

C#:   var value = data ?? "默认值";
来源：http://app.epnwcf.com

[A16] 真假值判断规则
来源：http://miq.zhiwuduotai.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://msk.jinqigufen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zeh.smart0.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kzf.xinyue.icu

TS:   if (!x) {}
来源：http://ibp.hammf.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yjt.shangyingyoupin.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sxs.zdqjudy.top

Ruby: unless x            # nil 与 false 为假
来源：http://vpv.shuidangran.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hru.meibo888.top

[A17] 位运算
来源：http://edz.9152youxi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pex.bjfxy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bgi.hnqzz.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hvz.shzxlz.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xps.sysykeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fel.kuanghao11.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wlw.xylfe.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zad.hesvh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xrg.zhaomingkeji.xyz

[A18] 字符与 ASCII 码互转
来源：http://bfn.aizwys.cn

Py:   ord("A"); chr(65)
来源：http://ljw.birdmap.top

PHP:  ord("A"); chr(65)
来源：http://esl.sjlbkw.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fvo.sweek.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yvi.hysaishi.cn

Java: (int) 'A'; (char) 65
来源：http://hhq.shangyingyoupin.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kyv.zhiwuduotai.top

Ruby: "A".ord; 65.chr
来源：http://wzv.havefunace.top

C#:   (int)'A'; (char)65
来源：http://ryo.hesvh.cn

[A19] 交换两个变量
来源：http://mny.sufxvd.cn

Py:   a, b = b, a
来源：http://byn.yfazqb.com

PHP:  [$a, $b] = [$b, $a];
来源：http://eim.jinqigufen.top

JS:   [a, b] = [b, a];
来源：http://csx.gaohongyu789.top

TS:   [a, b] = [b, a];
来源：http://vnm.cdnleiting.top

Java: int t = a; a = b; b = t;
来源：http://wmy.sysykeji.top

Go:   a, b = b, a
来源：http://iug.hysaishi.cn

Ruby: a, b = b, a
来源：http://mag.zhiwuduotai.top

C#:   (a, b) = (b, a);
来源：http://che.zhiwuduotai.top

[A20] 读取标准输入
来源：http://bns.feifeiyinyue.top

Py:   name = input("请输入：")
来源：http://etq.daxiang520.top

PHP:  $name = trim(fgets(STDIN));
来源：http://fyz.jianghu66.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ydb.ydjk.org.cn

TS:   // Node.js：readline 模块
来源：http://wjq.ydjk.org.cn

Java: new Scanner(System.in).nextLine()
来源：http://wre.ybcxt.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qsp.yj202588.top

Ruby: gets.chomp
来源：http://fec.xinyue.icu

C#:   Console.ReadLine();
来源：http://tqu.shzxlz.cn

[A21] 保留指定小数位输出
来源：http://xar.daxiang520.top

Py:   f"{3.14159:.2f}"
来源：http://qsb.cdnleiting.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bmo.shzxlz.cn

JS:   (3.14159).toFixed(2)
来源：http://jbv.sysykeji.top

TS:   (3.14159).toFixed(2)
来源：http://ylq.zhixingplan.top

Java: String.format("%.2f", 3.14159)
来源：http://mzn.dianchejie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rdg.gogol.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://wop.jyoumei.cn

C#:   3.14159.ToString("F2")
来源：http://dol.kuanghao11.cn

[A22] 获取字符串长度
来源：http://zwm.meibo888.top

Py:   len(s)
来源：http://auv.52xcode.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pbz.daria6918.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qqc.shuidangran.top

TS:   s.length
来源：http://lst.jqgufenzy.top

Java: s.length()
来源：http://uwq.zhixingplan.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://apo.feifeiyinyue.top

Ruby: s.length
来源：http://end.fengsongda.top

C#:   s.Length
来源：http://pki.zhaomingkeji.xyz

[A23] 大小写转换
来源：http://gkc.chenzaomai.com

Py:   s.upper(); s.lower(); s.title()
来源：http://qcb.jqgufenzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ckw.shanyushiyangtech.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qol.cdnleiting.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nfu.hammf.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uni.jianghu66.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jxb.daxiang520.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lzx.jiagoushi.top

C#:   s.ToUpper(); s.ToLower()
来源：http://cum.ywan-chungtsiang.top

[A24] 去除首尾空白
来源：http://gqr.guowangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cyk.zhixingplan.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uqg.fzhhl.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://srv.kuanghao11.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hbc.daxiang520.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://anr.fanxiaobao.xyz

Go:   strings.TrimSpace(s)
来源：http://axp.cashguo.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jxw.yj20258888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oyb.sjlbkw.cn

[A25] 字符串比较
来源：http://wlg.tarul.cn

Py:   s1 == s2; s1 != s2
来源：http://rwh.jinyuanbaomall.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://agd.birdmap.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ekh.shangyingyoupin.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://koy.dianchejie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uan.sjlbkw.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hvz.jiagoushi.top

Ruby: s1 == s2; s1 <=> s2
来源：http://swv.jinqigufen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://esr.fehbvm.com

[A26] 类型转换总览
来源：http://pci.9152youxi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ixt.yonumen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rio.dashuyun.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yqy.jinqigfzy.top

TS:   Number() String() Boolean() x as number
来源：http://awv.vehdjk.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vlm.ywan-chungtsiang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fgu.cqqwz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yzq.iojbl.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://trs.fehbvm.com

================================================================================
来源：http://rxe.shzxlz.cn

B. 流程控制
来源：http://beu.aizwys.cn

================================================================================
来源：http://xcn.pycfn.com

[B01] 条件判断 if / else
来源：http://pcq.cdnleiting.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jpn.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://alb.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qmf.cheryme.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bij.xingfuxueyuan.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://jfw.ydjk.org.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kiw.tian-w.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ycg.zhoulong.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mhg.zdbjq.cn

[B02] 多分支 else if / elif
来源：http://mso.hysaishi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hqj.feifeiyinyue.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dbi.havefunace.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qxk.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nsf.shangyingyoupin.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gjx.jyoumei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://itn.zdbjq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rlz.yj202588.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pqc.hfpthk.cn

[B03] switch / match / case
来源：http://gtd.tanke756.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xnf.fengsongda.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lnq.zhiwuduotai.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iol.svipenyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gll.zhijiandao.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fvd.fehbvm.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ari.shanyushiyangtech.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wun.haohaochexian.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lzy.nanxinkj.top

[B04] for 计数循环
来源：http://lrw.ydjk.org.cn

Py:   for i in range(10): print(i)
来源：http://vgk.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tlj.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ugh.redwolf501.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oaw.hywenlv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zvz.xuetiantiany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zpj.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://qro.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ywk.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://rmt.ehwqpu.com

Py:   for item in arr: print(item)
来源：http://vru.xuetiantiany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lye.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ijk.fzhhl.top

TS:   for (const item of arr) { console.log(item); }
来源：http://muz.yuxming.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://euv.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fqy.aizwys.cn

Ruby: arr.each { |item| puts item }
来源：http://gtv.uphjek.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lsb.quarkkingdee.top

[B06] 遍历字典 / 对象
来源：http://gtg.dianchejie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dgf.dianchejie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rjy.tarul.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pdw.havefunace.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bhj.jlsjyb.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mpi.ydzc1.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zqv.9152youxi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bkh.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zwe.cdnleiting.top

[B07] while 循环
来源：http://rcs.hfpthk.cn

Py:   while i < 10: i += 1
来源：http://vek.zhiwuduotai.top

PHP:  while ($i < 10) { $i++; }
来源：http://svo.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://jfb.sweek.top

TS:   while (i < 10) { i++; }
来源：http://pgn.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://yhz.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pes.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://dqk.shanyushiyangtech.top

C#:   while (i < 10) { i++; }
来源：http://ini.tarul.cn

[B08] do-while（至少执行一次）
来源：http://yzo.hongshengwenyu.top

Py:   # 无 do-while：用 while True + break
来源：http://vkr.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gjz.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://ypz.hnxiangtu.top

TS:   do { i++; } while (i < 10);
来源：http://ote.jlsjyb.cn

Java: do { i++; } while (i < 10);
来源：http://pcd.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://rch.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://jra.pengpengdd.cyou

C#:   do { i++; } while (i < 10);
来源：http://ytu.0kj1m.cn

[B09] break 与 continue
来源：http://wct.tanke756.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://btk.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uzd.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://puq.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://emj.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pqq.yongpay.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uqa.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kdf.tarul.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vew.dianchejie.cn

[B10] 遍历同时拿索引
来源：http://vxi.nwbrower.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bxj.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://igy.ivvv.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sec.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jao.ybcxt.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qnj.ivvv.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fjv.zhengqikj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wte.yonumen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mox.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://pyu.xingfuxueyuan.xyz

Py:   list(range(0, 10, 2))
来源：http://ksp.ivvv.top

PHP:  range(0, 10, 2);
来源：http://ojm.uphjek.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xrc.jinghuilouyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ntw.nwbrower.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ymq.hongshengwenyu.top


<!-- 参考信息 -->