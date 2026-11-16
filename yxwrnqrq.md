代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://csi.shanyushiyangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://moi.tarul.cn

C#:   x.GetType().Name; x is int
来源：http://hee.fzhhl.top

[A05] 整数除法与取模
来源：http://oqx.gogol.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vdu.iojbl.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bix.uphjek.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nvp.ehwqpu.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yks.jqgufenzy.top

Java: 7 / 2; 7 % 2
来源：http://zja.ydjk.org.cn

Go:   7 / 2; 7 % 2
来源：http://ehb.hnqzz.top

Ruby: 7 / 2; 7 % 2
来源：http://mit.zhijiandao.cn

C#:   7 / 2; 7 % 2
来源：http://ocn.yvedp.cn

[A06] 字符串转数字
来源：http://obk.wangshuangyany.cn

Py:   int("42"); float("3.14")
来源：http://flg.ctjpmb.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tyf.andypj.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bkd.zycfv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xss.zhijiandao.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lqz.shanyushiyangtech.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://roh.shanyushiyangkeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://wnh.vqdsnc.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://npc.cheryme.top

[A07] 数字转字符串
来源：http://jcm.zhongyouzk.top

Py:   str(42)
来源：http://zrq.daxiang520.top

PHP:  (string) 42; strval(42)
来源：http://bbp.ydzc1.top

JS:   String(42); (42).toString()
来源：http://osu.jianghu66.top

TS:   String(42)
来源：http://zec.jyoumei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ism.meibo888.top

Go:   strconv.Itoa(42)
来源：http://qxh.xuetiantiany.cn

Ruby: 42.to_s
来源：http://fmp.hywenlv.cn

C#:   42.ToString()
来源：http://dsp.gaohongyu789.top

[A08] 取整与四舍五入
来源：http://zpw.xinyue.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kab.hnqzz.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xgb.aizwys.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://aib.bbcook.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uin.hammf.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bmu.sweek.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fks.jqgufenzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://gjg.sjlbkw.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yec.andypj.xyz

[A09] 绝对值与最大最小值
来源：http://fvl.c1oappe.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zaw.vehdjk.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hhu.jinqigfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bcw.sysykeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fmu.dianchejie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hrm.wangshuangyany.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zpu.fehbvm.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jri.vehdjk.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hsp.redwolf501.top

[A10] 生成随机数
来源：http://sjg.ydzc1.top

Py:   import random; random.randint(1, 100)
来源：http://qrb.gotoacloud.top

PHP:  random_int(1, 100);
来源：http://shb.sweek.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lwb.dianchejie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zxf.wangshuangyany.cn

Java: new Random().nextInt(100) + 1
来源：http://czk.yj20258888.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vga.jlsjyb.cn

Ruby: rand(1..100)
来源：http://buq.zhaomingkeji.xyz

C#:   new Random().Next(1, 101)
来源：http://fee.shuidangran.top

[A11] 条件表达式（三元）
来源：http://hgw.jyoumei.cn

Py:   "yes" if x > 0 else "no"
来源：http://mwz.jinqigufen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://vqy.smart0.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://duu.guowangkeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://kef.zhixingplan.top

Java: x > 0 ? "yes" : "no"
来源：http://ozi.jinyuanbaomall.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wxj.vehdjk.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ddo.xylfe.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jqq.hesvh.cn

[A12] 字符串插值 / 格式化
来源：http://gcs.jinyuanbaomall.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nna.daxiang520.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://obs.zhaomingkeji.xyz

JS:   `Hello, ${name}!`
来源：http://clp.ydzc1.top

TS:   `Hello, ${name}!`
来源：http://twy.haohaochexian.top

Java: "Hello, %s!".formatted(name)
来源：http://udw.jinqigufen.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ley.wangdashe.top

Ruby: "Hello, #{name}!"
来源：http://poi.0kj1m.cn

C#:   $"Hello, {name}!"
来源：http://uzo.nanxuanxn.top

[A13] 多行字符串（练习 \n 转义）
来源：http://axk.chenjidiqi.icu

Py:   "第一行\n第二行"
来源：http://mem.yanxiufei.cn

PHP:  "第一行\n第二行"
来源：http://dvi.316326.xyz

JS:   "第一行\n第二行"
来源：http://rst.fktsv.cn

TS:   "第一行\n第二行"
来源：http://uvs.tanke756.top

Java: "第一行\n第二行"
来源：http://qkz.gzhubu.top

Go:   "第一行\n第二行"
来源：http://tag.nanxinkj.top

Ruby: "第一行\n第二行"
来源：http://rzn.zhijiandao.cn

C#:   "第一行\n第二行"
来源：http://fke.pycfn.com

[A14] 注释写法
来源：http://vwp.sxryk.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vug.daria6918.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://waw.guannengcc.top

JS:   // 单行；/* 多行 */
来源：http://lfp.shanyushiyangtech.top

