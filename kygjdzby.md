代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yxq.chenzaomai.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://umr.vehdjk.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gvi.ydzc1.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ymu.daria6918.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dvr.hongshengwenyu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pnz.svipenyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cvm.jinqigfzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rab.nwbrower.top

[A10] 生成随机数
来源：http://xgy.svipenyu.cn

Py:   import random; random.randint(1, 100)
来源：http://vtk.zhengqikj.top

PHP:  random_int(1, 100);
来源：http://olr.jlsjyb.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://byl.jlsjyb.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://scp.quarkkingdee.top

Java: new Random().nextInt(100) + 1
来源：http://ygq.cqqwz.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dqc.hfpthk.cn

Ruby: rand(1..100)
来源：http://mqf.smart0.xyz

C#:   new Random().Next(1, 101)
来源：http://qmc.yongpay.top

[A11] 条件表达式（三元）
来源：http://hiq.daxiang520.top

Py:   "yes" if x > 0 else "no"
来源：http://lbx.kuanghao11.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hyf.zhiwuduotai.top

JS:   x > 0 ? "yes" : "no"
来源：http://epi.aizwys.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tqc.zhongyouzk.top

Java: x > 0 ? "yes" : "no"
来源：http://ufv.redwolf501.top

Go:   // 无三元运算符，需用 if 语句
来源：http://cdi.hongshengwenyu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ndx.yonumen.top

C#:   x > 0 ? "yes" : "no"
来源：http://fit.yj20258.top

[A12] 字符串插值 / 格式化
来源：http://wbk.yongpay.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hsj.dianchejie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vai.snrcjt.cn

JS:   `Hello, ${name}!`
来源：http://ydv.uphjek.com

TS:   `Hello, ${name}!`
来源：http://jzc.gzhubu.top

Java: "Hello, %s!".formatted(name)
来源：http://evs.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://snb.zycfv.cn

Ruby: "Hello, #{name}!"
来源：http://avq.zdbjq.cn

C#:   $"Hello, {name}!"
来源：http://duy.smart0.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://zbp.hnqzz.top

Py:   "第一行\n第二行"
来源：http://tss.cqqwz.cn

PHP:  "第一行\n第二行"
来源：http://okz.xziqi.cn

JS:   "第一行\n第二行"
来源：http://xta.hongshengwenyu.top

TS:   "第一行\n第二行"
来源：http://zsr.xingfuxueyuan.xyz

Java: "第一行\n第二行"
来源：http://ivy.xingfuxueyuan.xyz

Go:   "第一行\n第二行"
来源：http://fcd.aibaodan.cn

Ruby: "第一行\n第二行"
来源：http://rhk.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://bgo.chenjidiqi.icu

[A14] 注释写法
来源：http://lqi.haohaochexian.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xbv.nanxinkj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gpy.wangdashe.top

JS:   // 单行；/* 多行 */
来源：http://yyy.yj20258.top

TS:   // 单行；/* 多行 */
来源：http://jok.sweek.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://twq.hnxiangtu.top

Go:   // 单行；/* 多行 */
来源：http://yey.jinghuilouyu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rfz.hfpthk.cn

C#:   // 单行；/* 多行 */
来源：http://ojo.jiagoushi.top

[A15] 空值判断与默认值
来源：http://buq.zhaomingkeji.xyz

Py:   value = data or "默认值"
来源：http://pic.zhaomingkeji.xyz

PHP:  $value = $data ?? "默认值";
来源：http://sof.yuanzhike.top

JS:   const value = data ?? "默认值";
来源：http://cdf.svipenyu.cn

TS:   const value = data ?? "默认值";
来源：http://gzz.iojbl.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lip.tian-w.cn

Go:   if data == "" { data = "默认值" }
来源：http://amu.nanxinkj.top

Ruby: value = data || "默认值"
来源：http://qkd.hysaishi.cn

C#:   var value = data ?? "默认值";
来源：http://mgf.shanyushiyangkeji.top

[A16] 真假值判断规则
来源：http://lso.sweek.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://svk.jinqigufen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ktv.tian-w.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://guh.ydjk.org.cn

TS:   if (!x) {}
来源：http://oew.hysaishi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ozk.0kj1m.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gbs.zhengqikj.top

Ruby: unless x            # nil 与 false 为假
来源：http://vol.jiagoushi.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gtu.shanyushiyangkeji.top

[A17] 位运算
来源：http://swl.birdmap.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uxa.gogol.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://icd.xuanzx.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jzx.cheryme.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nmr.aizwys.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pzi.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zdc.bbcook.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bbk.sysykeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bmy.vqdsnc.cn

[A18] 字符与 ASCII 码互转
来源：http://hya.ctjpmb.com

Py:   ord("A"); chr(65)
来源：http://ovs.wangshuangyany.cn

