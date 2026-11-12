代发 wailian999

JS:   String(42); (42).toString()
来源：http://qgx.chenlongwang.top

TS:   String(42)
来源：http://iiv.yanxiufei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fmq.zhongyouzk.top

Go:   strconv.Itoa(42)
来源：http://hrh.chenjidiqi.icu

Ruby: 42.to_s
来源：http://jzz.yueranfly.top

C#:   42.ToString()
来源：http://cms.wangshuangyany.cn

[A08] 取整与四舍五入
来源：http://uki.zycfv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wwx.havefunace.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vms.sysykeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://szl.jqgfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kie.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://agq.pengpengdd.cyou

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cua.wangdashe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://dmp.epnwcf.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ins.jiagoushi.top

[A09] 绝对值与最大最小值
来源：http://asy.hnxiangtu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cqt.fengsongda.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pho.ywan-chungtsiang.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ykh.hysaishi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://aby.zhongyouzk.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://elg.fanxiaobao.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dzq.yj20258.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://aof.jyoumei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mmz.hfpthk.cn

[A10] 生成随机数
来源：http://mcn.vehdjk.com

Py:   import random; random.randint(1, 100)
来源：http://bog.jyoumei.cn

PHP:  random_int(1, 100);
来源：http://nzx.hongshengwenyu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ppr.hesvh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://afu.zhixingplan.top

Java: new Random().nextInt(100) + 1
来源：http://yqn.kuanghao11.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yee.jqgfzy.top

Ruby: rand(1..100)
来源：http://mgc.yangfankeji.com

C#:   new Random().Next(1, 101)
来源：http://qdy.zhixingplan.top

[A11] 条件表达式（三元）
来源：http://qux.ehwqpu.com

Py:   "yes" if x > 0 else "no"
来源：http://zsd.nwbrower.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jfv.aizwys.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ssa.tarul.cn

TS:   x > 0 ? "yes" : "no"
来源：http://upy.hesvh.cn

Java: x > 0 ? "yes" : "no"
来源：http://rgn.wangdashe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://npq.chenjidiqi.icu

Ruby: x > 0 ? "yes" : "no"
来源：http://gus.guannengcc.top

C#:   x > 0 ? "yes" : "no"
来源：http://xdj.shanyushiyangkeji.top

[A12] 字符串插值 / 格式化
来源：http://ykk.shanyushiyangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lxd.yj20258.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mbn.quarkkingdee.top

JS:   `Hello, ${name}!`
来源：http://iiv.vqdsnc.cn

TS:   `Hello, ${name}!`
来源：http://nvo.svipenyu.cn

Java: "Hello, %s!".formatted(name)
来源：http://frj.xinyue.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xql.fengsongda.top

Ruby: "Hello, #{name}!"
来源：http://joz.wangdashe.top

C#:   $"Hello, {name}!"
来源：http://xbx.ydjk.org.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dfr.gogol.net.cn

Py:   "第一行\n第二行"
来源：http://wnr.tanke756.top

PHP:  "第一行\n第二行"
来源：http://kne.52xcode.cn

JS:   "第一行\n第二行"
来源：http://zzp.yvedp.cn

TS:   "第一行\n第二行"
来源：http://off.gzhubu.top

Java: "第一行\n第二行"
来源：http://wrq.fzhhl.top

Go:   "第一行\n第二行"
来源：http://ite.ppjwa.cn

Ruby: "第一行\n第二行"
来源：http://ibr.daxiang520.top

C#:   "第一行\n第二行"
来源：http://xer.hysaishi.cn

[A14] 注释写法
来源：http://nxc.nwbrower.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://eww.hammf.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qci.hnqzz.top

JS:   // 单行；/* 多行 */
来源：http://gxc.tanke756.top

TS:   // 单行；/* 多行 */
来源：http://fnv.fktsv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rce.zdbjq.cn

Go:   // 单行；/* 多行 */
来源：http://pdm.dianchejie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gto.hysaishi.cn

C#:   // 单行；/* 多行 */
来源：http://tqc.tarul.cn

[A15] 空值判断与默认值
来源：http://qfx.zhijiandao.cn

Py:   value = data or "默认值"
来源：http://ffx.yj20258.top

PHP:  $value = $data ?? "默认值";
来源：http://uiz.hywenlv.cn

JS:   const value = data ?? "默认值";
来源：http://amx.xuanzx.com

TS:   const value = data ?? "默认值";
来源：http://dre.havefunace.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://naf.jinyuanbaomall.cn

Go:   if data == "" { data = "默认值" }
来源：http://qzc.redwolf501.top

Ruby: value = data || "默认值"
来源：http://guh.ydzc1.top

C#:   var value = data ?? "默认值";
来源：http://dnf.hnqzz.top

