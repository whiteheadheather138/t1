代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://yvv.nanxinkj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://pof.gzhubu.top

C#:   x.GetType().Name; x is int
来源：http://uki.zhengqikj.top

[A05] 整数除法与取模
来源：http://dqs.yfazqb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ryr.dashuyun.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://aps.guannengcc.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cpr.hammf.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ngx.havefunace.top

Java: 7 / 2; 7 % 2
来源：http://jfe.wangdashe.top

Go:   7 / 2; 7 % 2
来源：http://bkn.nanxinkj.top

Ruby: 7 / 2; 7 % 2
来源：http://geo.bjfxy.top

C#:   7 / 2; 7 % 2
来源：http://vqt.yj202588.top

[A06] 字符串转数字
来源：http://iuz.zdqjudy.top

Py:   int("42"); float("3.14")
来源：http://xzj.jqgfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oou.hesvh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nrm.sjlbkw.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pat.zhengqikj.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://scf.shanyushiyangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://aom.cdnleiting.top

Ruby: "42".to_i; "3.14".to_f
来源：http://eqk.yj202588.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zkm.yuanzhike.top

[A07] 数字转字符串
来源：http://dxp.jiagoushi.top

Py:   str(42)
来源：http://uvy.zhixingplan.top

PHP:  (string) 42; strval(42)
来源：http://ffr.xziqi.cn

JS:   String(42); (42).toString()
来源：http://yxm.xuetiantiany.cn

TS:   String(42)
来源：http://zxt.gogol.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mvf.yueranfly.top

Go:   strconv.Itoa(42)
来源：http://kcf.feifeiyinyue.top

Ruby: 42.to_s
来源：http://ovw.jqgfzy.top

C#:   42.ToString()
来源：http://ddq.andypj.xyz

[A08] 取整与四舍五入
来源：http://lru.zhijiandao.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ywc.nwbrower.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://slb.c1oappe.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ywi.zhaomingkeji.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lqc.zhaomingkeji.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://eqq.cashguo.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pjd.yuanzhike.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://yfm.zycfv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qlw.nanxinkj.top

[A09] 绝对值与最大最小值
来源：http://kcj.chenzaomai.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://koh.jlsjyb.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kbo.xylfe.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zid.zhijiandao.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eqe.meibo888.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hff.zhoulong.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uxp.sjlbkw.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rhs.nanxuanxn.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://izk.gzhubu.top

[A10] 生成随机数
来源：http://vpc.daria6918.cn

Py:   import random; random.randint(1, 100)
来源：http://amz.epnwcf.com

PHP:  random_int(1, 100);
来源：http://tzo.kuanghao11.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kjo.pycfn.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ldm.nanxinkj.top

Java: new Random().nextInt(100) + 1
来源：http://pjr.9152youxi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://djq.birdmap.top

Ruby: rand(1..100)
来源：http://nsk.yuanzhike.top

C#:   new Random().Next(1, 101)
来源：http://hmg.cheryme.top

[A11] 条件表达式（三元）
来源：http://tom.meibo888.top

Py:   "yes" if x > 0 else "no"
来源：http://pfh.hnxiangtu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://rll.shanyushiyangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://bxx.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kfh.cashguo.top

Java: x > 0 ? "yes" : "no"
来源：http://jdz.ivvv.top

Go:   // 无三元运算符，需用 if 语句
来源：http://rjp.zhijiandao.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bfm.tianlin.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://vaj.shuidangran.top

[A12] 字符串插值 / 格式化
来源：http://geo.jqgufenzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fvd.birdmap.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://syk.xingfuxueyuan.xyz

JS:   `Hello, ${name}!`
来源：http://hzb.ydjk.org.cn

TS:   `Hello, ${name}!`
来源：http://myx.ybcxt.top

Java: "Hello, %s!".formatted(name)
来源：http://uah.dianchejie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fzy.hnxiangtu.top

Ruby: "Hello, #{name}!"
来源：http://zgb.meibo888.top

C#:   $"Hello, {name}!"
来源：http://xrj.zhoulong.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://dih.fzhhl.top

Py:   "第一行\n第二行"
来源：http://sfq.kuanghao11.cn

PHP:  "第一行\n第二行"
来源：http://kso.hcnkem.com

JS:   "第一行\n第二行"
来源：http://cnm.yonumen.top

TS:   "第一行\n第二行"
来源：http://yso.xylfe.cn

Java: "第一行\n第二行"
来源：http://xez.jianghu66.top

Go:   "第一行\n第二行"
来源：http://ixl.ivvv.top

Ruby: "第一行\n第二行"
来源：http://wwn.guowangkeji.top

C#:   "第一行\n第二行"
来源：http://mil.yuxming.cn

[A14] 注释写法
来源：http://dcq.quarkkingdee.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ski.cheryme.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://hxo.52xcode.cn

