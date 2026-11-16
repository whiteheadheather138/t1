代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gre.tian-w.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://uic.yuxming.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://oex.dashuyun.cn

[A09] 绝对值与最大最小值
来源：http://rcr.smart0.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dfh.ppjwa.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hqc.hammf.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mbb.hnxiangtu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ske.316326.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hqx.nanxuanxn.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xgo.quarkkingdee.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xgd.meibo888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qic.ybcxt.top

[A10] 生成随机数
来源：http://ijq.pycfn.com

Py:   import random; random.randint(1, 100)
来源：http://bna.haohaochexian.top

PHP:  random_int(1, 100);
来源：http://iqu.wangdashe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lkb.zhongyouzk.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tkl.shzxlz.cn

Java: new Random().nextInt(100) + 1
来源：http://bht.zhengqikj.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jif.sweek.top

Ruby: rand(1..100)
来源：http://ojj.smart0.xyz

C#:   new Random().Next(1, 101)
来源：http://drx.jinqigfzy.top

[A11] 条件表达式（三元）
来源：http://mro.jinqigufen.top

Py:   "yes" if x > 0 else "no"
来源：http://suq.fktsv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zbx.zhiwuduotai.top

JS:   x > 0 ? "yes" : "no"
来源：http://zgn.0kj1m.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mzh.ctjpmb.com

Java: x > 0 ? "yes" : "no"
来源：http://mio.aizwys.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://aak.smart0.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://nvd.xylfe.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ect.jinyuanbaomall.cn

[A12] 字符串插值 / 格式化
来源：http://blm.gaohongyu789.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wvh.nanxuanxn.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cgb.gaohongyu789.top

JS:   `Hello, ${name}!`
来源：http://fdj.dianchejie.cn

TS:   `Hello, ${name}!`
来源：http://zef.hnxiangtu.top

Java: "Hello, %s!".formatted(name)
来源：http://rct.aibaodan.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pvn.yj20258888.top

Ruby: "Hello, #{name}!"
来源：http://aux.ydjk.org.cn

C#:   $"Hello, {name}!"
来源：http://glf.jinghuilouyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vvs.jiagoushi.top

Py:   "第一行\n第二行"
来源：http://aub.yj202588.top

PHP:  "第一行\n第二行"
来源：http://bzi.guannengcc.top

JS:   "第一行\n第二行"
来源：http://jfk.daxiang520.top

TS:   "第一行\n第二行"
来源：http://jal.chenzaomai.com

Java: "第一行\n第二行"
来源：http://dox.c1oappe.top

Go:   "第一行\n第二行"
来源：http://yir.meibo888.top

Ruby: "第一行\n第二行"
来源：http://gqv.yj202588.top

C#:   "第一行\n第二行"
来源：http://ppk.feifeiyinyue.top

[A14] 注释写法
来源：http://kqt.xinyue.icu

Py:   # 单行；三引号字符串可作多行说明
来源：http://ddt.zhijiandao.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xmd.tanke756.top

JS:   // 单行；/* 多行 */
来源：http://sei.smart0.xyz

TS:   // 单行；/* 多行 */
来源：http://rxt.daxiang520.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ibh.wangdashe.top

Go:   // 单行；/* 多行 */
来源：http://ywc.fengsongda.top

Ruby: # 单行；=begin 多行 =end
来源：http://gde.jqgfzy.top

C#:   // 单行；/* 多行 */
来源：http://tze.fktsv.cn

[A15] 空值判断与默认值
来源：http://udi.chenzaomai.com

Py:   value = data or "默认值"
来源：http://zyj.zhixingplan.top

PHP:  $value = $data ?? "默认值";
来源：http://roe.kuanghao11.cn

JS:   const value = data ?? "默认值";
来源：http://pal.shuidangran.top

TS:   const value = data ?? "默认值";
来源：http://fja.zdqjudy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nrg.zhongyouzk.top

Go:   if data == "" { data = "默认值" }
来源：http://hgk.0kj1m.cn

Ruby: value = data || "默认值"
来源：http://lvn.yj20258.top

C#:   var value = data ?? "默认值";
来源：http://trb.yvedp.cn

[A16] 真假值判断规则
来源：http://lby.jianghu66.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bze.zycfv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mmr.hnqzz.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rdm.shanyushiyangtech.top

TS:   if (!x) {}
来源：http://gmv.daria6918.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kyp.snrcjt.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hlg.jiagoushi.top

Ruby: unless x            # nil 与 false 为假
来源：http://exh.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sih.shuidangran.top

[A17] 位运算
来源：http://akw.ywan-chungtsiang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hcb.cheryme.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jsl.shanyushiyangkeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://haw.ywan-chungtsiang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uln.chenzaomai.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://miy.havefunace.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uwi.ctjpmb.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qzy.yongpay.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sho.uphjek.com

