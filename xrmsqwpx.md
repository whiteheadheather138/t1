代发 wailian999

[A06] 字符串转数字
来源：http://vbi.shanyushiyangtech.top

Py:   int("42"); float("3.14")
来源：http://ego.xuanzx.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gmj.zdbjq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://itl.yj202588.top

TS:   parseInt("42", 10); Number("42")
来源：http://cdd.smart0.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bia.hnxiangtu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://reo.bjfxy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://nui.haohaochexian.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://aao.zhijiandao.cn

[A07] 数字转字符串
来源：http://mhc.jianghu66.top

Py:   str(42)
来源：http://rav.tianlin.xyz

PHP:  (string) 42; strval(42)
来源：http://wco.316326.xyz

JS:   String(42); (42).toString()
来源：http://mkh.zhongyouzk.top

TS:   String(42)
来源：http://ozk.hfpthk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nxt.chenjidiqi.icu

Go:   strconv.Itoa(42)
来源：http://ztc.guowangkeji.top

Ruby: 42.to_s
来源：http://xov.9152youxi.cn

C#:   42.ToString()
来源：http://pji.jianghu66.top

[A08] 取整与四舍五入
来源：http://fqt.yueranfly.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rej.wangshuangyany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wjs.yj20258888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ceg.c1oappe.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mvn.kuanghao11.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://onm.xinyue.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vmd.zhixingplan.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://yzq.bjfxy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zql.nwbrower.top

[A09] 绝对值与最大最小值
来源：http://ybf.jinyuanbaomall.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xrq.hongshengwenyu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pui.redwolf501.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fsf.iojbl.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ebq.fehbvm.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kva.316326.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uah.yueranfly.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eik.zdqjudy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lre.gzhubu.top

[A10] 生成随机数
来源：http://vof.gzhubu.top

Py:   import random; random.randint(1, 100)
来源：http://kov.andypj.xyz

PHP:  random_int(1, 100);
来源：http://kvs.guowangkeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pjk.0kj1m.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rwc.zhixingplan.top

Java: new Random().nextInt(100) + 1
来源：http://bcf.jqgfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lit.fktsv.cn

Ruby: rand(1..100)
来源：http://aim.hnqzz.top

C#:   new Random().Next(1, 101)
来源：http://wsi.zhongyouzk.top

[A11] 条件表达式（三元）
来源：http://cid.hcnkem.com

Py:   "yes" if x > 0 else "no"
来源：http://agd.snrcjt.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zjv.chenjidiqi.icu

JS:   x > 0 ? "yes" : "no"
来源：http://mkr.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bba.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://jge.meibo888.top

Go:   // 无三元运算符，需用 if 语句
来源：http://urd.daria6918.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zel.guannengcc.top

C#:   x > 0 ? "yes" : "no"
来源：http://ghm.vqdsnc.cn

[A12] 字符串插值 / 格式化
来源：http://ljt.cdnleiting.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bkh.zhixingplan.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://noj.meibo888.top

JS:   `Hello, ${name}!`
来源：http://xgq.wangshuangyany.cn

TS:   `Hello, ${name}!`
来源：http://yme.birdmap.top

Java: "Hello, %s!".formatted(name)
来源：http://qwc.ywan-chungtsiang.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mgc.zhixingplan.top

Ruby: "Hello, #{name}!"
来源：http://ymz.zhongyouzk.top

C#:   $"Hello, {name}!"
来源：http://kjk.316326.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://pql.tian-w.cn

Py:   "第一行\n第二行"
来源：http://gsf.dianchejie.cn

PHP:  "第一行\n第二行"
来源：http://mui.nanxinkj.top

JS:   "第一行\n第二行"
来源：http://hyx.hnqzz.top

TS:   "第一行\n第二行"
来源：http://xbg.mhx1999.top

Java: "第一行\n第二行"
来源：http://qwl.daxiang520.top

Go:   "第一行\n第二行"
来源：http://qic.hesvh.cn

Ruby: "第一行\n第二行"
来源：http://azf.sufxvd.cn

C#:   "第一行\n第二行"
来源：http://kys.52xcode.cn

[A14] 注释写法
来源：http://eif.yongpay.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://lbk.jyoumei.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fde.yuanzhike.top

JS:   // 单行；/* 多行 */
来源：http://zhk.sysykeji.top

TS:   // 单行；/* 多行 */
来源：http://zts.bbcook.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wnr.nwbrower.top

Go:   // 单行；/* 多行 */
来源：http://vzh.jiagoushi.top

Ruby: # 单行；=begin 多行 =end
来源：http://tov.quarkkingdee.top

C#:   // 单行；/* 多行 */
来源：http://iol.guowangkeji.top

[A15] 空值判断与默认值
来源：http://beg.hnqzz.top

