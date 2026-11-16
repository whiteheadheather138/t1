代发 wailian999

[A06] 字符串转数字
来源：http://par.xinyue.icu

Py:   int("42"); float("3.14")
来源：http://xin.guowangkeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tlx.cheryme.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uge.ivvv.top

TS:   parseInt("42", 10); Number("42")
来源：http://vfd.xinyue.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jsm.jiagoushi.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lcl.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://thv.xinyue.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vyo.gzhubu.top

[A07] 数字转字符串
来源：http://zuh.dianchejie.cn

Py:   str(42)
来源：http://hhz.ehwqpu.com

PHP:  (string) 42; strval(42)
来源：http://otv.jinqigfzy.top

JS:   String(42); (42).toString()
来源：http://wpw.bbcook.cn

TS:   String(42)
来源：http://ubi.yongpay.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://tpm.sysykeji.top

Go:   strconv.Itoa(42)
来源：http://hos.yuxming.cn

Ruby: 42.to_s
来源：http://ooq.52xcode.cn

C#:   42.ToString()
来源：http://xqf.quarkkingdee.top

[A08] 取整与四舍五入
来源：http://ggp.yanxiufei.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qbe.dashuyun.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://noc.feifeiyinyue.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rcf.zycfv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qcl.0kj1m.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gtt.gotoacloud.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dri.meibo888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://dth.hfpthk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ibf.vehdjk.com

[A09] 绝对值与最大最小值
来源：http://kzy.redwolf501.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ezp.quarkkingdee.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uwn.feifeiyinyue.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gfq.ppjwa.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gqv.quarkkingdee.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kdt.uphjek.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xzb.52xcode.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qwr.daxiang520.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oxe.shanyushiyangkeji.top

[A10] 生成随机数
来源：http://mef.ywan-chungtsiang.top

Py:   import random; random.randint(1, 100)
来源：http://pcg.cashguo.top

PHP:  random_int(1, 100);
来源：http://igi.iojbl.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qdx.sufxvd.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ltm.hesvh.cn

Java: new Random().nextInt(100) + 1
来源：http://kae.yuxming.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fth.aizwys.cn

Ruby: rand(1..100)
来源：http://des.sweek.top

C#:   new Random().Next(1, 101)
来源：http://gbw.jinyuanbaomall.cn

[A11] 条件表达式（三元）
来源：http://ptv.xinyue.icu

Py:   "yes" if x > 0 else "no"
来源：http://fcw.gzhubu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ajn.sweek.top

JS:   x > 0 ? "yes" : "no"
来源：http://oig.tarul.cn

TS:   x > 0 ? "yes" : "no"
来源：http://opi.shangyingyoupin.top

Java: x > 0 ? "yes" : "no"
来源：http://jrd.zhaomingkeji.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://wnk.mhx1999.top

Ruby: x > 0 ? "yes" : "no"
来源：http://wfn.jlsjyb.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hye.chenzaomai.com

[A12] 字符串插值 / 格式化
来源：http://bmp.daria6918.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://oet.yonumen.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tvh.jyoumei.cn

JS:   `Hello, ${name}!`
来源：http://nkv.fengsongda.top

TS:   `Hello, ${name}!`
来源：http://ffv.jqgufenzy.top

Java: "Hello, %s!".formatted(name)
来源：http://fzk.ehwqpu.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lfa.0kj1m.cn

Ruby: "Hello, #{name}!"
来源：http://sna.sweek.top

C#:   $"Hello, {name}!"
来源：http://goh.bjfxy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://mge.wangdashe.top

Py:   "第一行\n第二行"
来源：http://ard.yanxiufei.cn

PHP:  "第一行\n第二行"
来源：http://ejn.xinyue.icu

JS:   "第一行\n第二行"
来源：http://qpu.cqqwz.cn

TS:   "第一行\n第二行"
来源：http://cgc.chenlongwang.top

Java: "第一行\n第二行"
来源：http://onu.hesvh.cn

Go:   "第一行\n第二行"
来源：http://fhu.fengsongda.top

Ruby: "第一行\n第二行"
来源：http://gso.9152youxi.cn

C#:   "第一行\n第二行"
来源：http://lri.andypj.xyz

[A14] 注释写法
来源：http://bqo.ydjk.org.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hnv.yuanzhike.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://exo.hnqzz.top

JS:   // 单行；/* 多行 */
来源：http://bfd.shanyushiyangtech.top

TS:   // 单行；/* 多行 */
来源：http://guv.jinyuanbaomall.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hmi.hammf.cn

Go:   // 单行；/* 多行 */
来源：http://pli.ydzc1.top

Ruby: # 单行；=begin 多行 =end
来源：http://hje.dashuyun.cn

C#:   // 单行；/* 多行 */
来源：http://jze.smart0.xyz

