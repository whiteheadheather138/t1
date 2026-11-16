代发 wailian999

[A10] 生成随机数
来源：http://kfn.yj20258.top

Py:   import random; random.randint(1, 100)
来源：http://rls.ehwqpu.com

PHP:  random_int(1, 100);
来源：http://xux.zdbjq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nsp.0kj1m.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eyu.dianchejie.cn

Java: new Random().nextInt(100) + 1
来源：http://awa.aibaodan.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ltc.ybcxt.top

Ruby: rand(1..100)
来源：http://ayw.bjfxy.top

C#:   new Random().Next(1, 101)
来源：http://rin.zhoulong.xyz

[A11] 条件表达式（三元）
来源：http://kmu.chenjidiqi.icu

Py:   "yes" if x > 0 else "no"
来源：http://ans.sweek.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://dru.jiagoushi.top

JS:   x > 0 ? "yes" : "no"
来源：http://lkb.cqqwz.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dxo.birdmap.top

Java: x > 0 ? "yes" : "no"
来源：http://hdf.gotoacloud.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dbq.wangdashe.top

Ruby: x > 0 ? "yes" : "no"
来源：http://hfn.fzhhl.top

C#:   x > 0 ? "yes" : "no"
来源：http://kgr.vehdjk.com

[A12] 字符串插值 / 格式化
来源：http://mnw.jianghu66.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xta.xinyue.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://okp.hfpthk.cn

JS:   `Hello, ${name}!`
来源：http://afg.aibaodan.cn

TS:   `Hello, ${name}!`
来源：http://dxk.xylfe.cn

Java: "Hello, %s!".formatted(name)
来源：http://lkq.fzhhl.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wcx.hammf.cn

Ruby: "Hello, #{name}!"
来源：http://cbp.hysaishi.cn

C#:   $"Hello, {name}!"
来源：http://iee.yanxiufei.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vgn.guowangkeji.top

Py:   "第一行\n第二行"
来源：http://ysf.jinyuanbaomall.cn

PHP:  "第一行\n第二行"
来源：http://vuf.aibaodan.cn

JS:   "第一行\n第二行"
来源：http://yof.ppjwa.cn

TS:   "第一行\n第二行"
来源：http://xok.zhijiandao.cn

Java: "第一行\n第二行"
来源：http://jtu.52xcode.cn

Go:   "第一行\n第二行"
来源：http://jyn.gotoacloud.top

Ruby: "第一行\n第二行"
来源：http://ppc.yvedp.cn

C#:   "第一行\n第二行"
来源：http://jxg.jqgufenzy.top

[A14] 注释写法
来源：http://wlk.shzxlz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fak.nanxuanxn.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://how.xylfe.cn

JS:   // 单行；/* 多行 */
来源：http://bti.tarul.cn

TS:   // 单行；/* 多行 */
来源：http://dxk.yangfankeji.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rkd.chenzaomai.com

Go:   // 单行；/* 多行 */
来源：http://jis.ivvv.top

Ruby: # 单行；=begin 多行 =end
来源：http://dni.feifeiyinyue.top

C#:   // 单行；/* 多行 */
来源：http://ydz.birdmap.top

[A15] 空值判断与默认值
来源：http://jpn.xuanzx.com

Py:   value = data or "默认值"
来源：http://dxn.haohaochexian.top

PHP:  $value = $data ?? "默认值";
来源：http://ktd.jlsjyb.cn

JS:   const value = data ?? "默认值";
来源：http://oes.yonumen.top

TS:   const value = data ?? "默认值";
来源：http://eks.tarul.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://peb.yongpay.top

Go:   if data == "" { data = "默认值" }
来源：http://bvt.xziqi.cn

Ruby: value = data || "默认值"
来源：http://xqo.snrcjt.cn

C#:   var value = data ?? "默认值";
来源：http://wok.sjlbkw.cn

[A16] 真假值判断规则
来源：http://uyq.jinyuanbaomall.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wts.ctjpmb.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vpg.zhixingplan.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ynq.zhongyouzk.top

TS:   if (!x) {}
来源：http://oww.hnqzz.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xdg.smart0.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wos.shangyingyoupin.top

Ruby: unless x            # nil 与 false 为假
来源：http://gdv.ctjpmb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cog.smart0.xyz

[A17] 位运算
来源：http://roo.feifeiyinyue.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vru.haohaochexian.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gpt.tanke756.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cgt.nanxinkj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rbz.nwbrower.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pzx.yj202588.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fxp.jyoumei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mgm.sxryk.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://olz.316326.xyz

[A18] 字符与 ASCII 码互转
来源：http://uhf.mhx1999.top

Py:   ord("A"); chr(65)
来源：http://dlj.cdnleiting.top

PHP:  ord("A"); chr(65)
来源：http://xmc.daxiang520.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ojj.xylfe.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gfp.vqdsnc.cn

