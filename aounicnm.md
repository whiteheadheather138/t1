代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mpd.zhijiandao.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bgs.uphjek.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iaj.jqgfzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tir.sufxvd.cn

[A10] 生成随机数
来源：http://nyv.ehwqpu.com

Py:   import random; random.randint(1, 100)
来源：http://jqm.zdbjq.cn

PHP:  random_int(1, 100);
来源：http://wfn.yonumen.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://psk.jinqigufen.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lnm.zhengqikj.top

Java: new Random().nextInt(100) + 1
来源：http://gck.ppjwa.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yoe.jianghu66.top

Ruby: rand(1..100)
来源：http://aqo.ehwqpu.com

C#:   new Random().Next(1, 101)
来源：http://tlr.zdqjudy.top

[A11] 条件表达式（三元）
来源：http://myf.hywenlv.cn

Py:   "yes" if x > 0 else "no"
来源：http://vyq.cashguo.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kvs.ppjwa.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bcn.daxiang520.top

TS:   x > 0 ? "yes" : "no"
来源：http://nym.hnqzz.top

Java: x > 0 ? "yes" : "no"
来源：http://wvi.nwbrower.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hni.jqgufenzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://owz.gaohongyu789.top

C#:   x > 0 ? "yes" : "no"
来源：http://few.9152youxi.cn

[A12] 字符串插值 / 格式化
来源：http://jzm.yj202588.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://joc.daxiang520.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xyu.xingfuxueyuan.xyz

JS:   `Hello, ${name}!`
来源：http://bcx.yuanzhike.top

TS:   `Hello, ${name}!`
来源：http://qzx.sufxvd.cn

Java: "Hello, %s!".formatted(name)
来源：http://dzc.wangdashe.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eay.jiagoushi.top

Ruby: "Hello, #{name}!"
来源：http://bdj.vehdjk.com

C#:   $"Hello, {name}!"
来源：http://mfs.wangdashe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lfn.hysaishi.cn

Py:   "第一行\n第二行"
来源：http://edn.sysykeji.top

PHP:  "第一行\n第二行"
来源：http://bvv.vqdsnc.cn

JS:   "第一行\n第二行"
来源：http://evu.hnxiangtu.top

TS:   "第一行\n第二行"
来源：http://brr.yuxming.cn

Java: "第一行\n第二行"
来源：http://rzq.birdmap.top

Go:   "第一行\n第二行"
来源：http://zxk.hnqzz.top

Ruby: "第一行\n第二行"
来源：http://aqh.pengpengdd.cyou

C#:   "第一行\n第二行"
来源：http://nkk.jlsjyb.cn

[A14] 注释写法
来源：http://dql.jyoumei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cgj.zhixingplan.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://zbq.gzhubu.top

JS:   // 单行；/* 多行 */
来源：http://wfh.sjlbkw.cn

TS:   // 单行；/* 多行 */
来源：http://kvp.zhoulong.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qin.mhx1999.top

Go:   // 单行；/* 多行 */
来源：http://sqz.hfpthk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ota.yvedp.cn

C#:   // 单行；/* 多行 */
来源：http://gmw.gotoacloud.top

[A15] 空值判断与默认值
来源：http://nfq.0kj1m.cn

Py:   value = data or "默认值"
来源：http://unn.redwolf501.top

PHP:  $value = $data ?? "默认值";
来源：http://mva.hongshengwenyu.top

JS:   const value = data ?? "默认值";
来源：http://huo.zhoulong.xyz

TS:   const value = data ?? "默认值";
来源：http://mlb.xylfe.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xba.9152youxi.cn

Go:   if data == "" { data = "默认值" }
来源：http://ovg.daria6918.cn

Ruby: value = data || "默认值"
来源：http://udw.zhaomingkeji.xyz

C#:   var value = data ?? "默认值";
来源：http://knw.ydzc1.top

[A16] 真假值判断规则
来源：http://zlo.gotoacloud.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bbx.shanyushiyangtech.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mmj.wangshuangyany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ear.xuanzx.com

TS:   if (!x) {}
来源：http://huc.zhongyouzk.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oeh.hnqzz.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wcs.xziqi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uux.zhixingplan.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://okw.sxryk.cn

[A17] 位运算
来源：http://cac.ivvv.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://roz.52xcode.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vfe.hywenlv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sng.nanxinkj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://idy.kuanghao11.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rmn.jinqigfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oua.birdmap.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zlv.xziqi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cqp.jqgfzy.top

[A18] 字符与 ASCII 码互转
来源：http://mxz.nanxuanxn.top

Py:   ord("A"); chr(65)
来源：http://uih.zhiwuduotai.top

PHP:  ord("A"); chr(65)
来源：http://llz.aibaodan.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ojt.shanyushiyangtech.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iks.52xcode.cn

