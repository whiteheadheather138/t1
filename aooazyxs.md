代发 wailian999

[A06] 字符串转数字
来源：http://gzm.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://cbm.0kj1m.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jck.zhongyouzk.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ypv.hammf.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dvx.fanxiaobao.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lqt.jqgfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://unj.pycfn.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ulh.gogol.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ehs.hcnkem.com

[A07] 数字转字符串
来源：http://bto.jlsjyb.cn

Py:   str(42)
来源：http://evz.jlsjyb.cn

PHP:  (string) 42; strval(42)
来源：http://zal.pengpengdd.cyou

JS:   String(42); (42).toString()
来源：http://ewp.hammf.cn

TS:   String(42)
来源：http://pcz.hysaishi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://byb.xingfuxueyuan.xyz

Go:   strconv.Itoa(42)
来源：http://xgr.gzhubu.top

Ruby: 42.to_s
来源：http://ftp.epnwcf.com

C#:   42.ToString()
来源：http://oed.jinqigufen.top

[A08] 取整与四舍五入
来源：http://cud.c1oappe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dfp.52xcode.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cye.hnxiangtu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sky.ctjpmb.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dpt.andypj.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sxs.tarul.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dvk.cucudq.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://joo.pengpengdd.cyou

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rwz.ppjwa.cn

[A09] 绝对值与最大最小值
来源：http://phf.zhiwuduotai.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nmd.zdqjudy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uhl.zhoulong.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nsa.xziqi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qhg.shanyushiyangtech.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ssb.yj20258.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lri.dianchejie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pzn.feifeiyinyue.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://syw.zhiwuduotai.top

[A10] 生成随机数
来源：http://yue.shanyushiyangkeji.top

Py:   import random; random.randint(1, 100)
来源：http://jsk.shangyingyoupin.top

PHP:  random_int(1, 100);
来源：http://xvx.chenjidiqi.icu

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ptx.tianlin.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rgm.yongpay.top

Java: new Random().nextInt(100) + 1
来源：http://rnn.zhijiandao.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lwo.jinqigfzy.top

Ruby: rand(1..100)
来源：http://dom.pycfn.com

C#:   new Random().Next(1, 101)
来源：http://hgo.ehwqpu.com

[A11] 条件表达式（三元）
来源：http://dks.gzhubu.top

Py:   "yes" if x > 0 else "no"
来源：http://lln.tian-w.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ovv.chenjidiqi.icu

JS:   x > 0 ? "yes" : "no"
来源：http://qol.shuidangran.top

TS:   x > 0 ? "yes" : "no"
来源：http://ijk.hnqzz.top

Java: x > 0 ? "yes" : "no"
来源：http://jjo.xylfe.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://krn.vehdjk.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ase.sjlbkw.cn

C#:   x > 0 ? "yes" : "no"
来源：http://elb.iojbl.cn

[A12] 字符串插值 / 格式化
来源：http://vjv.xinyue.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tyz.daria6918.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://afd.kuanghao11.cn

JS:   `Hello, ${name}!`
来源：http://unx.tarul.cn

TS:   `Hello, ${name}!`
来源：http://upa.xuanzx.com

Java: "Hello, %s!".formatted(name)
来源：http://nxs.gzhubu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bnt.wangshuangyany.cn

Ruby: "Hello, #{name}!"
来源：http://wij.jqgfzy.top

C#:   $"Hello, {name}!"
来源：http://ooc.ybcxt.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ptc.fzhhl.top

Py:   "第一行\n第二行"
来源：http://txu.chenjidiqi.icu

PHP:  "第一行\n第二行"
来源：http://oeb.fktsv.cn

JS:   "第一行\n第二行"
来源：http://lkc.jinghuilouyu.cn

TS:   "第一行\n第二行"
来源：http://bcj.316326.xyz

Java: "第一行\n第二行"
来源：http://ofr.shuidangran.top

Go:   "第一行\n第二行"
来源：http://zwp.redwolf501.top

Ruby: "第一行\n第二行"
来源：http://qer.gogol.net.cn

C#:   "第一行\n第二行"
来源：http://jvx.chenlongwang.top

[A14] 注释写法
来源：http://fvk.yueranfly.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://nnu.xziqi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bpy.daxiang520.top

JS:   // 单行；/* 多行 */
来源：http://mka.pycfn.com

TS:   // 单行；/* 多行 */
来源：http://hks.ehwqpu.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://esc.andypj.xyz

Go:   // 单行；/* 多行 */
来源：http://uho.vqdsnc.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ldl.cashguo.top

C#:   // 单行；/* 多行 */
来源：http://ukb.daria6918.cn

[A15] 空值判断与默认值
来源：http://cor.yonumen.top

Py:   value = data or "默认值"
来源：http://ctd.fengsongda.top