[A15] 空值判断与默认值
来源：http://rmm.hfpthk.cn

Py:   value = data or "默认值"
来源：http://ssm.9152youxi.cn

PHP:  $value = $data ?? "默认值";
来源：http://tap.hnqzz.top

JS:   const value = data ?? "默认值";
来源：http://bvk.meibo888.top

TS:   const value = data ?? "默认值";
来源：http://axj.jinqigufen.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jko.shanyushiyangtech.top

Go:   if data == "" { data = "默认值" }
来源：http://qrn.hongshengwenyu.top

Ruby: value = data || "默认值"
来源：http://alr.ppjwa.cn

C#:   var value = data ?? "默认值";
来源：http://upe.epnwcf.com

[A16] 真假值判断规则
来源：http://stc.sjlbkw.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ukz.zhixingplan.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eui.c1oappe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gak.cqqwz.cn

TS:   if (!x) {}
来源：http://lyu.bjfxy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yaj.xingfuxueyuan.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xkn.jinqigfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://gfc.jyoumei.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uby.hywenlv.cn

[A17] 位运算
来源：http://rhu.hongshengwenyu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qfl.ydjk.org.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://thd.uphjek.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://prg.cdnleiting.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fus.pycfn.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wja.jqgufenzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mpx.tanke756.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tvf.cdnleiting.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://goa.daria6918.cn

[A18] 字符与 ASCII 码互转
来源：http://kqs.shangyingyoupin.top

Py:   ord("A"); chr(65)
来源：http://jlw.jinqigfzy.top

PHP:  ord("A"); chr(65)
来源：http://rqv.jinyuanbaomall.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rvk.snrcjt.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zaq.gogol.net.cn

Java: (int) 'A'; (char) 65
来源：http://rvy.guannengcc.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://eer.hfpthk.cn

Ruby: "A".ord; 65.chr
来源：http://nhp.daxiang520.top

C#:   (int)'A'; (char)65
来源：http://uwm.yj20258.top

[A19] 交换两个变量
来源：http://ysb.birdmap.top

Py:   a, b = b, a
来源：http://cpt.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://iwa.zhengqikj.top

JS:   [a, b] = [b, a];
来源：http://aqc.fzhhl.top

TS:   [a, b] = [b, a];
来源：http://cnl.hywenlv.cn

Java: int t = a; a = b; b = t;
来源：http://ski.dianchejie.cn

Go:   a, b = b, a
来源：http://jcw.kuanghao11.cn

Ruby: a, b = b, a
来源：http://fsu.andypj.xyz

C#:   (a, b) = (b, a);
来源：http://myd.gotoacloud.top

[A20] 读取标准输入
来源：http://zmi.aibaodan.cn

Py:   name = input("请输入：")
来源：http://jnu.xylfe.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rls.wangshuangyany.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vkl.0kj1m.cn

TS:   // Node.js：readline 模块
来源：http://juv.dianchejie.cn

Java: new Scanner(System.in).nextLine()
来源：http://anv.yj20258.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jew.cqqwz.cn

Ruby: gets.chomp
来源：http://zox.c1oappe.top

C#:   Console.ReadLine();
来源：http://fir.xuanzx.com

[A21] 保留指定小数位输出
来源：http://rts.wangshuangyany.cn

Py:   f"{3.14159:.2f}"
来源：http://nye.smart0.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jyi.vehdjk.com

JS:   (3.14159).toFixed(2)
来源：http://sdu.bbcook.cn

TS:   (3.14159).toFixed(2)
来源：http://mtt.zdbjq.cn

Java: String.format("%.2f", 3.14159)
来源：http://hyy.wangdashe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hkn.nwbrower.top

Ruby: format("%.2f", 3.14159)
来源：http://tfh.gogol.net.cn

C#:   3.14159.ToString("F2")
来源：http://atm.vqdsnc.cn

[A22] 获取字符串长度
来源：http://nhl.ybcxt.top

Py:   len(s)
来源：http://zec.zdbjq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yge.mhx1999.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://iei.xziqi.cn

TS:   s.length
来源：http://ejr.ivvv.top

Java: s.length()
来源：http://ngl.chenjidiqi.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dnz.xziqi.cn

Ruby: s.length
来源：http://fru.jyoumei.cn

C#:   s.Length
来源：http://poy.nanxuanxn.top

[A23] 大小写转换
来源：http://rdm.yueranfly.top

Py:   s.upper(); s.lower(); s.title()
来源：http://oad.hesvh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://myj.zhoulong.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xno.yj20258.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kpg.fengsongda.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ioc.fanxiaobao.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ucx.nwbrower.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ynb.hnxiangtu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gri.chenjidiqi.icu

