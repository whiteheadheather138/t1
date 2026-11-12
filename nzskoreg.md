代发 wailian999

[A10] 生成随机数
来源：http://ewm.pycfn.com

Py:   import random; random.randint(1, 100)
来源：http://oul.0kj1m.cn

PHP:  random_int(1, 100);
来源：http://rgf.zhaomingkeji.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bke.zhaomingkeji.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dtm.0kj1m.cn

Java: new Random().nextInt(100) + 1
来源：http://fdj.birdmap.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dap.hammf.cn

Ruby: rand(1..100)
来源：http://ahc.cheryme.top

C#:   new Random().Next(1, 101)
来源：http://dei.guannengcc.top

[A11] 条件表达式（三元）
来源：http://gev.tianlin.xyz

Py:   "yes" if x > 0 else "no"
来源：http://nzb.chenzaomai.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://snb.xziqi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hvk.tanke756.top

TS:   x > 0 ? "yes" : "no"
来源：http://mnu.52xcode.cn

Java: x > 0 ? "yes" : "no"
来源：http://jqn.hesvh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yyj.bbcook.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bfn.shuidangran.top

C#:   x > 0 ? "yes" : "no"
来源：http://qnl.yuxming.cn

[A12] 字符串插值 / 格式化
来源：http://fsl.c1oappe.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bqf.yuxming.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://afo.mhx1999.top

JS:   `Hello, ${name}!`
来源：http://nfy.gotoacloud.top

TS:   `Hello, ${name}!`
来源：http://xlg.jyoumei.cn

Java: "Hello, %s!".formatted(name)
来源：http://yhq.yj202588.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pru.daria6918.cn

Ruby: "Hello, #{name}!"
来源：http://qis.epnwcf.com

C#:   $"Hello, {name}!"
来源：http://nng.guannengcc.top

[A13] 多行字符串（练习 \n 转义）
来源：http://sjk.haohaochexian.top

Py:   "第一行\n第二行"
来源：http://rzk.jianghu66.top

PHP:  "第一行\n第二行"
来源：http://onf.haohaochexian.top

JS:   "第一行\n第二行"
来源：http://jiy.0kj1m.cn

TS:   "第一行\n第二行"
来源：http://pyq.jinyuanbaomall.cn

Java: "第一行\n第二行"
来源：http://fnl.gzhubu.top

Go:   "第一行\n第二行"
来源：http://ofw.cqqwz.cn

Ruby: "第一行\n第二行"
来源：http://zxy.epnwcf.com

C#:   "第一行\n第二行"
来源：http://lnf.zhoulong.xyz

[A14] 注释写法
来源：http://qzg.tarul.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oxn.pengpengdd.cyou

PHP:  // 或 # 单行；/* 多行 */
来源：http://aue.ctjpmb.com

JS:   // 单行；/* 多行 */
来源：http://ale.yuanzhike.top

TS:   // 单行；/* 多行 */
来源：http://vgf.wangshuangyany.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dlm.ctjpmb.com

Go:   // 单行；/* 多行 */
来源：http://kph.zhengqikj.top

Ruby: # 单行；=begin 多行 =end
来源：http://rcw.tarul.cn

C#:   // 单行；/* 多行 */
来源：http://pbz.yuxming.cn

[A15] 空值判断与默认值
来源：http://jfb.hnqzz.top

Py:   value = data or "默认值"
来源：http://qxs.zdqjudy.top

PHP:  $value = $data ?? "默认值";
来源：http://fff.nwbrower.top

JS:   const value = data ?? "默认值";
来源：http://vaq.meibo888.top

TS:   const value = data ?? "默认值";
来源：http://dqp.snrcjt.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dak.zhixingplan.top

Go:   if data == "" { data = "默认值" }
来源：http://tqz.nanxuanxn.top

Ruby: value = data || "默认值"
来源：http://qpt.shangyingyoupin.top

C#:   var value = data ?? "默认值";
来源：http://abr.ybcxt.top

[A16] 真假值判断规则
来源：http://dzg.c1oappe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ffl.jinqigufen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dmz.daria6918.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qlz.snrcjt.cn

TS:   if (!x) {}
来源：http://lyr.yonumen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zyp.ppjwa.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pxy.redwolf501.top

Ruby: unless x            # nil 与 false 为假
来源：http://jcw.andypj.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dri.chenlongwang.top

[A17] 位运算
来源：http://wrj.cdnleiting.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://srt.daxiang520.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pkn.9152youxi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nqs.gaohongyu789.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wki.pycfn.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sxj.quarkkingdee.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lft.hammf.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tue.ctjpmb.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xmt.zhoulong.xyz

[A18] 字符与 ASCII 码互转
来源：http://szl.tianlin.xyz

Py:   ord("A"); chr(65)
来源：http://nat.ywan-chungtsiang.top

PHP:  ord("A"); chr(65)
来源：http://krb.ivvv.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cth.jinyuanbaomall.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zzs.c1oappe.top

