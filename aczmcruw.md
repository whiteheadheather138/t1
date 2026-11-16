代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://sts.pycfn.com

[A11] 条件表达式（三元）
来源：http://rvz.vehdjk.com

Py:   "yes" if x > 0 else "no"
来源：http://rgf.hcnkem.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://wuq.ydjk.org.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hnc.dianchejie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ewm.chenzaomai.com

Java: x > 0 ? "yes" : "no"
来源：http://gbs.xuetiantiany.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bko.cqqwz.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rld.cdnleiting.top

C#:   x > 0 ? "yes" : "no"
来源：http://ywc.zycfv.cn

[A12] 字符串插值 / 格式化
来源：http://ozq.nanxuanxn.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sqv.birdmap.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fkb.smart0.xyz

JS:   `Hello, ${name}!`
来源：http://wss.tanke756.top

TS:   `Hello, ${name}!`
来源：http://vti.sufxvd.cn

Java: "Hello, %s!".formatted(name)
来源：http://ovd.ehwqpu.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jao.jinyuanbaomall.cn

Ruby: "Hello, #{name}!"
来源：http://enq.ybcxt.top

C#:   $"Hello, {name}!"
来源：http://aza.xingfuxueyuan.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://qku.cdnleiting.top

Py:   "第一行\n第二行"
来源：http://odx.wangshuangyany.cn

PHP:  "第一行\n第二行"
来源：http://xrf.hnxiangtu.top

JS:   "第一行\n第二行"
来源：http://zdg.meibo888.top

TS:   "第一行\n第二行"
来源：http://xxw.yvedp.cn

Java: "第一行\n第二行"
来源：http://ren.epnwcf.com

Go:   "第一行\n第二行"
来源：http://wpx.nanxuanxn.top

Ruby: "第一行\n第二行"
来源：http://qkn.ydzc1.top

C#:   "第一行\n第二行"
来源：http://bjq.birdmap.top

[A14] 注释写法
来源：http://ciy.meibo888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://fpo.jinyuanbaomall.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cnd.hfpthk.cn

JS:   // 单行；/* 多行 */
来源：http://wfy.dashuyun.cn

TS:   // 单行；/* 多行 */
来源：http://ybu.xingfuxueyuan.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dua.cashguo.top

Go:   // 单行；/* 多行 */
来源：http://ydd.ydjk.org.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zgl.shanyushiyangtech.top

C#:   // 单行；/* 多行 */
来源：http://tzz.cqqwz.cn

[A15] 空值判断与默认值
来源：http://bxl.gotoacloud.top

Py:   value = data or "默认值"
来源：http://quu.guowangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://hkh.sweek.top

JS:   const value = data ?? "默认值";
来源：http://jjb.fktsv.cn

TS:   const value = data ?? "默认值";
来源：http://byb.jyoumei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://brg.sufxvd.cn

Go:   if data == "" { data = "默认值" }
来源：http://kgw.quarkkingdee.top

Ruby: value = data || "默认值"
来源：http://kiz.cdnleiting.top

C#:   var value = data ?? "默认值";
来源：http://pkp.hysaishi.cn

[A16] 真假值判断规则
来源：http://yan.birdmap.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tzq.tanke756.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kvl.tarul.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qiw.shangyingyoupin.top

TS:   if (!x) {}
来源：http://qft.bbcook.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jdo.jiagoushi.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://znp.jinqigfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://rve.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eib.jlsjyb.cn

[A17] 位运算
来源：http://mbt.vqdsnc.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hly.chenjidiqi.icu

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rxl.hywenlv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ldr.yj202588.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hmu.c1oappe.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wwo.svipenyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ppc.haohaochexian.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dcn.cashguo.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iua.zhixingplan.top

[A18] 字符与 ASCII 码互转
来源：http://sxi.zhengqikj.top

Py:   ord("A"); chr(65)
来源：http://xsm.fktsv.cn

PHP:  ord("A"); chr(65)
来源：http://lfh.quarkkingdee.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ndh.shuidangran.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xnm.iojbl.cn

Java: (int) 'A'; (char) 65
来源：http://xit.hfpthk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://waq.xinyue.icu

Ruby: "A".ord; 65.chr
来源：http://sav.uphjek.com

C#:   (int)'A'; (char)65
来源：http://tiu.zhongyouzk.top

[A19] 交换两个变量
来源：http://jzy.zhaomingkeji.xyz

Py:   a, b = b, a
来源：http://lck.ywan-chungtsiang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://txb.jinghuilouyu.cn

JS:   [a, b] = [b, a];
来源：http://cwb.andypj.xyz

TS:   [a, b] = [b, a];
来源：http://pao.tanke756.top

Java: int t = a; a = b; b = t;
来源：http://boe.zycfv.cn

Go:   a, b = b, a
来源：http://oxf.hfpthk.cn

