代发 wailian999

Java: "第一行\n第二行"
来源：http://kit.sjlbkw.cn

Go:   "第一行\n第二行"
来源：http://ftj.gzhubu.top

Ruby: "第一行\n第二行"
来源：http://wrr.shanyushiyangkeji.top

C#:   "第一行\n第二行"
来源：http://gqx.yvedp.cn

[A14] 注释写法
来源：http://jgf.tanke756.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zxr.shangyingyoupin.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://tzc.zdbjq.cn

JS:   // 单行；/* 多行 */
来源：http://hfg.ehwqpu.com

TS:   // 单行；/* 多行 */
来源：http://ynk.hnqzz.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xuu.jinqigfzy.top

Go:   // 单行；/* 多行 */
来源：http://yub.bbcook.cn

Ruby: # 单行；=begin 多行 =end
来源：http://thy.jinqigufen.top

C#:   // 单行；/* 多行 */
来源：http://iil.aizwys.cn

[A15] 空值判断与默认值
来源：http://nhe.yongpay.top

Py:   value = data or "默认值"
来源：http://gmr.yuanzhike.top

PHP:  $value = $data ?? "默认值";
来源：http://duj.bbcook.cn

JS:   const value = data ?? "默认值";
来源：http://csv.feifeiyinyue.top

TS:   const value = data ?? "默认值";
来源：http://voy.vehdjk.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lxe.hesvh.cn

Go:   if data == "" { data = "默认值" }
来源：http://geg.vqdsnc.cn

Ruby: value = data || "默认值"
来源：http://vnh.birdmap.top

C#:   var value = data ?? "默认值";
来源：http://map.epnwcf.com

[A16] 真假值判断规则
来源：http://qdr.yuxming.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ihl.shanyushiyangtech.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fdj.jinqigufen.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hxs.havefunace.top

TS:   if (!x) {}
来源：http://jsn.sjlbkw.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wuf.fanxiaobao.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vef.shanyushiyangtech.top

Ruby: unless x            # nil 与 false 为假
来源：http://gew.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zbp.yfazqb.com

[A17] 位运算
来源：http://jfm.fktsv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://djp.fengsongda.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://imu.52xcode.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ebc.cashguo.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gca.fengsongda.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fze.havefunace.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wiy.sjlbkw.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gbx.mhx1999.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ual.ehwqpu.com

[A18] 字符与 ASCII 码互转
来源：http://vif.redwolf501.top

Py:   ord("A"); chr(65)
来源：http://zzk.yuxming.cn

PHP:  ord("A"); chr(65)
来源：http://zhe.xingfuxueyuan.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tcn.52xcode.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qlj.fktsv.cn

Java: (int) 'A'; (char) 65
来源：http://rgz.sufxvd.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rku.yvedp.cn

Ruby: "A".ord; 65.chr
来源：http://vuz.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://gce.yuxming.cn

[A19] 交换两个变量
来源：http://gzz.zhiwuduotai.top

Py:   a, b = b, a
来源：http://wsq.sufxvd.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fwi.fengsongda.top

JS:   [a, b] = [b, a];
来源：http://pha.xziqi.cn

TS:   [a, b] = [b, a];
来源：http://yka.cdnleiting.top

Java: int t = a; a = b; b = t;
来源：http://aaz.pycfn.com

Go:   a, b = b, a
来源：http://jvn.dashuyun.cn

Ruby: a, b = b, a
来源：http://lmc.mhx1999.top

C#:   (a, b) = (b, a);
来源：http://nvl.cashguo.top

[A20] 读取标准输入
来源：http://vgk.tianlin.xyz

Py:   name = input("请输入：")
来源：http://gro.quarkkingdee.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bvt.epnwcf.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gkb.cqqwz.cn

TS:   // Node.js：readline 模块
来源：http://ibe.dashuyun.cn

Java: new Scanner(System.in).nextLine()
来源：http://skx.bbcook.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kpt.hnqzz.top

Ruby: gets.chomp
来源：http://fdy.sjlbkw.cn

C#:   Console.ReadLine();
来源：http://vog.xylfe.cn

[A21] 保留指定小数位输出
来源：http://iqd.yanxiufei.cn

Py:   f"{3.14159:.2f}"
来源：http://wxt.daxiang520.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yyz.bjfxy.top

JS:   (3.14159).toFixed(2)
来源：http://nxt.jiagoushi.top

TS:   (3.14159).toFixed(2)
来源：http://mad.sweek.top

Java: String.format("%.2f", 3.14159)
来源：http://wbr.fanxiaobao.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ljy.zycfv.cn

