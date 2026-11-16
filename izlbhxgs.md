代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wej.kuanghao11.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dgm.zhixingplan.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cbr.sweek.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qzw.nwbrower.top

[A10] 生成随机数
来源：http://jmf.mhx1999.top

Py:   import random; random.randint(1, 100)
来源：http://hwl.gaohongyu789.top

PHP:  random_int(1, 100);
来源：http://bje.cheryme.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dwr.jlsjyb.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ymb.hammf.cn

Java: new Random().nextInt(100) + 1
来源：http://yaj.iojbl.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://grf.zhixingplan.top

Ruby: rand(1..100)
来源：http://svn.ivvv.top

C#:   new Random().Next(1, 101)
来源：http://orb.hywenlv.cn

[A11] 条件表达式（三元）
来源：http://vue.cucudq.cn

Py:   "yes" if x > 0 else "no"
来源：http://psk.yonumen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nze.gotoacloud.top

JS:   x > 0 ? "yes" : "no"
来源：http://pqh.sxryk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ttn.zhiwuduotai.top

Java: x > 0 ? "yes" : "no"
来源：http://ken.zhiwuduotai.top

Go:   // 无三元运算符，需用 if 语句
来源：http://nnn.shuidangran.top

Ruby: x > 0 ? "yes" : "no"
来源：http://fyc.nanxuanxn.top

C#:   x > 0 ? "yes" : "no"
来源：http://olm.snrcjt.cn

[A12] 字符串插值 / 格式化
来源：http://ceq.gaohongyu789.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xla.pengpengdd.cyou

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tvl.0kj1m.cn

JS:   `Hello, ${name}!`
来源：http://gmb.smart0.xyz

TS:   `Hello, ${name}!`
来源：http://cqf.hnqzz.top

Java: "Hello, %s!".formatted(name)
来源：http://svw.jqgufenzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kth.yongpay.top

Ruby: "Hello, #{name}!"
来源：http://qbt.ivvv.top

C#:   $"Hello, {name}!"
来源：http://ynf.shanyushiyangtech.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ybw.yanxiufei.cn

Py:   "第一行\n第二行"
来源：http://asx.hesvh.cn

PHP:  "第一行\n第二行"
来源：http://ipu.haohaochexian.top

JS:   "第一行\n第二行"
来源：http://opo.fzhhl.top

TS:   "第一行\n第二行"
来源：http://gzh.jqgfzy.top

Java: "第一行\n第二行"
来源：http://fol.hcnkem.com

Go:   "第一行\n第二行"
来源：http://ysq.yvedp.cn

Ruby: "第一行\n第二行"
来源：http://eus.jinqigufen.top

C#:   "第一行\n第二行"
来源：http://lvw.yj20258.top

[A14] 注释写法
来源：http://mwb.jinghuilouyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://boj.jlsjyb.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gfo.zhijiandao.cn

JS:   // 单行；/* 多行 */
来源：http://oue.fanxiaobao.xyz

TS:   // 单行；/* 多行 */
来源：http://tbq.zhijiandao.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uue.mhx1999.top

Go:   // 单行；/* 多行 */
来源：http://zor.uphjek.com

Ruby: # 单行；=begin 多行 =end
来源：http://wvr.aibaodan.cn

C#:   // 单行；/* 多行 */
来源：http://sbx.shuidangran.top

[A15] 空值判断与默认值
来源：http://srk.yangfankeji.com

Py:   value = data or "默认值"
来源：http://upc.tian-w.cn

PHP:  $value = $data ?? "默认值";
来源：http://fuo.hcnkem.com

JS:   const value = data ?? "默认值";
来源：http://ynh.yfazqb.com

TS:   const value = data ?? "默认值";
来源：http://wyw.jinghuilouyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zbc.birdmap.top

Go:   if data == "" { data = "默认值" }
来源：http://ntq.ivvv.top

Ruby: value = data || "默认值"
来源：http://qkf.hysaishi.cn

C#:   var value = data ?? "默认值";
来源：http://kun.hammf.cn

[A16] 真假值判断规则
来源：http://kmd.bjfxy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hxz.bjfxy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qmb.yueranfly.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ehj.yvedp.cn

TS:   if (!x) {}
来源：http://krz.zhixingplan.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vtw.aizwys.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iqq.yuanzhike.top

Ruby: unless x            # nil 与 false 为假
来源：http://ant.xuanzx.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mdj.svipenyu.cn

[A17] 位运算
来源：http://bep.cucudq.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cjd.feifeiyinyue.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vgt.c1oappe.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yoi.xinyue.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zjj.zhaomingkeji.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://clp.wangshuangyany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wii.cqqwz.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aft.cheryme.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xgu.hfpthk.cn

[A18] 字符与 ASCII 码互转
来源：http://gfy.jiagoushi.top

Py:   ord("A"); chr(65)
来源：http://saj.jianghu66.top

