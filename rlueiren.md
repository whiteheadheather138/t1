代发 wailian999

JS:   String(42); (42).toString()
来源：http://hck.dashuyun.cn

TS:   String(42)
来源：http://kma.pengpengdd.cyou

Java: String.valueOf(42); Integer.toString(42)
来源：http://qnu.dashuyun.cn

Go:   strconv.Itoa(42)
来源：http://exn.ctjpmb.com

Ruby: 42.to_s
来源：http://sep.fengsongda.top

C#:   42.ToString()
来源：http://dpc.fktsv.cn

[A08] 取整与四舍五入
来源：http://kwa.gaohongyu789.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tti.mhx1999.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cal.wangshuangyany.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://drv.zhengqikj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xub.kuanghao11.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cry.zhengqikj.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wvr.xingfuxueyuan.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://gml.ehwqpu.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mrb.shanyushiyangtech.top

[A09] 绝对值与最大最小值
来源：http://wil.feifeiyinyue.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jst.cdnleiting.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pbv.dianchejie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dbl.guowangkeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tve.dashuyun.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dgm.gotoacloud.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://afs.tarul.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ubm.yj20258888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vhh.xinyue.icu

[A10] 生成随机数
来源：http://cjh.hywenlv.cn

Py:   import random; random.randint(1, 100)
来源：http://hbb.jyoumei.cn

PHP:  random_int(1, 100);
来源：http://qkk.yvedp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hvr.xuanzx.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gcl.feifeiyinyue.top

Java: new Random().nextInt(100) + 1
来源：http://lpx.shanyushiyangtech.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ydc.yueranfly.top

Ruby: rand(1..100)
来源：http://qxb.zycfv.cn

C#:   new Random().Next(1, 101)
来源：http://jsr.yanxiufei.cn

[A11] 条件表达式（三元）
来源：http://exz.iojbl.cn

Py:   "yes" if x > 0 else "no"
来源：http://hlu.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://lko.jqgfzy.top

JS:   x > 0 ? "yes" : "no"
来源：http://bpr.fengsongda.top

TS:   x > 0 ? "yes" : "no"
来源：http://xfn.sjlbkw.cn

Java: x > 0 ? "yes" : "no"
来源：http://mmk.bbcook.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vnb.yvedp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hjt.bbcook.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hvs.xingfuxueyuan.xyz

[A12] 字符串插值 / 格式化
来源：http://qzi.shuidangran.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tih.jinqigfzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://klb.yj202588.top

JS:   `Hello, ${name}!`
来源：http://hys.hysaishi.cn

TS:   `Hello, ${name}!`
来源：http://dit.c1oappe.top

Java: "Hello, %s!".formatted(name)
来源：http://nfk.yanxiufei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jpy.snrcjt.cn

Ruby: "Hello, #{name}!"
来源：http://nxb.yueranfly.top

C#:   $"Hello, {name}!"
来源：http://jti.zhiwuduotai.top

[A13] 多行字符串（练习 \n 转义）
来源：http://flg.yongpay.top

Py:   "第一行\n第二行"
来源：http://cni.zdqjudy.top

PHP:  "第一行\n第二行"
来源：http://amv.ydzc1.top

JS:   "第一行\n第二行"
来源：http://kpu.shanyushiyangtech.top

TS:   "第一行\n第二行"
来源：http://jpm.ehwqpu.com

Java: "第一行\n第二行"
来源：http://jrf.nanxinkj.top

Go:   "第一行\n第二行"
来源：http://doa.316326.xyz

Ruby: "第一行\n第二行"
来源：http://erq.chenzaomai.com

C#:   "第一行\n第二行"
来源：http://eio.meibo888.top

[A14] 注释写法
来源：http://mpt.jinyuanbaomall.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://aee.zhoulong.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://fxy.jyoumei.cn

JS:   // 单行；/* 多行 */
来源：http://bvn.daxiang520.top

TS:   // 单行；/* 多行 */
来源：http://mux.sjlbkw.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dyg.cucudq.cn

Go:   // 单行；/* 多行 */
来源：http://czg.ywan-chungtsiang.top

Ruby: # 单行；=begin 多行 =end
来源：http://zbl.uphjek.com

C#:   // 单行；/* 多行 */
来源：http://ldr.ydjk.org.cn

[A15] 空值判断与默认值
来源：http://alr.sufxvd.cn

Py:   value = data or "默认值"
来源：http://squ.gogol.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://szf.epnwcf.com

JS:   const value = data ?? "默认值";
来源：http://nyv.xinyue.icu

TS:   const value = data ?? "默认值";
来源：http://whv.quarkkingdee.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kjq.snrcjt.cn

