代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://btp.yonumen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zwn.jqgufenzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uos.shanyushiyangkeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vec.xuetiantiany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pga.xinyue.icu

[A07] 数字转字符串
来源：http://kbr.yfazqb.com

Py:   str(42)
来源：http://tvl.ppjwa.cn

PHP:  (string) 42; strval(42)
来源：http://jkn.vehdjk.com

JS:   String(42); (42).toString()
来源：http://hip.hnqzz.top

TS:   String(42)
来源：http://yvi.9152youxi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://opr.feifeiyinyue.top

Go:   strconv.Itoa(42)
来源：http://aik.yj202588.top

Ruby: 42.to_s
来源：http://wcm.c1oappe.top

C#:   42.ToString()
来源：http://zng.fktsv.cn

[A08] 取整与四舍五入
来源：http://nqb.uphjek.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lbq.zdbjq.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lyi.uphjek.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bwt.guannengcc.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mrg.hcnkem.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xav.shzxlz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xfx.zhiwuduotai.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ney.dashuyun.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fhz.gogol.net.cn

[A09] 绝对值与最大最小值
来源：http://esg.ivvv.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dpv.zhixingplan.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://umo.vehdjk.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ctp.cucudq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mgy.zdbjq.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ejl.dianchejie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://duw.jianghu66.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://udl.shuidangran.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vhb.316326.xyz

[A10] 生成随机数
来源：http://xsp.cheryme.top

Py:   import random; random.randint(1, 100)
来源：http://fvu.zdbjq.cn

PHP:  random_int(1, 100);
来源：http://wrb.bjfxy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tqk.ehwqpu.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wrw.xinyue.icu

Java: new Random().nextInt(100) + 1
来源：http://sfq.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kgo.ppjwa.cn

Ruby: rand(1..100)
来源：http://ami.yanxiufei.cn

C#:   new Random().Next(1, 101)
来源：http://ask.shzxlz.cn

[A11] 条件表达式（三元）
来源：http://jia.yueranfly.top

Py:   "yes" if x > 0 else "no"
来源：http://uhs.xuanzx.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://qhx.yangfankeji.com

JS:   x > 0 ? "yes" : "no"
来源：http://snl.zhoulong.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://mcn.wangshuangyany.cn

Java: x > 0 ? "yes" : "no"
来源：http://sxa.hammf.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fzy.zdbjq.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ihr.ppjwa.cn

C#:   x > 0 ? "yes" : "no"
来源：http://udr.snrcjt.cn

[A12] 字符串插值 / 格式化
来源：http://oji.sjlbkw.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nli.xinyue.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://suq.yj20258.top

JS:   `Hello, ${name}!`
来源：http://cey.yonumen.top

TS:   `Hello, ${name}!`
来源：http://gzy.wangshuangyany.cn

Java: "Hello, %s!".formatted(name)
来源：http://alk.cucudq.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ydo.jiagoushi.top

Ruby: "Hello, #{name}!"
来源：http://nvh.jlsjyb.cn

C#:   $"Hello, {name}!"
来源：http://ndl.nanxinkj.top

[A13] 多行字符串（练习 \n 转义）
来源：http://nce.dianchejie.cn

Py:   "第一行\n第二行"
来源：http://oli.c1oappe.top

PHP:  "第一行\n第二行"
来源：http://jas.jinqigufen.top

JS:   "第一行\n第二行"
来源：http://hhp.hnqzz.top

TS:   "第一行\n第二行"
来源：http://xdn.cucudq.cn

Java: "第一行\n第二行"
来源：http://enj.52xcode.cn

Go:   "第一行\n第二行"
来源：http://wso.bjfxy.top

Ruby: "第一行\n第二行"
来源：http://ciq.guowangkeji.top

C#:   "第一行\n第二行"
来源：http://dui.feifeiyinyue.top

[A14] 注释写法
来源：http://oxs.aibaodan.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jyr.gotoacloud.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pfq.shzxlz.cn

JS:   // 单行；/* 多行 */
来源：http://ium.jiagoushi.top

TS:   // 单行；/* 多行 */
来源：http://wfr.ybcxt.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://itl.fktsv.cn

Go:   // 单行；/* 多行 */
来源：http://jvt.ehwqpu.com

Ruby: # 单行；=begin 多行 =end
来源：http://der.zhengqikj.top

C#:   // 单行；/* 多行 */
来源：http://kuz.zhoulong.xyz

[A15] 空值判断与默认值
来源：http://tfo.birdmap.top

Py:   value = data or "默认值"
来源：http://qkz.gotoacloud.top

PHP:  $value = $data ?? "默认值";
来源：http://fwo.vehdjk.com

JS:   const value = data ?? "默认值";
来源：http://vbt.316326.xyz