PHP:  $value = $data ?? "默认值";
来源：http://hfc.jiagoushi.top

JS:   const value = data ?? "默认值";
来源：http://eaj.yuanzhike.top

TS:   const value = data ?? "默认值";
来源：http://jxu.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dan.ivvv.top

Go:   if data == "" { data = "默认值" }
来源：http://dvi.haohaochexian.top

Ruby: value = data || "默认值"
来源：http://pmi.yanxiufei.cn

C#:   var value = data ?? "默认值";
来源：http://bam.fzhhl.top

[A16] 真假值判断规则
来源：http://hyw.nanxuanxn.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://shi.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nhd.cashguo.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://axq.jlsjyb.cn

TS:   if (!x) {}
来源：http://fcr.cdnleiting.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://iso.zdbjq.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pjg.cheryme.top

Ruby: unless x            # nil 与 false 为假
来源：http://wwp.ydzc1.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://voh.zhiwuduotai.top

[A17] 位运算
来源：http://syl.uphjek.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xut.hcnkem.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qvj.fehbvm.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oyk.iojbl.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qns.yangfankeji.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eer.ivvv.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://okf.havefunace.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gla.smart0.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uxw.vqdsnc.cn

[A18] 字符与 ASCII 码互转
来源：http://lcu.vqdsnc.cn

Py:   ord("A"); chr(65)
来源：http://mwo.jinyuanbaomall.cn

PHP:  ord("A"); chr(65)
来源：http://ybe.cdnleiting.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rec.sjlbkw.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lhx.shanyushiyangtech.top

Java: (int) 'A'; (char) 65
来源：http://hsc.316326.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wyj.birdmap.top

Ruby: "A".ord; 65.chr
来源：http://qyk.gotoacloud.top

C#:   (int)'A'; (char)65
来源：http://esm.yanxiufei.cn

[A19] 交换两个变量
来源：http://uiz.hywenlv.cn

Py:   a, b = b, a
来源：http://jxi.ctjpmb.com

PHP:  [$a, $b] = [$b, $a];
来源：http://ker.pengpengdd.cyou

JS:   [a, b] = [b, a];
来源：http://etf.316326.xyz

TS:   [a, b] = [b, a];
来源：http://oma.hcnkem.com

Java: int t = a; a = b; b = t;
来源：http://jqn.shanyushiyangtech.top

Go:   a, b = b, a
来源：http://hri.jinqigfzy.top

Ruby: a, b = b, a
来源：http://bby.hywenlv.cn

C#:   (a, b) = (b, a);
来源：http://sqb.andypj.xyz

[A20] 读取标准输入
来源：http://ehz.smart0.xyz

Py:   name = input("请输入：")
来源：http://yjv.jiagoushi.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vwp.dashuyun.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xph.zdbjq.cn

TS:   // Node.js：readline 模块
来源：http://flp.daxiang520.top

Java: new Scanner(System.in).nextLine()
来源：http://idb.zhoulong.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lqo.yvedp.cn

Ruby: gets.chomp
来源：http://xsx.iojbl.cn

C#:   Console.ReadLine();
来源：http://hjd.hammf.cn

[A21] 保留指定小数位输出
来源：http://yuw.ydzc1.top

Py:   f"{3.14159:.2f}"
来源：http://okc.zhongyouzk.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://exp.hesvh.cn

JS:   (3.14159).toFixed(2)
来源：http://lyn.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://xvr.ybcxt.top

Java: String.format("%.2f", 3.14159)
来源：http://wub.mhx1999.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vwj.wangshuangyany.cn

Ruby: format("%.2f", 3.14159)
来源：http://nya.tanke756.top

C#:   3.14159.ToString("F2")
来源：http://kmc.zdqjudy.top

[A22] 获取字符串长度
来源：http://kyo.hnqzz.top

Py:   len(s)
来源：http://adm.yj20258.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dss.birdmap.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tff.guowangkeji.top

TS:   s.length
来源：http://wxi.pengpengdd.cyou

Java: s.length()
来源：http://ryl.yvedp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://awi.shzxlz.cn

Ruby: s.length
来源：http://dbk.zhijiandao.cn

C#:   s.Length
来源：http://ami.wangdashe.top

[A23] 大小写转换
来源：http://pro.tanke756.top

Py:   s.upper(); s.lower(); s.title()
来源：http://yox.ybcxt.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fgg.epnwcf.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ewu.hywenlv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uyd.feifeiyinyue.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gwa.feifeiyinyue.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://scx.andypj.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lwn.xylfe.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://osd.feifeiyinyue.top

[A24] 去除首尾空白
来源：http://nzy.yonumen.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://auk.zhaomingkeji.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rgt.sjlbkw.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ioj.fktsv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dfj.fehbvm.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jfd.kuanghao11.cn

