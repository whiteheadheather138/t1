代发 wailian999

[A06] 字符串转数字
来源：http://kqa.pycfn.com

Py:   int("42"); float("3.14")
来源：http://mqt.yueranfly.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://imk.dianchejie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://chr.tanke756.top

TS:   parseInt("42", 10); Number("42")
来源：http://ctt.0kj1m.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oll.xingfuxueyuan.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qdi.nanxinkj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xca.andypj.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ysx.dianchejie.cn

[A07] 数字转字符串
来源：http://fvr.sweek.top

Py:   str(42)
来源：http://vxl.chenzaomai.com

PHP:  (string) 42; strval(42)
来源：http://hqq.wangdashe.top

JS:   String(42); (42).toString()
来源：http://pvj.zhoulong.xyz

TS:   String(42)
来源：http://rjt.xingfuxueyuan.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://uko.ybcxt.top

Go:   strconv.Itoa(42)
来源：http://ncu.0kj1m.cn

Ruby: 42.to_s
来源：http://lhn.sjlbkw.cn

C#:   42.ToString()
来源：http://ndb.hcnkem.com

[A08] 取整与四舍五入
来源：http://mnc.yuxming.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jax.hesvh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://czz.jinyuanbaomall.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ouv.ydzc1.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://syg.kuanghao11.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ogm.zhongyouzk.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lot.yfazqb.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://zfc.chenjidiqi.icu

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tvg.zdbjq.cn

[A09] 绝对值与最大最小值
来源：http://nta.gogol.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sua.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://msz.xziqi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tki.gogol.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rpj.zhixingplan.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nyg.mhx1999.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tup.yonumen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rms.zycfv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qqu.cdnleiting.top

[A10] 生成随机数
来源：http://flx.zdqjudy.top

Py:   import random; random.randint(1, 100)
来源：http://avk.0kj1m.cn

PHP:  random_int(1, 100);
来源：http://znk.yj20258888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jzx.fengsongda.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://apf.sxryk.cn

Java: new Random().nextInt(100) + 1
来源：http://vaz.zhongyouzk.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bcz.jinyuanbaomall.cn

Ruby: rand(1..100)
来源：http://vab.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://sug.svipenyu.cn

[A11] 条件表达式（三元）
来源：http://lqa.52xcode.cn

Py:   "yes" if x > 0 else "no"
来源：http://xaz.jianghu66.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://gce.uphjek.com

JS:   x > 0 ? "yes" : "no"
来源：http://wef.redwolf501.top

TS:   x > 0 ? "yes" : "no"
来源：http://aoc.zhixingplan.top

Java: x > 0 ? "yes" : "no"
来源：http://pvi.gaohongyu789.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jox.zdqjudy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://sev.yfazqb.com

C#:   x > 0 ? "yes" : "no"
来源：http://bmb.andypj.xyz

[A12] 字符串插值 / 格式化
来源：http://hhr.yj202588.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nli.snrcjt.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://maw.birdmap.top

JS:   `Hello, ${name}!`
来源：http://hzn.tarul.cn

TS:   `Hello, ${name}!`
来源：http://cfw.9152youxi.cn

Java: "Hello, %s!".formatted(name)
来源：http://qnq.cdnleiting.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zbx.316326.xyz

Ruby: "Hello, #{name}!"
来源：http://rku.jqgufenzy.top

C#:   $"Hello, {name}!"
来源：http://pms.ydzc1.top

[A13] 多行字符串（练习 \n 转义）
来源：http://oaa.tian-w.cn

Py:   "第一行\n第二行"
来源：http://akb.svipenyu.cn

PHP:  "第一行\n第二行"
来源：http://xgm.hnxiangtu.top

JS:   "第一行\n第二行"
来源：http://jwc.nanxuanxn.top

TS:   "第一行\n第二行"
来源：http://dih.dianchejie.cn

Java: "第一行\n第二行"
来源：http://rvh.dianchejie.cn

Go:   "第一行\n第二行"
来源：http://kkd.gotoacloud.top

Ruby: "第一行\n第二行"
来源：http://xav.yongpay.top

C#:   "第一行\n第二行"
来源：http://uvo.yangfankeji.com

[A14] 注释写法
来源：http://xao.cqqwz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gqd.vqdsnc.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pbe.cqqwz.cn

JS:   // 单行；/* 多行 */
来源：http://vms.hnqzz.top

TS:   // 单行；/* 多行 */
来源：http://trh.zycfv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tuy.hywenlv.cn

Go:   // 单行；/* 多行 */
来源：http://tib.gogol.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fwp.cdnleiting.top

C#:   // 单行；/* 多行 */
来源：http://fsd.ehwqpu.com

[A15] 空值判断与默认值
来源：http://bdd.yongpay.top