TS:   const value = data ?? "默认值";
来源：http://ovu.hongshengwenyu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://htb.yuanzhike.top

Go:   if data == "" { data = "默认值" }
来源：http://qzh.xingfuxueyuan.xyz

Ruby: value = data || "默认值"
来源：http://jbc.xziqi.cn

C#:   var value = data ?? "默认值";
来源：http://wqj.jqgufenzy.top

[A16] 真假值判断规则
来源：http://pyq.bjfxy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ynw.hnqzz.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fse.sysykeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oyt.xingfuxueyuan.xyz

TS:   if (!x) {}
来源：http://osh.svipenyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://afm.shangyingyoupin.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ocg.bbcook.cn

Ruby: unless x            # nil 与 false 为假
来源：http://auf.daxiang520.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lip.hfpthk.cn

[A17] 位运算
来源：http://jsb.zhongyouzk.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ypl.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bdz.9152youxi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ymm.hysaishi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lvi.cdnleiting.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jnz.zdbjq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zfq.jlsjyb.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vnf.daria6918.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rub.xylfe.cn

[A18] 字符与 ASCII 码互转
来源：http://wtu.daria6918.cn

Py:   ord("A"); chr(65)
来源：http://lfg.vqdsnc.cn

PHP:  ord("A"); chr(65)
来源：http://gka.yonumen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uqs.jyoumei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://amh.wangdashe.top

Java: (int) 'A'; (char) 65
来源：http://hcn.zhengqikj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tab.vqdsnc.cn

Ruby: "A".ord; 65.chr
来源：http://qna.zhaomingkeji.xyz

C#:   (int)'A'; (char)65
来源：http://ftd.jiagoushi.top

[A19] 交换两个变量
来源：http://ubc.yonumen.top

Py:   a, b = b, a
来源：http://tvh.birdmap.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jgj.ybcxt.top

JS:   [a, b] = [b, a];
来源：http://idk.aibaodan.cn

TS:   [a, b] = [b, a];
来源：http://qrz.daxiang520.top

Java: int t = a; a = b; b = t;
来源：http://rds.hongshengwenyu.top

Go:   a, b = b, a
来源：http://sze.tarul.cn

Ruby: a, b = b, a
来源：http://rhu.tianlin.xyz

C#:   (a, b) = (b, a);
来源：http://trp.52xcode.cn

[A20] 读取标准输入
来源：http://ryd.tanke756.top

Py:   name = input("请输入：")
来源：http://lqr.nwbrower.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tdk.zhengqikj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xoe.sweek.top

TS:   // Node.js：readline 模块
来源：http://cgk.yonumen.top

Java: new Scanner(System.in).nextLine()
来源：http://xti.0kj1m.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uwz.cashguo.top

Ruby: gets.chomp
来源：http://vxn.zhiwuduotai.top

C#:   Console.ReadLine();
来源：http://xtx.ppjwa.cn

[A21] 保留指定小数位输出
来源：http://ajf.xziqi.cn

Py:   f"{3.14159:.2f}"
来源：http://qks.nanxinkj.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ayv.cashguo.top

JS:   (3.14159).toFixed(2)
来源：http://aiz.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://gzt.dashuyun.cn

Java: String.format("%.2f", 3.14159)
来源：http://zmd.meibo888.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nzx.quarkkingdee.top

Ruby: format("%.2f", 3.14159)
来源：http://ukg.jinyuanbaomall.cn

C#:   3.14159.ToString("F2")
来源：http://qjs.fzhhl.top

[A22] 获取字符串长度
来源：http://ubp.ywan-chungtsiang.top

Py:   len(s)
来源：http://lah.nanxuanxn.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vmc.cheryme.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://drx.haohaochexian.top

TS:   s.length
来源：http://pyr.tarul.cn

Java: s.length()
来源：http://igc.hammf.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ibw.gzhubu.top

Ruby: s.length
来源：http://uyc.cashguo.top

C#:   s.Length
来源：http://glu.gotoacloud.top

[A23] 大小写转换
来源：http://plb.mhx1999.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nte.zhijiandao.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jln.smart0.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uyx.ppjwa.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wvr.sjlbkw.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fia.xylfe.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bhg.zhijiandao.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nqj.gzhubu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xbq.shangyingyoupin.top

[A24] 去除首尾空白
来源：http://fzd.sjlbkw.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://klo.zhiwuduotai.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://isw.shangyingyoupin.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://izg.sufxvd.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uuu.tianlin.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vow.wangshuangyany.cn

Go:   strings.TrimSpace(s)
来源：http://quv.hnxiangtu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oaw.nanxinkj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zrm.yonumen.top

[A25] 字符串比较
来源：http://dvu.52xcode.cn

