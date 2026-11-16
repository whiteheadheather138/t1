代发 wailian999

[A10] 生成随机数
来源：http://mzc.daxiang520.top

Py:   import random; random.randint(1, 100)
来源：http://jnf.316326.xyz

PHP:  random_int(1, 100);
来源：http://wvd.jlsjyb.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lza.aizwys.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://soa.jyoumei.cn

Java: new Random().nextInt(100) + 1
来源：http://hom.havefunace.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://diw.vqdsnc.cn

Ruby: rand(1..100)
来源：http://zli.shanyushiyangkeji.top

C#:   new Random().Next(1, 101)
来源：http://rxw.zdbjq.cn

[A11] 条件表达式（三元）
来源：http://muq.yj202588.top

Py:   "yes" if x > 0 else "no"
来源：http://wgq.zhongyouzk.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://vxs.dianchejie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qid.jinqigufen.top

TS:   x > 0 ? "yes" : "no"
来源：http://hgp.pycfn.com

Java: x > 0 ? "yes" : "no"
来源：http://ped.zhongyouzk.top

Go:   // 无三元运算符，需用 if 语句
来源：http://osn.havefunace.top

Ruby: x > 0 ? "yes" : "no"
来源：http://jqa.52xcode.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jiv.jinghuilouyu.cn

[A12] 字符串插值 / 格式化
来源：http://sei.yueranfly.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vhj.gogol.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lkk.xuanzx.com

JS:   `Hello, ${name}!`
来源：http://nmo.bjfxy.top

TS:   `Hello, ${name}!`
来源：http://sxf.quarkkingdee.top

Java: "Hello, %s!".formatted(name)
来源：http://wma.jinqigfzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qdu.zhengqikj.top

Ruby: "Hello, #{name}!"
来源：http://nmx.xziqi.cn

C#:   $"Hello, {name}!"
来源：http://tcc.zdbjq.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bgr.gzhubu.top

Py:   "第一行\n第二行"
来源：http://yjd.yanxiufei.cn

PHP:  "第一行\n第二行"
来源：http://uch.jqgfzy.top

JS:   "第一行\n第二行"
来源：http://iox.feifeiyinyue.top

TS:   "第一行\n第二行"
来源：http://wla.hcnkem.com

Java: "第一行\n第二行"
来源：http://xck.c1oappe.top

Go:   "第一行\n第二行"
来源：http://knx.zhiwuduotai.top

Ruby: "第一行\n第二行"
来源：http://kol.cucudq.cn

C#:   "第一行\n第二行"
来源：http://ynk.birdmap.top

[A14] 注释写法
来源：http://srf.tarul.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ffp.daxiang520.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rzp.chenjidiqi.icu

JS:   // 单行；/* 多行 */
来源：http://knt.birdmap.top

TS:   // 单行；/* 多行 */
来源：http://ats.hfpthk.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nuz.gzhubu.top

Go:   // 单行；/* 多行 */
来源：http://gqh.yueranfly.top

Ruby: # 单行；=begin 多行 =end
来源：http://oum.nanxuanxn.top

C#:   // 单行；/* 多行 */
来源：http://lya.andypj.xyz

[A15] 空值判断与默认值
来源：http://llb.gotoacloud.top

Py:   value = data or "默认值"
来源：http://ggi.hesvh.cn

PHP:  $value = $data ?? "默认值";
来源：http://gtj.zhoulong.xyz

JS:   const value = data ?? "默认值";
来源：http://vmt.mhx1999.top

TS:   const value = data ?? "默认值";
来源：http://mws.dashuyun.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ruk.ydjk.org.cn

Go:   if data == "" { data = "默认值" }
来源：http://pog.guowangkeji.top

Ruby: value = data || "默认值"
来源：http://fhu.hcnkem.com

C#:   var value = data ?? "默认值";
来源：http://uze.gaohongyu789.top

[A16] 真假值判断规则
来源：http://aon.hcnkem.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lzj.wangdashe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ign.xingfuxueyuan.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vvz.sjlbkw.cn

TS:   if (!x) {}
来源：http://iyp.aizwys.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gwc.jinyuanbaomall.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lcl.gotoacloud.top

Ruby: unless x            # nil 与 false 为假
来源：http://hhn.yfazqb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tnc.quarkkingdee.top

[A17] 位运算
来源：http://ijf.epnwcf.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zqg.jiagoushi.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://occ.feifeiyinyue.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zzo.sweek.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pde.pycfn.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oiy.tianlin.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dgf.jinqigufen.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hau.fengsongda.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rdn.tianlin.xyz

[A18] 字符与 ASCII 码互转
来源：http://wea.hesvh.cn

Py:   ord("A"); chr(65)
来源：http://dbg.cucudq.cn

PHP:  ord("A"); chr(65)
来源：http://hxm.andypj.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zxw.shuidangran.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://chx.ydzc1.top

Java: (int) 'A'; (char) 65
来源：http://rkq.jqgufenzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xcz.cdnleiting.top