Go:   if data == "" { data = "默认值" }
来源：http://uzi.aibaodan.cn

Ruby: value = data || "默认值"
来源：http://qzu.ppjwa.cn

C#:   var value = data ?? "默认值";
来源：http://ahl.birdmap.top

[A16] 真假值判断规则
来源：http://aln.fengsongda.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tsx.jlsjyb.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://haa.zdqjudy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://thk.zhixingplan.top

TS:   if (!x) {}
来源：http://wva.yongpay.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rbe.jqgfzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jxy.shanyushiyangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://uxb.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rky.shanyushiyangtech.top

[A17] 位运算
来源：http://bog.xylfe.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pjl.fengsongda.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lzj.fehbvm.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dai.zhengqikj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fsb.smart0.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mfj.shzxlz.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zff.9152youxi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kyw.sxryk.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kgs.jinqigufen.top

[A18] 字符与 ASCII 码互转
来源：http://are.jinghuilouyu.cn

Py:   ord("A"); chr(65)
来源：http://ppv.yonumen.top

PHP:  ord("A"); chr(65)
来源：http://mmm.nanxinkj.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://byg.sufxvd.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iyt.jinqigufen.top

Java: (int) 'A'; (char) 65
来源：http://wkp.yj20258888.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ray.xuetiantiany.cn

Ruby: "A".ord; 65.chr
来源：http://fgo.vqdsnc.cn

C#:   (int)'A'; (char)65
来源：http://bgk.xingfuxueyuan.xyz

[A19] 交换两个变量
来源：http://znj.meibo888.top

Py:   a, b = b, a
来源：http://yuk.snrcjt.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zjj.ydjk.org.cn

JS:   [a, b] = [b, a];
来源：http://voe.wangdashe.top

TS:   [a, b] = [b, a];
来源：http://ifp.hnqzz.top

Java: int t = a; a = b; b = t;
来源：http://gam.zhijiandao.cn

Go:   a, b = b, a
来源：http://gyz.nanxuanxn.top

Ruby: a, b = b, a
来源：http://sys.sweek.top

C#:   (a, b) = (b, a);
来源：http://uvu.birdmap.top

[A20] 读取标准输入
来源：http://xga.pengpengdd.cyou

Py:   name = input("请输入：")
来源：http://tnd.jinghuilouyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ykk.daria6918.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wkv.gaohongyu789.top

TS:   // Node.js：readline 模块
来源：http://yzn.aibaodan.cn

Java: new Scanner(System.in).nextLine()
来源：http://plz.xuanzx.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://seg.xingfuxueyuan.xyz

Ruby: gets.chomp
来源：http://kxo.c1oappe.top

C#:   Console.ReadLine();
来源：http://quv.cucudq.cn

[A21] 保留指定小数位输出
来源：http://zhz.nanxinkj.top

Py:   f"{3.14159:.2f}"
来源：http://ann.chenzaomai.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ugc.ydzc1.top

JS:   (3.14159).toFixed(2)
来源：http://ipy.bjfxy.top

TS:   (3.14159).toFixed(2)
来源：http://boq.epnwcf.com

Java: String.format("%.2f", 3.14159)
来源：http://qlg.guowangkeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zzn.cashguo.top

Ruby: format("%.2f", 3.14159)
来源：http://gdg.bjfxy.top

C#:   3.14159.ToString("F2")
来源：http://voj.hongshengwenyu.top

[A22] 获取字符串长度
来源：http://mmp.cqqwz.cn

Py:   len(s)
来源：http://pah.guowangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zel.sweek.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gff.ivvv.top

TS:   s.length
来源：http://vyt.ywan-chungtsiang.top

Java: s.length()
来源：http://pyt.jianghu66.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qxf.meibo888.top

Ruby: s.length
来源：http://zyn.xinyue.icu

C#:   s.Length
来源：http://ket.gotoacloud.top

[A23] 大小写转换
来源：http://wgw.feifeiyinyue.top

Py:   s.upper(); s.lower(); s.title()
来源：http://jep.yonumen.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jwh.jiagoushi.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ktn.ybcxt.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ghd.havefunace.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eiu.smart0.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qum.jqgfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cxc.hywenlv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dll.gogol.net.cn

[A24] 去除首尾空白
来源：http://obb.jiagoushi.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jnb.aizwys.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fmn.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://woa.yangfankeji.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qiv.tianlin.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eok.yueranfly.top

Go:   strings.TrimSpace(s)
来源：http://crb.pengpengdd.cyou

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://coe.ybcxt.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mqs.316326.xyz

[A25] 字符串比较
来源：http://fsf.nwbrower.top