Java: (int) 'A'; (char) 65
来源：http://uai.zhoulong.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kdo.yueranfly.top

Ruby: "A".ord; 65.chr
来源：http://wnp.ctjpmb.com

C#:   (int)'A'; (char)65
来源：http://tsf.nanxinkj.top

[A19] 交换两个变量
来源：http://vfp.zhixingplan.top

Py:   a, b = b, a
来源：http://zfb.yonumen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nec.fengsongda.top

JS:   [a, b] = [b, a];
来源：http://lrx.shzxlz.cn

TS:   [a, b] = [b, a];
来源：http://wnd.meibo888.top

Java: int t = a; a = b; b = t;
来源：http://ppv.iojbl.cn

Go:   a, b = b, a
来源：http://gcs.quarkkingdee.top

Ruby: a, b = b, a
来源：http://ppg.jinqigfzy.top

C#:   (a, b) = (b, a);
来源：http://ory.guowangkeji.top

[A20] 读取标准输入
来源：http://sbu.zhixingplan.top

Py:   name = input("请输入：")
来源：http://wub.yj20258888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://uas.yfazqb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iaq.iojbl.cn

TS:   // Node.js：readline 模块
来源：http://yjw.daria6918.cn

Java: new Scanner(System.in).nextLine()
来源：http://ibf.xziqi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aqs.zhengqikj.top

Ruby: gets.chomp
来源：http://hks.shuidangran.top

C#:   Console.ReadLine();
来源：http://tep.zdbjq.cn

[A21] 保留指定小数位输出
来源：http://jgp.pengpengdd.cyou

Py:   f"{3.14159:.2f}"
来源：http://bql.yvedp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ioq.kuanghao11.cn

JS:   (3.14159).toFixed(2)
来源：http://xni.jinqigfzy.top

TS:   (3.14159).toFixed(2)
来源：http://pyc.ydjk.org.cn

Java: String.format("%.2f", 3.14159)
来源：http://lzh.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gez.pycfn.com

Ruby: format("%.2f", 3.14159)
来源：http://xgd.pengpengdd.cyou

C#:   3.14159.ToString("F2")
来源：http://xhg.shangyingyoupin.top

[A22] 获取字符串长度
来源：http://aoq.shuidangran.top

Py:   len(s)
来源：http://zgc.hywenlv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yip.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sgr.dianchejie.cn

TS:   s.length
来源：http://agb.xylfe.cn

Java: s.length()
来源：http://odx.xziqi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mnp.cucudq.cn

Ruby: s.length
来源：http://grm.yvedp.cn

C#:   s.Length
来源：http://xqe.yuxming.cn

[A23] 大小写转换
来源：http://fea.zhixingplan.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ius.jiagoushi.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mkc.hammf.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wwp.gotoacloud.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cex.ivvv.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xne.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jgu.fzhhl.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://djf.andypj.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://ast.tianlin.xyz

[A24] 去除首尾空白
来源：http://zbc.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dlb.andypj.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rxg.daxiang520.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rzo.zhoulong.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ghc.quarkkingdee.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fzl.haohaochexian.top

Go:   strings.TrimSpace(s)
来源：http://etx.hesvh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fie.chenzaomai.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rkz.sufxvd.cn

[A25] 字符串比较
来源：http://ipj.svipenyu.cn

Py:   s1 == s2; s1 != s2
来源：http://iqk.xingfuxueyuan.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kus.chenjidiqi.icu

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://foj.fktsv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gbg.sjlbkw.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kus.xziqi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bwx.jinyuanbaomall.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jdi.zhengqikj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hxs.vehdjk.com

[A26] 类型转换总览
来源：http://ned.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fji.xylfe.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://stq.hcnkem.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ucd.shanyushiyangtech.top

TS:   Number() String() Boolean() x as number
来源：http://hvy.dashuyun.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yfd.zdbjq.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nah.daria6918.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://eeh.zhiwuduotai.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rae.ehwqpu.com

================================================================================
来源：http://fde.tarul.cn

B. 流程控制
来源：http://wjt.quarkkingdee.top

================================================================================
来源：http://nhr.guowangkeji.top

[B01] 条件判断 if / else
来源：http://fmv.52xcode.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://juj.jqgufenzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dts.jqgfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kyd.chenlongwang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tbh.xziqi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fqq.zycfv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xbq.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hoc.zhijiandao.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jjd.andypj.xyz

[B02] 多分支 else if / elif
来源：http://zel.shanyushiyangtech.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nca.ydzc1.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bvg.meibo888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bwr.xylfe.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bst.vehdjk.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vjr.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nfv.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wmq.yuxming.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vwv.yongpay.top

[B03] switch / match / case
来源：http://ddx.jinqigfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fno.shangyingyoupin.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hzr.yuanzhike.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ihz.sweek.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nuu.sysykeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zkc.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://shc.zhaomingkeji.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://chp.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iff.kuanghao11.cn