Ruby: format("%.2f", 3.14159)
来源：http://eww.andypj.xyz

C#:   3.14159.ToString("F2")
来源：http://toa.ydzc1.top

[A22] 获取字符串长度
来源：http://shu.cucudq.cn

Py:   len(s)
来源：http://dal.mhx1999.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xme.svipenyu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hvz.zhengqikj.top

TS:   s.length
来源：http://xjg.meibo888.top

Java: s.length()
来源：http://ayr.c1oappe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fgg.haohaochexian.top

Ruby: s.length
来源：http://kbm.cdnleiting.top

C#:   s.Length
来源：http://vix.zhaomingkeji.xyz

[A23] 大小写转换
来源：http://wuz.yuxming.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lfg.yfazqb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jlp.yonumen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qvu.shuidangran.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lzt.shzxlz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bon.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eex.gotoacloud.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gkn.chenjidiqi.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://vtu.ivvv.top

[A24] 去除首尾空白
来源：http://xjs.pengpengdd.cyou

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bkj.yuxming.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pwe.chenjidiqi.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cof.gotoacloud.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eaa.guannengcc.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zmq.sysykeji.top

Go:   strings.TrimSpace(s)
来源：http://hzp.meibo888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cqk.jinyuanbaomall.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wur.hongshengwenyu.top

[A25] 字符串比较
来源：http://ush.jinghuilouyu.cn

Py:   s1 == s2; s1 != s2
来源：http://ogq.guowangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jcu.smart0.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xfm.hnqzz.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nht.fengsongda.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cbu.wangdashe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xbc.wangdashe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://guc.bjfxy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fza.yuxming.cn

[A26] 类型转换总览
来源：http://tpg.yj20258.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fko.jinqigfzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dsl.sweek.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vja.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://yyc.shanyushiyangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ejt.fanxiaobao.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sgc.shangyingyoupin.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vtt.9152youxi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cus.yj20258.top

================================================================================
来源：http://rwg.gaohongyu789.top

B. 流程控制
来源：http://vqv.xziqi.cn

================================================================================
来源：http://apt.uphjek.com

[B01] 条件判断 if / else
来源：http://ogy.hywenlv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sgg.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aus.tian-w.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xud.haohaochexian.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rly.nwbrower.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ebw.birdmap.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vpf.fanxiaobao.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ffo.gogol.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qsi.ydzc1.top

[B02] 多分支 else if / elif
来源：http://llc.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://haj.cashguo.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pyp.hywenlv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofh.nanxuanxn.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xpk.jqgfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lsi.meibo888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tvl.xziqi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://erv.aizwys.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://umq.havefunace.top

[B03] switch / match / case
来源：http://swx.sweek.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cjq.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dns.tarul.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jta.zycfv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jbv.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nce.havefunace.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://azg.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ypo.jqgfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jtg.zhaomingkeji.xyz

[B04] for 计数循环
来源：http://oua.redwolf501.top

Py:   for i in range(10): print(i)
来源：http://tdu.uphjek.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dpu.52xcode.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ooi.yfazqb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zeq.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lxl.hongshengwenyu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yct.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://pzj.zycfv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sct.pycfn.com

[B05] 遍历数组 / 列表
来源：http://zpi.birdmap.top

Py:   for item in arr: print(item)
来源：http://zix.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jop.chenjidiqi.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://xxg.sxryk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pau.nanxuanxn.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://knm.xinyue.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mqs.zhixingplan.top

Ruby: arr.each { |item| puts item }
来源：http://ufp.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rki.zhengqikj.top

[B06] 遍历字典 / 对象
来源：http://xjg.cucudq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pjr.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yvu.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://reb.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sxi.gogol.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hnq.tianlin.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vuo.ppjwa.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pyq.fktsv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://osy.zhaomingkeji.xyz

[B07] while 循环
来源：http://orm.hnxiangtu.top

Py:   while i < 10: i += 1
来源：http://dyj.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://fpy.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://kvv.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://dwn.mhx1999.top

Java: while (i < 10) { i++; }
来源：http://xvl.wangshuangyany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lxh.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://met.0kj1m.cn

C#:   while (i < 10) { i++; }
来源：http://wra.zhiwuduotai.top

[B08] do-while（至少执行一次）
来源：http://yoy.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://xie.tian-w.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jow.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://dah.meibo888.top

TS:   do { i++; } while (i < 10);
来源：http://qas.tanke756.top

Java: do { i++; } while (i < 10);
来源：http://qsn.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fom.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://dan.jinqigfzy.top

