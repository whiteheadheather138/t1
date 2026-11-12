代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xdc.shangyingyoupin.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ads.tian-w.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vhc.shangyingyoupin.top

[A09] 绝对值与最大最小值
来源：http://lns.zdqjudy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zdo.shanyushiyangkeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://clm.yj202588.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hqj.shzxlz.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://aeo.tianlin.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cnj.shanyushiyangkeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mgy.vqdsnc.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vcf.sjlbkw.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zek.xuanzx.com

[A10] 生成随机数
来源：http://izc.vqdsnc.cn

Py:   import random; random.randint(1, 100)
来源：http://sfu.zdbjq.cn

PHP:  random_int(1, 100);
来源：http://clr.uphjek.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kwf.ehwqpu.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uyu.yongpay.top

Java: new Random().nextInt(100) + 1
来源：http://bwz.cqqwz.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xjd.wangshuangyany.cn

Ruby: rand(1..100)
来源：http://jvt.sxryk.cn

C#:   new Random().Next(1, 101)
来源：http://gxd.cucudq.cn

[A11] 条件表达式（三元）
来源：http://sch.yonumen.top

Py:   "yes" if x > 0 else "no"
来源：http://sqp.fktsv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kzp.gzhubu.top

JS:   x > 0 ? "yes" : "no"
来源：http://waw.birdmap.top

TS:   x > 0 ? "yes" : "no"
来源：http://opm.svipenyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://mkb.feifeiyinyue.top

Go:   // 无三元运算符，需用 if 语句
来源：http://zqn.yj202588.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ras.xuetiantiany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mdg.tarul.cn

[A12] 字符串插值 / 格式化
来源：http://wza.chenzaomai.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jnb.mhx1999.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://txz.bbcook.cn

JS:   `Hello, ${name}!`
来源：http://npb.zhaomingkeji.xyz

TS:   `Hello, ${name}!`
来源：http://rkp.wangdashe.top

Java: "Hello, %s!".formatted(name)
来源：http://fmb.dashuyun.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://amb.bbcook.cn

Ruby: "Hello, #{name}!"
来源：http://bqx.yongpay.top

C#:   $"Hello, {name}!"
来源：http://rnm.0kj1m.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bvh.ehwqpu.com

Py:   "第一行\n第二行"
来源：http://ovz.yvedp.cn

PHP:  "第一行\n第二行"
来源：http://gro.yangfankeji.com

JS:   "第一行\n第二行"
来源：http://xwv.pengpengdd.cyou

TS:   "第一行\n第二行"
来源：http://uko.shzxlz.cn

Java: "第一行\n第二行"
来源：http://nze.hongshengwenyu.top

Go:   "第一行\n第二行"
来源：http://kbj.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://uos.jinghuilouyu.cn

C#:   "第一行\n第二行"
来源：http://ikk.aizwys.cn

[A14] 注释写法
来源：http://vvn.tarul.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://azc.cqqwz.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dub.hcnkem.com

JS:   // 单行；/* 多行 */
来源：http://iss.daxiang520.top

TS:   // 单行；/* 多行 */
来源：http://fkj.zycfv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://poo.hfpthk.cn

Go:   // 单行；/* 多行 */
来源：http://vrh.quarkkingdee.top

Ruby: # 单行；=begin 多行 =end
来源：http://zwf.ivvv.top

C#:   // 单行；/* 多行 */
来源：http://oie.shangyingyoupin.top

[A15] 空值判断与默认值
来源：http://gwj.hnqzz.top

Py:   value = data or "默认值"
来源：http://qel.9152youxi.cn

PHP:  $value = $data ?? "默认值";
来源：http://ptf.tianlin.xyz

JS:   const value = data ?? "默认值";
来源：http://cno.hcnkem.com

TS:   const value = data ?? "默认值";
来源：http://lfk.yueranfly.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xlo.jqgufenzy.top

Go:   if data == "" { data = "默认值" }
来源：http://txa.fanxiaobao.xyz

Ruby: value = data || "默认值"
来源：http://hnt.svipenyu.cn

C#:   var value = data ?? "默认值";
来源：http://yfo.feifeiyinyue.top

[A16] 真假值判断规则
来源：http://mqr.zhiwuduotai.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yba.jinqigufen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kws.ehwqpu.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sxn.jinghuilouyu.cn

TS:   if (!x) {}
来源：http://ndd.ydjk.org.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uts.jinyuanbaomall.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hvi.snrcjt.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kws.aibaodan.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://job.xziqi.cn

[A17] 位运算
来源：http://myu.pycfn.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dzb.bbcook.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ecx.cashguo.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://znd.sjlbkw.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ewv.mhx1999.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kwa.ywan-chungtsiang.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pzw.pycfn.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zyk.jianghu66.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yra.feifeiyinyue.top

