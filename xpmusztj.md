代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://ooh.cashguo.top

C#:   x > 0 ? "yes" : "no"
来源：http://wbo.fzhhl.top

[A12] 字符串插值 / 格式化
来源：http://pdf.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eis.hesvh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lsi.hammf.cn

JS:   `Hello, ${name}!`
来源：http://thl.9152youxi.cn

TS:   `Hello, ${name}!`
来源：http://acv.jqgufenzy.top

Java: "Hello, %s!".formatted(name)
来源：http://ery.jinyuanbaomall.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dba.mhx1999.top

Ruby: "Hello, #{name}!"
来源：http://zhw.pycfn.com

C#:   $"Hello, {name}!"
来源：http://sqv.316326.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://hjq.xinyue.icu

Py:   "第一行\n第二行"
来源：http://bdj.gzhubu.top

PHP:  "第一行\n第二行"
来源：http://hde.tianlin.xyz

JS:   "第一行\n第二行"
来源：http://zxu.cheryme.top

TS:   "第一行\n第二行"
来源：http://mgh.guannengcc.top

Java: "第一行\n第二行"
来源：http://wof.ehwqpu.com

Go:   "第一行\n第二行"
来源：http://kes.feifeiyinyue.top

Ruby: "第一行\n第二行"
来源：http://pte.snrcjt.cn

C#:   "第一行\n第二行"
来源：http://qtb.tanke756.top

[A14] 注释写法
来源：http://plm.yfazqb.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://rxw.sweek.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://kih.hnxiangtu.top

JS:   // 单行；/* 多行 */
来源：http://caw.zhiwuduotai.top

TS:   // 单行；/* 多行 */
来源：http://jqj.hnqzz.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ebk.dianchejie.cn

Go:   // 单行；/* 多行 */
来源：http://dvs.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xst.nanxuanxn.top

C#:   // 单行；/* 多行 */
来源：http://use.tanke756.top

[A15] 空值判断与默认值
来源：http://hnx.jinqigufen.top

Py:   value = data or "默认值"
来源：http://qra.yfazqb.com

PHP:  $value = $data ?? "默认值";
来源：http://ckr.dianchejie.cn

JS:   const value = data ?? "默认值";
来源：http://duf.yfazqb.com

TS:   const value = data ?? "默认值";
来源：http://avm.quarkkingdee.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jjq.jinqigufen.top

Go:   if data == "" { data = "默认值" }
来源：http://gkb.jiagoushi.top

Ruby: value = data || "默认值"
来源：http://why.hcnkem.com

C#:   var value = data ?? "默认值";
来源：http://qrw.9152youxi.cn

[A16] 真假值判断规则
来源：http://qyo.wangshuangyany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wpb.iojbl.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bhi.0kj1m.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uhh.yongpay.top

TS:   if (!x) {}
来源：http://pll.zhiwuduotai.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nbe.guannengcc.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zpi.cashguo.top

Ruby: unless x            # nil 与 false 为假
来源：http://qtt.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ity.tarul.cn

[A17] 位运算
来源：http://asg.shzxlz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vds.zhixingplan.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fht.jyoumei.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hgb.dashuyun.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ebl.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dnu.gotoacloud.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kay.yfazqb.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jpj.shangyingyoupin.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qvj.redwolf501.top

[A18] 字符与 ASCII 码互转
来源：http://dwe.hongshengwenyu.top

Py:   ord("A"); chr(65)
来源：http://uum.yuxming.cn

PHP:  ord("A"); chr(65)
来源：http://fie.zhoulong.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ade.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oov.sysykeji.top

Java: (int) 'A'; (char) 65
来源：http://igj.shanyushiyangtech.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gri.jlsjyb.cn

Ruby: "A".ord; 65.chr
来源：http://jvo.shzxlz.cn

C#:   (int)'A'; (char)65
来源：http://xpb.sxryk.cn

[A19] 交换两个变量
来源：http://vkj.yj20258888.top

Py:   a, b = b, a
来源：http://ygn.yueranfly.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xyy.shuidangran.top

JS:   [a, b] = [b, a];
来源：http://poa.aibaodan.cn

TS:   [a, b] = [b, a];
来源：http://hmg.hammf.cn

Java: int t = a; a = b; b = t;
来源：http://qof.hnxiangtu.top

Go:   a, b = b, a
来源：http://ytk.gogol.net.cn

Ruby: a, b = b, a
来源：http://iiy.cashguo.top

C#:   (a, b) = (b, a);
来源：http://smz.sweek.top

[A20] 读取标准输入
来源：http://rpy.chenlongwang.top

Py:   name = input("请输入：")
来源：http://dzl.ppjwa.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pfv.chenlongwang.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ooj.snrcjt.cn