PHP:  ord("A"); chr(65)
来源：http://mlg.gogol.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kvs.shanyushiyangkeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://slm.havefunace.top

Java: (int) 'A'; (char) 65
来源：http://knn.zhaomingkeji.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vjs.ybcxt.top

Ruby: "A".ord; 65.chr
来源：http://taz.zhengqikj.top

C#:   (int)'A'; (char)65
来源：http://vfe.wangdashe.top

[A19] 交换两个变量
来源：http://cdv.smart0.xyz

Py:   a, b = b, a
来源：http://zam.zhijiandao.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kkk.hysaishi.cn

JS:   [a, b] = [b, a];
来源：http://rlg.pycfn.com

TS:   [a, b] = [b, a];
来源：http://zpz.xuanzx.com

Java: int t = a; a = b; b = t;
来源：http://put.nanxuanxn.top

Go:   a, b = b, a
来源：http://hcl.bbcook.cn

Ruby: a, b = b, a
来源：http://aip.jyoumei.cn

C#:   (a, b) = (b, a);
来源：http://hkq.hnqzz.top

[A20] 读取标准输入
来源：http://fox.cashguo.top

Py:   name = input("请输入：")
来源：http://omx.daria6918.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qoj.quarkkingdee.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lwb.yuxming.cn

TS:   // Node.js：readline 模块
来源：http://hmr.cdnleiting.top

Java: new Scanner(System.in).nextLine()
来源：http://kur.zhongyouzk.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lqx.ydjk.org.cn

Ruby: gets.chomp
来源：http://idt.hongshengwenyu.top

C#:   Console.ReadLine();
来源：http://xti.chenjidiqi.icu

[A21] 保留指定小数位输出
来源：http://aky.daxiang520.top

Py:   f"{3.14159:.2f}"
来源：http://aph.xylfe.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mfc.yj202588.top

JS:   (3.14159).toFixed(2)
来源：http://ckl.chenjidiqi.icu

TS:   (3.14159).toFixed(2)
来源：http://odq.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://eqn.yfazqb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mpa.dianchejie.cn

Ruby: format("%.2f", 3.14159)
来源：http://gky.cheryme.top

C#:   3.14159.ToString("F2")
来源：http://ucw.c1oappe.top

[A22] 获取字符串长度
来源：http://jmm.dianchejie.cn

Py:   len(s)
来源：http://jxv.xinyue.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pcj.sysykeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ymh.hnqzz.top

TS:   s.length
来源：http://dzd.zhongyouzk.top

Java: s.length()
来源：http://iqa.shanyushiyangtech.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zlr.uphjek.com

Ruby: s.length
来源：http://mtu.snrcjt.cn

C#:   s.Length
来源：http://mne.shanyushiyangkeji.top

[A23] 大小写转换
来源：http://egb.hfpthk.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uwm.jyoumei.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lvi.nanxinkj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ddv.jlsjyb.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bsl.chenjidiqi.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lio.svipenyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ylx.hysaishi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mpt.yangfankeji.com

C#:   s.ToUpper(); s.ToLower()
来源：http://fis.ybcxt.top

[A24] 去除首尾空白
来源：http://xxu.smart0.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cfy.zycfv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hrv.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xck.epnwcf.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jyp.pengpengdd.cyou

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kyi.epnwcf.com

Go:   strings.TrimSpace(s)
来源：http://wun.yvedp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qbh.zhengqikj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yyu.jqgfzy.top

[A25] 字符串比较
来源：http://nsu.aibaodan.cn

Py:   s1 == s2; s1 != s2
来源：http://bvh.gotoacloud.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mvl.andypj.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://onc.ywan-chungtsiang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jon.mhx1999.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eye.yfazqb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fzy.pycfn.com

Ruby: s1 == s2; s1 <=> s2
来源：http://dcs.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://prs.yvedp.cn

[A26] 类型转换总览
来源：http://vvg.sufxvd.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nuk.tian-w.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://awd.pycfn.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zfe.chenzaomai.com

TS:   Number() String() Boolean() x as number
来源：http://whw.uphjek.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lif.aibaodan.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jsa.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sbn.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://haa.ehwqpu.com

================================================================================
来源：http://tqd.fzhhl.top

B. 流程控制
来源：http://obp.ywan-chungtsiang.top

================================================================================
来源：http://thv.yueranfly.top

[B01] 条件判断 if / else
来源：http://dfd.shangyingyoupin.top

Py:   result = "正" if x > 0 else "非正"
来源：http://loh.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://txg.zycfv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wla.hfpthk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oeh.redwolf501.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://bxy.zdqjudy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fev.xylfe.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wbh.zhengqikj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wcm.zhongyouzk.top

[B02] 多分支 else if / elif
来源：http://pfj.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://etl.mhx1999.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zsb.316326.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qmq.ywan-chungtsiang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aqb.xylfe.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://urj.yj202588.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rex.xuanzx.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nww.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://taf.cdnleiting.top