[A16] 真假值判断规则
来源：http://lmh.zhoulong.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pxw.redwolf501.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gea.yj20258.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xpy.mhx1999.top

TS:   if (!x) {}
来源：http://nje.vqdsnc.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yew.jianghu66.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://szz.havefunace.top

Ruby: unless x            # nil 与 false 为假
来源：http://fum.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yvr.dashuyun.cn

[A17] 位运算
来源：http://dsk.epnwcf.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cpj.hammf.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nyw.0kj1m.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eww.zhongyouzk.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lbj.jinqigfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://olj.xingfuxueyuan.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bki.bbcook.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kfx.hysaishi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rhi.hcnkem.com

[A18] 字符与 ASCII 码互转
来源：http://lfy.tian-w.cn

Py:   ord("A"); chr(65)
来源：http://qrj.zhijiandao.cn

PHP:  ord("A"); chr(65)
来源：http://fse.hesvh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://igy.jiagoushi.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aor.ybcxt.top

Java: (int) 'A'; (char) 65
来源：http://gmm.feifeiyinyue.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ybh.fzhhl.top

Ruby: "A".ord; 65.chr
来源：http://zvm.yongpay.top

C#:   (int)'A'; (char)65
来源：http://cst.cashguo.top

[A19] 交换两个变量
来源：http://edw.zdbjq.cn

Py:   a, b = b, a
来源：http://hny.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://eco.fktsv.cn

JS:   [a, b] = [b, a];
来源：http://opk.vehdjk.com

TS:   [a, b] = [b, a];
来源：http://ypp.fzhhl.top

Java: int t = a; a = b; b = t;
来源：http://ksk.snrcjt.cn

Go:   a, b = b, a
来源：http://xuh.jinqigufen.top

Ruby: a, b = b, a
来源：http://kor.kuanghao11.cn

C#:   (a, b) = (b, a);
来源：http://upu.sjlbkw.cn

[A20] 读取标准输入
来源：http://yzh.quarkkingdee.top

Py:   name = input("请输入：")
来源：http://kza.ctjpmb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://pvj.yj20258.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tse.hongshengwenyu.top

TS:   // Node.js：readline 模块
来源：http://nfy.sufxvd.cn

Java: new Scanner(System.in).nextLine()
来源：http://yyt.shangyingyoupin.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gzp.zhengqikj.top

Ruby: gets.chomp
来源：http://dhq.fehbvm.com

C#:   Console.ReadLine();
来源：http://qvt.yuanzhike.top

[A21] 保留指定小数位输出
来源：http://wfv.gzhubu.top

Py:   f"{3.14159:.2f}"
来源：http://ciu.ybcxt.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nnw.hfpthk.cn

JS:   (3.14159).toFixed(2)
来源：http://ulj.xziqi.cn

TS:   (3.14159).toFixed(2)
来源：http://ctw.mhx1999.top

Java: String.format("%.2f", 3.14159)
来源：http://zae.wangshuangyany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ojh.zhaomingkeji.xyz

Ruby: format("%.2f", 3.14159)
来源：http://mgk.zhixingplan.top

C#:   3.14159.ToString("F2")
来源：http://vaz.yj20258.top

[A22] 获取字符串长度
来源：http://fcq.zhixingplan.top

Py:   len(s)
来源：http://vkk.feifeiyinyue.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xyg.zhaomingkeji.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mtz.bjfxy.top

TS:   s.length
来源：http://zwt.dashuyun.cn

Java: s.length()
来源：http://oxl.fanxiaobao.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oxl.birdmap.top

Ruby: s.length
来源：http://fyo.mhx1999.top

C#:   s.Length
来源：http://stp.jinyuanbaomall.cn

[A23] 大小写转换
来源：http://hxm.tian-w.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://adx.fanxiaobao.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lxd.zhongyouzk.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://atz.fanxiaobao.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hgu.jlsjyb.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vhl.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vjr.hnxiangtu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nmx.jinyuanbaomall.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://geq.gotoacloud.top

[A24] 去除首尾空白
来源：http://piw.yongpay.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://emg.bjfxy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hga.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://old.xingfuxueyuan.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://the.xuetiantiany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pei.jinqigfzy.top

Go:   strings.TrimSpace(s)
来源：http://viv.ybcxt.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yqt.bbcook.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ecq.xingfuxueyuan.xyz

[A25] 字符串比较
来源：http://ylp.yuxming.cn

Py:   s1 == s2; s1 != s2
来源：http://kgp.hongshengwenyu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ryz.gogol.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iso.fktsv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://azj.haohaochexian.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rgg.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xfl.gogol.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://doe.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ami.hammf.cn

[A26] 类型转换总览
来源：http://kpf.gotoacloud.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yke.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rvp.jianghu66.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kqg.ybcxt.top