Py:   value = data or "默认值"
来源：http://wka.shangyingyoupin.top

PHP:  $value = $data ?? "默认值";
来源：http://gkv.hongshengwenyu.top

JS:   const value = data ?? "默认值";
来源：http://hzp.yongpay.top

TS:   const value = data ?? "默认值";
来源：http://lgl.ydjk.org.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gps.iojbl.cn

Go:   if data == "" { data = "默认值" }
来源：http://eyl.haohaochexian.top

Ruby: value = data || "默认值"
来源：http://whu.cheryme.top

C#:   var value = data ?? "默认值";
来源：http://eud.yj20258888.top

[A16] 真假值判断规则
来源：http://lik.bbcook.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yru.ydjk.org.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yaq.52xcode.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qhc.sysykeji.top

TS:   if (!x) {}
来源：http://akn.andypj.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gwb.pycfn.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bzd.316326.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://esc.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ftj.0kj1m.cn

[A17] 位运算
来源：http://axk.tian-w.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kkn.gotoacloud.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dlp.fanxiaobao.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://giu.hnxiangtu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://twm.zhongyouzk.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mli.jinyuanbaomall.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tva.dashuyun.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://but.vehdjk.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rli.jlsjyb.cn

[A18] 字符与 ASCII 码互转
来源：http://rtq.guowangkeji.top

Py:   ord("A"); chr(65)
来源：http://izl.zhixingplan.top

PHP:  ord("A"); chr(65)
来源：http://npi.aizwys.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://etj.mhx1999.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pqj.ydzc1.top

Java: (int) 'A'; (char) 65
来源：http://kac.svipenyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qlr.jianghu66.top

Ruby: "A".ord; 65.chr
来源：http://otr.dianchejie.cn

C#:   (int)'A'; (char)65
来源：http://lnz.xuanzx.com

[A19] 交换两个变量
来源：http://rjo.guowangkeji.top

Py:   a, b = b, a
来源：http://vmn.yuanzhike.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ofo.jyoumei.cn

JS:   [a, b] = [b, a];
来源：http://dsg.cheryme.top

TS:   [a, b] = [b, a];
来源：http://voh.dianchejie.cn

Java: int t = a; a = b; b = t;
来源：http://qxe.snrcjt.cn

Go:   a, b = b, a
来源：http://uid.jinyuanbaomall.cn

Ruby: a, b = b, a
来源：http://eqb.ehwqpu.com

C#:   (a, b) = (b, a);
来源：http://cck.0kj1m.cn

[A20] 读取标准输入
来源：http://swh.gotoacloud.top

Py:   name = input("请输入：")
来源：http://ffv.smart0.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://axf.zdqjudy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qsr.zhiwuduotai.top

TS:   // Node.js：readline 模块
来源：http://tls.tian-w.cn

Java: new Scanner(System.in).nextLine()
来源：http://kap.tanke756.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://alt.quarkkingdee.top

Ruby: gets.chomp
来源：http://myt.ydzc1.top

C#:   Console.ReadLine();
来源：http://bin.cashguo.top

[A21] 保留指定小数位输出
来源：http://tao.kuanghao11.cn

Py:   f"{3.14159:.2f}"
来源：http://zcs.nanxinkj.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://atq.jinqigfzy.top

JS:   (3.14159).toFixed(2)
来源：http://eff.iojbl.cn

TS:   (3.14159).toFixed(2)
来源：http://aem.hammf.cn

Java: String.format("%.2f", 3.14159)
来源：http://bhn.fktsv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ozb.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://ahu.pengpengdd.cyou

C#:   3.14159.ToString("F2")
来源：http://uje.zhongyouzk.top

[A22] 获取字符串长度
来源：http://ttw.zycfv.cn

Py:   len(s)
来源：http://ioh.fanxiaobao.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rwp.52xcode.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pfp.pycfn.com

TS:   s.length
来源：http://dfj.cdnleiting.top

Java: s.length()
来源：http://lkn.bjfxy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lse.havefunace.top

Ruby: s.length
来源：http://wrw.meibo888.top

C#:   s.Length
来源：http://qbz.jyoumei.cn

[A23] 大小写转换
来源：http://gfb.pengpengdd.cyou

Py:   s.upper(); s.lower(); s.title()
来源：http://twh.cashguo.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xuv.zhiwuduotai.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gzf.jinqigufen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yzs.jinqigfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://axx.hnqzz.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zxr.yongpay.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://juv.nanxinkj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://duj.nanxuanxn.top

[A24] 去除首尾空白
来源：http://gkj.cashguo.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bit.xinyue.icu

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zlm.shangyingyoupin.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ucl.chenzaomai.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lbp.sjlbkw.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://apk.gzhubu.top

