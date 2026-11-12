代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lyw.uphjek.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://nth.gogol.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vhm.sysykeji.top

[A09] 绝对值与最大最小值
来源：http://bkl.ctjpmb.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wrq.dianchejie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kwb.fanxiaobao.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dcx.zhengqikj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ctf.tian-w.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sop.nwbrower.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wfh.xingfuxueyuan.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kin.c1oappe.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ifw.316326.xyz

[A10] 生成随机数
来源：http://jmj.tian-w.cn

Py:   import random; random.randint(1, 100)
来源：http://rbk.zhengqikj.top

PHP:  random_int(1, 100);
来源：http://rdy.birdmap.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rib.chenlongwang.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tlg.chenzaomai.com

Java: new Random().nextInt(100) + 1
来源：http://dhv.shuidangran.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vei.aizwys.cn

Ruby: rand(1..100)
来源：http://rmd.tian-w.cn

C#:   new Random().Next(1, 101)
来源：http://vkt.gzhubu.top

[A11] 条件表达式（三元）
来源：http://hzz.cashguo.top

Py:   "yes" if x > 0 else "no"
来源：http://npi.cucudq.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jqe.dianchejie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://myl.ywan-chungtsiang.top

TS:   x > 0 ? "yes" : "no"
来源：http://xjp.ydjk.org.cn

Java: x > 0 ? "yes" : "no"
来源：http://fha.c1oappe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qzj.ywan-chungtsiang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://swt.iojbl.cn

C#:   x > 0 ? "yes" : "no"
来源：http://iie.ctjpmb.com

[A12] 字符串插值 / 格式化
来源：http://trf.yj20258.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jvv.hywenlv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tgy.iojbl.cn

JS:   `Hello, ${name}!`
来源：http://ydn.fengsongda.top

TS:   `Hello, ${name}!`
来源：http://zbc.nwbrower.top

Java: "Hello, %s!".formatted(name)
来源：http://dzr.sxryk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kih.sxryk.cn

Ruby: "Hello, #{name}!"
来源：http://zfx.gzhubu.top

C#:   $"Hello, {name}!"
来源：http://dox.cdnleiting.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lzp.xingfuxueyuan.xyz

Py:   "第一行\n第二行"
来源：http://kdu.yvedp.cn

PHP:  "第一行\n第二行"
来源：http://kmg.cheryme.top

JS:   "第一行\n第二行"
来源：http://djb.ywan-chungtsiang.top

TS:   "第一行\n第二行"
来源：http://nas.jinqigufen.top

Java: "第一行\n第二行"
来源：http://jzi.yfazqb.com

Go:   "第一行\n第二行"
来源：http://fgn.vqdsnc.cn

Ruby: "第一行\n第二行"
来源：http://tjs.chenjidiqi.icu

C#:   "第一行\n第二行"
来源：http://pni.nanxinkj.top

[A14] 注释写法
来源：http://stt.sweek.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ufp.jinghuilouyu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mid.yuxming.cn

JS:   // 单行；/* 多行 */
来源：http://bkn.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://mlz.guannengcc.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vrg.52xcode.cn

Go:   // 单行；/* 多行 */
来源：http://jba.xuetiantiany.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dom.haohaochexian.top

C#:   // 单行；/* 多行 */
来源：http://yyh.cucudq.cn

[A15] 空值判断与默认值
来源：http://foy.yj20258888.top

Py:   value = data or "默认值"
来源：http://jbq.uphjek.com

PHP:  $value = $data ?? "默认值";
来源：http://jsz.zhoulong.xyz

JS:   const value = data ?? "默认值";
来源：http://uxz.wangshuangyany.cn

TS:   const value = data ?? "默认值";
来源：http://mzv.52xcode.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rjq.mhx1999.top

Go:   if data == "" { data = "默认值" }
来源：http://qmh.9152youxi.cn

Ruby: value = data || "默认值"
来源：http://wwk.cucudq.cn

C#:   var value = data ?? "默认值";
来源：http://puj.guowangkeji.top

[A16] 真假值判断规则
来源：http://vdb.bjfxy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ghb.c1oappe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://foz.aibaodan.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zvh.jyoumei.cn

TS:   if (!x) {}
来源：http://zew.hammf.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wpd.vehdjk.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ivj.sufxvd.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uzg.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://exx.zhengqikj.top

[A17] 位运算
来源：http://vnt.jlsjyb.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yko.ybcxt.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ocl.quarkkingdee.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kth.uphjek.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kqa.nanxuanxn.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://quh.snrcjt.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hem.gzhubu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xyb.nanxuanxn.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://axh.fzhhl.top