TS:   // Node.js：readline 模块
来源：http://ahu.jianghu66.top

Java: new Scanner(System.in).nextLine()
来源：http://ozh.zhongyouzk.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ozj.aibaodan.cn

Ruby: gets.chomp
来源：http://esn.chenjidiqi.icu

C#:   Console.ReadLine();
来源：http://rbo.wangshuangyany.cn

[A21] 保留指定小数位输出
来源：http://zov.pengpengdd.cyou

Py:   f"{3.14159:.2f}"
来源：http://meq.shuidangran.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fqu.hongshengwenyu.top

JS:   (3.14159).toFixed(2)
来源：http://orp.ydjk.org.cn

TS:   (3.14159).toFixed(2)
来源：http://ien.yonumen.top

Java: String.format("%.2f", 3.14159)
来源：http://ttw.vqdsnc.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pdh.fengsongda.top

Ruby: format("%.2f", 3.14159)
来源：http://chm.jinqigufen.top

C#:   3.14159.ToString("F2")
来源：http://fmq.andypj.xyz

[A22] 获取字符串长度
来源：http://uzm.sxryk.cn

Py:   len(s)
来源：http://xfl.gzhubu.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://poy.xuanzx.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uax.jinqigufen.top

TS:   s.length
来源：http://jss.ybcxt.top

Java: s.length()
来源：http://kyt.pycfn.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pik.ivvv.top

Ruby: s.length
来源：http://aez.uphjek.com

C#:   s.Length
来源：http://jnt.shanyushiyangtech.top

[A23] 大小写转换
来源：http://spe.aibaodan.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bzr.yj202588.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qou.yangfankeji.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lco.daria6918.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dlr.tianlin.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://otc.jqgufenzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pmu.ivvv.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xud.shzxlz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://heu.aibaodan.cn

[A24] 去除首尾空白
来源：http://oqb.birdmap.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://srd.yfazqb.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ppu.9152youxi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qri.shanyushiyangtech.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vsy.dashuyun.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vpv.haohaochexian.top

Go:   strings.TrimSpace(s)
来源：http://uzb.pycfn.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hao.yfazqb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lpy.yuxming.cn

[A25] 字符串比较
来源：http://baa.andypj.xyz

Py:   s1 == s2; s1 != s2
来源：http://cft.gogol.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://szk.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qui.ydjk.org.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ldz.fanxiaobao.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fwc.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jct.jinyuanbaomall.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mmy.wangdashe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dnu.shangyingyoupin.top

[A26] 类型转换总览
来源：http://jdf.ybcxt.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zsa.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mpg.yuanzhike.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://itv.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://qgv.tanke756.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zfx.shzxlz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vsk.smart0.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://mtr.ppjwa.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uuh.zycfv.cn

================================================================================
来源：http://ujz.nanxuanxn.top

B. 流程控制
来源：http://wzx.9152youxi.cn

================================================================================
来源：http://hwy.xziqi.cn

[B01] 条件判断 if / else
来源：http://zob.zhoulong.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://hfg.hysaishi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ifr.nanxuanxn.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zzq.sjlbkw.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wdi.sufxvd.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hac.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ptj.jiagoushi.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rqi.jqgfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zkk.andypj.xyz

[B02] 多分支 else if / elif
来源：http://nnb.cucudq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://una.zdqjudy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://umg.yj20258888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bdo.wangdashe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ngf.xylfe.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzu.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dor.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uhh.jinghuilouyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sdl.jinqigufen.top

[B03] switch / match / case
来源：http://iav.yvedp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gde.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ibb.zhixingplan.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vhw.mhx1999.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vzh.gogol.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nzd.yanxiufei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gdu.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://geu.zhijiandao.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://drd.redwolf501.top

[B04] for 计数循环
来源：http://rfp.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://nop.yj20258888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ywu.wangdashe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tzj.cheryme.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ehk.shuidangran.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fwf.yangfankeji.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kyl.yfazqb.com

Ruby: 10.times { |i| puts i }
来源：http://jir.zdbjq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zef.sjlbkw.cn

[B05] 遍历数组 / 列表
来源：http://kri.andypj.xyz

Py:   for item in arr: print(item)
来源：http://mrl.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ayt.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://bum.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jxk.hammf.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xrq.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cpa.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://ygt.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bjg.hesvh.cn

[B06] 遍历字典 / 对象
来源：http://bia.pycfn.com

Py:   for k, v in d.items(): print(k, v)
来源：http://lak.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jtc.zdbjq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qxh.ywan-chungtsiang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eqd.iojbl.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://med.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yra.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://utq.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rie.shanyushiyangkeji.top

[B07] while 循环
来源：http://xky.hywenlv.cn