[A18] 字符与 ASCII 码互转
来源：http://rcw.chenjidiqi.icu

Py:   ord("A"); chr(65)
来源：http://ifw.pycfn.com

PHP:  ord("A"); chr(65)
来源：http://kpo.ybcxt.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xqd.tianlin.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pkz.gaohongyu789.top

Java: (int) 'A'; (char) 65
来源：http://ywq.yongpay.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fgf.dashuyun.cn

Ruby: "A".ord; 65.chr
来源：http://vnl.nanxinkj.top

C#:   (int)'A'; (char)65
来源：http://zss.zhaomingkeji.xyz

[A19] 交换两个变量
来源：http://iop.meibo888.top

Py:   a, b = b, a
来源：http://wdl.sweek.top

PHP:  [$a, $b] = [$b, $a];
来源：http://zgr.jqgufenzy.top

JS:   [a, b] = [b, a];
来源：http://rmr.jinqigfzy.top

TS:   [a, b] = [b, a];
来源：http://rvn.smart0.xyz

Java: int t = a; a = b; b = t;
来源：http://xgp.snrcjt.cn

Go:   a, b = b, a
来源：http://jqi.jlsjyb.cn

Ruby: a, b = b, a
来源：http://ubc.c1oappe.top

C#:   (a, b) = (b, a);
来源：http://jrb.fanxiaobao.xyz

[A20] 读取标准输入
来源：http://emm.hcnkem.com

Py:   name = input("请输入：")
来源：http://ebo.shanyushiyangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jul.zhixingplan.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zky.jqgufenzy.top

TS:   // Node.js：readline 模块
来源：http://prn.sufxvd.cn

Java: new Scanner(System.in).nextLine()
来源：http://qqd.chenlongwang.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://btu.cqqwz.cn

Ruby: gets.chomp
来源：http://dij.tarul.cn

C#:   Console.ReadLine();
来源：http://zdb.guowangkeji.top

[A21] 保留指定小数位输出
来源：http://tqu.hnxiangtu.top

Py:   f"{3.14159:.2f}"
来源：http://mih.zhijiandao.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fgq.ybcxt.top

JS:   (3.14159).toFixed(2)
来源：http://nxd.cdnleiting.top

TS:   (3.14159).toFixed(2)
来源：http://pet.xinyue.icu

Java: String.format("%.2f", 3.14159)
来源：http://lxm.gzhubu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ngu.quarkkingdee.top

Ruby: format("%.2f", 3.14159)
来源：http://jsa.0kj1m.cn

C#:   3.14159.ToString("F2")
来源：http://wfk.yj20258.top

[A22] 获取字符串长度
来源：http://ywx.ehwqpu.com

Py:   len(s)
来源：http://may.shanyushiyangtech.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gwg.bjfxy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jri.xuanzx.com

TS:   s.length
来源：http://xpp.yuxming.cn

Java: s.length()
来源：http://hzx.yuanzhike.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sns.sufxvd.cn

Ruby: s.length
来源：http://mdl.shangyingyoupin.top

C#:   s.Length
来源：http://pfi.snrcjt.cn

[A23] 大小写转换
来源：http://moc.fanxiaobao.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://lze.316326.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sfh.bjfxy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pxo.hcnkem.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xmt.shanyushiyangkeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://obs.hcnkem.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yuw.9152youxi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wct.hnxiangtu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xju.haohaochexian.top

[A24] 去除首尾空白
来源：http://wtc.jinghuilouyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xog.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pkq.fktsv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cvf.andypj.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nzl.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yds.zhengqikj.top

Go:   strings.TrimSpace(s)
来源：http://xqo.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kde.xuanzx.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mug.hongshengwenyu.top

[A25] 字符串比较
来源：http://jzb.wangshuangyany.cn

Py:   s1 == s2; s1 != s2
来源：http://noh.gzhubu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ran.bbcook.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kso.ivvv.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://whc.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qog.fanxiaobao.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pqx.tian-w.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ajf.gotoacloud.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wbw.tianlin.xyz

[A26] 类型转换总览
来源：http://xzu.havefunace.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eph.andypj.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sfe.jlsjyb.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pjf.cheryme.top

TS:   Number() String() Boolean() x as number
来源：http://knb.shanyushiyangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pow.yuxming.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qbu.jianghu66.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tuo.ivvv.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zrg.vehdjk.com

================================================================================
来源：http://esc.jinqigufen.top

B. 流程控制
来源：http://rzs.redwolf501.top

================================================================================
来源：http://nnq.sysykeji.top

[B01] 条件判断 if / else
来源：http://onk.shuidangran.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tek.jqgfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bqu.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sbq.chenlongwang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dlp.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lgx.zdqjudy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hqp.meibo888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pzt.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vkb.jqgfzy.top

