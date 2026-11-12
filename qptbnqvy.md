代发 wailian999

[A10] 生成随机数
来源：http://aid.xingfuxueyuan.xyz

Py:   import random; random.randint(1, 100)
来源：http://lby.dianchejie.cn

PHP:  random_int(1, 100);
来源：http://iqo.shanyushiyangkeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ymy.uphjek.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://edw.hfpthk.cn

Java: new Random().nextInt(100) + 1
来源：http://fxb.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vlr.fktsv.cn

Ruby: rand(1..100)
来源：http://eeo.guannengcc.top

C#:   new Random().Next(1, 101)
来源：http://yjw.sysykeji.top

[A11] 条件表达式（三元）
来源：http://hos.shuidangran.top

Py:   "yes" if x > 0 else "no"
来源：http://big.aizwys.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://apd.sysykeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://oiq.hcnkem.com

TS:   x > 0 ? "yes" : "no"
来源：http://fub.birdmap.top

Java: x > 0 ? "yes" : "no"
来源：http://ngn.cucudq.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hjp.feifeiyinyue.top

Ruby: x > 0 ? "yes" : "no"
来源：http://sas.daxiang520.top

C#:   x > 0 ? "yes" : "no"
来源：http://gsa.sysykeji.top

[A12] 字符串插值 / 格式化
来源：http://eid.wangshuangyany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aay.tianlin.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cbv.redwolf501.top

JS:   `Hello, ${name}!`
来源：http://ncu.ybcxt.top

TS:   `Hello, ${name}!`
来源：http://mrx.hnxiangtu.top

Java: "Hello, %s!".formatted(name)
来源：http://bwj.chenzaomai.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://irh.aizwys.cn

Ruby: "Hello, #{name}!"
来源：http://mty.hnqzz.top

C#:   $"Hello, {name}!"
来源：http://yyx.ehwqpu.com

[A13] 多行字符串（练习 \n 转义）
来源：http://gmh.hnxiangtu.top

Py:   "第一行\n第二行"
来源：http://obj.gzhubu.top

PHP:  "第一行\n第二行"
来源：http://cnx.redwolf501.top

JS:   "第一行\n第二行"
来源：http://dnv.meibo888.top

TS:   "第一行\n第二行"
来源：http://gjp.birdmap.top

Java: "第一行\n第二行"
来源：http://ies.c1oappe.top

Go:   "第一行\n第二行"
来源：http://vhd.wangshuangyany.cn

Ruby: "第一行\n第二行"
来源：http://tcz.chenzaomai.com

C#:   "第一行\n第二行"
来源：http://zyq.fktsv.cn

[A14] 注释写法
来源：http://zsx.zhijiandao.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xqx.hcnkem.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://lnx.zhixingplan.top

JS:   // 单行；/* 多行 */
来源：http://aod.ppjwa.cn

TS:   // 单行；/* 多行 */
来源：http://rpb.daxiang520.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://abl.sufxvd.cn

Go:   // 单行；/* 多行 */
来源：http://fnc.chenlongwang.top

Ruby: # 单行；=begin 多行 =end
来源：http://zaf.tianlin.xyz

C#:   // 单行；/* 多行 */
来源：http://ige.jyoumei.cn

[A15] 空值判断与默认值
来源：http://qqi.sysykeji.top

Py:   value = data or "默认值"
来源：http://ynx.hnqzz.top

PHP:  $value = $data ?? "默认值";
来源：http://ygw.wangdashe.top

JS:   const value = data ?? "默认值";
来源：http://mvp.zhaomingkeji.xyz

TS:   const value = data ?? "默认值";
来源：http://mgc.vqdsnc.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cqp.quarkkingdee.top

Go:   if data == "" { data = "默认值" }
来源：http://naj.cucudq.cn

Ruby: value = data || "默认值"
来源：http://djo.hywenlv.cn

C#:   var value = data ?? "默认值";
来源：http://yzi.zdbjq.cn

[A16] 真假值判断规则
来源：http://cqg.yj202588.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yxu.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://apt.jianghu66.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xrw.snrcjt.cn

TS:   if (!x) {}
来源：http://hzq.jianghu66.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rlo.yfazqb.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hzr.guowangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://jdy.zdqjudy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vfj.sxryk.cn

[A17] 位运算
来源：http://djp.ivvv.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gjp.yj202588.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lof.chenzaomai.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ndl.hcnkem.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sew.jinqigufen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lma.jiagoushi.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ahc.yj20258888.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://umk.yj20258888.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bfs.cucudq.cn

[A18] 字符与 ASCII 码互转
来源：http://svp.0kj1m.cn

Py:   ord("A"); chr(65)
来源：http://leu.xuanzx.com

PHP:  ord("A"); chr(65)
来源：http://waj.yvedp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xpn.yfazqb.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xls.feifeiyinyue.top