C#:   do { i++; } while (i < 10);
来源：http://occ.yueranfly.top

[B09] break 与 continue
来源：http://gvp.xingfuxueyuan.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://acz.pengpengdd.cyou

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cli.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oez.meibo888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zix.jqgufenzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wxx.feifeiyinyue.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zpg.chenlongwang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yii.0kj1m.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yfy.zhixingplan.top

[B10] 遍历同时拿索引
来源：http://pmi.shuidangran.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bqc.sjlbkw.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bgk.ehwqpu.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xvz.xziqi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mtc.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://csn.xziqi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://emg.chenzaomai.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wxb.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kyq.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://cya.zhijiandao.cn

Py:   list(range(0, 10, 2))
来源：http://gex.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://kpa.hysaishi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bga.mhx1999.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ufy.sweek.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pet.guannengcc.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pzk.tanke756.top

Ruby: (0...10).step(2).to_a
来源：http://jik.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zse.kuanghao11.cn

[B12] 跳出多层循环
来源：http://izq.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://shp.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cjq.kuanghao11.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gvw.316326.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wes.xingfuxueyuan.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ctb.nanxuanxn.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ovv.zhixingplan.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ucp.hammf.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qbz.kuanghao11.cn

[B13] 判断是否为数字
来源：http://wyo.jinqigfzy.top

Py:   isinstance(x, (int, float))
来源：http://byg.hammf.cn

PHP:  is_numeric($x)
来源：http://fij.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rti.wangdashe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vxs.zhixingplan.top

Java: x instanceof Number
来源：http://iap.ydzc1.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://shf.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://huf.guannengcc.top

C#:   x is int or double or decimal
来源：http://rts.pycfn.com

[B14] 判断值是否在集合内
来源：http://ltq.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qxp.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pjm.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://uiy.bjfxy.top

TS:   [1, 2, 3].includes(x)
来源：http://ffy.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://srf.hammf.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ozp.sufxvd.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gkv.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://spf.xinyue.icu

[B15] 布尔运算与取反
来源：http://bgg.nanxinkj.top

Py:   a and b or not c
来源：http://lez.redwolf501.top

PHP:  $a && $b || !$c
来源：http://sfn.ybcxt.top

JS:   a && b || !c
来源：http://foz.shanyushiyangkeji.top

TS:   a && b || !c
来源：http://cvk.yj20258888.top

Java: a && b || !c
来源：http://qlf.ivvv.top

Go:   a && b || !c
来源：http://cuz.cucudq.cn

Ruby: a && b || !c
来源：http://zhw.gogol.net.cn

C#:   a && b || !c
来源：http://tnw.ydzc1.top

[B16] 卫语句：不满足条件提前返回
来源：http://kut.ctjpmb.com

Py:   if not data: return
来源：http://ihx.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://ufr.yj20258888.top

JS:   if (!data) return;
来源：http://xgq.nwbrower.top

TS:   if (!data) return;
来源：http://rbf.quarkkingdee.top

Java: if (data == null) return;
来源：http://mtr.gzhubu.top

Go:   if data == nil { return }
来源：http://abn.fanxiaobao.xyz

Ruby: return if data.nil?
来源：http://fak.jqgufenzy.top

C#:   if (data == null) return;
来源：http://dco.svipenyu.cn

================================================================================
来源：http://jum.quarkkingdee.top

C. 函数与作用域
来源：http://emh.haohaochexian.top

================================================================================
来源：http://ndp.smart0.xyz

[C01] 定义函数
来源：http://vzl.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://dfm.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ndc.guannengcc.top

JS:   function add(a, b) { return a + b; }
来源：http://kpd.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kjj.fktsv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fsi.shuidangran.top

Go:   func add(a, b int) int { return a + b }
来源：http://hgv.gzhubu.top

Ruby: def add(a, b); a + b; end
来源：http://gzw.shanyushiyangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dbn.ydjk.org.cn

[C02] 默认参数
来源：http://zui.chenjidiqi.icu

Py:   def greet(name="World"): return name
来源：http://ljg.haohaochexian.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yaj.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://jhs.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wtu.dianchejie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nux.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://elk.shanyushiyangtech.top

Ruby: def greet(name = "World") = name
来源：http://fdz.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://ioy.nwbrower.top

[C03] 可变参数
来源：http://goo.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://lol.jyoumei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://trw.wangdashe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wrm.ivvv.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wqo.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://apd.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://win.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://tyi.hesvh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tyq.cheryme.top

[C04] 命名参数 / 关键字参数
来源：http://gjx.hammf.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lgb.hnqzz.top


<!-- 参考信息 -->