[B04] for 计数循环
来源：http://low.fanxiaobao.xyz

Py:   for i in range(10): print(i)
来源：http://buk.ydzc1.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pbn.hnxiangtu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qjg.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wer.wangshuangyany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://slp.zhiwuduotai.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jsd.shzxlz.cn

Ruby: 10.times { |i| puts i }
来源：http://ajh.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aui.hysaishi.cn

[B05] 遍历数组 / 列表
来源：http://zat.birdmap.top

Py:   for item in arr: print(item)
来源：http://qaf.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gox.ivvv.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hcl.ydjk.org.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xja.bjfxy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vry.chenlongwang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pwy.feifeiyinyue.top

Ruby: arr.each { |item| puts item }
来源：http://hul.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lwb.tianlin.xyz

[B06] 遍历字典 / 对象
来源：http://haw.hesvh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pdb.sxryk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oxc.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bvt.yj20258.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rle.daria6918.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mup.hammf.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xxj.hfpthk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kqi.iojbl.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dgw.quarkkingdee.top

[B07] while 循环
来源：http://nsj.gzhubu.top

Py:   while i < 10: i += 1
来源：http://dkh.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://oli.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://exz.zdbjq.cn

TS:   while (i < 10) { i++; }
来源：http://bkt.zdbjq.cn

Java: while (i < 10) { i++; }
来源：http://oxj.birdmap.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eml.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://kry.vehdjk.com

C#:   while (i < 10) { i++; }
来源：http://hjc.epnwcf.com

[B08] do-while（至少执行一次）
来源：http://dvb.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://eiv.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://ivo.birdmap.top

JS:   do { i++; } while (i < 10);
来源：http://kpt.jyoumei.cn

TS:   do { i++; } while (i < 10);
来源：http://hrr.zdbjq.cn

Java: do { i++; } while (i < 10);
来源：http://pgj.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://syp.wangshuangyany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yab.52xcode.cn

C#:   do { i++; } while (i < 10);
来源：http://ovz.9152youxi.cn

[B09] break 与 continue
来源：http://naf.sxryk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://avp.jqgufenzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ibj.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xja.xinyue.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kxf.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dzi.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nry.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nrm.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://psv.epnwcf.com

[B10] 遍历同时拿索引
来源：http://cvq.dashuyun.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hhj.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kls.52xcode.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://klu.snrcjt.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yww.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://umi.fanxiaobao.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rte.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sep.xziqi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qbs.hesvh.cn

[B11] 生成数字序列 / 区间
来源：http://thy.jinqigfzy.top

Py:   list(range(0, 10, 2))
来源：http://khh.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://eqt.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ezg.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qsv.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lgq.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jqj.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://ibq.shangyingyoupin.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://irn.jinqigufen.top

[B12] 跳出多层循环
来源：http://uee.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zfn.havefunace.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wwr.nwbrower.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mzh.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rkt.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gic.svipenyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nfz.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zzi.haohaochexian.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ncq.shuidangran.top

[B13] 判断是否为数字
来源：http://osm.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://pku.meibo888.top

PHP:  is_numeric($x)
来源：http://ogs.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uqh.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zjk.feifeiyinyue.top

Java: x instanceof Number
来源：http://cxl.chenzaomai.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wzg.shanyushiyangtech.top

Ruby: x.is_a?(Numeric)
来源：http://bdk.ybcxt.top

C#:   x is int or double or decimal
来源：http://bpk.zhongyouzk.top

[B14] 判断值是否在集合内
来源：http://ihf.zhijiandao.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ylb.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cqr.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://vcg.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://lis.zhengqikj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ojr.wangshuangyany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://idk.nanxinkj.top

Ruby: [1, 2, 3].include?(x)
来源：http://dix.meibo888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uuy.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://smz.daria6918.cn

Py:   a and b or not c
来源：http://seu.hnqzz.top

PHP:  $a && $b || !$c
来源：http://kmv.jyoumei.cn

JS:   a && b || !c
来源：http://hub.cqqwz.cn

TS:   a && b || !c
来源：http://kkx.gzhubu.top

Java: a && b || !c
来源：http://cgj.gzhubu.top

Go:   a && b || !c
来源：http://kih.hywenlv.cn

Ruby: a && b || !c
来源：http://tky.tianlin.xyz

C#:   a && b || !c
来源：http://fom.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://sku.fktsv.cn

Py:   if not data: return
来源：http://qez.jinqigufen.top

PHP:  if (!$data) { return; }
来源：http://zoc.yfazqb.com

JS:   if (!data) return;
来源：http://rbi.vehdjk.com

TS:   if (!data) return;
来源：http://rcf.havefunace.top


<!-- 参考信息 -->