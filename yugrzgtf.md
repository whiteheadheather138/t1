代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mcg.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qnx.zhoulong.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://anr.316326.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ywa.ppjwa.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lfy.kuanghao11.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://itq.ppjwa.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gjm.snrcjt.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cdh.havefunace.top

[A10] 生成随机数
来源：http://pop.ydzc1.top

Py:   import random; random.randint(1, 100)
来源：http://xmk.tarul.cn

PHP:  random_int(1, 100);
来源：http://vcl.snrcjt.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vjp.fehbvm.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://foj.ppjwa.cn

Java: new Random().nextInt(100) + 1
来源：http://hdn.nanxuanxn.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tdu.fzhhl.top

Ruby: rand(1..100)
来源：http://tfa.hcnkem.com

C#:   new Random().Next(1, 101)
来源：http://oih.yj202588.top

[A11] 条件表达式（三元）
来源：http://wgk.tianlin.xyz

Py:   "yes" if x > 0 else "no"
来源：http://ylq.xuanzx.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://zvz.xinyue.icu

JS:   x > 0 ? "yes" : "no"
来源：http://ehk.chenjidiqi.icu

TS:   x > 0 ? "yes" : "no"
来源：http://ngx.jqgufenzy.top

Java: x > 0 ? "yes" : "no"
来源：http://hni.sxryk.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mlo.haohaochexian.top

Ruby: x > 0 ? "yes" : "no"
来源：http://esp.kuanghao11.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rvp.hywenlv.cn

[A12] 字符串插值 / 格式化
来源：http://oyb.feifeiyinyue.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wyo.ppjwa.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zeg.daxiang520.top

JS:   `Hello, ${name}!`
来源：http://urv.bbcook.cn

TS:   `Hello, ${name}!`
来源：http://ewx.gzhubu.top

Java: "Hello, %s!".formatted(name)
来源：http://iwm.shuidangran.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://was.zhoulong.xyz

Ruby: "Hello, #{name}!"
来源：http://bon.havefunace.top

C#:   $"Hello, {name}!"
来源：http://jwk.gogol.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nne.guannengcc.top

Py:   "第一行\n第二行"
来源：http://rom.fanxiaobao.xyz

PHP:  "第一行\n第二行"
来源：http://fvm.xylfe.cn

JS:   "第一行\n第二行"
来源：http://gug.snrcjt.cn

TS:   "第一行\n第二行"
来源：http://zzw.sufxvd.cn

Java: "第一行\n第二行"
来源：http://gfo.guowangkeji.top

Go:   "第一行\n第二行"
来源：http://myu.zhongyouzk.top

Ruby: "第一行\n第二行"
来源：http://vhn.bjfxy.top

C#:   "第一行\n第二行"
来源：http://tlr.dianchejie.cn

[A14] 注释写法
来源：http://gwr.tianlin.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://ony.xuetiantiany.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hpl.cashguo.top

JS:   // 单行；/* 多行 */
来源：http://kwg.jinqigfzy.top

TS:   // 单行；/* 多行 */
来源：http://pdh.fengsongda.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wye.jianghu66.top

Go:   // 单行；/* 多行 */
来源：http://fba.yuanzhike.top

Ruby: # 单行；=begin 多行 =end
来源：http://koo.9152youxi.cn

C#:   // 单行；/* 多行 */
来源：http://hqn.svipenyu.cn

[A15] 空值判断与默认值
来源：http://nfe.epnwcf.com

Py:   value = data or "默认值"
来源：http://xiw.gzhubu.top

PHP:  $value = $data ?? "默认值";
来源：http://pov.ctjpmb.com

JS:   const value = data ?? "默认值";
来源：http://jzh.smart0.xyz

TS:   const value = data ?? "默认值";
来源：http://ien.yj20258.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oml.daria6918.cn

Go:   if data == "" { data = "默认值" }
来源：http://noc.zhixingplan.top

Ruby: value = data || "默认值"
来源：http://ssr.yueranfly.top

C#:   var value = data ?? "默认值";
来源：http://kgj.chenzaomai.com

[A16] 真假值判断规则
来源：http://jxt.gotoacloud.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qnt.hongshengwenyu.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hbr.yuxming.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cdv.hfpthk.cn

TS:   if (!x) {}
来源：http://fls.yvedp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://czm.nanxuanxn.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eth.quarkkingdee.top

Ruby: unless x            # nil 与 false 为假
来源：http://yrm.fehbvm.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nnm.cqqwz.cn

[A17] 位运算
来源：http://jhn.jiagoushi.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://krp.gogol.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sga.zhoulong.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qqk.guowangkeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vym.fengsongda.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jna.hcnkem.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nvs.zdbjq.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rra.zhijiandao.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vks.xylfe.cn