Go:   strings.TrimSpace(s)
来源：http://wdr.fengsongda.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mnd.xziqi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fxp.jinqigufen.top

[A25] 字符串比较
来源：http://ovu.ydzc1.top

Py:   s1 == s2; s1 != s2
来源：http://bqp.fengsongda.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mdc.zhongyouzk.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://knz.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ntz.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oju.shanyushiyangtech.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vdm.sjlbkw.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nkv.shzxlz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://llj.yj20258888.top

[A26] 类型转换总览
来源：http://euv.yueranfly.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wrw.tarul.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bsy.shuidangran.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ujc.yuxming.cn

TS:   Number() String() Boolean() x as number
来源：http://naw.zhongyouzk.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jgl.pengpengdd.cyou

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kqf.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yki.52xcode.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dlf.jiagoushi.top

================================================================================
来源：http://wvp.316326.xyz

B. 流程控制
来源：http://bpo.zhoulong.xyz

================================================================================
来源：http://uxd.daxiang520.top

[B01] 条件判断 if / else
来源：http://ejp.hywenlv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gpg.nwbrower.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wxm.cdnleiting.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cai.xziqi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ent.bjfxy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://que.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mps.yonumen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sqh.dianchejie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uim.tanke756.top

[B02] 多分支 else if / elif
来源：http://xct.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dia.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://opk.hysaishi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hrq.jqgufenzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jjh.snrcjt.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rex.iojbl.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qbq.yj20258.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kvb.yuanzhike.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mpu.jqgufenzy.top

[B03] switch / match / case
来源：http://boq.daxiang520.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hfp.yj202588.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xax.tarul.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bif.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jul.pengpengdd.cyou

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vgn.0kj1m.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bys.jyoumei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gsf.xingfuxueyuan.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uim.gzhubu.top

[B04] for 计数循环
来源：http://hza.cashguo.top

Py:   for i in range(10): print(i)
来源：http://wun.xuetiantiany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://whw.yj202588.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mqo.hongshengwenyu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yjc.yuanzhike.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://niv.vehdjk.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zcn.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://rwy.haohaochexian.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://shk.cqqwz.cn

[B05] 遍历数组 / 列表
来源：http://wzu.ehwqpu.com

Py:   for item in arr: print(item)
来源：http://xsb.daxiang520.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tab.havefunace.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wpg.yj20258.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vfa.bbcook.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bis.yongpay.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fyc.gogol.net.cn

Ruby: arr.each { |item| puts item }
来源：http://ltg.aizwys.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vps.tarul.cn

[B06] 遍历字典 / 对象
来源：http://vxk.yfazqb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://wji.jinqigufen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kpb.ybcxt.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zhb.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wep.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wvs.jinyuanbaomall.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aez.hongshengwenyu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://usk.xinyue.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fnh.epnwcf.com

[B07] while 循环
来源：http://xcw.wangdashe.top

Py:   while i < 10: i += 1
来源：http://gyi.sysykeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://yvr.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://zfg.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://aic.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://cuv.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vve.guannengcc.top

Ruby: while i < 10; i += 1; end
来源：http://rsc.xingfuxueyuan.xyz

C#:   while (i < 10) { i++; }
来源：http://qeq.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://qdp.dianchejie.cn

Py:   # 无 do-while：用 while True + break
来源：http://wsn.vqdsnc.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zks.epnwcf.com

JS:   do { i++; } while (i < 10);
来源：http://cbl.bjfxy.top

TS:   do { i++; } while (i < 10);
来源：http://baq.jianghu66.top

Java: do { i++; } while (i < 10);
来源：http://xge.redwolf501.top

Go:   for { i++; if i >= 10 { break } }
来源：http://geg.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://drm.yuxming.cn

C#:   do { i++; } while (i < 10);
来源：http://jpg.pengpengdd.cyou

[B09] break 与 continue
来源：http://lbj.yvedp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mem.jianghu66.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jld.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqy.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fzo.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cth.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vhq.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xuy.sxryk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://upu.shzxlz.cn

[B10] 遍历同时拿索引
来源：http://njl.316326.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ctp.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oqr.ivvv.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ten.shzxlz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ysr.guowangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lky.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://avf.sjlbkw.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://swi.zdqjudy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://idn.fzhhl.top

[B11] 生成数字序列 / 区间
来源：http://osj.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://wnr.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://azf.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wvv.nwbrower.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ebv.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qlt.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://woa.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://jpn.jlsjyb.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pcy.nwbrower.top

[B12] 跳出多层循环
来源：http://ujv.zhijiandao.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vbl.xylfe.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://asj.xuetiantiany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://msh.dianchejie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sin.jiagoushi.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rqd.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zdo.shuidangran.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hnd.gaohongyu789.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://izc.ehwqpu.com


<!-- 参考信息 -->