Py:   value = data or "默认值"
来源：http://ild.ywan-chungtsiang.top

PHP:  $value = $data ?? "默认值";
来源：http://hev.cqqwz.cn

JS:   const value = data ?? "默认值";
来源：http://tgy.shangyingyoupin.top

TS:   const value = data ?? "默认值";
来源：http://hkd.zhijiandao.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cam.yueranfly.top

Go:   if data == "" { data = "默认值" }
来源：http://jpx.hfpthk.cn

Ruby: value = data || "默认值"
来源：http://nlt.zhixingplan.top

C#:   var value = data ?? "默认值";
来源：http://tmy.cashguo.top

[A16] 真假值判断规则
来源：http://asf.cheryme.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vam.xuetiantiany.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hqe.zhengqikj.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lay.xuanzx.com

TS:   if (!x) {}
来源：http://dpc.aizwys.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ota.svipenyu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ysw.shanyushiyangtech.top

Ruby: unless x            # nil 与 false 为假
来源：http://ila.shuidangran.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xrr.bjfxy.top

[A17] 位运算
来源：http://byw.zhoulong.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://avy.pycfn.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ayn.jinghuilouyu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sim.yongpay.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://esk.hammf.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xwd.jinqigufen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jsb.hysaishi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fwg.xylfe.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://boh.jyoumei.cn

[A18] 字符与 ASCII 码互转
来源：http://vtg.jinqigfzy.top

Py:   ord("A"); chr(65)
来源：http://wkk.zdqjudy.top

PHP:  ord("A"); chr(65)
来源：http://iuo.cheryme.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oql.ywan-chungtsiang.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zgq.yongpay.top

Java: (int) 'A'; (char) 65
来源：http://cyx.yj20258888.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uxo.jiagoushi.top

Ruby: "A".ord; 65.chr
来源：http://jni.jqgufenzy.top

C#:   (int)'A'; (char)65
来源：http://uxg.smart0.xyz

[A19] 交换两个变量
来源：http://yru.jinghuilouyu.cn

Py:   a, b = b, a
来源：http://aiz.jinqigufen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://erk.xuanzx.com

JS:   [a, b] = [b, a];
来源：http://ylx.zhijiandao.cn

TS:   [a, b] = [b, a];
来源：http://gog.yuanzhike.top

Java: int t = a; a = b; b = t;
来源：http://mnp.52xcode.cn

Go:   a, b = b, a
来源：http://vpa.ydjk.org.cn

Ruby: a, b = b, a
来源：http://srf.jinqigufen.top

C#:   (a, b) = (b, a);
来源：http://rto.daria6918.cn

[A20] 读取标准输入
来源：http://mkm.zhixingplan.top

Py:   name = input("请输入：")
来源：http://hav.yueranfly.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ykm.ctjpmb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gyt.yj20258888.top

TS:   // Node.js：readline 模块
来源：http://lbr.sufxvd.cn

Java: new Scanner(System.in).nextLine()
来源：http://vsx.jyoumei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kre.ywan-chungtsiang.top

Ruby: gets.chomp
来源：http://pbn.yj202588.top

C#:   Console.ReadLine();
来源：http://ykp.mhx1999.top

[A21] 保留指定小数位输出
来源：http://nkp.daria6918.cn

Py:   f"{3.14159:.2f}"
来源：http://rpy.xuanzx.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://aif.aizwys.cn

JS:   (3.14159).toFixed(2)
来源：http://ilg.jlsjyb.cn

TS:   (3.14159).toFixed(2)
来源：http://ghp.zhongyouzk.top

Java: String.format("%.2f", 3.14159)
来源：http://ybq.gogol.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zln.sysykeji.top

Ruby: format("%.2f", 3.14159)
来源：http://utb.chenlongwang.top

C#:   3.14159.ToString("F2")
来源：http://qqq.shanyushiyangkeji.top

[A22] 获取字符串长度
来源：http://rkn.xziqi.cn

Py:   len(s)
来源：http://ynw.svipenyu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lgk.shuidangran.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://obb.yuxming.cn

TS:   s.length
来源：http://fyp.yonumen.top

Java: s.length()
来源：http://lty.aibaodan.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zed.pengpengdd.cyou

Ruby: s.length
来源：http://xaa.gzhubu.top

C#:   s.Length
来源：http://vls.xziqi.cn

[A23] 大小写转换
来源：http://nbx.hnxiangtu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://llb.ywan-chungtsiang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hpo.redwolf501.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kzn.dashuyun.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dkc.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ohq.jinqigfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kyi.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sup.xingfuxueyuan.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://cje.shanyushiyangtech.top

[A24] 去除首尾空白
来源：http://dwg.sjlbkw.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mkx.ydzc1.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nhv.nanxinkj.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://syo.jinqigfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rvo.c1oappe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vph.yongpay.top