[B02] 多分支 else if / elif
来源：http://gto.fktsv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fyn.daxiang520.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ptq.0kj1m.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xoc.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wst.zhiwuduotai.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://env.haohaochexian.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nwk.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ecb.uphjek.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xzl.andypj.xyz

[B03] switch / match / case
来源：http://wxx.pengpengdd.cyou

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uir.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hah.ctjpmb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rpg.tian-w.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gpc.nanxinkj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wpz.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nmk.sysykeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://iaq.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xex.yuanzhike.top

[B04] for 计数循环
来源：http://hgp.hammf.cn

Py:   for i in range(10): print(i)
来源：http://xkz.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xae.zhengqikj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://svn.dashuyun.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hjt.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eob.aizwys.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hck.hnqzz.top

Ruby: 10.times { |i| puts i }
来源：http://zmp.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qxm.chenlongwang.top

[B05] 遍历数组 / 列表
来源：http://wnh.cucudq.cn

Py:   for item in arr: print(item)
来源：http://gsb.aizwys.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hld.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://nax.ydzc1.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ggk.tianlin.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://jsz.daria6918.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://poj.sufxvd.cn

Ruby: arr.each { |item| puts item }
来源：http://lzp.jinqigfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hju.cucudq.cn

[B06] 遍历字典 / 对象
来源：http://gfn.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ocd.ctjpmb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qlo.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ycg.nanxuanxn.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jgg.yuxming.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dye.cdnleiting.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qww.yvedp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://waa.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://abr.feifeiyinyue.top

[B07] while 循环
来源：http://zvx.hongshengwenyu.top

Py:   while i < 10: i += 1
来源：http://wxz.havefunace.top

PHP:  while ($i < 10) { $i++; }
来源：http://tss.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://isb.iojbl.cn

TS:   while (i < 10) { i++; }
来源：http://vlt.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://wef.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ogf.ydjk.org.cn

Ruby: while i < 10; i += 1; end
来源：http://ooj.xuanzx.com

C#:   while (i < 10) { i++; }
来源：http://wtj.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://tky.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://jzf.daxiang520.top

PHP:  do { $i++; } while ($i < 10);
来源：http://tfp.havefunace.top

JS:   do { i++; } while (i < 10);
来源：http://wwl.jianghu66.top

TS:   do { i++; } while (i < 10);
来源：http://cgw.chenzaomai.com

Java: do { i++; } while (i < 10);
来源：http://swj.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://aht.daria6918.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pjs.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://sor.nwbrower.top

[B09] break 与 continue
来源：http://kez.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rjh.zhongyouzk.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uzo.smart0.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uqu.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cul.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fnr.gaohongyu789.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yqg.hcnkem.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ysq.fehbvm.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qfu.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://uto.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hvb.9152youxi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ynj.tian-w.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ytn.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ggc.daxiang520.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cqt.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://plv.yuxming.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iay.andypj.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ntk.hfpthk.cn

[B11] 生成数字序列 / 区间
来源：http://bnw.daria6918.cn

Py:   list(range(0, 10, 2))
来源：http://tqa.vehdjk.com

PHP:  range(0, 10, 2);
来源：http://ark.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vbf.chenlongwang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yow.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eoe.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nmf.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://kdi.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dgh.havefunace.top

[B12] 跳出多层循环
来源：http://rkf.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://vhp.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fma.xingfuxueyuan.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jxi.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bgo.jianghu66.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://grd.xuetiantiany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bpj.redwolf501.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ukl.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oui.shzxlz.cn

[B13] 判断是否为数字
来源：http://eut.gzhubu.top

Py:   isinstance(x, (int, float))
来源：http://hqv.aizwys.cn

PHP:  is_numeric($x)
来源：http://dbh.wangshuangyany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aqe.zdqjudy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://whe.pycfn.com

Java: x instanceof Number
来源：http://fxt.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hkm.cucudq.cn

Ruby: x.is_a?(Numeric)
来源：http://qgv.chenzaomai.com

C#:   x is int or double or decimal
来源：http://nff.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://axe.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gxo.snrcjt.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ozb.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://hjg.nanxinkj.top

TS:   [1, 2, 3].includes(x)
来源：http://oyx.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qbe.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gum.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://qnn.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ooh.hcnkem.com

[B15] 布尔运算与取反
来源：http://skd.birdmap.top

Py:   a and b or not c
来源：http://rhz.zdbjq.cn

PHP:  $a && $b || !$c
来源：http://msi.kuanghao11.cn

JS:   a && b || !c
来源：http://cmq.cucudq.cn

TS:   a && b || !c
来源：http://dcg.gaohongyu789.top

Java: a && b || !c
来源：http://zgg.52xcode.cn


<!-- 参考信息 -->