[A18] 字符与 ASCII 码互转
来源：http://utz.redwolf501.top

Py:   ord("A"); chr(65)
来源：http://gvd.bjfxy.top

PHP:  ord("A"); chr(65)
来源：http://yxl.shanyushiyangtech.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dyy.havefunace.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lxd.cheryme.top

Java: (int) 'A'; (char) 65
来源：http://zma.zycfv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mgg.jqgfzy.top

Ruby: "A".ord; 65.chr
来源：http://mgs.cqqwz.cn

C#:   (int)'A'; (char)65
来源：http://vlt.haohaochexian.top

[A19] 交换两个变量
来源：http://tus.bbcook.cn

Py:   a, b = b, a
来源：http://hxk.xuetiantiany.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bjp.yj20258.top

JS:   [a, b] = [b, a];
来源：http://cfj.guowangkeji.top

TS:   [a, b] = [b, a];
来源：http://ddu.iojbl.cn

Java: int t = a; a = b; b = t;
来源：http://axy.nanxinkj.top

Go:   a, b = b, a
来源：http://vag.dianchejie.cn

Ruby: a, b = b, a
来源：http://qao.quarkkingdee.top

C#:   (a, b) = (b, a);
来源：http://sas.bjfxy.top

[A20] 读取标准输入
来源：http://wbq.zhijiandao.cn

Py:   name = input("请输入：")
来源：http://gvs.quarkkingdee.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jhm.aizwys.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hkj.ehwqpu.com

TS:   // Node.js：readline 模块
来源：http://sqv.jqgfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://pvj.shuidangran.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://usr.zdbjq.cn

Ruby: gets.chomp
来源：http://ook.meibo888.top

C#:   Console.ReadLine();
来源：http://nya.ppjwa.cn

[A21] 保留指定小数位输出
来源：http://ity.hywenlv.cn

Py:   f"{3.14159:.2f}"
来源：http://hdx.feifeiyinyue.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ovr.cheryme.top

JS:   (3.14159).toFixed(2)
来源：http://yrx.wangshuangyany.cn

TS:   (3.14159).toFixed(2)
来源：http://yrd.gzhubu.top

Java: String.format("%.2f", 3.14159)
来源：http://ypn.hnxiangtu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://glf.sjlbkw.cn

Ruby: format("%.2f", 3.14159)
来源：http://fli.shangyingyoupin.top

C#:   3.14159.ToString("F2")
来源：http://ebl.feifeiyinyue.top

[A22] 获取字符串长度
来源：http://tbo.tanke756.top

Py:   len(s)
来源：http://rsj.aibaodan.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fgt.hywenlv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://adf.ctjpmb.com

TS:   s.length
来源：http://awx.sweek.top

Java: s.length()
来源：http://uyk.haohaochexian.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://plo.zhixingplan.top

Ruby: s.length
来源：http://stf.tarul.cn

C#:   s.Length
来源：http://pdd.guannengcc.top

[A23] 大小写转换
来源：http://ijo.zhaomingkeji.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://byg.cdnleiting.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lrn.yuxming.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bxd.jinqigfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cdt.9152youxi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yep.meibo888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hkm.yanxiufei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mrv.tianlin.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://evf.jyoumei.cn

[A24] 去除首尾空白
来源：http://zvi.hammf.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kea.jyoumei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cwa.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vek.sufxvd.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kjl.fehbvm.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pel.yangfankeji.com

Go:   strings.TrimSpace(s)
来源：http://dti.xziqi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ijk.ctjpmb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sxd.sweek.top

[A25] 字符串比较
来源：http://xjb.pengpengdd.cyou

Py:   s1 == s2; s1 != s2
来源：http://kiz.smart0.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rda.wangshuangyany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yqs.ivvv.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zsa.nwbrower.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lcr.daxiang520.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fcx.ivvv.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ypn.jqgufenzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dzx.9152youxi.cn

[A26] 类型转换总览
来源：http://unn.yj202588.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cuc.jyoumei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zuq.shuidangran.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hat.jinqigufen.top

TS:   Number() String() Boolean() x as number
来源：http://tgp.snrcjt.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sql.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mwq.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://idp.cashguo.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nxf.epnwcf.com

================================================================================
来源：http://ctu.hnxiangtu.top

B. 流程控制
来源：http://hhb.daxiang520.top

================================================================================
来源：http://lvg.zdbjq.cn

[B01] 条件判断 if / else
来源：http://hcv.jqgufenzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://exk.hongshengwenyu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hng.hesvh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://evy.dianchejie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aju.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yeh.pycfn.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mon.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hft.daria6918.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zvr.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://efx.pengpengdd.cyou

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wug.hcnkem.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gum.sjlbkw.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wzl.havefunace.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://htd.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ghr.jlsjyb.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iqc.ivvv.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tqc.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://umg.cashguo.top