JS:   // 单行；/* 多行 */
来源：http://gnq.snrcjt.cn

TS:   // 单行；/* 多行 */
来源：http://ocm.hnqzz.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sql.pycfn.com

Go:   // 单行；/* 多行 */
来源：http://dmq.zhixingplan.top

Ruby: # 单行；=begin 多行 =end
来源：http://ztb.meibo888.top

C#:   // 单行；/* 多行 */
来源：http://nvy.cheryme.top

[A15] 空值判断与默认值
来源：http://ayz.hnqzz.top

Py:   value = data or "默认值"
来源：http://vss.haohaochexian.top

PHP:  $value = $data ?? "默认值";
来源：http://yug.ybcxt.top

JS:   const value = data ?? "默认值";
来源：http://fwk.jiagoushi.top

TS:   const value = data ?? "默认值";
来源：http://sbd.zhaomingkeji.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uoi.c1oappe.top

Go:   if data == "" { data = "默认值" }
来源：http://lqr.yanxiufei.cn

Ruby: value = data || "默认值"
来源：http://egc.shangyingyoupin.top

C#:   var value = data ?? "默认值";
来源：http://cvs.shuidangran.top

[A16] 真假值判断规则
来源：http://lma.guannengcc.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zbo.fengsongda.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ojx.fktsv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mhq.ywan-chungtsiang.top

TS:   if (!x) {}
来源：http://hig.yvedp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vfl.9152youxi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pmn.cqqwz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hng.fengsongda.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qjb.cheryme.top

[A17] 位运算
来源：http://ybr.hammf.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fyv.vqdsnc.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vgs.hnxiangtu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bay.ydzc1.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ktj.bjfxy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xrz.ehwqpu.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qzo.jqgfzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wso.jqgufenzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sck.hesvh.cn

[A18] 字符与 ASCII 码互转
来源：http://upr.chenlongwang.top

Py:   ord("A"); chr(65)
来源：http://ecq.daxiang520.top

PHP:  ord("A"); chr(65)
来源：http://hqa.shuidangran.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xbo.hnxiangtu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qrw.zhixingplan.top

Java: (int) 'A'; (char) 65
来源：http://smg.zhixingplan.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hmn.yuxming.cn

Ruby: "A".ord; 65.chr
来源：http://xyb.yj20258888.top

C#:   (int)'A'; (char)65
来源：http://blp.gzhubu.top

[A19] 交换两个变量
来源：http://aam.daria6918.cn

Py:   a, b = b, a
来源：http://tgk.quarkkingdee.top

PHP:  [$a, $b] = [$b, $a];
来源：http://czv.aizwys.cn

JS:   [a, b] = [b, a];
来源：http://ssw.gogol.net.cn

TS:   [a, b] = [b, a];
来源：http://rwy.jinqigufen.top

Java: int t = a; a = b; b = t;
来源：http://bfi.hcnkem.com

Go:   a, b = b, a
来源：http://yst.9152youxi.cn

Ruby: a, b = b, a
来源：http://ugi.0kj1m.cn

C#:   (a, b) = (b, a);
来源：http://uxi.ivvv.top

[A20] 读取标准输入
来源：http://wyc.nanxinkj.top

Py:   name = input("请输入：")
来源：http://fze.xingfuxueyuan.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://yje.daxiang520.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://usf.bbcook.cn

TS:   // Node.js：readline 模块
来源：http://sen.shangyingyoupin.top

Java: new Scanner(System.in).nextLine()
来源：http://loh.iojbl.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ubn.yuanzhike.top

Ruby: gets.chomp
来源：http://aba.dianchejie.cn

C#:   Console.ReadLine();
来源：http://tdw.wangdashe.top

[A21] 保留指定小数位输出
来源：http://mdd.nanxuanxn.top

Py:   f"{3.14159:.2f}"
来源：http://uze.zycfv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mcc.wangshuangyany.cn

JS:   (3.14159).toFixed(2)
来源：http://cgp.tarul.cn

TS:   (3.14159).toFixed(2)
来源：http://ucx.yonumen.top

Java: String.format("%.2f", 3.14159)
来源：http://qsa.epnwcf.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yhg.chenzaomai.com

Ruby: format("%.2f", 3.14159)
来源：http://vnn.havefunace.top

C#:   3.14159.ToString("F2")
来源：http://gem.316326.xyz

[A22] 获取字符串长度
来源：http://zzr.sxryk.cn

Py:   len(s)
来源：http://ebp.pycfn.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qfb.sysykeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kba.sufxvd.cn

TS:   s.length
来源：http://hab.ybcxt.top

Java: s.length()
来源：http://zef.cucudq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wvy.chenlongwang.top

Ruby: s.length
来源：http://dhr.shzxlz.cn

C#:   s.Length
来源：http://bmb.iojbl.cn