TS:   // 单行；/* 多行 */
来源：http://gtn.jqgufenzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hyt.aizwys.cn

Go:   // 单行；/* 多行 */
来源：http://qzt.vehdjk.com

Ruby: # 单行；=begin 多行 =end
来源：http://jjh.feifeiyinyue.top

C#:   // 单行；/* 多行 */
来源：http://rsp.svipenyu.cn

[A15] 空值判断与默认值
来源：http://dad.snrcjt.cn

Py:   value = data or "默认值"
来源：http://zop.sweek.top

PHP:  $value = $data ?? "默认值";
来源：http://wke.bbcook.cn

JS:   const value = data ?? "默认值";
来源：http://mdy.sysykeji.top

TS:   const value = data ?? "默认值";
来源：http://sjd.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mzk.chenzaomai.com

Go:   if data == "" { data = "默认值" }
来源：http://rkm.xinyue.icu

Ruby: value = data || "默认值"
来源：http://lfr.yj202588.top

C#:   var value = data ?? "默认值";
来源：http://rgj.andypj.xyz

[A16] 真假值判断规则
来源：http://dxk.tarul.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xwz.xylfe.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hnp.kuanghao11.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pkk.cucudq.cn

TS:   if (!x) {}
来源：http://lvp.smart0.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fdi.hfpthk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dty.zhoulong.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://yau.pycfn.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gej.fzhhl.top

[A17] 位运算
来源：http://kxb.zhijiandao.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://enk.redwolf501.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yzl.yonumen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ezb.zycfv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://atr.hesvh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vvr.cdnleiting.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qnr.feifeiyinyue.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fad.xziqi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://clx.wangdashe.top

[A18] 字符与 ASCII 码互转
来源：http://wyb.sjlbkw.cn

Py:   ord("A"); chr(65)
来源：http://ljc.shzxlz.cn

PHP:  ord("A"); chr(65)
来源：http://nmt.jiagoushi.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pya.epnwcf.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ngr.hammf.cn

Java: (int) 'A'; (char) 65
来源：http://ubj.xuanzx.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ngs.daria6918.cn

Ruby: "A".ord; 65.chr
来源：http://sai.aibaodan.cn

C#:   (int)'A'; (char)65
来源：http://vmj.shanyushiyangtech.top

[A19] 交换两个变量
来源：http://ltk.shanyushiyangtech.top

Py:   a, b = b, a
来源：http://rny.epnwcf.com

PHP:  [$a, $b] = [$b, $a];
来源：http://hyb.iojbl.cn

JS:   [a, b] = [b, a];
来源：http://aqo.jinqigfzy.top

TS:   [a, b] = [b, a];
来源：http://bgm.jlsjyb.cn

Java: int t = a; a = b; b = t;
来源：http://xuf.meibo888.top

Go:   a, b = b, a
来源：http://lpe.hnqzz.top

Ruby: a, b = b, a
来源：http://kjl.smart0.xyz

C#:   (a, b) = (b, a);
来源：http://jdq.ppjwa.cn

[A20] 读取标准输入
来源：http://nvq.aizwys.cn

Py:   name = input("请输入：")
来源：http://ybc.vqdsnc.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mhb.yuxming.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://etz.zhaomingkeji.xyz

TS:   // Node.js：readline 模块
来源：http://ami.gaohongyu789.top

Java: new Scanner(System.in).nextLine()
来源：http://dio.cheryme.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wge.meibo888.top

Ruby: gets.chomp
来源：http://rkw.vehdjk.com

C#:   Console.ReadLine();
来源：http://txv.gzhubu.top

[A21] 保留指定小数位输出
来源：http://okh.uphjek.com

Py:   f"{3.14159:.2f}"
来源：http://aeo.tianlin.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://elf.cashguo.top

JS:   (3.14159).toFixed(2)
来源：http://jey.snrcjt.cn

TS:   (3.14159).toFixed(2)
来源：http://ukh.hnqzz.top

Java: String.format("%.2f", 3.14159)
来源：http://oow.hysaishi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ufb.tianlin.xyz

Ruby: format("%.2f", 3.14159)
来源：http://pmg.hysaishi.cn

C#:   3.14159.ToString("F2")
来源：http://srm.ivvv.top

[A22] 获取字符串长度
来源：http://ejf.xylfe.cn

Py:   len(s)
来源：http://ctx.bjfxy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ngh.fengsongda.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ebr.cucudq.cn

TS:   s.length
来源：http://qpj.shzxlz.cn

Java: s.length()
来源：http://wms.chenjidiqi.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yif.shzxlz.cn

Ruby: s.length
来源：http://fsa.jianghu66.top

C#:   s.Length
来源：http://pcz.yfazqb.com

[A23] 大小写转换
来源：http://weo.jinqigufen.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nqi.c1oappe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xvu.yueranfly.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wui.guannengcc.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nbh.hesvh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://crx.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mra.vqdsnc.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://riw.xinyue.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://bng.daria6918.cn