[A18] 字符与 ASCII 码互转
来源：http://kzc.yj20258.top

Py:   ord("A"); chr(65)
来源：http://ayr.chenjidiqi.icu

PHP:  ord("A"); chr(65)
来源：http://dro.wangshuangyany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fbk.hnxiangtu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://srf.jinyuanbaomall.cn

Java: (int) 'A'; (char) 65
来源：http://rwz.jlsjyb.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bim.316326.xyz

Ruby: "A".ord; 65.chr
来源：http://ink.snrcjt.cn

C#:   (int)'A'; (char)65
来源：http://laq.hnxiangtu.top

[A19] 交换两个变量
来源：http://bfa.tian-w.cn

Py:   a, b = b, a
来源：http://mbk.hnqzz.top

PHP:  [$a, $b] = [$b, $a];
来源：http://uwz.c1oappe.top

JS:   [a, b] = [b, a];
来源：http://yqn.fengsongda.top

TS:   [a, b] = [b, a];
来源：http://kko.zdbjq.cn

Java: int t = a; a = b; b = t;
来源：http://pxv.hysaishi.cn

Go:   a, b = b, a
来源：http://mmb.hongshengwenyu.top

Ruby: a, b = b, a
来源：http://yri.yvedp.cn

C#:   (a, b) = (b, a);
来源：http://wfi.gzhubu.top

[A20] 读取标准输入
来源：http://cls.dianchejie.cn

Py:   name = input("请输入：")
来源：http://vqm.ppjwa.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fkz.gaohongyu789.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wdy.tianlin.xyz

TS:   // Node.js：readline 模块
来源：http://jxd.shanyushiyangtech.top

Java: new Scanner(System.in).nextLine()
来源：http://eoe.snrcjt.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://oif.snrcjt.cn

Ruby: gets.chomp
来源：http://znt.xziqi.cn

C#:   Console.ReadLine();
来源：http://agz.pycfn.com

[A21] 保留指定小数位输出
来源：http://egs.yj20258888.top

Py:   f"{3.14159:.2f}"
来源：http://tad.gaohongyu789.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fxf.cqqwz.cn

JS:   (3.14159).toFixed(2)
来源：http://zxq.chenlongwang.top

TS:   (3.14159).toFixed(2)
来源：http://fbh.cashguo.top

Java: String.format("%.2f", 3.14159)
来源：http://idi.gogol.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hea.zhixingplan.top

Ruby: format("%.2f", 3.14159)
来源：http://pmt.fzhhl.top

C#:   3.14159.ToString("F2")
来源：http://otb.hnxiangtu.top

[A22] 获取字符串长度
来源：http://vxu.hongshengwenyu.top

Py:   len(s)
来源：http://unr.guowangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gwd.shuidangran.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rrq.tanke756.top

TS:   s.length
来源：http://wge.xuanzx.com

Java: s.length()
来源：http://mhh.daria6918.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qew.zdqjudy.top

Ruby: s.length
来源：http://hnp.yfazqb.com

C#:   s.Length
来源：http://xut.jyoumei.cn

[A23] 大小写转换
来源：http://jjg.ctjpmb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://tty.shzxlz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rfq.quarkkingdee.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vst.chenlongwang.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lqp.ywan-chungtsiang.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jej.birdmap.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bst.yj202588.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dni.sweek.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lww.shanyushiyangkeji.top

[A24] 去除首尾空白
来源：http://gud.fanxiaobao.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rlb.ydjk.org.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wvd.fanxiaobao.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xzi.hysaishi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yod.fzhhl.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yvk.shzxlz.cn

Go:   strings.TrimSpace(s)
来源：http://xbl.sufxvd.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hqs.shzxlz.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uef.nanxinkj.top

[A25] 字符串比较
来源：http://ezr.jqgfzy.top

Py:   s1 == s2; s1 != s2
来源：http://xyk.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rah.jiagoushi.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ptx.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://skc.sjlbkw.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nsy.aizwys.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://van.aizwys.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fyr.guannengcc.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://usy.dianchejie.cn

[A26] 类型转换总览
来源：http://unj.yvedp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xbz.quarkkingdee.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iuv.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wuv.hysaishi.cn

TS:   Number() String() Boolean() x as number
来源：http://uzu.0kj1m.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hxx.yuxming.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pxb.ppjwa.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cvd.ppjwa.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qbl.feifeiyinyue.top

================================================================================
来源：http://iqa.yj202588.top

B. 流程控制
来源：http://gdv.xingfuxueyuan.xyz

================================================================================
来源：http://glm.ppjwa.cn