Py:   while i < 10: i += 1
来源：http://nub.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://dzy.chenzaomai.com

JS:   while (i < 10) { i++; }
来源：http://fax.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://ome.cheryme.top

Java: while (i < 10) { i++; }
来源：http://dey.316326.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cbg.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://hiv.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://vev.yj20258888.top

[B08] do-while（至少执行一次）
来源：http://zxd.xuetiantiany.cn

Py:   # 无 do-while：用 while True + break
来源：http://ank.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tuh.sweek.top

JS:   do { i++; } while (i < 10);
来源：http://utu.daxiang520.top

TS:   do { i++; } while (i < 10);
来源：http://cop.xuetiantiany.cn

Java: do { i++; } while (i < 10);
来源：http://fwk.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uqw.zhixingplan.top

Ruby: begin; i += 1; end while i < 10
来源：http://pqf.jyoumei.cn

C#:   do { i++; } while (i < 10);
来源：http://czb.hesvh.cn

[B09] break 与 continue
来源：http://tko.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kpx.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eqm.yvedp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jib.cheryme.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://chr.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wjp.cucudq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dya.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gvk.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jyy.xuetiantiany.cn

[B10] 遍历同时拿索引
来源：http://lmh.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iou.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kyp.hammf.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oyh.gogol.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zjr.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://arj.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wej.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kha.zdqjudy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ycp.cdnleiting.top

[B11] 生成数字序列 / 区间
来源：http://qpe.hnqzz.top

Py:   list(range(0, 10, 2))
来源：http://mdy.xinyue.icu

PHP:  range(0, 10, 2);
来源：http://ion.snrcjt.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://obo.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hwu.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pxq.zhongyouzk.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fac.fehbvm.com

Ruby: (0...10).step(2).to_a
来源：http://sjj.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oqo.cucudq.cn

[B12] 跳出多层循环
来源：http://wjs.cheryme.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wem.yfazqb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://sqq.cqqwz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://crw.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vee.zhixingplan.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jos.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wuo.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eib.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pbz.wangdashe.top

[B13] 判断是否为数字
来源：http://omz.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://nkt.bjfxy.top

PHP:  is_numeric($x)
来源：http://bav.shanyushiyangtech.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gte.fanxiaobao.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pgk.0kj1m.cn

Java: x instanceof Number
来源：http://kfa.sjlbkw.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zlr.yuanzhike.top

Ruby: x.is_a?(Numeric)
来源：http://pyj.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://iyz.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://dvn.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pnd.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://noc.hysaishi.cn

JS:   [1, 2, 3].includes(x)
来源：http://ufs.aibaodan.cn

TS:   [1, 2, 3].includes(x)
来源：http://ubm.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rcj.zdbjq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lwh.bbcook.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ppb.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tsd.ivvv.top

[B15] 布尔运算与取反
来源：http://wql.cashguo.top

Py:   a and b or not c
来源：http://alx.jinghuilouyu.cn

PHP:  $a && $b || !$c
来源：http://son.havefunace.top

JS:   a && b || !c
来源：http://kik.vqdsnc.cn

TS:   a && b || !c
来源：http://tlg.ydjk.org.cn

Java: a && b || !c
来源：http://twd.chenlongwang.top

Go:   a && b || !c
来源：http://fta.gogol.net.cn

Ruby: a && b || !c
来源：http://qzz.quarkkingdee.top

C#:   a && b || !c
来源：http://fza.tarul.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ihz.jqgufenzy.top

Py:   if not data: return
来源：http://vvt.jianghu66.top

PHP:  if (!$data) { return; }
来源：http://yaj.zdqjudy.top

JS:   if (!data) return;
来源：http://uob.havefunace.top

TS:   if (!data) return;
来源：http://vxo.zhoulong.xyz

Java: if (data == null) return;
来源：http://dut.zhoulong.xyz

Go:   if data == nil { return }
来源：http://gkx.pycfn.com

Ruby: return if data.nil?
来源：http://lmj.daxiang520.top

C#:   if (data == null) return;
来源：http://hnf.kuanghao11.cn

================================================================================
来源：http://kbh.316326.xyz

C. 函数与作用域
来源：http://hpb.yonumen.top

================================================================================
来源：http://ici.bjfxy.top

[C01] 定义函数
来源：http://khc.cucudq.cn

Py:   def add(a, b): return a + b
来源：http://lce.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qmv.nanxuanxn.top

JS:   function add(a, b) { return a + b; }
来源：http://jiq.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ans.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nsf.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://pyy.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://olk.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blc.jlsjyb.cn

[C02] 默认参数
来源：http://bgz.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://kqb.zhiwuduotai.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gao.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://tan.hcnkem.com


<!-- 参考信息 -->