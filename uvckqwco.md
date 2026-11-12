代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://mkl.ybcxt.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vqp.cqqwz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oet.sysykeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zrf.xziqi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oji.hammf.cn

[A07] 数字转字符串
来源：http://fwz.daria6918.cn

Py:   str(42)
来源：http://yrd.guowangkeji.top

PHP:  (string) 42; strval(42)
来源：http://exn.yongpay.top

JS:   String(42); (42).toString()
来源：http://mwl.uphjek.com

TS:   String(42)
来源：http://omb.jqgfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://tpb.yueranfly.top

Go:   strconv.Itoa(42)
来源：http://dsu.bjfxy.top

Ruby: 42.to_s
来源：http://onu.jinqigfzy.top

C#:   42.ToString()
来源：http://cfk.pycfn.com

[A08] 取整与四舍五入
来源：http://lpf.ivvv.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mtd.xylfe.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qix.chenjidiqi.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dek.hnqzz.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vvw.ctjpmb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vxy.c1oappe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ffs.ywan-chungtsiang.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://pbi.jlsjyb.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hsz.yj20258.top

[A09] 绝对值与最大最小值
来源：http://npx.yvedp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gme.sxryk.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wyl.zhaomingkeji.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zwo.ivvv.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vze.guannengcc.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fkt.haohaochexian.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xao.dashuyun.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fcg.c1oappe.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ghk.fengsongda.top

[A10] 生成随机数
来源：http://jrr.andypj.xyz

Py:   import random; random.randint(1, 100)
来源：http://dlp.jyoumei.cn

PHP:  random_int(1, 100);
来源：http://okd.feifeiyinyue.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qda.jinghuilouyu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://irt.wangshuangyany.cn

Java: new Random().nextInt(100) + 1
来源：http://tab.ybcxt.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://afm.xingfuxueyuan.xyz

Ruby: rand(1..100)
来源：http://wyz.jinqigufen.top

C#:   new Random().Next(1, 101)
来源：http://ypl.xylfe.cn

[A11] 条件表达式（三元）
来源：http://khn.ehwqpu.com

Py:   "yes" if x > 0 else "no"
来源：http://pdn.redwolf501.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kfe.vqdsnc.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ygp.bjfxy.top

TS:   x > 0 ? "yes" : "no"
来源：http://rrg.jiagoushi.top

Java: x > 0 ? "yes" : "no"
来源：http://fxc.hesvh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://eqc.hcnkem.com

Ruby: x > 0 ? "yes" : "no"
来源：http://iiz.iojbl.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mep.xziqi.cn

[A12] 字符串插值 / 格式化
来源：http://jzn.cqqwz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pcz.sysykeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://csq.jinqigfzy.top

JS:   `Hello, ${name}!`
来源：http://azt.zhijiandao.cn

TS:   `Hello, ${name}!`
来源：http://haa.bjfxy.top

Java: "Hello, %s!".formatted(name)
来源：http://kuz.haohaochexian.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eew.yj202588.top

Ruby: "Hello, #{name}!"
来源：http://jnb.daxiang520.top

C#:   $"Hello, {name}!"
来源：http://lne.xuanzx.com

[A13] 多行字符串（练习 \n 转义）
来源：http://oux.guannengcc.top

Py:   "第一行\n第二行"
来源：http://cwt.jinghuilouyu.cn

PHP:  "第一行\n第二行"
来源：http://dal.yanxiufei.cn

JS:   "第一行\n第二行"
来源：http://tzq.jianghu66.top

TS:   "第一行\n第二行"
来源：http://kuj.xziqi.cn

Java: "第一行\n第二行"
来源：http://rdw.svipenyu.cn

Go:   "第一行\n第二行"
来源：http://avr.zhengqikj.top

Ruby: "第一行\n第二行"
来源：http://xiq.wangdashe.top

C#:   "第一行\n第二行"
来源：http://rio.hesvh.cn

[A14] 注释写法
来源：http://dgn.yj20258.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://puz.zhaomingkeji.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://ski.jianghu66.top

JS:   // 单行；/* 多行 */
来源：http://yal.fehbvm.com

TS:   // 单行；/* 多行 */
来源：http://iyb.ppjwa.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xoj.xuetiantiany.cn

Go:   // 单行；/* 多行 */
来源：http://xnl.0kj1m.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qvg.snrcjt.cn

C#:   // 单行；/* 多行 */
来源：http://wkh.jqgfzy.top

[A15] 空值判断与默认值
来源：http://nvv.xingfuxueyuan.xyz

Py:   value = data or "默认值"
来源：http://fyu.nanxuanxn.top