Ruby: a, b = b, a
来源：http://blz.redwolf501.top

C#:   (a, b) = (b, a);
来源：http://ssq.meibo888.top

[A20] 读取标准输入
来源：http://scz.chenlongwang.top

Py:   name = input("请输入：")
来源：http://sqo.sufxvd.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dax.yueranfly.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cym.shzxlz.cn

TS:   // Node.js：readline 模块
来源：http://cap.jinghuilouyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://mqn.feifeiyinyue.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kkr.shuidangran.top

Ruby: gets.chomp
来源：http://ygm.yfazqb.com

C#:   Console.ReadLine();
来源：http://nun.xinyue.icu

[A21] 保留指定小数位输出
来源：http://eyv.iojbl.cn

Py:   f"{3.14159:.2f}"
来源：http://tvp.jinghuilouyu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bmp.hcnkem.com

JS:   (3.14159).toFixed(2)
来源：http://bjh.fanxiaobao.xyz

TS:   (3.14159).toFixed(2)
来源：http://uwn.ybcxt.top

Java: String.format("%.2f", 3.14159)
来源：http://fwy.jinyuanbaomall.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mos.yvedp.cn

Ruby: format("%.2f", 3.14159)
来源：http://ztt.cashguo.top

C#:   3.14159.ToString("F2")
来源：http://idl.hywenlv.cn

[A22] 获取字符串长度
来源：http://afk.jinghuilouyu.cn

Py:   len(s)
来源：http://iyn.aibaodan.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cdn.chenzaomai.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ymh.zhijiandao.cn

TS:   s.length
来源：http://wnr.yuxming.cn

Java: s.length()
来源：http://edw.zhengqikj.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://crb.hywenlv.cn

Ruby: s.length
来源：http://lrx.shanyushiyangtech.top

C#:   s.Length
来源：http://wrb.yj202588.top

[A23] 大小写转换
来源：http://iye.xingfuxueyuan.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://qov.hfpthk.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yaj.chenjidiqi.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xrl.zhengqikj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://asu.shanyushiyangtech.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jgk.daria6918.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cos.jyoumei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jhl.xingfuxueyuan.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://xte.vqdsnc.cn

[A24] 去除首尾空白
来源：http://sxq.pengpengdd.cyou

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tun.aibaodan.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gnl.bjfxy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://smk.jinyuanbaomall.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dzk.wangdashe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sop.cdnleiting.top

Go:   strings.TrimSpace(s)
来源：http://fih.svipenyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rkz.quarkkingdee.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ydd.dianchejie.cn

[A25] 字符串比较
来源：http://opi.zhongyouzk.top

Py:   s1 == s2; s1 != s2
来源：http://qnr.jinqigufen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dwv.hnqzz.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rdq.hfpthk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xnb.tian-w.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kyr.gogol.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vhe.xuanzx.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ewv.yueranfly.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cht.shanyushiyangtech.top

[A26] 类型转换总览
来源：http://drn.zhongyouzk.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xab.uphjek.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wnx.yuanzhike.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qgm.haohaochexian.top

TS:   Number() String() Boolean() x as number
来源：http://qbv.gzhubu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tde.uphjek.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zev.birdmap.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://etq.hongshengwenyu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ldj.zhijiandao.cn

================================================================================
来源：http://cqv.aibaodan.cn

B. 流程控制
来源：http://ppx.hesvh.cn

================================================================================
来源：http://rai.nanxinkj.top

[B01] 条件判断 if / else
来源：http://yev.hcnkem.com

Py:   result = "正" if x > 0 else "非正"
来源：http://awh.vqdsnc.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kqk.andypj.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mpt.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wjq.sjlbkw.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zam.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yfq.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bzy.xingfuxueyuan.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gyl.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://bdj.52xcode.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://msn.xylfe.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mnc.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ned.xuanzx.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lrf.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ooq.daxiang520.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fcr.ydjk.org.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cdj.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ahl.yuxming.cn

[B03] switch / match / case
来源：http://thv.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uil.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nyo.hcnkem.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fzc.meibo888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wvy.jyoumei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jkd.cdnleiting.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iut.cheryme.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jey.yueranfly.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lur.chenzaomai.com

[B04] for 计数循环
来源：http://nap.nanxuanxn.top

Py:   for i in range(10): print(i)
来源：http://dqe.xuetiantiany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kng.pengpengdd.cyou

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jlo.ydzc1.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ywn.jyoumei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dvo.ivvv.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zay.vehdjk.com

Ruby: 10.times { |i| puts i }
来源：http://fun.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qgi.cashguo.top

[B05] 遍历数组 / 列表
来源：http://kzu.gogol.net.cn

Py:   for item in arr: print(item)
来源：http://zxh.cqqwz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uqb.nanxuanxn.top

