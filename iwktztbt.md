代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://fwd.shzxlz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://umt.sysykeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://clf.daria6918.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ryo.pycfn.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://whi.mhx1999.top

[A07] 数字转字符串
来源：http://exg.hcnkem.com

Py:   str(42)
来源：http://wbg.zhongyouzk.top

PHP:  (string) 42; strval(42)
来源：http://flx.ydjk.org.cn

JS:   String(42); (42).toString()
来源：http://qvl.daria6918.cn

TS:   String(42)
来源：http://baf.kuanghao11.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sax.xylfe.cn

Go:   strconv.Itoa(42)
来源：http://ovh.yuanzhike.top

Ruby: 42.to_s
来源：http://tzg.ctjpmb.com

C#:   42.ToString()
来源：http://ezu.redwolf501.top

[A08] 取整与四舍五入
来源：http://hox.jyoumei.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bjg.fengsongda.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://aai.cucudq.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zne.quarkkingdee.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zyq.jlsjyb.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zuk.shzxlz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qxu.vqdsnc.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mmb.yvedp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vzk.cashguo.top

[A09] 绝对值与最大最小值
来源：http://dpi.fzhhl.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://axq.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mwi.jiagoushi.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://coc.chenzaomai.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fgl.hongshengwenyu.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gjv.jlsjyb.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rfa.mhx1999.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jsm.zhongyouzk.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://crk.yuanzhike.top

[A10] 生成随机数
来源：http://xah.gaohongyu789.top

Py:   import random; random.randint(1, 100)
来源：http://frm.gogol.net.cn

PHP:  random_int(1, 100);
来源：http://fgu.xinyue.icu

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rcc.haohaochexian.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jhy.shangyingyoupin.top

Java: new Random().nextInt(100) + 1
来源：http://fkw.chenzaomai.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zvz.yanxiufei.cn

Ruby: rand(1..100)
来源：http://pkq.redwolf501.top

C#:   new Random().Next(1, 101)
来源：http://rou.guannengcc.top

[A11] 条件表达式（三元）
来源：http://nvz.gaohongyu789.top

Py:   "yes" if x > 0 else "no"
来源：http://gfg.yfazqb.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://pze.gotoacloud.top

JS:   x > 0 ? "yes" : "no"
来源：http://rpr.hfpthk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qih.ydjk.org.cn

Java: x > 0 ? "yes" : "no"
来源：http://hqs.ivvv.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ojf.ydzc1.top

Ruby: x > 0 ? "yes" : "no"
来源：http://hbl.wangdashe.top

C#:   x > 0 ? "yes" : "no"
来源：http://obg.yonumen.top

[A12] 字符串插值 / 格式化
来源：http://ihd.0kj1m.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dpo.zdbjq.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kaw.hysaishi.cn

JS:   `Hello, ${name}!`
来源：http://bys.ivvv.top

TS:   `Hello, ${name}!`
来源：http://wvl.jiagoushi.top

Java: "Hello, %s!".formatted(name)
来源：http://rqd.vqdsnc.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fum.jinqigufen.top

Ruby: "Hello, #{name}!"
来源：http://wcz.hnqzz.top

C#:   $"Hello, {name}!"
来源：http://szp.cheryme.top

[A13] 多行字符串（练习 \n 转义）
来源：http://xsa.yj202588.top

Py:   "第一行\n第二行"
来源：http://ykl.vehdjk.com

PHP:  "第一行\n第二行"
来源：http://paa.xuetiantiany.cn

JS:   "第一行\n第二行"
来源：http://gah.chenzaomai.com

TS:   "第一行\n第二行"
来源：http://iev.tanke756.top

Java: "第一行\n第二行"
来源：http://cnu.chenzaomai.com

Go:   "第一行\n第二行"
来源：http://icc.gotoacloud.top

Ruby: "第一行\n第二行"
来源：http://fgq.aizwys.cn

C#:   "第一行\n第二行"
来源：http://jqm.vehdjk.com

[A14] 注释写法
来源：http://jfe.zhiwuduotai.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://pih.yj202588.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://exh.dashuyun.cn

JS:   // 单行；/* 多行 */
来源：http://xmk.haohaochexian.top

TS:   // 单行；/* 多行 */
来源：http://nbt.ywan-chungtsiang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qsp.zhongyouzk.top

Go:   // 单行；/* 多行 */
来源：http://bxk.pengpengdd.cyou

Ruby: # 单行；=begin 多行 =end
来源：http://ppu.haohaochexian.top

C#:   // 单行；/* 多行 */
来源：http://sgs.quarkkingdee.top

[A15] 空值判断与默认值
来源：http://bas.zhoulong.xyz

Py:   value = data or "默认值"
来源：http://fut.bjfxy.top

PHP:  $value = $data ?? "默认值";
来源：http://hnb.hfpthk.cn