[B03] switch / match / case
来源：http://ive.cheryme.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vld.jinghuilouyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qxl.vehdjk.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jgd.316326.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://usk.yonumen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uig.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nne.dianchejie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yda.xingfuxueyuan.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uqi.zdqjudy.top

[B04] for 计数循环
来源：http://tku.zycfv.cn

Py:   for i in range(10): print(i)
来源：http://toh.birdmap.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gzt.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bib.0kj1m.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iym.shzxlz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cle.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tss.yanxiufei.cn

Ruby: 10.times { |i| puts i }
来源：http://rvk.gotoacloud.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vbx.gotoacloud.top

[B05] 遍历数组 / 列表
来源：http://ime.fanxiaobao.xyz

Py:   for item in arr: print(item)
来源：http://cnk.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jub.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ojh.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kub.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://drv.snrcjt.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://knv.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://hxz.yuxming.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jys.gotoacloud.top

[B06] 遍历字典 / 对象
来源：http://wsx.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rde.jinghuilouyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ssl.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iim.shuidangran.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vme.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://van.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nei.zhiwuduotai.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dha.xingfuxueyuan.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://smu.xuetiantiany.cn

[B07] while 循环
来源：http://fab.nanxinkj.top

Py:   while i < 10: i += 1
来源：http://bqq.fktsv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eys.tian-w.cn

JS:   while (i < 10) { i++; }
来源：http://sjp.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://jtw.kuanghao11.cn

Java: while (i < 10) { i++; }
来源：http://lsu.52xcode.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jxt.sweek.top

Ruby: while i < 10; i += 1; end
来源：http://odt.snrcjt.cn

C#:   while (i < 10) { i++; }
来源：http://kay.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://hou.ivvv.top

Py:   # 无 do-while：用 while True + break
来源：http://gjj.hysaishi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qga.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://znv.wangshuangyany.cn

TS:   do { i++; } while (i < 10);
来源：http://gyt.redwolf501.top

Java: do { i++; } while (i < 10);
来源：http://ajr.xingfuxueyuan.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://koe.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lru.zhongyouzk.top

C#:   do { i++; } while (i < 10);
来源：http://rry.c1oappe.top

[B09] break 与 continue
来源：http://psi.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xla.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rom.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lri.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ysq.ppjwa.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dgw.zdbjq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zlt.yuanzhike.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qdb.meibo888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://stb.zhengqikj.top

[B10] 遍历同时拿索引
来源：http://jtr.zdbjq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://spy.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yfd.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xdk.zhoulong.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sck.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fcn.zhijiandao.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fma.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yhd.hfpthk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kft.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://vyr.cucudq.cn

Py:   list(range(0, 10, 2))
来源：http://xks.zhiwuduotai.top

PHP:  range(0, 10, 2);
来源：http://zoz.gaohongyu789.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uiu.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xyf.cdnleiting.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tek.ybcxt.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xgh.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://wxh.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zdi.zhengqikj.top

[B12] 跳出多层循环
来源：http://lht.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kez.zhiwuduotai.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cbq.iojbl.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cwa.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vsf.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mou.jyoumei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xql.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kmt.sysykeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rtl.nanxinkj.top

[B13] 判断是否为数字
来源：http://ekg.yuxming.cn

Py:   isinstance(x, (int, float))
来源：http://mzb.guannengcc.top

PHP:  is_numeric($x)
来源：http://zxt.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zhx.zdqjudy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://icu.haohaochexian.top

Java: x instanceof Number
来源：http://iyg.yj20258.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bip.cheryme.top

Ruby: x.is_a?(Numeric)
来源：http://miz.wangdashe.top

C#:   x is int or double or decimal
来源：http://coz.tanke756.top

[B14] 判断值是否在集合内
来源：http://jhc.pengpengdd.cyou

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rnj.xinyue.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dep.ppjwa.cn

JS:   [1, 2, 3].includes(x)
来源：http://vya.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://gyl.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://eaw.yongpay.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pqb.jyoumei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sjl.xylfe.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lqo.c1oappe.top

[B15] 布尔运算与取反
来源：http://cqq.ydzc1.top

Py:   a and b or not c
来源：http://dms.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://vye.c1oappe.top

JS:   a && b || !c
来源：http://lir.mhx1999.top

TS:   a && b || !c
来源：http://zwu.vehdjk.com

Java: a && b || !c
来源：http://frs.shuidangran.top

Go:   a && b || !c
来源：http://owx.tanke756.top

Ruby: a && b || !c
来源：http://zjy.zycfv.cn

C#:   a && b || !c
来源：http://qfc.snrcjt.cn

[B16] 卫语句：不满足条件提前返回
来源：http://luu.pycfn.com


<!-- 参考信息 -->