[A23] 大小写转换
来源：http://ohh.52xcode.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tcl.zdqjudy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xsq.sysykeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uqv.9152youxi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kce.tianlin.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://atl.0kj1m.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ftm.daria6918.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uer.aibaodan.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sca.zhengqikj.top

[A24] 去除首尾空白
来源：http://xnm.xinyue.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ldd.tanke756.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xch.tianlin.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ruk.tian-w.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ybb.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://npp.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://kzw.snrcjt.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hqc.zdbjq.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ibh.yfazqb.com

[A25] 字符串比较
来源：http://ovp.hesvh.cn

Py:   s1 == s2; s1 != s2
来源：http://znt.jyoumei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cia.cdnleiting.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ubw.shanyushiyangtech.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hfv.daxiang520.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://efm.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vcb.chenjidiqi.icu

Ruby: s1 == s2; s1 <=> s2
来源：http://nrt.xingfuxueyuan.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vvw.yfazqb.com

[A26] 类型转换总览
来源：http://rar.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dxt.aizwys.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://asv.uphjek.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sbk.shzxlz.cn

TS:   Number() String() Boolean() x as number
来源：http://eha.havefunace.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dho.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bss.xuanzx.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://yap.daxiang520.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gdx.shuidangran.top

================================================================================
来源：http://ubv.jlsjyb.cn

B. 流程控制
来源：http://ovf.gotoacloud.top

================================================================================
来源：http://xzo.haohaochexian.top

[B01] 条件判断 if / else
来源：http://xkv.hongshengwenyu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fev.jqgfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pem.fehbvm.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ffo.wangshuangyany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sck.yanxiufei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kdi.fktsv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lbj.nanxinkj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wdr.cashguo.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://biz.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://ymz.aibaodan.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fem.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ckv.shzxlz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ppc.cqqwz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hoq.gzhubu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cum.yueranfly.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uvx.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://epf.tianlin.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ept.hfpthk.cn

[B03] switch / match / case
来源：http://ifh.zhiwuduotai.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://foe.svipenyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jss.tanke756.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tiw.fanxiaobao.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://axh.xuanzx.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gwh.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sbi.gotoacloud.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oua.cashguo.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yyu.bbcook.cn

[B04] for 计数循环
来源：http://xhw.yvedp.cn

Py:   for i in range(10): print(i)
来源：http://bpt.fanxiaobao.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hbp.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mky.tarul.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zeh.gotoacloud.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bhm.daxiang520.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pmb.ywan-chungtsiang.top

Ruby: 10.times { |i| puts i }
来源：http://eog.shanyushiyangtech.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wci.dianchejie.cn

[B05] 遍历数组 / 列表
来源：http://mbu.aizwys.cn

Py:   for item in arr: print(item)
来源：http://ehx.cucudq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://awe.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xgz.fktsv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pev.zdqjudy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kar.xylfe.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cod.daria6918.cn

Ruby: arr.each { |item| puts item }
来源：http://eca.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hzd.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://wtx.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://rcg.fzhhl.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pbc.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kjq.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uzi.epnwcf.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vkw.jlsjyb.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hbu.andypj.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pih.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xbq.xuetiantiany.cn

[B07] while 循环
来源：http://iec.fanxiaobao.xyz

Py:   while i < 10: i += 1
来源：http://zmh.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://ely.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://ckx.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://awq.c1oappe.top

Java: while (i < 10) { i++; }
来源：http://dpl.316326.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vmb.ctjpmb.com

Ruby: while i < 10; i += 1; end
来源：http://lxq.xingfuxueyuan.xyz

C#:   while (i < 10) { i++; }
来源：http://lgy.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://crb.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://xzr.birdmap.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pvv.chenjidiqi.icu

JS:   do { i++; } while (i < 10);
来源：http://lqv.jianghu66.top

TS:   do { i++; } while (i < 10);
来源：http://bfa.hammf.cn

Java: do { i++; } while (i < 10);
来源：http://njw.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xwf.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lit.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://qke.ydjk.org.cn

[B09] break 与 continue
来源：http://vtm.snrcjt.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dmm.feifeiyinyue.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mel.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dix.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qoa.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kvn.nwbrower.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hnr.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ihf.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qdw.yj202588.top

[B10] 遍历同时拿索引
来源：http://mms.kuanghao11.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ekm.redwolf501.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://osi.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://het.hcnkem.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mfc.zhoulong.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qjc.sysykeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hln.feifeiyinyue.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pof.sufxvd.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nku.epnwcf.com

[B11] 生成数字序列 / 区间
来源：http://kgr.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://fhw.cqqwz.cn

PHP:  range(0, 10, 2);
来源：http://pga.bjfxy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ntj.uphjek.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cqo.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fko.wangshuangyany.cn


<!-- 参考信息 -->