Ruby: "A".ord; 65.chr
来源：http://xbg.cashguo.top

C#:   (int)'A'; (char)65
来源：http://oru.shuidangran.top

[A19] 交换两个变量
来源：http://quk.hfpthk.cn

Py:   a, b = b, a
来源：http://exh.tanke756.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qec.hnqzz.top

JS:   [a, b] = [b, a];
来源：http://vzi.ywan-chungtsiang.top

TS:   [a, b] = [b, a];
来源：http://cko.ydzc1.top

Java: int t = a; a = b; b = t;
来源：http://qwr.ydzc1.top

Go:   a, b = b, a
来源：http://wvi.shanyushiyangkeji.top

Ruby: a, b = b, a
来源：http://hxv.yuanzhike.top

C#:   (a, b) = (b, a);
来源：http://hfk.cqqwz.cn

[A20] 读取标准输入
来源：http://bwq.nanxuanxn.top

Py:   name = input("请输入：")
来源：http://knh.redwolf501.top

PHP:  $name = trim(fgets(STDIN));
来源：http://efp.hongshengwenyu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fda.xingfuxueyuan.xyz

TS:   // Node.js：readline 模块
来源：http://goi.nwbrower.top

Java: new Scanner(System.in).nextLine()
来源：http://rsl.cdnleiting.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://olk.jinqigfzy.top

Ruby: gets.chomp
来源：http://tun.meibo888.top

C#:   Console.ReadLine();
来源：http://bof.cheryme.top

[A21] 保留指定小数位输出
来源：http://cig.fktsv.cn

Py:   f"{3.14159:.2f}"
来源：http://eue.zhongyouzk.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pmx.hfpthk.cn

JS:   (3.14159).toFixed(2)
来源：http://sgj.shuidangran.top

TS:   (3.14159).toFixed(2)
来源：http://uio.gaohongyu789.top

Java: String.format("%.2f", 3.14159)
来源：http://yid.hysaishi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rge.jinqigfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://kja.yfazqb.com

C#:   3.14159.ToString("F2")
来源：http://pav.havefunace.top

[A22] 获取字符串长度
来源：http://smc.nanxuanxn.top

Py:   len(s)
来源：http://eud.hesvh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zph.fengsongda.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://anu.jqgfzy.top

TS:   s.length
来源：http://exg.dianchejie.cn

Java: s.length()
来源：http://nph.ctjpmb.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rly.hcnkem.com

Ruby: s.length
来源：http://bcj.gzhubu.top

C#:   s.Length
来源：http://wkr.yonumen.top

[A23] 大小写转换
来源：http://pmf.xinyue.icu

Py:   s.upper(); s.lower(); s.title()
来源：http://eao.jlsjyb.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://avj.bjfxy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ior.vqdsnc.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yxy.zhaomingkeji.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ruv.zycfv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mkm.zdqjudy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pgk.jianghu66.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jat.guannengcc.top

[A24] 去除首尾空白
来源：http://dim.guannengcc.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ptc.yanxiufei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sjz.yj20258.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lpu.jiagoushi.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qth.iojbl.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iym.nanxinkj.top

Go:   strings.TrimSpace(s)
来源：http://jbx.shangyingyoupin.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ety.fanxiaobao.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jii.cucudq.cn

[A25] 字符串比较
来源：http://ymy.yj20258.top

Py:   s1 == s2; s1 != s2
来源：http://ofk.svipenyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://myr.epnwcf.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://omb.fengsongda.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iwx.cheryme.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://awp.gotoacloud.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://veu.chenjidiqi.icu

Ruby: s1 == s2; s1 <=> s2
来源：http://hxi.nanxuanxn.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hju.xingfuxueyuan.xyz

[A26] 类型转换总览
来源：http://aof.sufxvd.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hry.gotoacloud.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eiv.ydjk.org.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pmh.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://kri.yonumen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xqr.hnxiangtu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lat.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://kck.vehdjk.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://acj.xziqi.cn

================================================================================
来源：http://npd.jianghu66.top

B. 流程控制
来源：http://lsv.yonumen.top

================================================================================
来源：http://sir.havefunace.top

[B01] 条件判断 if / else
来源：http://ior.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jgw.kuanghao11.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qbe.ybcxt.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wtf.ctjpmb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ddy.redwolf501.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://psu.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qyv.shangyingyoupin.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ooq.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rsb.wangdashe.top

[B02] 多分支 else if / elif
来源：http://ddo.nwbrower.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uqa.zhongyouzk.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jam.chenjidiqi.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://phi.bbcook.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iov.zhijiandao.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cwc.52xcode.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gtg.jyoumei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fck.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ggl.zhongyouzk.top

[B03] switch / match / case
来源：http://vkv.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cad.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kzg.cdnleiting.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ylu.jiagoushi.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lzz.zhaomingkeji.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://snm.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xht.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://opv.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fer.hammf.cn

[B04] for 计数循环
来源：http://mli.gaohongyu789.top