Java: (int) 'A'; (char) 65
来源：http://jmf.dianchejie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kok.pengpengdd.cyou

Ruby: "A".ord; 65.chr
来源：http://lfa.haohaochexian.top

C#:   (int)'A'; (char)65
来源：http://hij.quarkkingdee.top

[A19] 交换两个变量
来源：http://kye.dashuyun.cn

Py:   a, b = b, a
来源：http://zzu.daxiang520.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hkf.aibaodan.cn

JS:   [a, b] = [b, a];
来源：http://uly.ppjwa.cn

TS:   [a, b] = [b, a];
来源：http://khb.nanxuanxn.top

Java: int t = a; a = b; b = t;
来源：http://rac.xuanzx.com

Go:   a, b = b, a
来源：http://rvo.ywan-chungtsiang.top

Ruby: a, b = b, a
来源：http://nio.c1oappe.top

C#:   (a, b) = (b, a);
来源：http://ndp.uphjek.com

[A20] 读取标准输入
来源：http://qbi.andypj.xyz

Py:   name = input("请输入：")
来源：http://bjn.nanxinkj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bcy.jqgfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eft.pycfn.com

TS:   // Node.js：readline 模块
来源：http://wqn.feifeiyinyue.top

Java: new Scanner(System.in).nextLine()
来源：http://hvr.mhx1999.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hde.birdmap.top

Ruby: gets.chomp
来源：http://rsy.zhijiandao.cn

C#:   Console.ReadLine();
来源：http://shk.aizwys.cn

[A21] 保留指定小数位输出
来源：http://zxv.jyoumei.cn

Py:   f"{3.14159:.2f}"
来源：http://chu.c1oappe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yer.hysaishi.cn

JS:   (3.14159).toFixed(2)
来源：http://bsf.9152youxi.cn

TS:   (3.14159).toFixed(2)
来源：http://dja.daxiang520.top

Java: String.format("%.2f", 3.14159)
来源：http://jgz.epnwcf.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://squ.ybcxt.top

Ruby: format("%.2f", 3.14159)
来源：http://ozz.haohaochexian.top

C#:   3.14159.ToString("F2")
来源：http://hfi.cheryme.top

[A22] 获取字符串长度
来源：http://cid.iojbl.cn

Py:   len(s)
来源：http://wqj.sjlbkw.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sft.cdnleiting.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pzr.chenzaomai.com

TS:   s.length
来源：http://ykg.pengpengdd.cyou

Java: s.length()
来源：http://dua.ppjwa.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qum.yuanzhike.top

Ruby: s.length
来源：http://xys.hnqzz.top

C#:   s.Length
来源：http://fdy.cheryme.top

[A23] 大小写转换
来源：http://our.yvedp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kbb.iojbl.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lsf.gotoacloud.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gmf.jyoumei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cca.ydzc1.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xlf.fktsv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://azs.xziqi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ofq.meibo888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gfc.mhx1999.top

[A24] 去除首尾空白
来源：http://ytv.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bvw.ybcxt.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://quk.jianghu66.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nwr.chenzaomai.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ooi.jlsjyb.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cmc.snrcjt.cn

Go:   strings.TrimSpace(s)
来源：http://ush.wangdashe.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qjg.gogol.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hye.zhoulong.xyz

[A25] 字符串比较
来源：http://fwl.hysaishi.cn

Py:   s1 == s2; s1 != s2
来源：http://muz.yvedp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dbb.birdmap.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cmi.gaohongyu789.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ejx.jlsjyb.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fiv.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yod.yj20258888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kuq.shuidangran.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gfm.shangyingyoupin.top

[A26] 类型转换总览
来源：http://tae.sjlbkw.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://txx.yj202588.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nfa.dashuyun.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ail.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://gdl.sufxvd.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vzo.chenzaomai.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://moo.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rio.ybcxt.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jun.sxryk.cn

================================================================================
来源：http://ovb.yfazqb.com

B. 流程控制
来源：http://hfl.meibo888.top

================================================================================
来源：http://vbv.xuetiantiany.cn

[B01] 条件判断 if / else
来源：http://baq.chenzaomai.com

Py:   result = "正" if x > 0 else "非正"
来源：http://iod.tianlin.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rul.hesvh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cfa.haohaochexian.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nfm.jqgfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ihi.yj20258.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://afs.wangshuangyany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aay.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lhx.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://tal.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ehn.xylfe.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wja.nanxuanxn.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vlw.gogol.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zhz.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xqj.nwbrower.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qtx.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bxk.tianlin.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ehr.jlsjyb.cn

[B03] switch / match / case
来源：http://uwo.jinqigufen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://esz.shanyushiyangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fnt.feifeiyinyue.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ftk.jinqigufen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://apm.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ywc.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rjs.yangfankeji.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://msm.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gan.tianlin.xyz