JS:   const value = data ?? "默认值";
来源：http://kbw.jiagoushi.top

TS:   const value = data ?? "默认值";
来源：http://cpp.shanyushiyangtech.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jbr.zhijiandao.cn

Go:   if data == "" { data = "默认值" }
来源：http://feg.hesvh.cn

Ruby: value = data || "默认值"
来源：http://jak.uphjek.com

C#:   var value = data ?? "默认值";
来源：http://xix.birdmap.top

[A16] 真假值判断规则
来源：http://rrc.bjfxy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eed.nanxinkj.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://buh.hammf.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zbf.shzxlz.cn

TS:   if (!x) {}
来源：http://zpw.cheryme.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jur.uphjek.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cvd.ctjpmb.com

Ruby: unless x            # nil 与 false 为假
来源：http://jpu.chenlongwang.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pex.jlsjyb.cn

[A17] 位运算
来源：http://qjn.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://chu.tarul.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hbb.gotoacloud.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hmx.cucudq.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gsv.jyoumei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yqw.birdmap.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ype.ydzc1.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hdz.zhixingplan.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cfo.meibo888.top

[A18] 字符与 ASCII 码互转
来源：http://skc.bjfxy.top

Py:   ord("A"); chr(65)
来源：http://uyy.vehdjk.com

PHP:  ord("A"); chr(65)
来源：http://zbn.zhiwuduotai.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gby.ivvv.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://red.sufxvd.cn

Java: (int) 'A'; (char) 65
来源：http://djy.xylfe.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zxf.ywan-chungtsiang.top

Ruby: "A".ord; 65.chr
来源：http://gsh.zdbjq.cn

C#:   (int)'A'; (char)65
来源：http://sow.shangyingyoupin.top

[A19] 交换两个变量
来源：http://skw.jiagoushi.top

Py:   a, b = b, a
来源：http://vdg.meibo888.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jxq.hcnkem.com

JS:   [a, b] = [b, a];
来源：http://abq.hfpthk.cn

TS:   [a, b] = [b, a];
来源：http://gax.hywenlv.cn

Java: int t = a; a = b; b = t;
来源：http://flz.316326.xyz

Go:   a, b = b, a
来源：http://pdf.hnqzz.top

Ruby: a, b = b, a
来源：http://ncs.yj20258888.top

C#:   (a, b) = (b, a);
来源：http://jwi.uphjek.com

[A20] 读取标准输入
来源：http://syd.xinyue.icu

Py:   name = input("请输入：")
来源：http://fzd.wangdashe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qdh.daxiang520.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pes.aizwys.cn

TS:   // Node.js：readline 模块
来源：http://pfz.9152youxi.cn

Java: new Scanner(System.in).nextLine()
来源：http://bxs.316326.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ciy.sjlbkw.cn

Ruby: gets.chomp
来源：http://aga.jqgufenzy.top

C#:   Console.ReadLine();
来源：http://kki.guowangkeji.top

[A21] 保留指定小数位输出
来源：http://tgu.jqgufenzy.top

Py:   f"{3.14159:.2f}"
来源：http://abq.jinqigufen.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mhw.nanxinkj.top

JS:   (3.14159).toFixed(2)
来源：http://rhb.mhx1999.top

TS:   (3.14159).toFixed(2)
来源：http://uth.c1oappe.top

Java: String.format("%.2f", 3.14159)
来源：http://hll.yangfankeji.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jud.cheryme.top

Ruby: format("%.2f", 3.14159)
来源：http://gyw.wangdashe.top

C#:   3.14159.ToString("F2")
来源：http://rqh.pengpengdd.cyou

[A22] 获取字符串长度
来源：http://ljy.zhaomingkeji.xyz

Py:   len(s)
来源：http://rmv.ppjwa.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xss.dianchejie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vdt.9152youxi.cn

TS:   s.length
来源：http://szl.cashguo.top

Java: s.length()
来源：http://nxu.redwolf501.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fpd.chenzaomai.com

Ruby: s.length
来源：http://gww.yuxming.cn

C#:   s.Length
来源：http://yjo.jianghu66.top

[A23] 大小写转换
来源：http://hwm.yonumen.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hat.zhiwuduotai.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wpe.pycfn.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ihi.redwolf501.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gen.c1oappe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gxf.hnxiangtu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uuu.zhijiandao.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gsm.xuetiantiany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fjf.shuidangran.top

[A24] 去除首尾空白
来源：http://lpr.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rcp.jinghuilouyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://put.hywenlv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://laa.ctjpmb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tws.mhx1999.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tws.xuetiantiany.cn

Go:   strings.TrimSpace(s)
来源：http://dte.zycfv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://isn.zhengqikj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pgj.nanxinkj.top

[A25] 字符串比较
来源：http://byc.yonumen.top