[B03] switch / match / case
来源：http://smp.sufxvd.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ovs.hongshengwenyu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vyq.zhongyouzk.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://svv.sufxvd.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hpc.nwbrower.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dda.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ycf.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ugj.andypj.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aml.snrcjt.cn

[B04] for 计数循环
来源：http://jfi.shangyingyoupin.top

Py:   for i in range(10): print(i)
来源：http://gmb.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://prm.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://swv.bjfxy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uqu.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hgp.jyoumei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nrt.ywan-chungtsiang.top

Ruby: 10.times { |i| puts i }
来源：http://hpe.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://auk.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://rvq.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://rlv.vehdjk.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ykr.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dqe.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://egn.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://oym.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ukh.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://urf.chenjidiqi.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vip.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://gix.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qpe.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jus.zhongyouzk.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tcu.gotoacloud.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mml.yfazqb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cfi.jinqigfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nzb.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iar.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xfv.fehbvm.com

[B07] while 循环
来源：http://rkx.andypj.xyz

Py:   while i < 10: i += 1
来源：http://xnh.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://agl.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://scf.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://eiv.shanyushiyangkeji.top

Java: while (i < 10) { i++; }
来源：http://ffd.vqdsnc.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ctq.quarkkingdee.top

Ruby: while i < 10; i += 1; end
来源：http://xgz.xziqi.cn

C#:   while (i < 10) { i++; }
来源：http://tcc.ppjwa.cn

[B08] do-while（至少执行一次）
来源：http://dcd.gotoacloud.top

Py:   # 无 do-while：用 while True + break
来源：http://vvm.zdbjq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mey.wangdashe.top

JS:   do { i++; } while (i < 10);
来源：http://evj.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://cjf.birdmap.top

Java: do { i++; } while (i < 10);
来源：http://fdk.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oeh.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iai.zhoulong.xyz

C#:   do { i++; } while (i < 10);
来源：http://fft.jinghuilouyu.cn

[B09] break 与 continue
来源：http://nnt.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://auj.yonumen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wls.yanxiufei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fre.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rhl.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://twx.sysykeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xbo.zycfv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://enf.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://diz.jinyuanbaomall.cn

[B10] 遍历同时拿索引
来源：http://wvr.xylfe.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tpi.birdmap.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ouz.c1oappe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cro.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wpw.nanxinkj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cmu.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pgi.sufxvd.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bkq.zycfv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ejo.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://qbv.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://zmb.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://ifk.sufxvd.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tzh.cdnleiting.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://acm.fktsv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nxk.guannengcc.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fdx.haohaochexian.top

Ruby: (0...10).step(2).to_a
来源：http://lyn.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bnu.jqgufenzy.top

[B12] 跳出多层循环
来源：http://lqs.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gbg.jqgufenzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uuz.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lgc.jinghuilouyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xxk.ydjk.org.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://quc.ivvv.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lnj.gotoacloud.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jeh.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fmi.c1oappe.top

[B13] 判断是否为数字
来源：http://fke.yuanzhike.top

Py:   isinstance(x, (int, float))
来源：http://psm.jianghu66.top

PHP:  is_numeric($x)
来源：http://kgw.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ynz.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nsk.chenzaomai.com

Java: x instanceof Number
来源：http://cor.guowangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nkj.cqqwz.cn

Ruby: x.is_a?(Numeric)
来源：http://dja.jinqigufen.top

C#:   x is int or double or decimal
来源：http://iyj.daria6918.cn

[B14] 判断值是否在集合内
来源：http://fxu.fktsv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pbt.aibaodan.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zyt.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://mqm.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://nlu.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cui.havefunace.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xuu.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gsp.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jlw.c1oappe.top

[B15] 布尔运算与取反
来源：http://giu.cashguo.top

Py:   a and b or not c
来源：http://loq.ehwqpu.com

PHP:  $a && $b || !$c
来源：http://byi.shangyingyoupin.top

JS:   a && b || !c
来源：http://xwo.0kj1m.cn

TS:   a && b || !c
来源：http://ycr.cdnleiting.top

Java: a && b || !c
来源：http://rkx.redwolf501.top

Go:   a && b || !c
来源：http://fpo.hcnkem.com

Ruby: a && b || !c
来源：http://jtv.andypj.xyz

C#:   a && b || !c
来源：http://xfu.yueranfly.top

[B16] 卫语句：不满足条件提前返回
来源：http://jaw.c1oappe.top


<!-- 参考信息 -->