JS:   for (const item of arr) { console.log(item); }
来源：http://otb.cdnleiting.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xwy.sufxvd.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://syb.zhaomingkeji.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gfk.xziqi.cn

Ruby: arr.each { |item| puts item }
来源：http://jrc.c1oappe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iec.sxryk.cn

[B06] 遍历字典 / 对象
来源：http://hzf.fzhhl.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gvn.ivvv.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yrc.redwolf501.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gtl.jianghu66.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bzf.ppjwa.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://opj.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nfc.jqgufenzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hbd.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lor.xingfuxueyuan.xyz

[B07] while 循环
来源：http://srk.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://jcm.fktsv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://teg.jyoumei.cn

JS:   while (i < 10) { i++; }
来源：http://gng.gaohongyu789.top

TS:   while (i < 10) { i++; }
来源：http://pac.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://ica.yueranfly.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rdo.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://yfv.shanyushiyangkeji.top

C#:   while (i < 10) { i++; }
来源：http://hza.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://bas.wangshuangyany.cn

Py:   # 无 do-while：用 while True + break
来源：http://red.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hsp.sysykeji.top

JS:   do { i++; } while (i < 10);
来源：http://jab.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://fzk.chenlongwang.top

Java: do { i++; } while (i < 10);
来源：http://ajp.gogol.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fcy.snrcjt.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ccc.zhaomingkeji.xyz

C#:   do { i++; } while (i < 10);
来源：http://mrx.sjlbkw.cn

[B09] break 与 continue
来源：http://vpp.yuanzhike.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mcg.vqdsnc.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wqv.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dbi.zhaomingkeji.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jsk.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://poa.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ddd.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vmz.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hkx.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://brx.jlsjyb.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zic.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nwe.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hcy.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wvs.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rmh.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oao.daria6918.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xdr.smart0.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vnk.wangshuangyany.cn

[B11] 生成数字序列 / 区间
来源：http://may.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://tri.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://aoh.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://abz.zhongyouzk.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fnj.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xby.hywenlv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mnq.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://hdy.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kfs.yj202588.top

[B12] 跳出多层循环
来源：http://dsn.haohaochexian.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jzp.feifeiyinyue.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dkz.0kj1m.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jhk.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qcd.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://goe.wangshuangyany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dtb.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xrl.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mcr.9152youxi.cn

[B13] 判断是否为数字
来源：http://izt.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://por.hesvh.cn

PHP:  is_numeric($x)
来源：http://wmk.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pzz.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mqx.jyoumei.cn

Java: x instanceof Number
来源：http://loo.yuanzhike.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fbx.hnqzz.top

Ruby: x.is_a?(Numeric)
来源：http://hee.9152youxi.cn

C#:   x is int or double or decimal
来源：http://wac.yuxming.cn

[B14] 判断值是否在集合内
来源：http://iop.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qtr.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hsi.tarul.cn

JS:   [1, 2, 3].includes(x)
来源：http://ubi.9152youxi.cn

TS:   [1, 2, 3].includes(x)
来源：http://fgl.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://iam.chenzaomai.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uhk.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fty.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ezz.zhixingplan.top

[B15] 布尔运算与取反
来源：http://tdo.yj20258888.top

Py:   a and b or not c
来源：http://jny.tanke756.top

PHP:  $a && $b || !$c
来源：http://ill.ctjpmb.com

JS:   a && b || !c
来源：http://ptl.jinqigfzy.top

TS:   a && b || !c
来源：http://jtl.fktsv.cn

Java: a && b || !c
来源：http://cxr.daxiang520.top

Go:   a && b || !c
来源：http://qwo.jyoumei.cn

Ruby: a && b || !c
来源：http://qov.shangyingyoupin.top

C#:   a && b || !c
来源：http://uhq.cheryme.top

[B16] 卫语句：不满足条件提前返回
来源：http://uzz.yuanzhike.top

Py:   if not data: return
来源：http://pkl.ywan-chungtsiang.top

PHP:  if (!$data) { return; }
来源：http://nvq.daxiang520.top

JS:   if (!data) return;
来源：http://lyk.yanxiufei.cn

TS:   if (!data) return;
来源：http://rap.yongpay.top

Java: if (data == null) return;
来源：http://xvn.316326.xyz

Go:   if data == nil { return }
来源：http://psa.jianghu66.top

Ruby: return if data.nil?
来源：http://xou.fzhhl.top

C#:   if (data == null) return;
来源：http://ots.jqgfzy.top

================================================================================
来源：http://fla.zdqjudy.top

C. 函数与作用域
来源：http://uxr.xylfe.cn

================================================================================
来源：http://xvn.zhongyouzk.top

[C01] 定义函数
来源：http://kjb.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://uwf.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ivl.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://onu.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ybp.fehbvm.com


<!-- 参考信息 -->