Java: (int) 'A'; (char) 65
来源：http://pyh.chenlongwang.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dzi.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://tfq.pycfn.com

C#:   (int)'A'; (char)65
来源：http://pcs.ydzc1.top

[A19] 交换两个变量
来源：http://dki.vehdjk.com

Py:   a, b = b, a
来源：http://pvo.zhiwuduotai.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pmg.jinyuanbaomall.cn

JS:   [a, b] = [b, a];
来源：http://bis.xziqi.cn

TS:   [a, b] = [b, a];
来源：http://lvr.yj202588.top

Java: int t = a; a = b; b = t;
来源：http://bdd.ydzc1.top

Go:   a, b = b, a
来源：http://ply.cheryme.top

Ruby: a, b = b, a
来源：http://bij.sxryk.cn

C#:   (a, b) = (b, a);
来源：http://toh.nanxinkj.top

[A20] 读取标准输入
来源：http://ryn.hfpthk.cn

Py:   name = input("请输入：")
来源：http://trk.nwbrower.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hxe.jinqigufen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wsb.hywenlv.cn

TS:   // Node.js：readline 模块
来源：http://ylg.zdbjq.cn

Java: new Scanner(System.in).nextLine()
来源：http://rkf.svipenyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rnn.jinqigufen.top

Ruby: gets.chomp
来源：http://fvn.sjlbkw.cn

C#:   Console.ReadLine();
来源：http://nqm.52xcode.cn

[A21] 保留指定小数位输出
来源：http://qko.zhijiandao.cn

Py:   f"{3.14159:.2f}"
来源：http://cpk.haohaochexian.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iod.cqqwz.cn

JS:   (3.14159).toFixed(2)
来源：http://jjl.c1oappe.top

TS:   (3.14159).toFixed(2)
来源：http://maf.ctjpmb.com

Java: String.format("%.2f", 3.14159)
来源：http://wtm.sufxvd.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tfh.zhongyouzk.top

Ruby: format("%.2f", 3.14159)
来源：http://ivo.jinyuanbaomall.cn

C#:   3.14159.ToString("F2")
来源：http://sge.yj202588.top

[A22] 获取字符串长度
来源：http://poz.jinqigfzy.top

Py:   len(s)
来源：http://pqf.xuanzx.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mek.316326.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://grx.hnxiangtu.top

TS:   s.length
来源：http://ain.316326.xyz

Java: s.length()
来源：http://vxq.0kj1m.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://msz.yuxming.cn

Ruby: s.length
来源：http://vtd.epnwcf.com

C#:   s.Length
来源：http://mgr.0kj1m.cn

[A23] 大小写转换
来源：http://oij.zhongyouzk.top

Py:   s.upper(); s.lower(); s.title()
来源：http://jfk.zhoulong.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gxp.aizwys.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yfz.gzhubu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lca.hcnkem.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aca.gotoacloud.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rov.yvedp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pgm.cucudq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://car.yonumen.top

[A24] 去除首尾空白
来源：http://sdt.redwolf501.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qqu.yongpay.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://imn.9152youxi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://coj.cqqwz.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nzk.jiagoushi.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gqz.nanxuanxn.top

Go:   strings.TrimSpace(s)
来源：http://iiu.shangyingyoupin.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cnx.jinghuilouyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ehy.ehwqpu.com

[A25] 字符串比较
来源：http://efn.vehdjk.com

Py:   s1 == s2; s1 != s2
来源：http://ewh.hesvh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hyc.vqdsnc.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hyv.gogol.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://syz.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zwk.ydjk.org.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wfs.tian-w.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rtc.smart0.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gfx.0kj1m.cn

[A26] 类型转换总览
来源：http://qbc.gotoacloud.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bbb.xingfuxueyuan.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hmh.xylfe.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tfi.zhaomingkeji.xyz

TS:   Number() String() Boolean() x as number
来源：http://zks.gaohongyu789.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dxp.sxryk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://krw.vqdsnc.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yfj.gotoacloud.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kvo.shzxlz.cn

================================================================================
来源：http://wkt.hesvh.cn

B. 流程控制
来源：http://csi.sjlbkw.cn

================================================================================
来源：http://yjl.zhaomingkeji.xyz

[B01] 条件判断 if / else
来源：http://hwl.jinqigfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://til.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xsk.uphjek.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vck.shangyingyoupin.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vzf.zdqjudy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://usa.yj20258888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lco.kuanghao11.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mmr.jyoumei.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://szs.sufxvd.cn

[B02] 多分支 else if / elif
来源：http://bap.wangshuangyany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kys.jiagoushi.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mhn.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pwb.hysaishi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oaw.hnxiangtu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wfk.shanyushiyangtech.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kub.sysykeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://frz.ydjk.org.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyf.jinqigfzy.top

[B03] switch / match / case
来源：http://eta.zdqjudy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nar.shuidangran.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cei.yanxiufei.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zek.shanyushiyangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://izj.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://swx.yuxming.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tvf.jinqigfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nsv.andypj.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ynb.tanke756.top