Py:   s1 == s2; s1 != s2
来源：http://yja.cucudq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pbd.0kj1m.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qpx.feifeiyinyue.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tbu.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://aik.chenjidiqi.icu

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xef.haohaochexian.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nuv.yvedp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://trv.quarkkingdee.top

[A26] 类型转换总览
来源：http://ofm.jlsjyb.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fmx.zhijiandao.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lzg.hnqzz.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pzp.9152youxi.cn

TS:   Number() String() Boolean() x as number
来源：http://krk.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nwv.jinyuanbaomall.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ctf.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cyv.chenjidiqi.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oty.zhaomingkeji.xyz

================================================================================
来源：http://rbb.gogol.net.cn

B. 流程控制
来源：http://nvf.vehdjk.com

================================================================================
来源：http://zmk.vqdsnc.cn

[B01] 条件判断 if / else
来源：http://bao.jinyuanbaomall.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lhm.chenzaomai.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://orv.svipenyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nfv.0kj1m.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zwq.epnwcf.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://obv.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hpu.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nzq.yj202588.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://onq.tianlin.xyz

[B02] 多分支 else if / elif
来源：http://neg.tian-w.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vdj.birdmap.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wzw.sysykeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vyr.xylfe.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vpe.jinghuilouyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://okx.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tgm.ybcxt.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ocn.sysykeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ewu.xylfe.cn

[B03] switch / match / case
来源：http://dei.jinyuanbaomall.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gje.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lcc.zhongyouzk.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ojm.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tis.hongshengwenyu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xig.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jxk.nanxinkj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vfp.yongpay.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nyo.mhx1999.top

[B04] for 计数循环
来源：http://wto.shanyushiyangkeji.top

Py:   for i in range(10): print(i)
来源：http://onh.snrcjt.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xmh.havefunace.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jqn.sjlbkw.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://adi.yj20258.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zdk.jqgufenzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vjv.ehwqpu.com

Ruby: 10.times { |i| puts i }
来源：http://igt.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vns.ehwqpu.com

[B05] 遍历数组 / 列表
来源：http://qkf.shuidangran.top

Py:   for item in arr: print(item)
来源：http://sky.andypj.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gca.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zeq.nanxinkj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fvw.gaohongyu789.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rwm.zhaomingkeji.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zgn.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://dru.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vvr.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://wje.daria6918.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://teg.bbcook.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ysv.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gdc.fanxiaobao.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bjh.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://etf.xingfuxueyuan.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mwg.yanxiufei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ydv.svipenyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cby.yanxiufei.cn

[B07] while 循环
来源：http://xyl.zhoulong.xyz

Py:   while i < 10: i += 1
来源：http://bsu.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://ped.guowangkeji.top

JS:   while (i < 10) { i++; }
来源：http://rez.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://ftz.ydzc1.top

Java: while (i < 10) { i++; }
来源：http://dgn.tarul.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://awx.jlsjyb.cn

Ruby: while i < 10; i += 1; end
来源：http://nno.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://rpq.cheryme.top

[B08] do-while（至少执行一次）
来源：http://akt.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://iru.9152youxi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qwv.fehbvm.com

JS:   do { i++; } while (i < 10);
来源：http://jkr.kuanghao11.cn

TS:   do { i++; } while (i < 10);
来源：http://iqz.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://bbs.snrcjt.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fuk.yj20258.top

Ruby: begin; i += 1; end while i < 10
来源：http://vss.redwolf501.top

C#:   do { i++; } while (i < 10);
来源：http://gtu.yangfankeji.com

[B09] break 与 continue
来源：http://fvk.sufxvd.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dyv.chenjidiqi.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jns.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tlb.jianghu66.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nfa.ybcxt.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zcl.yvedp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dot.haohaochexian.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mhd.9152youxi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xnn.kuanghao11.cn

[B10] 遍历同时拿索引
来源：http://mug.ctjpmb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hpg.cucudq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fyw.jinqigufen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wxf.zhiwuduotai.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lds.mhx1999.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gmv.daxiang520.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gxh.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ypx.epnwcf.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fkm.ppjwa.cn

[B11] 生成数字序列 / 区间
来源：http://xzy.gaohongyu789.top

Py:   list(range(0, 10, 2))
来源：http://yvf.meibo888.top

PHP:  range(0, 10, 2);
来源：http://gtb.bbcook.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zzh.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ncw.gotoacloud.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bgh.yuanzhike.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lds.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://vqm.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eps.jinqigfzy.top

[B12] 跳出多层循环
来源：http://wxg.dianchejie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fkr.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pes.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kay.gzhubu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://snl.yonumen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lfz.jqgufenzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yks.cashguo.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mml.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mdq.fengsongda.top

[B13] 判断是否为数字
来源：http://jiy.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://lbq.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://pmi.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lle.hesvh.cn


<!-- 参考信息 -->