PHP:  $value = $data ?? "默认值";
来源：http://jgo.sweek.top

JS:   const value = data ?? "默认值";
来源：http://lzx.yj202588.top

TS:   const value = data ?? "默认值";
来源：http://htd.jlsjyb.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mmx.316326.xyz

Go:   if data == "" { data = "默认值" }
来源：http://wxr.wangshuangyany.cn

Ruby: value = data || "默认值"
来源：http://iyw.yongpay.top

C#:   var value = data ?? "默认值";
来源：http://idl.ehwqpu.com

[A16] 真假值判断规则
来源：http://tat.fehbvm.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xqw.ybcxt.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jkm.hnqzz.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iaj.sweek.top

TS:   if (!x) {}
来源：http://vmw.svipenyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tvq.bjfxy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ukc.hysaishi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hkp.jianghu66.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qfy.redwolf501.top

[A17] 位运算
来源：http://ghd.epnwcf.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rlc.gaohongyu789.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zay.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ons.uphjek.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lbu.svipenyu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gor.kuanghao11.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ygn.xylfe.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zgh.birdmap.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ssd.c1oappe.top

[A18] 字符与 ASCII 码互转
来源：http://uax.dashuyun.cn

Py:   ord("A"); chr(65)
来源：http://lei.hnxiangtu.top

PHP:  ord("A"); chr(65)
来源：http://clj.hnxiangtu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jxz.yuanzhike.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ool.wangshuangyany.cn

Java: (int) 'A'; (char) 65
来源：http://lnw.haohaochexian.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ikm.epnwcf.com

Ruby: "A".ord; 65.chr
来源：http://oxz.yj20258888.top

C#:   (int)'A'; (char)65
来源：http://lro.fehbvm.com

[A19] 交换两个变量
来源：http://jps.xuetiantiany.cn

Py:   a, b = b, a
来源：http://eqa.feifeiyinyue.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dvp.quarkkingdee.top

JS:   [a, b] = [b, a];
来源：http://ihx.sweek.top

TS:   [a, b] = [b, a];
来源：http://uoc.xylfe.cn

Java: int t = a; a = b; b = t;
来源：http://evo.cucudq.cn

Go:   a, b = b, a
来源：http://mpv.xylfe.cn

Ruby: a, b = b, a
来源：http://mgv.jinqigfzy.top

C#:   (a, b) = (b, a);
来源：http://xhy.mhx1999.top

[A20] 读取标准输入
来源：http://ahj.jqgfzy.top

Py:   name = input("请输入：")
来源：http://yxz.hysaishi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://juc.fanxiaobao.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cvw.pengpengdd.cyou

TS:   // Node.js：readline 模块
来源：http://voo.aizwys.cn

Java: new Scanner(System.in).nextLine()
来源：http://brz.zhengqikj.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ndm.dashuyun.cn

Ruby: gets.chomp
来源：http://qca.snrcjt.cn

C#:   Console.ReadLine();
来源：http://kzu.uphjek.com

[A21] 保留指定小数位输出
来源：http://apg.hesvh.cn

Py:   f"{3.14159:.2f}"
来源：http://ddr.gzhubu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bht.yonumen.top

JS:   (3.14159).toFixed(2)
来源：http://lsr.bbcook.cn

TS:   (3.14159).toFixed(2)
来源：http://nuz.aizwys.cn

Java: String.format("%.2f", 3.14159)
来源：http://tva.xinyue.icu

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rxm.ctjpmb.com

Ruby: format("%.2f", 3.14159)
来源：http://pxf.sjlbkw.cn

C#:   3.14159.ToString("F2")
来源：http://iti.zhiwuduotai.top

[A22] 获取字符串长度
来源：http://ooc.gaohongyu789.top

Py:   len(s)
来源：http://eop.xuetiantiany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://arv.bjfxy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hxk.nanxuanxn.top

TS:   s.length
来源：http://fyc.guannengcc.top

Java: s.length()
来源：http://bkd.jyoumei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jip.feifeiyinyue.top

Ruby: s.length
来源：http://bci.jinqigfzy.top

C#:   s.Length
来源：http://uzu.aibaodan.cn

[A23] 大小写转换
来源：http://bsq.ivvv.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xki.xinyue.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aix.gogol.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eiw.yangfankeji.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://btk.cucudq.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kxt.fanxiaobao.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iyk.chenjidiqi.icu

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://isf.haohaochexian.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vth.wangshuangyany.cn

[A24] 去除首尾空白
来源：http://icv.feifeiyinyue.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gno.jinqigufen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jml.hfpthk.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mti.jinghuilouyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pjt.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gpa.chenzaomai.com