[B01] 条件判断 if / else
来源：http://xhl.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uux.zhixingplan.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ejf.fehbvm.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ijx.nanxinkj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nts.wangdashe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xax.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jqa.havefunace.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wjy.xuetiantiany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jxn.sysykeji.top

[B02] 多分支 else if / elif
来源：http://wuo.yanxiufei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://upj.havefunace.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vdb.meibo888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dsp.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pki.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ykt.jqgufenzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ksv.ppjwa.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bez.yj20258.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://opt.ctjpmb.com

[B03] switch / match / case
来源：http://ojt.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://llc.jlsjyb.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rvv.shanyushiyangtech.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hbf.mhx1999.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://soy.haohaochexian.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kcl.meibo888.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qyy.sjlbkw.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fji.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ibq.quarkkingdee.top

[B04] for 计数循环
来源：http://epm.shanyushiyangkeji.top

Py:   for i in range(10): print(i)
来源：http://zmn.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jif.yuxming.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bjt.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nfa.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://whq.xuetiantiany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dyx.vehdjk.com

Ruby: 10.times { |i| puts i }
来源：http://slj.zhiwuduotai.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rax.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://yeb.zhengqikj.top

Py:   for item in arr: print(item)
来源：http://zuf.hywenlv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tqf.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://htv.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jlp.epnwcf.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mlo.quarkkingdee.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zqf.cheryme.top

Ruby: arr.each { |item| puts item }
来源：http://rni.jlsjyb.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fps.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://qhe.tarul.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jdy.316326.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vpg.shzxlz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://puc.tarul.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jme.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hui.sufxvd.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ozz.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pse.ehwqpu.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rxd.yj20258888.top

[B07] while 循环
来源：http://ffv.bjfxy.top

Py:   while i < 10: i += 1
来源：http://nsg.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://bqy.gzhubu.top

JS:   while (i < 10) { i++; }
来源：http://pyz.zhengqikj.top

TS:   while (i < 10) { i++; }
来源：http://doz.kuanghao11.cn

Java: while (i < 10) { i++; }
来源：http://ewp.9152youxi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rxp.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://nje.fengsongda.top

C#:   while (i < 10) { i++; }
来源：http://kre.hnqzz.top

[B08] do-while（至少执行一次）
来源：http://ukt.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://cwx.jlsjyb.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fap.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://coh.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://ncw.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://csq.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://rtk.daxiang520.top

Ruby: begin; i += 1; end while i < 10
来源：http://vab.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://ret.yongpay.top

[B09] break 与 continue
来源：http://drn.cheryme.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://coc.epnwcf.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rqv.sjlbkw.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbn.chenzaomai.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gap.shanyushiyangtech.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dpj.gaohongyu789.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wys.zhaomingkeji.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fvr.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qwm.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://dbg.dashuyun.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iyh.yfazqb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mvb.birdmap.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qpx.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vxk.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dxt.cheryme.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dni.yj202588.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pzb.sysykeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dxv.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://ppz.yangfankeji.com

Py:   list(range(0, 10, 2))
来源：http://igf.bjfxy.top

PHP:  range(0, 10, 2);
来源：http://pnj.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nzk.xingfuxueyuan.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pnw.ppjwa.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://orf.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kvn.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://dfq.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vlp.gogol.net.cn

[B12] 跳出多层循环
来源：http://zjo.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yqy.svipenyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://quo.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sgg.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xya.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bzo.hongshengwenyu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nas.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sdb.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ksd.316326.xyz

[B13] 判断是否为数字
来源：http://zzq.andypj.xyz

Py:   isinstance(x, (int, float))
来源：http://bqo.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://niz.yongpay.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://beb.316326.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gkd.yj20258.top

Java: x instanceof Number
来源：http://vam.guowangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jcx.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://uwd.fktsv.cn

C#:   x is int or double or decimal
来源：http://gyz.316326.xyz

[B14] 判断值是否在集合内
来源：http://jaj.redwolf501.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cga.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ebp.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://qdc.sysykeji.top

TS:   [1, 2, 3].includes(x)
来源：http://yyk.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jtw.gaohongyu789.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cod.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://xmg.hywenlv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://igp.hysaishi.cn

[B15] 布尔运算与取反
来源：http://nwg.quarkkingdee.top

Py:   a and b or not c
来源：http://wck.guannengcc.top

PHP:  $a && $b || !$c
来源：http://rdl.daxiang520.top

JS:   a && b || !c
来源：http://ejl.hysaishi.cn

TS:   a && b || !c
来源：http://ubi.nanxinkj.top

Java: a && b || !c
来源：http://ykv.kuanghao11.cn


<!-- 参考信息 -->