[A24] 去除首尾空白
来源：http://cob.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dba.zhiwuduotai.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pla.shangyingyoupin.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kxl.ywan-chungtsiang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vep.zhengqikj.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ghx.hesvh.cn

Go:   strings.TrimSpace(s)
来源：http://cag.hongshengwenyu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aub.c1oappe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mtw.ydjk.org.cn

[A25] 字符串比较
来源：http://lko.hfpthk.cn

Py:   s1 == s2; s1 != s2
来源：http://rev.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dnr.ydzc1.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ffw.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dbo.jinqigfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bcu.ppjwa.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hzz.hnqzz.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ddh.c1oappe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dzp.yvedp.cn

[A26] 类型转换总览
来源：http://ddo.yanxiufei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hbs.guowangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iof.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://khi.nanxuanxn.top

TS:   Number() String() Boolean() x as number
来源：http://kyz.dashuyun.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fdp.ywan-chungtsiang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://koz.birdmap.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ikt.yanxiufei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tgp.snrcjt.cn

================================================================================
来源：http://asr.xingfuxueyuan.xyz

B. 流程控制
来源：http://arv.yvedp.cn

================================================================================
来源：http://zot.xziqi.cn

[B01] 条件判断 if / else
来源：http://sel.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://nyk.svipenyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mct.cheryme.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yrh.fengsongda.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ums.quarkkingdee.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yxx.yj20258888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hmg.sxryk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gxr.sxryk.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sno.zycfv.cn

[B02] 多分支 else if / elif
来源：http://rdr.yueranfly.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zav.meibo888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wgi.wangdashe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ecr.zhijiandao.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kaq.shzxlz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xhs.shanyushiyangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mdu.daxiang520.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oyp.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wgm.jinqigufen.top

[B03] switch / match / case
来源：http://lea.gogol.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ylx.guannengcc.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cfk.iojbl.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://res.hongshengwenyu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vax.jyoumei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rwf.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://erf.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mji.cdnleiting.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wqy.bbcook.cn

[B04] for 计数循环
来源：http://nay.aizwys.cn

Py:   for i in range(10): print(i)
来源：http://dje.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hbp.jinyuanbaomall.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iud.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vpv.ppjwa.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jls.gotoacloud.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hug.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://lne.hfpthk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kva.cdnleiting.top

[B05] 遍历数组 / 列表
来源：http://rzx.aibaodan.cn

Py:   for item in arr: print(item)
来源：http://ojx.tanke756.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vdl.yongpay.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fzg.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jjl.fanxiaobao.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://ceh.bbcook.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lgl.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://qtw.zdbjq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bgx.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://trw.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://slb.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://npy.daria6918.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zlx.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ctv.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wll.yfazqb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jiw.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fsg.bjfxy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ats.wangdashe.top

[B07] while 循环
来源：http://rsh.yuxming.cn

Py:   while i < 10: i += 1
来源：http://wxw.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ssd.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://qfb.jlsjyb.cn

TS:   while (i < 10) { i++; }
来源：http://dwd.zhoulong.xyz

Java: while (i < 10) { i++; }
来源：http://erh.fzhhl.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ykg.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://kjx.pengpengdd.cyou

C#:   while (i < 10) { i++; }
来源：http://tak.zhaomingkeji.xyz

[B08] do-while（至少执行一次）
来源：http://zow.cashguo.top

Py:   # 无 do-while：用 while True + break
来源：http://tni.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://ymr.snrcjt.cn

JS:   do { i++; } while (i < 10);
来源：http://vnm.kuanghao11.cn

TS:   do { i++; } while (i < 10);
来源：http://run.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://daa.cqqwz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nsl.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://nzo.birdmap.top

C#:   do { i++; } while (i < 10);
来源：http://imz.mhx1999.top

[B09] break 与 continue
来源：http://zyd.hnxiangtu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ram.gotoacloud.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wsd.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ige.sysykeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://raz.ivvv.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lsj.ywan-chungtsiang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wdd.shanyushiyangtech.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kus.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zst.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://huz.hfpthk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://twk.yj202588.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cqu.daria6918.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lll.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hhy.hesvh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gve.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vds.ehwqpu.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sna.yongpay.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vaq.jinyuanbaomall.cn

[B11] 生成数字序列 / 区间
来源：http://zvv.shanyushiyangkeji.top

Py:   list(range(0, 10, 2))
来源：http://zrd.uphjek.com

PHP:  range(0, 10, 2);
来源：http://wye.52xcode.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dnt.aibaodan.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hdl.tian-w.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gvw.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cdv.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://uoy.jinghuilouyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gvj.yfazqb.com

[B12] 跳出多层循环
来源：http://duw.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xrz.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lqu.kuanghao11.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://npu.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qui.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://frt.tarul.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zef.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://llz.gogol.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ulo.tianlin.xyz


<!-- 参考信息 -->