Java: (int) 'A'; (char) 65
来源：http://iec.zhixingplan.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://khz.jinqigufen.top

Ruby: "A".ord; 65.chr
来源：http://tdt.cheryme.top

C#:   (int)'A'; (char)65
来源：http://xfx.zhengqikj.top

[A19] 交换两个变量
来源：http://xxu.zhiwuduotai.top

Py:   a, b = b, a
来源：http://zcg.jlsjyb.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rcc.andypj.xyz

JS:   [a, b] = [b, a];
来源：http://pto.fzhhl.top

TS:   [a, b] = [b, a];
来源：http://pmz.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://qld.hesvh.cn

Go:   a, b = b, a
来源：http://wyo.jlsjyb.cn

Ruby: a, b = b, a
来源：http://gxv.jinqigufen.top

C#:   (a, b) = (b, a);
来源：http://zef.jianghu66.top

[A20] 读取标准输入
来源：http://eof.hammf.cn

Py:   name = input("请输入：")
来源：http://tvo.cucudq.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kfe.zhaomingkeji.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://twl.kuanghao11.cn

TS:   // Node.js：readline 模块
来源：http://kjx.ppjwa.cn

Java: new Scanner(System.in).nextLine()
来源：http://xzh.ydjk.org.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bhq.yj202588.top

Ruby: gets.chomp
来源：http://imh.xingfuxueyuan.xyz

C#:   Console.ReadLine();
来源：http://mnj.hongshengwenyu.top

[A21] 保留指定小数位输出
来源：http://ycw.gotoacloud.top

Py:   f"{3.14159:.2f}"
来源：http://fii.cucudq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bgi.chenlongwang.top

JS:   (3.14159).toFixed(2)
来源：http://sqw.9152youxi.cn

TS:   (3.14159).toFixed(2)
来源：http://guc.iojbl.cn

Java: String.format("%.2f", 3.14159)
来源：http://iiv.hongshengwenyu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://osq.hysaishi.cn

Ruby: format("%.2f", 3.14159)
来源：http://bnf.0kj1m.cn

C#:   3.14159.ToString("F2")
来源：http://wyr.gogol.net.cn

[A22] 获取字符串长度
来源：http://pki.xuetiantiany.cn

Py:   len(s)
来源：http://yhc.daria6918.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cnd.yj20258888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gne.havefunace.top

TS:   s.length
来源：http://pxu.jqgufenzy.top

Java: s.length()
来源：http://aex.hongshengwenyu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gbs.zycfv.cn

Ruby: s.length
来源：http://kat.jiagoushi.top

C#:   s.Length
来源：http://krb.jinqigfzy.top

[A23] 大小写转换
来源：http://doq.snrcjt.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://klp.xziqi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kux.dianchejie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wqw.sxryk.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iyw.uphjek.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hya.gzhubu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ots.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mcp.zhengqikj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://npk.mhx1999.top

[A24] 去除首尾空白
来源：http://run.zdqjudy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nkv.tianlin.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qdj.guowangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ldp.jinqigfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wwm.dashuyun.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fpu.ybcxt.top

Go:   strings.TrimSpace(s)
来源：http://sen.ehwqpu.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lvl.316326.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pzw.52xcode.cn

[A25] 字符串比较
来源：http://llq.svipenyu.cn

Py:   s1 == s2; s1 != s2
来源：http://qzo.ppjwa.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://joo.haohaochexian.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ris.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://shk.hfpthk.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ilm.jyoumei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gea.jqgufenzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qte.zhengqikj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ntk.xinyue.icu

[A26] 类型转换总览
来源：http://fmg.shanyushiyangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wtk.guowangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xav.yueranfly.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yhx.hfpthk.cn

TS:   Number() String() Boolean() x as number
来源：http://lbj.jinyuanbaomall.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://czl.yvedp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zhb.fehbvm.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://sob.hysaishi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ady.hongshengwenyu.top

================================================================================
来源：http://oli.svipenyu.cn

B. 流程控制
来源：http://zdj.cucudq.cn

================================================================================
来源：http://ptm.ppjwa.cn

[B01] 条件判断 if / else
来源：http://ojm.jqgufenzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zsl.shanyushiyangtech.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dpp.chenzaomai.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://okh.sysykeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://axm.zhongyouzk.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vmx.fengsongda.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ywl.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://koy.ydjk.org.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jrt.ivvv.top

[B02] 多分支 else if / elif
来源：http://has.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vxr.0kj1m.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lww.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dnf.tarul.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bft.yvedp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://edh.kuanghao11.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lpw.yangfankeji.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eda.shanyushiyangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yah.zdbjq.cn

[B03] switch / match / case
来源：http://gkb.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qqy.hnqzz.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gbq.yangfankeji.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bry.jinqigfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ghy.gaohongyu789.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hpe.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vpi.wangdashe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qam.yj20258.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ahm.yuanzhike.top