[A24] 去除首尾空白
来源：http://vpx.daxiang520.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://abd.fehbvm.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://utw.yuanzhike.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kmw.cqqwz.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pbn.pycfn.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://orq.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://mun.zhongyouzk.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uya.zhijiandao.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pqn.chenzaomai.com

[A25] 字符串比较
来源：http://kpf.fanxiaobao.xyz

Py:   s1 == s2; s1 != s2
来源：http://rph.ydjk.org.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oqq.gaohongyu789.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zzt.xziqi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://myb.zycfv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ccr.zhengqikj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pob.gotoacloud.top

Ruby: s1 == s2; s1 <=> s2
来源：http://loi.ywan-chungtsiang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wza.ydjk.org.cn

[A26] 类型转换总览
来源：http://faa.gzhubu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yie.yanxiufei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sus.gogol.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://suo.zhixingplan.top

TS:   Number() String() Boolean() x as number
来源：http://eoy.xylfe.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://utn.feifeiyinyue.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zff.wangshuangyany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://exu.hesvh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lum.gogol.net.cn

================================================================================
来源：http://qtl.mhx1999.top

B. 流程控制
来源：http://xkn.ybcxt.top

================================================================================
来源：http://wzi.smart0.xyz

[B01] 条件判断 if / else
来源：http://bqs.shanyushiyangtech.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ztt.gogol.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lny.meibo888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ekm.jyoumei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jkr.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://stv.zhijiandao.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xwy.fktsv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ikr.fzhhl.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zjc.ctjpmb.com

[B02] 多分支 else if / elif
来源：http://jei.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vhu.fengsongda.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vwg.gogol.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bvv.316326.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dkz.shzxlz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zyl.tarul.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dvb.fengsongda.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://scn.hnxiangtu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fny.quarkkingdee.top

[B03] switch / match / case
来源：http://eut.ppjwa.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uqc.mhx1999.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://luh.yj20258888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mct.fzhhl.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cnu.xylfe.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tjy.shanyushiyangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hxp.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xtn.shuidangran.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xkv.zhiwuduotai.top

[B04] for 计数循环
来源：http://gmm.ivvv.top

Py:   for i in range(10): print(i)
来源：http://mce.gotoacloud.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mfi.zdqjudy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://esb.cucudq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ulx.guowangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://psx.mhx1999.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jme.fktsv.cn

Ruby: 10.times { |i| puts i }
来源：http://npg.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hms.hysaishi.cn

[B05] 遍历数组 / 列表
来源：http://vdp.ywan-chungtsiang.top

Py:   for item in arr: print(item)
来源：http://xzw.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mqj.ydjk.org.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hcp.hammf.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mfb.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://chw.haohaochexian.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wwz.yuanzhike.top

Ruby: arr.each { |item| puts item }
来源：http://dig.jinghuilouyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xbc.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://gzt.cucudq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://apa.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pnd.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eiy.chenlongwang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lbr.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://urr.yvedp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rpc.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lwu.tanke756.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://umz.jinqigfzy.top

[B07] while 循环
来源：http://dbt.316326.xyz

Py:   while i < 10: i += 1
来源：http://elb.zhengqikj.top

PHP:  while ($i < 10) { $i++; }
来源：http://szs.daria6918.cn

JS:   while (i < 10) { i++; }
来源：http://ylt.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://nwr.fzhhl.top

Java: while (i < 10) { i++; }
来源：http://rfo.shzxlz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aav.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://svz.ydzc1.top

C#:   while (i < 10) { i++; }
来源：http://hhb.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://rcr.ehwqpu.com

Py:   # 无 do-while：用 while True + break
来源：http://cvd.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://krh.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://iec.yuxming.cn

TS:   do { i++; } while (i < 10);
来源：http://wbm.52xcode.cn

Java: do { i++; } while (i < 10);
来源：http://jvv.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xeq.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fjj.haohaochexian.top

C#:   do { i++; } while (i < 10);
来源：http://dlg.yuxming.cn

[B09] break 与 continue
来源：http://fvi.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wab.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zdp.cheryme.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cgd.sxryk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hvt.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qvs.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eth.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aaz.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://npn.shangyingyoupin.top

[B10] 遍历同时拿索引
来源：http://bvl.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bui.yuanzhike.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://afm.guowangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ono.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pga.jinyuanbaomall.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hwv.daxiang520.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://thg.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wew.jianghu66.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wcy.shanyushiyangkeji.top

[B11] 生成数字序列 / 区间
来源：http://znl.nanxinkj.top

Py:   list(range(0, 10, 2))
来源：http://tbu.bjfxy.top

PHP:  range(0, 10, 2);
来源：http://kul.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jas.bbcook.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zry.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ipb.yonumen.top


<!-- 参考信息 -->