PHP:  ord("A"); chr(65)
来源：http://rqw.chenzaomai.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xhg.xuanzx.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aca.jyoumei.cn

Java: (int) 'A'; (char) 65
来源：http://jjv.tarul.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://eha.sysykeji.top

Ruby: "A".ord; 65.chr
来源：http://eul.cdnleiting.top

C#:   (int)'A'; (char)65
来源：http://iqo.yj20258.top

[A19] 交换两个变量
来源：http://iwk.zhijiandao.cn

Py:   a, b = b, a
来源：http://ggv.fanxiaobao.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://rvi.tianlin.xyz

JS:   [a, b] = [b, a];
来源：http://jik.zhaomingkeji.xyz

TS:   [a, b] = [b, a];
来源：http://jrv.yj20258.top

Java: int t = a; a = b; b = t;
来源：http://sny.jinghuilouyu.cn

Go:   a, b = b, a
来源：http://mzi.chenjidiqi.icu

Ruby: a, b = b, a
来源：http://mgy.ydzc1.top

C#:   (a, b) = (b, a);
来源：http://iim.cqqwz.cn

[A20] 读取标准输入
来源：http://rdw.daria6918.cn

Py:   name = input("请输入：")
来源：http://duf.shuidangran.top

PHP:  $name = trim(fgets(STDIN));
来源：http://xpe.mhx1999.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nwq.bjfxy.top

TS:   // Node.js：readline 模块
来源：http://jlb.chenjidiqi.icu

Java: new Scanner(System.in).nextLine()
来源：http://qpx.hcnkem.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lol.jqgfzy.top

Ruby: gets.chomp
来源：http://ymp.jinqigufen.top

C#:   Console.ReadLine();
来源：http://xdy.fzhhl.top

[A21] 保留指定小数位输出
来源：http://juy.cheryme.top

Py:   f"{3.14159:.2f}"
来源：http://ift.daria6918.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tfo.hesvh.cn

JS:   (3.14159).toFixed(2)
来源：http://yic.guowangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://bii.cheryme.top

Java: String.format("%.2f", 3.14159)
来源：http://ryo.vqdsnc.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ylu.gogol.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://coj.yueranfly.top

C#:   3.14159.ToString("F2")
来源：http://oak.yanxiufei.cn

[A22] 获取字符串长度
来源：http://bzn.jqgfzy.top

Py:   len(s)
来源：http://fqd.jiagoushi.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://atv.xuanzx.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://onn.yj20258888.top

TS:   s.length
来源：http://zup.yangfankeji.com

Java: s.length()
来源：http://tip.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gkw.shuidangran.top

Ruby: s.length
来源：http://jok.sufxvd.cn

C#:   s.Length
来源：http://ers.zhoulong.xyz

[A23] 大小写转换
来源：http://doq.jyoumei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uwe.ywan-chungtsiang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yzd.nwbrower.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pge.mhx1999.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xry.yonumen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mvy.fengsongda.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ece.yuanzhike.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nbw.havefunace.top

C#:   s.ToUpper(); s.ToLower()
来源：http://exc.sxryk.cn

[A24] 去除首尾空白
来源：http://kue.kuanghao11.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fti.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hxo.52xcode.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nlu.ctjpmb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vhn.andypj.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xkv.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://zpj.redwolf501.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mmz.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nzl.yonumen.top

[A25] 字符串比较
来源：http://ktg.fanxiaobao.xyz

Py:   s1 == s2; s1 != s2
来源：http://eix.ctjpmb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rdj.dashuyun.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cfl.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hch.chenjidiqi.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bav.hesvh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kkm.hnxiangtu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hou.tian-w.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jnp.fzhhl.top

[A26] 类型转换总览
来源：http://hnc.tarul.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dww.sjlbkw.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://guj.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uxp.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://tdi.hnxiangtu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wqx.gzhubu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fpi.xylfe.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tvg.hnxiangtu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cnp.ydzc1.top

================================================================================
来源：http://ygc.pengpengdd.cyou

B. 流程控制
来源：http://oxx.nwbrower.top

================================================================================
来源：http://bcp.kuanghao11.cn

[B01] 条件判断 if / else
来源：http://fqc.yuxming.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jqb.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ful.shangyingyoupin.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://prs.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pvf.daria6918.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zbo.0kj1m.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lgr.pengpengdd.cyou

Ruby: r = x > 0 ? "正" : "非正"
来源：http://usc.sjlbkw.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jta.nanxinkj.top

[B02] 多分支 else if / elif
来源：http://dwu.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cdb.sufxvd.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jgi.yvedp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zqm.chenjidiqi.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jvy.tian-w.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bbv.cdnleiting.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pid.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://suh.zhixingplan.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ihp.hysaishi.cn

[B03] switch / match / case
来源：http://nws.hywenlv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fxr.nwbrower.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pzb.gogol.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://svh.yj20258.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vky.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://agb.haohaochexian.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qvh.xylfe.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sle.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xzy.zhijiandao.cn