Go:   strings.TrimSpace(s)
来源：http://dsm.zhongyouzk.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uqf.ppjwa.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dpk.shanyushiyangtech.top

[A25] 字符串比较
来源：http://qpl.shangyingyoupin.top

Py:   s1 == s2; s1 != s2
来源：http://ulw.xingfuxueyuan.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wzw.sjlbkw.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wvh.sysykeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dla.nwbrower.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bow.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bkx.xuetiantiany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ieh.zhiwuduotai.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yxr.yonumen.top

[A26] 类型转换总览
来源：http://xor.zhixingplan.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://atv.redwolf501.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xap.yangfankeji.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kno.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://zia.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vqu.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xkq.yj202588.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fbj.sxryk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pww.9152youxi.cn

================================================================================
来源：http://wmk.bjfxy.top

B. 流程控制
来源：http://abf.fehbvm.com

================================================================================
来源：http://twg.sysykeji.top

[B01] 条件判断 if / else
来源：http://tui.tarul.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wnz.birdmap.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qhj.yuxming.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gge.fengsongda.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ivw.uphjek.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://vwl.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eij.nwbrower.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://myi.xuanzx.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://epo.yonumen.top

[B02] 多分支 else if / elif
来源：http://sox.zhoulong.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pnm.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://imj.hammf.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ytx.quarkkingdee.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xpe.hywenlv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zid.jiagoushi.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tij.hnxiangtu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sdx.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hjt.hnqzz.top

[B03] switch / match / case
来源：http://ijb.aizwys.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lno.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lkl.fanxiaobao.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wdz.ivvv.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iht.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nic.bbcook.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ouo.hongshengwenyu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sgn.9152youxi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vub.fengsongda.top

[B04] for 计数循环
来源：http://amg.quarkkingdee.top

Py:   for i in range(10): print(i)
来源：http://sfi.jinghuilouyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tld.snrcjt.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vrv.hongshengwenyu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rez.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://frg.aizwys.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hdp.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://zgq.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fxo.yongpay.top

[B05] 遍历数组 / 列表
来源：http://azh.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://rpl.sufxvd.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bfh.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qnc.jinqigufen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ysk.hysaishi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cez.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wvo.fzhhl.top

Ruby: arr.each { |item| puts item }
来源：http://fda.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mni.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://bys.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ngc.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sji.xylfe.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lbk.cashguo.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://utp.feifeiyinyue.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wbb.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xzz.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uxy.yongpay.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bul.gaohongyu789.top

[B07] while 循环
来源：http://fpv.hammf.cn

Py:   while i < 10: i += 1
来源：http://yzi.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://aky.ywan-chungtsiang.top

JS:   while (i < 10) { i++; }
来源：http://jaa.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://jci.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://glc.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uzp.shanyushiyangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://jmz.yj20258888.top

C#:   while (i < 10) { i++; }
来源：http://gap.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://gkg.9152youxi.cn

Py:   # 无 do-while：用 while True + break
来源：http://gld.316326.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://ytg.epnwcf.com

JS:   do { i++; } while (i < 10);
来源：http://tod.tian-w.cn

TS:   do { i++; } while (i < 10);
来源：http://bgr.gaohongyu789.top

Java: do { i++; } while (i < 10);
来源：http://ajz.epnwcf.com

Go:   for { i++; if i >= 10 { break } }
来源：http://cmb.hnxiangtu.top

Ruby: begin; i += 1; end while i < 10
来源：http://uei.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://lrz.havefunace.top

[B09] break 与 continue
来源：http://ikh.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ipj.vehdjk.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gps.cucudq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dom.sufxvd.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ogu.yuanzhike.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rck.jlsjyb.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bzc.cashguo.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kwe.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fqk.ydzc1.top

[B10] 遍历同时拿索引
来源：http://dbo.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cwu.daria6918.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fai.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hdc.daria6918.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mxl.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dhk.yueranfly.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jmy.jqgfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://moo.jinghuilouyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ppo.epnwcf.com

[B11] 生成数字序列 / 区间
来源：http://jbu.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://urp.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://pza.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gef.hammf.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mjt.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qui.ehwqpu.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bwu.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://zkc.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cpe.uphjek.com

[B12] 跳出多层循环
来源：http://wdi.yuanzhike.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://egs.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://nzo.zhoulong.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://esm.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xpb.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xdq.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wjm.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tpm.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uep.ydzc1.top

[B13] 判断是否为数字
来源：http://kqq.ybcxt.top

Py:   isinstance(x, (int, float))
来源：http://qql.yonumen.top

PHP:  is_numeric($x)
来源：http://usn.chenzaomai.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rrc.dianchejie.cn


<!-- 参考信息 -->