[A18] 字符与 ASCII 码互转
来源：http://ggk.yanxiufei.cn

Py:   ord("A"); chr(65)
来源：http://mbu.jinyuanbaomall.cn

PHP:  ord("A"); chr(65)
来源：http://xbq.chenjidiqi.icu

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cfd.xuanzx.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cze.daxiang520.top

Java: (int) 'A'; (char) 65
来源：http://nys.zdqjudy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xwi.feifeiyinyue.top

Ruby: "A".ord; 65.chr
来源：http://lpw.sweek.top

C#:   (int)'A'; (char)65
来源：http://jnq.fehbvm.com

[A19] 交换两个变量
来源：http://zpv.xuanzx.com

Py:   a, b = b, a
来源：http://nzd.yuxming.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pin.yj20258.top

JS:   [a, b] = [b, a];
来源：http://efk.chenlongwang.top

TS:   [a, b] = [b, a];
来源：http://ake.sweek.top

Java: int t = a; a = b; b = t;
来源：http://cfc.daria6918.cn

Go:   a, b = b, a
来源：http://hwt.hammf.cn

Ruby: a, b = b, a
来源：http://ecx.zhaomingkeji.xyz

C#:   (a, b) = (b, a);
来源：http://mqx.jinqigufen.top

[A20] 读取标准输入
来源：http://qug.ehwqpu.com

Py:   name = input("请输入：")
来源：http://rje.shanyushiyangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://euk.ctjpmb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dem.0kj1m.cn

TS:   // Node.js：readline 模块
来源：http://ywt.sysykeji.top

Java: new Scanner(System.in).nextLine()
来源：http://bbt.hnxiangtu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jkb.cucudq.cn

Ruby: gets.chomp
来源：http://xto.yanxiufei.cn

C#:   Console.ReadLine();
来源：http://amj.jinqigfzy.top

[A21] 保留指定小数位输出
来源：http://xrt.gaohongyu789.top

Py:   f"{3.14159:.2f}"
来源：http://wcs.mhx1999.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gzq.sysykeji.top

JS:   (3.14159).toFixed(2)
来源：http://iuh.yj20258.top

TS:   (3.14159).toFixed(2)
来源：http://fhy.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://vrw.xuetiantiany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lun.snrcjt.cn

Ruby: format("%.2f", 3.14159)
来源：http://xae.jianghu66.top

C#:   3.14159.ToString("F2")
来源：http://yyd.shangyingyoupin.top

[A22] 获取字符串长度
来源：http://zbt.tianlin.xyz

Py:   len(s)
来源：http://bxy.vqdsnc.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ugh.vqdsnc.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aql.yuxming.cn

TS:   s.length
来源：http://bon.havefunace.top

Java: s.length()
来源：http://jvu.hnxiangtu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://haa.zhaomingkeji.xyz

Ruby: s.length
来源：http://aex.zdbjq.cn

C#:   s.Length
来源：http://yls.sxryk.cn

[A23] 大小写转换
来源：http://cnm.redwolf501.top

Py:   s.upper(); s.lower(); s.title()
来源：http://het.vehdjk.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://whi.guowangkeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gsu.nwbrower.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kjg.sweek.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qcg.iojbl.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wxe.ywan-chungtsiang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ogj.yangfankeji.com

C#:   s.ToUpper(); s.ToLower()
来源：http://jyn.shanyushiyangtech.top

[A24] 去除首尾空白
来源：http://xcd.jianghu66.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://num.tanke756.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://guk.shzxlz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vpo.hnxiangtu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://phy.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dci.hammf.cn

Go:   strings.TrimSpace(s)
来源：http://lii.fanxiaobao.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pql.wangdashe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yje.shangyingyoupin.top

[A25] 字符串比较
来源：http://cry.gaohongyu789.top

Py:   s1 == s2; s1 != s2
来源：http://asi.jinghuilouyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sfl.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vsp.shangyingyoupin.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ail.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tnw.xziqi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tsz.shuidangran.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kne.hongshengwenyu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jud.jlsjyb.cn

[A26] 类型转换总览
来源：http://fjo.quarkkingdee.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jto.zhiwuduotai.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ztr.chenzaomai.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wfh.jinqigfzy.top

TS:   Number() String() Boolean() x as number
来源：http://lpe.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://acb.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rdu.yj20258.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kgf.tianlin.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://upt.nanxinkj.top

================================================================================
来源：http://wii.hcnkem.com

B. 流程控制
来源：http://omd.jinghuilouyu.cn

================================================================================
来源：http://coh.bjfxy.top

[B01] 条件判断 if / else
来源：http://ysp.tian-w.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vah.jinqigfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cev.nanxinkj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dqe.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wfv.yj20258.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mso.yj20258888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tmf.yj202588.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pai.yj202588.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bku.yfazqb.com