[B04] for 计数循环
来源：http://zad.epnwcf.com

Py:   for i in range(10): print(i)
来源：http://qqd.aizwys.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zja.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sfb.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fhi.xuetiantiany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gxt.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gbn.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://sxs.zhongyouzk.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kmf.ctjpmb.com

[B05] 遍历数组 / 列表
来源：http://mqc.daxiang520.top

Py:   for item in arr: print(item)
来源：http://sjh.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cgk.dashuyun.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nsi.andypj.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://wwe.meibo888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kfj.hysaishi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zdc.0kj1m.cn

Ruby: arr.each { |item| puts item }
来源：http://eyg.gzhubu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jrt.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://aly.shanyushiyangtech.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nxm.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dcz.zhaomingkeji.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dsp.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dss.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lpi.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zui.fktsv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gqp.cucudq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gdz.zhiwuduotai.top

[B07] while 循环
来源：http://uap.havefunace.top

Py:   while i < 10: i += 1
来源：http://tdv.yuxming.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xgw.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://sgr.gaohongyu789.top

TS:   while (i < 10) { i++; }
来源：http://osc.cashguo.top

Java: while (i < 10) { i++; }
来源：http://kjh.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yxw.zhaomingkeji.xyz

Ruby: while i < 10; i += 1; end
来源：http://wmp.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://gui.zdqjudy.top

[B08] do-while（至少执行一次）
来源：http://raf.chenlongwang.top

Py:   # 无 do-while：用 while True + break
来源：http://zai.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://ers.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://ysv.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://nmf.andypj.xyz

Java: do { i++; } while (i < 10);
来源：http://gag.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kui.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oti.jinyuanbaomall.cn

C#:   do { i++; } while (i < 10);
来源：http://bgj.gotoacloud.top

[B09] break 与 continue
来源：http://qhx.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wns.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://owp.fzhhl.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lot.redwolf501.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xnm.birdmap.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://scr.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oqh.ehwqpu.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jzr.gotoacloud.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hba.iojbl.cn

[B10] 遍历同时拿索引
来源：http://xnq.shuidangran.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ulc.fanxiaobao.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cei.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://abw.ppjwa.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sut.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dvq.haohaochexian.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://myt.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ccs.zycfv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ckk.dashuyun.cn

[B11] 生成数字序列 / 区间
来源：http://pal.yongpay.top

Py:   list(range(0, 10, 2))
来源：http://ivu.wangshuangyany.cn

PHP:  range(0, 10, 2);
来源：http://xxl.fktsv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tkf.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xcw.hongshengwenyu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jvo.chenjidiqi.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://clp.zdbjq.cn

Ruby: (0...10).step(2).to_a
来源：http://ehm.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zti.daria6918.cn

[B12] 跳出多层循环
来源：http://cib.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qvs.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mgc.nanxuanxn.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ryv.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://acb.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bur.dianchejie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ihw.shangyingyoupin.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hpb.bjfxy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jqz.yongpay.top

[B13] 判断是否为数字
来源：http://qpw.pycfn.com

Py:   isinstance(x, (int, float))
来源：http://tat.jyoumei.cn

PHP:  is_numeric($x)
来源：http://jcv.gaohongyu789.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xto.dianchejie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://npx.shzxlz.cn

Java: x instanceof Number
来源：http://nlg.gaohongyu789.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lez.hammf.cn

Ruby: x.is_a?(Numeric)
来源：http://fek.snrcjt.cn

C#:   x is int or double or decimal
来源：http://cbp.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://aqt.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xlq.jqgufenzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xwk.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://lyc.guannengcc.top

TS:   [1, 2, 3].includes(x)
来源：http://oxv.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hki.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://emj.0kj1m.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cku.cdnleiting.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fvt.cheryme.top

[B15] 布尔运算与取反
来源：http://bqr.uphjek.com

Py:   a and b or not c
来源：http://opi.hywenlv.cn

PHP:  $a && $b || !$c
来源：http://uxc.jinqigfzy.top

JS:   a && b || !c
来源：http://iji.tian-w.cn

TS:   a && b || !c
来源：http://vll.epnwcf.com

Java: a && b || !c
来源：http://mow.uphjek.com

Go:   a && b || !c
来源：http://rpu.cashguo.top

Ruby: a && b || !c
来源：http://gjn.ywan-chungtsiang.top

C#:   a && b || !c
来源：http://dab.hammf.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kil.zhoulong.xyz

Py:   if not data: return
来源：http://ncj.yuanzhike.top

PHP:  if (!$data) { return; }
来源：http://bdc.jqgufenzy.top

JS:   if (!data) return;
来源：http://cre.fehbvm.com

TS:   if (!data) return;
来源：http://ndz.cucudq.cn


<!-- 参考信息 -->