Py:   s1 == s2; s1 != s2
来源：http://imp.shuidangran.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ini.jinyuanbaomall.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ldk.zhiwuduotai.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jfr.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://khf.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://stv.yonumen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xrd.hnqzz.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://btj.ywan-chungtsiang.top

[A26] 类型转换总览
来源：http://aaa.jlsjyb.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wuh.zhiwuduotai.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tzl.vehdjk.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zcx.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://zkm.iojbl.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cgx.yvedp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nrr.dashuyun.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jlc.jinqigufen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wlm.ehwqpu.com

================================================================================
来源：http://pst.52xcode.cn

B. 流程控制
来源：http://nbh.ydjk.org.cn

================================================================================
来源：http://dgv.zhoulong.xyz

[B01] 条件判断 if / else
来源：http://azc.meibo888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ies.bjfxy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://azw.fengsongda.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://chw.ydzc1.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yyn.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wuz.sysykeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zaf.ivvv.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ryk.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uyz.tianlin.xyz

[B02] 多分支 else if / elif
来源：http://jso.ehwqpu.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wjy.gaohongyu789.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cxg.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mhv.zycfv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cjc.haohaochexian.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nir.jinghuilouyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ezz.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nqu.zhongyouzk.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pnp.jyoumei.cn

[B03] switch / match / case
来源：http://quk.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lmi.hywenlv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tpt.zhengqikj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yuq.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wyx.cdnleiting.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wpe.shzxlz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wea.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jtw.hysaishi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vlo.hnxiangtu.top

[B04] for 计数循环
来源：http://koe.birdmap.top

Py:   for i in range(10): print(i)
来源：http://thn.hnqzz.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lip.zhoulong.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wvz.birdmap.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lha.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rvx.andypj.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pst.dianchejie.cn

Ruby: 10.times { |i| puts i }
来源：http://ryu.ywan-chungtsiang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tku.hcnkem.com

[B05] 遍历数组 / 列表
来源：http://gii.c1oappe.top

Py:   for item in arr: print(item)
来源：http://spx.yuanzhike.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iom.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kld.cdnleiting.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zxy.bjfxy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ndx.shzxlz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dpd.zhixingplan.top

Ruby: arr.each { |item| puts item }
来源：http://ved.tanke756.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yge.nanxuanxn.top

[B06] 遍历字典 / 对象
来源：http://vgk.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://urs.nanxuanxn.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wnl.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nwd.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aao.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kzm.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ufr.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tev.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://adr.cashguo.top

[B07] while 循环
来源：http://agu.shangyingyoupin.top

Py:   while i < 10: i += 1
来源：http://slz.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ssv.aibaodan.cn

JS:   while (i < 10) { i++; }
来源：http://mne.nanxuanxn.top

TS:   while (i < 10) { i++; }
来源：http://llp.ywan-chungtsiang.top

Java: while (i < 10) { i++; }
来源：http://yvj.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qcd.chenzaomai.com

Ruby: while i < 10; i += 1; end
来源：http://ndf.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://dos.mhx1999.top

[B08] do-while（至少执行一次）
来源：http://iue.ctjpmb.com

Py:   # 无 do-while：用 while True + break
来源：http://vdp.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yuc.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://euq.zhixingplan.top

TS:   do { i++; } while (i < 10);
来源：http://xyj.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://vrc.xingfuxueyuan.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://jyz.cheryme.top

Ruby: begin; i += 1; end while i < 10
来源：http://hlz.52xcode.cn

C#:   do { i++; } while (i < 10);
来源：http://qqz.yj20258.top

[B09] break 与 continue
来源：http://ath.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lhg.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lye.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wrk.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mbj.epnwcf.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yoz.jinqigfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fpz.gogol.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://brk.xuetiantiany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://agh.yongpay.top

[B10] 遍历同时拿索引
来源：http://cfs.xingfuxueyuan.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pwa.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rnz.tian-w.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tif.ppjwa.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yug.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ktr.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nuf.yueranfly.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blb.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sen.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://tof.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://iic.zhongyouzk.top

PHP:  range(0, 10, 2);
来源：http://ule.wangdashe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://exf.hnqzz.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://npw.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vma.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mqz.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://bac.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ini.jinqigufen.top

[B12] 跳出多层循环
来源：http://hbl.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wse.shanyushiyangtech.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://sgw.yuxming.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iys.chenlongwang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://evo.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://maq.ivvv.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cya.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cbr.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tsi.daria6918.cn

[B13] 判断是否为数字
来源：http://kqp.hysaishi.cn

Py:   isinstance(x, (int, float))
来源：http://vao.cqqwz.cn

PHP:  is_numeric($x)
来源：http://fmv.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qwi.hammf.cn


<!-- 参考信息 -->