Py:   for i in range(10): print(i)
来源：http://vit.fktsv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://knr.hnxiangtu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://thv.yanxiufei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hzr.tanke756.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uvo.yj202588.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://otb.hammf.cn

Ruby: 10.times { |i| puts i }
来源：http://ftk.hongshengwenyu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rsz.wangshuangyany.cn

[B05] 遍历数组 / 列表
来源：http://gzk.redwolf501.top

Py:   for item in arr: print(item)
来源：http://dxu.ydjk.org.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yyl.pengpengdd.cyou

JS:   for (const item of arr) { console.log(item); }
来源：http://fyi.zhongyouzk.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cxy.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mqi.hammf.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aye.aizwys.cn

Ruby: arr.each { |item| puts item }
来源：http://hty.gaohongyu789.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jqo.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://ugp.andypj.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://klm.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mlh.zhijiandao.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jyo.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pad.yj20258888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kll.ydzc1.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ahw.zhiwuduotai.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dct.fehbvm.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ojh.birdmap.top

[B07] while 循环
来源：http://tdv.xylfe.cn

Py:   while i < 10: i += 1
来源：http://yqg.9152youxi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sca.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://nfq.jyoumei.cn

TS:   while (i < 10) { i++; }
来源：http://zvz.aibaodan.cn

Java: while (i < 10) { i++; }
来源：http://ilv.ehwqpu.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vwj.c1oappe.top

Ruby: while i < 10; i += 1; end
来源：http://kvq.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://cvv.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://qum.havefunace.top

Py:   # 无 do-while：用 while True + break
来源：http://qbs.daxiang520.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ype.zhaomingkeji.xyz

JS:   do { i++; } while (i < 10);
来源：http://edo.zdqjudy.top

TS:   do { i++; } while (i < 10);
来源：http://xic.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://ldu.chenjidiqi.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://eqw.shzxlz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mef.ybcxt.top

C#:   do { i++; } while (i < 10);
来源：http://fqx.yj202588.top

[B09] break 与 continue
来源：http://gxt.hywenlv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ydd.andypj.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ycd.bjfxy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qxj.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vav.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ctm.jianghu66.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://npn.hfpthk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kun.316326.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fno.tianlin.xyz

[B10] 遍历同时拿索引
来源：http://fjb.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://coo.nanxuanxn.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hiu.jiagoushi.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wai.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://twp.shzxlz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aii.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jkf.jiagoushi.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ebj.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wle.xingfuxueyuan.xyz

[B11] 生成数字序列 / 区间
来源：http://gam.hnqzz.top

Py:   list(range(0, 10, 2))
来源：http://wab.yongpay.top

PHP:  range(0, 10, 2);
来源：http://byb.hesvh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tbu.hfpthk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://otz.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zol.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uvt.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://ank.quarkkingdee.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xjo.fzhhl.top

[B12] 跳出多层循环
来源：http://nmx.nwbrower.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ily.gogol.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ere.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://crb.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://scw.hfpthk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sqt.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zzn.nanxuanxn.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jcg.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uoj.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://ghy.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://ies.sxryk.cn

PHP:  is_numeric($x)
来源：http://iml.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zfv.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rkv.tian-w.cn

Java: x instanceof Number
来源：http://pjz.yj202588.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uqc.andypj.xyz

Ruby: x.is_a?(Numeric)
来源：http://cnh.yueranfly.top

C#:   x is int or double or decimal
来源：http://vnt.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://orh.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nbh.zhiwuduotai.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tiw.yj20258888.top

JS:   [1, 2, 3].includes(x)
来源：http://yct.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://kap.smart0.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://tfn.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lak.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://gij.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ybq.sysykeji.top

[B15] 布尔运算与取反
来源：http://xfs.hammf.cn

Py:   a and b or not c
来源：http://mjy.pycfn.com

PHP:  $a && $b || !$c
来源：http://faw.fktsv.cn

JS:   a && b || !c
来源：http://yah.jyoumei.cn

TS:   a && b || !c
来源：http://qap.tarul.cn

Java: a && b || !c
来源：http://csr.zhengqikj.top

Go:   a && b || !c
来源：http://alq.redwolf501.top

Ruby: a && b || !c
来源：http://agx.xuetiantiany.cn

C#:   a && b || !c
来源：http://wrh.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dnu.jqgfzy.top

Py:   if not data: return
来源：http://zxc.yonumen.top

PHP:  if (!$data) { return; }
来源：http://zjj.iojbl.cn

JS:   if (!data) return;
来源：http://ngj.gaohongyu789.top

TS:   if (!data) return;
来源：http://tpc.fehbvm.com

Java: if (data == null) return;
来源：http://goh.birdmap.top

Go:   if data == nil { return }
来源：http://ptj.hywenlv.cn

Ruby: return if data.nil?
来源：http://yun.fanxiaobao.xyz

C#:   if (data == null) return;
来源：http://kyb.zhengqikj.top


<!-- 参考信息 -->