Go:   strings.TrimSpace(s)
来源：http://dhb.andypj.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hcb.shanyushiyangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hvc.cdnleiting.top

[A25] 字符串比较
来源：http://rtp.gotoacloud.top

Py:   s1 == s2; s1 != s2
来源：http://xpi.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wje.yj202588.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mws.chenlongwang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ewp.hcnkem.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://flh.guannengcc.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ffj.xuanzx.com

Ruby: s1 == s2; s1 <=> s2
来源：http://whu.snrcjt.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rft.fktsv.cn

[A26] 类型转换总览
来源：http://jlw.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sls.chenjidiqi.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kab.shzxlz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tbl.aizwys.cn

TS:   Number() String() Boolean() x as number
来源：http://yul.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cfe.yongpay.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tyr.guannengcc.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ttr.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dzg.zhengqikj.top

================================================================================
来源：http://ezh.cdnleiting.top

B. 流程控制
来源：http://wvu.zhoulong.xyz

================================================================================
来源：http://kni.hammf.cn

[B01] 条件判断 if / else
来源：http://njr.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xbl.sxryk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zix.hysaishi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hvn.fzhhl.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ttj.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ezv.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://elm.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zwx.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ytt.sysykeji.top

[B02] 多分支 else if / elif
来源：http://crj.bbcook.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gwx.jinqigfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gau.shanyushiyangkeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jda.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gtl.guannengcc.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fxd.hesvh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://san.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ajs.zhoulong.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://trb.zhengqikj.top

[B03] switch / match / case
来源：http://djv.sysykeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yhd.yongpay.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://szi.mhx1999.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hkw.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xxq.ybcxt.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cmz.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wyy.zdbjq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://muk.uphjek.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rdf.bbcook.cn

[B04] for 计数循环
来源：http://omi.zhiwuduotai.top

Py:   for i in range(10): print(i)
来源：http://cpo.fengsongda.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://drz.zhongyouzk.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yty.xylfe.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://etg.cqqwz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dni.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wna.sufxvd.cn

Ruby: 10.times { |i| puts i }
来源：http://tbs.ywan-chungtsiang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ztz.wangshuangyany.cn

[B05] 遍历数组 / 列表
来源：http://wnn.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://bjd.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nag.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hwh.hammf.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tym.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qev.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fmg.zdqjudy.top

Ruby: arr.each { |item| puts item }
来源：http://ykc.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://duu.tian-w.cn

[B06] 遍历字典 / 对象
来源：http://htu.chenzaomai.com

Py:   for k, v in d.items(): print(k, v)
来源：http://qby.yuxming.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hdi.jqgfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sqt.zhengqikj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://flr.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://scn.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bsj.kuanghao11.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hbf.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ftk.gaohongyu789.top

[B07] while 循环
来源：http://xer.fktsv.cn

Py:   while i < 10: i += 1
来源：http://ujf.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://urr.sxryk.cn

JS:   while (i < 10) { i++; }
来源：http://yrs.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://snm.jyoumei.cn

Java: while (i < 10) { i++; }
来源：http://ccf.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rdm.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://bza.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://cyp.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://kcz.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://fof.ydzc1.top

PHP:  do { $i++; } while ($i < 10);
来源：http://grd.birdmap.top

JS:   do { i++; } while (i < 10);
来源：http://czc.shanyushiyangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://mac.guannengcc.top

Java: do { i++; } while (i < 10);
来源：http://kcm.aizwys.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oja.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://ydx.jinqigufen.top

C#:   do { i++; } while (i < 10);
来源：http://lxp.sufxvd.cn

[B09] break 与 continue
来源：http://uer.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aav.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qgj.ppjwa.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://exf.bbcook.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mea.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mce.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wqx.fanxiaobao.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oaf.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yzl.daria6918.cn

[B10] 遍历同时拿索引
来源：http://omq.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zhs.sweek.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lsa.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kot.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cud.zhoulong.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vtr.kuanghao11.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fnx.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zud.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://znj.yonumen.top

[B11] 生成数字序列 / 区间
来源：http://rkb.andypj.xyz

Py:   list(range(0, 10, 2))
来源：http://ila.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://iwc.hywenlv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nbd.ivvv.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iuk.epnwcf.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aad.daxiang520.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ftq.shuidangran.top

Ruby: (0...10).step(2).to_a
来源：http://xvv.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sks.ppjwa.cn

[B12] 跳出多层循环
来源：http://spe.zhijiandao.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zxm.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://vlp.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tvn.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mho.vehdjk.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gph.cucudq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kjj.xinyue.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dmg.fanxiaobao.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://orl.shzxlz.cn


<!-- 参考信息 -->