Go:   strings.TrimSpace(s)
来源：http://rrh.daria6918.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pit.hnqzz.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://txd.jyoumei.cn

[A25] 字符串比较
来源：http://mpw.xuetiantiany.cn

Py:   s1 == s2; s1 != s2
来源：http://hrl.zhijiandao.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ppt.chenzaomai.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bwk.fehbvm.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hrq.jlsjyb.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tch.52xcode.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yoc.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://erh.xingfuxueyuan.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rru.guannengcc.top

[A26] 类型转换总览
来源：http://iqj.ydjk.org.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://prg.haohaochexian.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lsz.316326.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nqu.ydzc1.top

TS:   Number() String() Boolean() x as number
来源：http://qcx.zhoulong.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pdr.jlsjyb.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uxe.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pac.zdqjudy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tax.cqqwz.cn

================================================================================
来源：http://abp.9152youxi.cn

B. 流程控制
来源：http://xco.fanxiaobao.xyz

================================================================================
来源：http://ors.chenlongwang.top

[B01] 条件判断 if / else
来源：http://jcr.9152youxi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uin.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mbx.feifeiyinyue.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://smh.tarul.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sez.hnxiangtu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ouv.shuidangran.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jkd.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lml.iojbl.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rqh.xingfuxueyuan.xyz

[B02] 多分支 else if / elif
来源：http://nvf.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wfr.yonumen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cer.chenjidiqi.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sls.gogol.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tmk.ivvv.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ygy.yuanzhike.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tas.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mmc.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ept.fktsv.cn

[B03] switch / match / case
来源：http://rpx.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mxh.yuxming.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://isu.chenlongwang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lkj.dashuyun.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gjf.zdbjq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://swh.ppjwa.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kzm.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fys.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qka.yfazqb.com

[B04] for 计数循环
来源：http://ohu.ybcxt.top

Py:   for i in range(10): print(i)
来源：http://bah.jinqigufen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ugo.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oze.zycfv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uih.guowangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cfc.feifeiyinyue.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dbm.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://fki.bbcook.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://syo.shangyingyoupin.top

[B05] 遍历数组 / 列表
来源：http://tna.dashuyun.cn

Py:   for item in arr: print(item)
来源：http://aew.haohaochexian.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zrs.hesvh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://njj.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gcv.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vpc.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pls.shanyushiyangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://bnw.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vks.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://nlb.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nbu.nanxinkj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bpq.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vdf.tanke756.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ifs.yueranfly.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tdv.hongshengwenyu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zax.0kj1m.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vpr.zhongyouzk.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hre.zhongyouzk.top

[B07] while 循环
来源：http://yav.gotoacloud.top

Py:   while i < 10: i += 1
来源：http://jzs.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://vzd.ydzc1.top

JS:   while (i < 10) { i++; }
来源：http://kpk.daxiang520.top

TS:   while (i < 10) { i++; }
来源：http://plw.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://avo.ppjwa.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kpn.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://egm.yangfankeji.com

C#:   while (i < 10) { i++; }
来源：http://yui.chenzaomai.com

[B08] do-while（至少执行一次）
来源：http://vla.tanke756.top

Py:   # 无 do-while：用 while True + break
来源：http://fvw.pycfn.com

PHP:  do { $i++; } while ($i < 10);
来源：http://nkf.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://vrn.jlsjyb.cn

TS:   do { i++; } while (i < 10);
来源：http://ojb.feifeiyinyue.top

Java: do { i++; } while (i < 10);
来源：http://cvg.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://glk.chenjidiqi.icu

Ruby: begin; i += 1; end while i < 10
来源：http://klg.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://cer.nanxinkj.top

[B09] break 与 continue
来源：http://kej.xinyue.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jye.cqqwz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xcp.cdnleiting.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ezw.gotoacloud.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tnn.jianghu66.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oex.nanxinkj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zdh.smart0.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://imb.yfazqb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cco.0kj1m.cn

[B10] 遍历同时拿索引
来源：http://cxi.jianghu66.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yuq.jqgfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://auc.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ftk.9152youxi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gdv.zhengqikj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fbf.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mwc.zdbjq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ryl.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xzj.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://qey.havefunace.top

Py:   list(range(0, 10, 2))
来源：http://urf.yuanzhike.top

PHP:  range(0, 10, 2);
来源：http://scp.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ndb.ehwqpu.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://djf.yvedp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kxs.hnqzz.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bgi.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://icr.hywenlv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://isy.fengsongda.top

[B12] 跳出多层循环
来源：http://cvn.fzhhl.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wry.hywenlv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ytn.chenzaomai.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ozh.fehbvm.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yns.nwbrower.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xfp.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rxv.ctjpmb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gqe.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yvj.pycfn.com


<!-- 参考信息 -->