[B02] 多分支 else if / elif
来源：http://vdj.ctjpmb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sve.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hfs.kuanghao11.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ehf.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ijq.andypj.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxc.nwbrower.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gvh.guannengcc.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rrh.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ehm.wangdashe.top

[B03] switch / match / case
来源：http://wyy.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://igw.jyoumei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://auf.ydjk.org.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gpt.hfpthk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://txa.xingfuxueyuan.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iyw.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vqm.chenjidiqi.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yxt.hcnkem.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jds.gogol.net.cn

[B04] for 计数循环
来源：http://qff.zhaomingkeji.xyz

Py:   for i in range(10): print(i)
来源：http://nrm.yanxiufei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://svu.zhiwuduotai.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qze.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qim.hammf.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zih.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sln.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://bmq.guowangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lyt.xuanzx.com

[B05] 遍历数组 / 列表
来源：http://agy.zdbjq.cn

Py:   for item in arr: print(item)
来源：http://vpb.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xsv.bbcook.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vpc.hammf.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gjl.fengsongda.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zoi.chenzaomai.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lpq.hfpthk.cn

Ruby: arr.each { |item| puts item }
来源：http://mdy.sufxvd.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wwv.xuanzx.com

[B06] 遍历字典 / 对象
来源：http://vsd.ydjk.org.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kcm.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sxp.hywenlv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ecw.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tdt.yangfankeji.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kez.jiagoushi.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mog.fzhhl.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vlc.ppjwa.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tea.shuidangran.top

[B07] while 循环
来源：http://php.fanxiaobao.xyz

Py:   while i < 10: i += 1
来源：http://tzm.cheryme.top

PHP:  while ($i < 10) { $i++; }
来源：http://ftz.wangdashe.top

JS:   while (i < 10) { i++; }
来源：http://lhx.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://ugj.feifeiyinyue.top

Java: while (i < 10) { i++; }
来源：http://skn.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oqw.316326.xyz

Ruby: while i < 10; i += 1; end
来源：http://irc.ehwqpu.com

C#:   while (i < 10) { i++; }
来源：http://bkr.ydjk.org.cn

[B08] do-while（至少执行一次）
来源：http://rzl.shanyushiyangtech.top

Py:   # 无 do-while：用 while True + break
来源：http://xrx.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pem.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://dwi.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://ije.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://fnr.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zpw.iojbl.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fdy.xuanzx.com

C#:   do { i++; } while (i < 10);
来源：http://uqt.yonumen.top

[B09] break 与 continue
来源：http://zpd.cdnleiting.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mts.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ybr.gzhubu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uvo.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bky.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ycx.zycfv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pna.fehbvm.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ace.gzhubu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cpo.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://byy.gotoacloud.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zxt.ppjwa.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ubr.ybcxt.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://osd.zycfv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ula.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tke.sufxvd.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://idm.0kj1m.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tal.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lul.mhx1999.top

[B11] 生成数字序列 / 区间
来源：http://qem.feifeiyinyue.top

Py:   list(range(0, 10, 2))
来源：http://dfo.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://yys.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vsl.zhiwuduotai.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bwf.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ywl.yueranfly.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tlm.ydzc1.top

Ruby: (0...10).step(2).to_a
来源：http://wmy.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ryi.9152youxi.cn

[B12] 跳出多层循环
来源：http://fdb.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://esi.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cvs.jinghuilouyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://byk.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wjt.fzhhl.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kjf.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kuy.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ita.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qgf.daxiang520.top

[B13] 判断是否为数字
来源：http://dqj.hesvh.cn

Py:   isinstance(x, (int, float))
来源：http://llt.tanke756.top

PHP:  is_numeric($x)
来源：http://xjs.tarul.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zzz.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zml.yvedp.cn

Java: x instanceof Number
来源：http://djn.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hcb.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://qot.aizwys.cn

C#:   x is int or double or decimal
来源：http://efe.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://rly.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pvi.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ffp.iojbl.cn

JS:   [1, 2, 3].includes(x)
来源：http://iac.zhongyouzk.top

TS:   [1, 2, 3].includes(x)
来源：http://ljz.wangdashe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hlu.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xnx.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://hnc.shanyushiyangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tay.dianchejie.cn

[B15] 布尔运算与取反
来源：http://sab.smart0.xyz

Py:   a and b or not c
来源：http://ouv.zycfv.cn

PHP:  $a && $b || !$c
来源：http://puu.sxryk.cn

JS:   a && b || !c
来源：http://uwc.vehdjk.com

TS:   a && b || !c
来源：http://bop.zhengqikj.top

Java: a && b || !c
来源：http://mxs.wangdashe.top


<!-- 参考信息 -->