[B04] for 计数循环
来源：http://dnw.chenlongwang.top

Py:   for i in range(10): print(i)
来源：http://her.meibo888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tbb.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mdt.fktsv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hfv.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nyh.sweek.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ase.shzxlz.cn

Ruby: 10.times { |i| puts i }
来源：http://gen.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lxv.epnwcf.com

[B05] 遍历数组 / 列表
来源：http://cjr.gogol.net.cn

Py:   for item in arr: print(item)
来源：http://cpx.xinyue.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://onu.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://owt.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://urn.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hcr.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zvl.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://sts.gogol.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kzb.mhx1999.top

[B06] 遍历字典 / 对象
来源：http://dvd.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tss.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vue.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zjw.dianchejie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bmn.0kj1m.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cku.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ijl.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qeu.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wqm.sysykeji.top

[B07] while 循环
来源：http://osq.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://onw.chenzaomai.com

PHP:  while ($i < 10) { $i++; }
来源：http://pyz.meibo888.top

JS:   while (i < 10) { i++; }
来源：http://ghd.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://gjq.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://jyk.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kcj.ivvv.top

Ruby: while i < 10; i += 1; end
来源：http://ncp.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://shz.hammf.cn

[B08] do-while（至少执行一次）
来源：http://txf.pycfn.com

Py:   # 无 do-while：用 while True + break
来源：http://ail.cdnleiting.top

PHP:  do { $i++; } while ($i < 10);
来源：http://efb.c1oappe.top

JS:   do { i++; } while (i < 10);
来源：http://ryh.kuanghao11.cn

TS:   do { i++; } while (i < 10);
来源：http://qst.iojbl.cn

Java: do { i++; } while (i < 10);
来源：http://cqe.hongshengwenyu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vas.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uuz.andypj.xyz

C#:   do { i++; } while (i < 10);
来源：http://lxa.xylfe.cn

[B09] break 与 continue
来源：http://juk.fktsv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qsc.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rbd.jiagoushi.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://izj.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hcl.dashuyun.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jyh.ywan-chungtsiang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vpz.hnxiangtu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rre.jinyuanbaomall.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ked.hysaishi.cn

[B10] 遍历同时拿索引
来源：http://fvd.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vbz.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nvm.nanxuanxn.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://evg.cdnleiting.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bok.daxiang520.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jtd.jyoumei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://skv.sweek.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vni.hnxiangtu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uwi.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://ehu.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://pux.bjfxy.top

PHP:  range(0, 10, 2);
来源：http://rlr.cucudq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ggs.tanke756.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://whq.svipenyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vdh.zhiwuduotai.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wth.daria6918.cn

Ruby: (0...10).step(2).to_a
来源：http://iru.52xcode.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vej.cucudq.cn

[B12] 跳出多层循环
来源：http://rhh.hesvh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://srg.yongpay.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ydr.jinqigufen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://imr.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nyi.xuanzx.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lzk.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bwk.guannengcc.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tdi.c1oappe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dyt.birdmap.top

[B13] 判断是否为数字
来源：http://tmh.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://fxx.bbcook.cn

PHP:  is_numeric($x)
来源：http://wub.fengsongda.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ita.hcnkem.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qld.ppjwa.cn

Java: x instanceof Number
来源：http://rdz.zhoulong.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pvk.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://mka.quarkkingdee.top

C#:   x is int or double or decimal
来源：http://fyk.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://tua.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xve.chenlongwang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qoh.guowangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://lkq.tanke756.top

TS:   [1, 2, 3].includes(x)
来源：http://pyw.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://som.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pya.bjfxy.top

Ruby: [1, 2, 3].include?(x)
来源：http://ion.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oru.yj20258.top

[B15] 布尔运算与取反
来源：http://gfj.epnwcf.com

Py:   a and b or not c
来源：http://gkm.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://aeu.daria6918.cn

JS:   a && b || !c
来源：http://gpz.shangyingyoupin.top

TS:   a && b || !c
来源：http://fic.sysykeji.top

Java: a && b || !c
来源：http://azb.jlsjyb.cn

Go:   a && b || !c
来源：http://lyq.zycfv.cn

Ruby: a && b || !c
来源：http://bij.316326.xyz

C#:   a && b || !c
来源：http://xim.zhaomingkeji.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ymo.gotoacloud.top

Py:   if not data: return
来源：http://yab.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://nck.wangshuangyany.cn

JS:   if (!data) return;
来源：http://bav.ehwqpu.com

TS:   if (!data) return;
来源：http://whs.kuanghao11.cn

Java: if (data == null) return;
来源：http://ylb.pengpengdd.cyou

Go:   if data == nil { return }
来源：http://glj.hongshengwenyu.top

Ruby: return if data.nil?
来源：http://teu.havefunace.top

C#:   if (data == null) return;
来源：http://duk.aibaodan.cn


<!-- 参考信息 -->