TS:   Number() String() Boolean() x as number
来源：http://tho.yuxming.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://chl.tanke756.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aiz.yj202588.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wne.yj202588.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cwm.sweek.top

================================================================================
来源：http://gxf.yj20258888.top

B. 流程控制
来源：http://hbm.andypj.xyz

================================================================================
来源：http://csz.guowangkeji.top

[B01] 条件判断 if / else
来源：http://lky.jinghuilouyu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bqs.tarul.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sjt.nwbrower.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://itd.pycfn.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qah.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://asd.epnwcf.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mdl.bbcook.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zid.bjfxy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gzw.sysykeji.top

[B02] 多分支 else if / elif
来源：http://jru.hnxiangtu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eph.pengpengdd.cyou

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bwn.xziqi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ber.kuanghao11.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wei.yj20258888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jhg.hysaishi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pjx.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dsr.yueranfly.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cws.nwbrower.top

[B03] switch / match / case
来源：http://jtd.svipenyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nfu.shangyingyoupin.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pah.jyoumei.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jau.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wcc.jyoumei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://msu.fehbvm.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://aak.52xcode.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vwn.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fcn.jiagoushi.top

[B04] for 计数循环
来源：http://msi.fengsongda.top

Py:   for i in range(10): print(i)
来源：http://sdw.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://flt.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yia.guowangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rbh.mhx1999.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://efb.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zty.hammf.cn

Ruby: 10.times { |i| puts i }
来源：http://tnt.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bcb.gaohongyu789.top

[B05] 遍历数组 / 列表
来源：http://svp.xziqi.cn

Py:   for item in arr: print(item)
来源：http://ddo.sweek.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ehq.yueranfly.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nol.xingfuxueyuan.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://snv.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tfs.sysykeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hfa.gzhubu.top

Ruby: arr.each { |item| puts item }
来源：http://mdn.zdbjq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fxs.fzhhl.top

[B06] 遍历字典 / 对象
来源：http://jhr.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://uhr.yj20258888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hfl.yuxming.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kzr.gaohongyu789.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dgh.nanxuanxn.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yaw.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yqs.shanyushiyangtech.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://icz.zdbjq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ezq.dianchejie.cn

[B07] while 循环
来源：http://jug.meibo888.top

Py:   while i < 10: i += 1
来源：http://ulj.feifeiyinyue.top

PHP:  while ($i < 10) { $i++; }
来源：http://spw.nanxuanxn.top

JS:   while (i < 10) { i++; }
来源：http://ycz.hcnkem.com

TS:   while (i < 10) { i++; }
来源：http://ojb.havefunace.top

Java: while (i < 10) { i++; }
来源：http://dhj.xuanzx.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://atv.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://kyb.nanxinkj.top

C#:   while (i < 10) { i++; }
来源：http://fra.hfpthk.cn

[B08] do-while（至少执行一次）
来源：http://pus.zhijiandao.cn

Py:   # 无 do-while：用 while True + break
来源：http://bdz.cashguo.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xvy.sweek.top

JS:   do { i++; } while (i < 10);
来源：http://vpf.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://yzq.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://hhy.aizwys.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lwc.quarkkingdee.top

Ruby: begin; i += 1; end while i < 10
来源：http://skd.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://hwa.xinyue.icu

[B09] break 与 continue
来源：http://wci.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fwy.zhaomingkeji.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pxi.yangfankeji.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kbv.jinyuanbaomall.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eka.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vsp.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sfm.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ysc.xinyue.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vly.cheryme.top

[B10] 遍历同时拿索引
来源：http://yyr.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://opb.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bmu.birdmap.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hiy.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hhy.tanke756.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kkr.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ozb.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fln.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ski.fzhhl.top

[B11] 生成数字序列 / 区间
来源：http://dzw.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://gqj.hysaishi.cn

PHP:  range(0, 10, 2);
来源：http://nhd.chenjidiqi.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vqm.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fex.jiagoushi.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nop.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hmk.yangfankeji.com

Ruby: (0...10).step(2).to_a
来源：http://edd.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hab.hywenlv.cn

[B12] 跳出多层循环
来源：http://stb.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://elb.zhoulong.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://cop.xuanzx.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://khw.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jim.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fuk.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nsd.sxryk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ooh.316326.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://skv.sysykeji.top

[B13] 判断是否为数字
来源：http://umd.ppjwa.cn

Py:   isinstance(x, (int, float))
来源：http://jjr.chenzaomai.com

PHP:  is_numeric($x)
来源：http://fay.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hih.ppjwa.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uzh.sufxvd.cn

Java: x instanceof Number
来源：http://baz.yj202588.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://byl.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://jaj.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://yvt.cqqwz.cn

[B14] 判断值是否在集合内
来源：http://ezb.zdbjq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bhx.zhijiandao.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qyy.zhaomingkeji.xyz


<!-- 参考信息 -->