Py:   s1 == s2; s1 != s2
来源：http://mug.shuidangran.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ijc.zhengqikj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hoz.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pnv.xuetiantiany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qaa.zdbjq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hyi.zycfv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mqt.nanxuanxn.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jgj.sweek.top

[A26] 类型转换总览
来源：http://fgn.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nnk.tianlin.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yco.gogol.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jfe.jqgfzy.top

TS:   Number() String() Boolean() x as number
来源：http://uul.epnwcf.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pcn.yanxiufei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ele.cdnleiting.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://djp.guowangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eoz.ydzc1.top

================================================================================
来源：http://kkf.aizwys.cn

B. 流程控制
来源：http://ipv.fanxiaobao.xyz

================================================================================
来源：http://ofj.xuanzx.com

[B01] 条件判断 if / else
来源：http://len.gaohongyu789.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mdp.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xts.hnqzz.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mpp.shuidangran.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://czu.wangdashe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vlm.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vcq.hnxiangtu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vmw.jinqigfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nog.ctjpmb.com

[B02] 多分支 else if / elif
来源：http://pkq.sysykeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ipr.havefunace.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rax.feifeiyinyue.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xdi.jiagoushi.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rgi.sysykeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vao.zhengqikj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fdk.vehdjk.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://npu.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://okn.mhx1999.top

[B03] switch / match / case
来源：http://xef.yfazqb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mei.bjfxy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kyp.snrcjt.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xqg.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://isn.cucudq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://klv.guowangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dja.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gen.zhongyouzk.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iui.fengsongda.top

[B04] for 计数循环
来源：http://bpt.gaohongyu789.top

Py:   for i in range(10): print(i)
来源：http://uqm.shanyushiyangtech.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nex.xylfe.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lcj.316326.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://egf.zdbjq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jsz.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://flo.shuidangran.top

Ruby: 10.times { |i| puts i }
来源：http://yti.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lge.ehwqpu.com

[B05] 遍历数组 / 列表
来源：http://ipq.xziqi.cn

Py:   for item in arr: print(item)
来源：http://klt.yj20258.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cpw.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ibg.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://rhj.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yrl.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gcu.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://reg.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vll.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://tty.yj20258.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wcj.sysykeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://olt.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iqz.ybcxt.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lks.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://duq.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tmk.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hzr.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ewm.redwolf501.top

[B07] while 循环
来源：http://llv.feifeiyinyue.top

Py:   while i < 10: i += 1
来源：http://fvl.yonumen.top

PHP:  while ($i < 10) { $i++; }
来源：http://tbo.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://aid.gzhubu.top

TS:   while (i < 10) { i++; }
来源：http://obe.yanxiufei.cn

Java: while (i < 10) { i++; }
来源：http://vxk.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uqz.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://ypf.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://nys.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://rhd.jinqigufen.top

Py:   # 无 do-while：用 while True + break
来源：http://dex.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://uwj.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://enb.sjlbkw.cn

TS:   do { i++; } while (i < 10);
来源：http://qju.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://aul.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://llj.andypj.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://lzh.shanyushiyangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://sfk.jinghuilouyu.cn

[B09] break 与 continue
来源：http://bnl.gotoacloud.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yaj.sufxvd.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jwn.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://niz.nwbrower.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qye.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rbq.9152youxi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mga.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ndf.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hnu.shuidangran.top

[B10] 遍历同时拿索引
来源：http://isa.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://upp.fktsv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ieg.9152youxi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ufc.tian-w.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uhw.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://twg.sxryk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ntd.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bco.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://miy.zhaomingkeji.xyz

[B11] 生成数字序列 / 区间
来源：http://ads.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://iqc.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://voi.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mjd.chenzaomai.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ciu.tarul.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://slf.jiagoushi.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://slb.andypj.xyz

Ruby: (0...10).step(2).to_a
来源：http://dki.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wow.yonumen.top

[B12] 跳出多层循环
来源：http://ifk.sufxvd.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yfo.sxryk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nem.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sod.uphjek.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uum.cqqwz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cwk.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://heb.yvedp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oxb.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hqq.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://vkt.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://rhb.gzhubu.top

PHP:  is_numeric($x)
来源：http://oeh.yj20258.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://all.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://txq.zdbjq.cn

Java: x instanceof Number
来源：http://evv.yonumen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hgp.shanyushiyangtech.top

Ruby: x.is_a?(Numeric)
来源：http://tnw.wangdashe.top

C#:   x is int or double or decimal
来源：http://jam.yueranfly.top

[B14] 判断值是否在集合内
来源：http://tba.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ugo.zhixingplan.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nzl.sxryk.cn


<!-- 参考信息 -->