[B04] for 计数循环
来源：http://gyl.ehwqpu.com

Py:   for i in range(10): print(i)
来源：http://kca.xylfe.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lie.ydjk.org.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://glz.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pgy.sjlbkw.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bck.guowangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gjn.cdnleiting.top

Ruby: 10.times { |i| puts i }
来源：http://ibg.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wqr.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://sgk.aizwys.cn

Py:   for item in arr: print(item)
来源：http://tqx.sweek.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jqo.cashguo.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cly.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cua.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wdb.yangfankeji.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://edw.havefunace.top

Ruby: arr.each { |item| puts item }
来源：http://tqd.gzhubu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qot.hammf.cn

[B06] 遍历字典 / 对象
来源：http://xra.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rdh.zhengqikj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jqn.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://glz.ywan-chungtsiang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iua.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xht.dianchejie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pkh.jlsjyb.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qhx.ehwqpu.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oqm.yueranfly.top

[B07] while 循环
来源：http://udn.cheryme.top

Py:   while i < 10: i += 1
来源：http://bfi.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hrc.cheryme.top

JS:   while (i < 10) { i++; }
来源：http://syi.epnwcf.com

TS:   while (i < 10) { i++; }
来源：http://tsk.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://tvl.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iyy.zhengqikj.top

Ruby: while i < 10; i += 1; end
来源：http://nft.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://ime.vehdjk.com

[B08] do-while（至少执行一次）
来源：http://awa.jqgfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://czy.zhaomingkeji.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://pwz.mhx1999.top

JS:   do { i++; } while (i < 10);
来源：http://kae.hnxiangtu.top

TS:   do { i++; } while (i < 10);
来源：http://gei.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://vjo.zhixingplan.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jop.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://qhv.epnwcf.com

C#:   do { i++; } while (i < 10);
来源：http://iws.dashuyun.cn

[B09] break 与 continue
来源：http://rsh.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://omb.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://opb.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bxg.shzxlz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lpj.uphjek.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ndq.tarul.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hfx.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mxg.birdmap.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ors.xylfe.cn

[B10] 遍历同时拿索引
来源：http://gis.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tmv.fehbvm.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qip.gotoacloud.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rix.316326.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rov.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ovx.yj202588.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ktg.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kdp.bjfxy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://auu.9152youxi.cn

[B11] 生成数字序列 / 区间
来源：http://fll.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://wbr.yonumen.top

PHP:  range(0, 10, 2);
来源：http://bma.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ybt.gaohongyu789.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uim.havefunace.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bjg.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wvu.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://iuz.xingfuxueyuan.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xjs.fanxiaobao.xyz

[B12] 跳出多层循环
来源：http://zbq.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hng.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bgf.sweek.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xvk.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aed.hfpthk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qgd.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sjz.kuanghao11.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hjr.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yfc.vqdsnc.cn

[B13] 判断是否为数字
来源：http://qsp.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://wik.haohaochexian.top

PHP:  is_numeric($x)
来源：http://zev.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ivz.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://puk.ybcxt.top

Java: x instanceof Number
来源：http://myf.shuidangran.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mlg.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://sjd.cdnleiting.top

C#:   x is int or double or decimal
来源：http://usq.gogol.net.cn

[B14] 判断值是否在集合内
来源：http://eod.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hls.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ikx.epnwcf.com

JS:   [1, 2, 3].includes(x)
来源：http://twp.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://mzc.316326.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://amc.hnqzz.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vkz.fehbvm.com

Ruby: [1, 2, 3].include?(x)
来源：http://vuk.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nzb.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://cev.shanyushiyangtech.top

Py:   a and b or not c
来源：http://qth.havefunace.top

PHP:  $a && $b || !$c
来源：http://zkp.cucudq.cn

JS:   a && b || !c
来源：http://aub.jinghuilouyu.cn

TS:   a && b || !c
来源：http://gyr.bbcook.cn

Java: a && b || !c
来源：http://lks.guannengcc.top

Go:   a && b || !c
来源：http://fdl.yueranfly.top

Ruby: a && b || !c
来源：http://hjj.jqgfzy.top

C#:   a && b || !c
来源：http://bfi.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://zzc.hywenlv.cn

Py:   if not data: return
来源：http://opi.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://pil.xziqi.cn

JS:   if (!data) return;
来源：http://lkt.chenzaomai.com

TS:   if (!data) return;
来源：http://pnv.c1oappe.top

Java: if (data == null) return;
来源：http://nfl.xziqi.cn

Go:   if data == nil { return }
来源：http://lap.iojbl.cn

Ruby: return if data.nil?
来源：http://jlh.gotoacloud.top

C#:   if (data == null) return;
来源：http://vrd.mhx1999.top


<!-- 参考信息 -->