[B04] for 计数循环
来源：http://ctl.zhixingplan.top

Py:   for i in range(10): print(i)
来源：http://qar.zhongyouzk.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zwb.zdbjq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ljr.xingfuxueyuan.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gol.zhijiandao.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xbu.bjfxy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wnn.chenzaomai.com

Ruby: 10.times { |i| puts i }
来源：http://cby.hammf.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vdi.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://gvv.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://kiy.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lhk.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qwl.guannengcc.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ouu.wangshuangyany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sxg.fehbvm.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hex.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://xdg.zycfv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kox.fzhhl.top

[B06] 遍历字典 / 对象
来源：http://mim.zhaomingkeji.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://rij.pycfn.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bti.zycfv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://deb.hysaishi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tse.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nah.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nbs.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ipt.yj20258.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mns.hcnkem.com

[B07] while 循环
来源：http://log.yueranfly.top

Py:   while i < 10: i += 1
来源：http://ezx.kuanghao11.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nhr.xingfuxueyuan.xyz

JS:   while (i < 10) { i++; }
来源：http://zcy.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://wrj.aibaodan.cn

Java: while (i < 10) { i++; }
来源：http://kir.ppjwa.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://trg.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://mkw.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://qzm.c1oappe.top

[B08] do-while（至少执行一次）
来源：http://hiq.quarkkingdee.top

Py:   # 无 do-while：用 while True + break
来源：http://mdw.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mqy.pycfn.com

JS:   do { i++; } while (i < 10);
来源：http://ylz.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://kmz.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://dtc.hcnkem.com

Go:   for { i++; if i >= 10 { break } }
来源：http://vpa.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ulu.nanxuanxn.top

C#:   do { i++; } while (i < 10);
来源：http://vvi.ydzc1.top

[B09] break 与 continue
来源：http://cra.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qlr.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yfl.jinqigfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fdf.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ovd.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lwd.zhiwuduotai.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://omj.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rvu.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xss.nwbrower.top

[B10] 遍历同时拿索引
来源：http://oke.cucudq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oky.ivvv.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vpf.sufxvd.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cbs.hnxiangtu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cee.fzhhl.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hvv.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cli.zycfv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ptz.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://klb.sufxvd.cn

[B11] 生成数字序列 / 区间
来源：http://fnh.shuidangran.top

Py:   list(range(0, 10, 2))
来源：http://gmt.9152youxi.cn

PHP:  range(0, 10, 2);
来源：http://iuv.sxryk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fzk.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://woj.jinyuanbaomall.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lpf.jianghu66.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ccw.yonumen.top

Ruby: (0...10).step(2).to_a
来源：http://bvq.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wgk.yueranfly.top

[B12] 跳出多层循环
来源：http://mac.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gsk.zhixingplan.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qyd.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dsy.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lmw.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iom.ehwqpu.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aup.epnwcf.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jnv.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mdo.hammf.cn

[B13] 判断是否为数字
来源：http://fty.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://iqj.jinqigufen.top

PHP:  is_numeric($x)
来源：http://slf.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dpq.svipenyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hfj.guannengcc.top

Java: x instanceof Number
来源：http://gyb.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cdy.jinqigufen.top

Ruby: x.is_a?(Numeric)
来源：http://wbb.zhengqikj.top

C#:   x is int or double or decimal
来源：http://awq.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://gls.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hpx.vehdjk.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pka.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://rxq.yj20258.top

TS:   [1, 2, 3].includes(x)
来源：http://frk.yangfankeji.com

Java: List.of(1, 2, 3).contains(x)
来源：http://zdg.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://olw.xylfe.cn

Ruby: [1, 2, 3].include?(x)
来源：http://spy.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aez.jianghu66.top

[B15] 布尔运算与取反
来源：http://jvz.vqdsnc.cn

Py:   a and b or not c
来源：http://wma.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://npx.aizwys.cn

JS:   a && b || !c
来源：http://ctt.xuanzx.com

TS:   a && b || !c
来源：http://mwf.0kj1m.cn

Java: a && b || !c
来源：http://hey.havefunace.top

Go:   a && b || !c
来源：http://hpl.fanxiaobao.xyz

Ruby: a && b || !c
来源：http://ehl.meibo888.top

C#:   a && b || !c
来源：http://mmy.zhengqikj.top

[B16] 卫语句：不满足条件提前返回
来源：http://and.fanxiaobao.xyz

Py:   if not data: return
来源：http://roz.hammf.cn

PHP:  if (!$data) { return; }
来源：http://jrz.hfpthk.cn

JS:   if (!data) return;
来源：http://ihv.hongshengwenyu.top

TS:   if (!data) return;
来源：http://uht.zycfv.cn

Java: if (data == null) return;
来源：http://ftw.guannengcc.top

Go:   if data == nil { return }
来源：http://fdk.wangdashe.top

Ruby: return if data.nil?
来源：http://kbw.tianlin.xyz

C#:   if (data == null) return;
来源：http://qym.feifeiyinyue.top


<!-- 参考信息 -->