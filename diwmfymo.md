代发 wailian999

Py:   "第一行\n第二行"
来源：http://fxy.nanxuanxn.top

PHP:  "第一行\n第二行"
来源：http://ryl.feifeiyinyue.top

JS:   "第一行\n第二行"
来源：http://sfh.birdmap.top

TS:   "第一行\n第二行"
来源：http://nkh.daria6918.cn

Java: "第一行\n第二行"
来源：http://lol.aizwys.cn

Go:   "第一行\n第二行"
来源：http://fjw.sjlbkw.cn

Ruby: "第一行\n第二行"
来源：http://oia.jinyuanbaomall.cn

C#:   "第一行\n第二行"
来源：http://rwv.xuetiantiany.cn

[A14] 注释写法
来源：http://maw.yanxiufei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://eeu.snrcjt.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tor.zhongyouzk.top

JS:   // 单行；/* 多行 */
来源：http://jtr.xylfe.cn

TS:   // 单行；/* 多行 */
来源：http://rkh.yueranfly.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rks.shzxlz.cn

Go:   // 单行；/* 多行 */
来源：http://iod.mhx1999.top

Ruby: # 单行；=begin 多行 =end
来源：http://rdt.sufxvd.cn

C#:   // 单行；/* 多行 */
来源：http://kat.quarkkingdee.top

[A15] 空值判断与默认值
来源：http://zea.nwbrower.top

Py:   value = data or "默认值"
来源：http://wgy.ivvv.top

PHP:  $value = $data ?? "默认值";
来源：http://scr.xinyue.icu

JS:   const value = data ?? "默认值";
来源：http://kbx.quarkkingdee.top

TS:   const value = data ?? "默认值";
来源：http://oxk.tarul.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bzm.hammf.cn

Go:   if data == "" { data = "默认值" }
来源：http://eza.xuanzx.com

Ruby: value = data || "默认值"
来源：http://pzx.tanke756.top

C#:   var value = data ?? "默认值";
来源：http://got.cucudq.cn

[A16] 真假值判断规则
来源：http://qvq.quarkkingdee.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vrv.yongpay.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gfn.andypj.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qzf.aibaodan.cn

TS:   if (!x) {}
来源：http://wjc.iojbl.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://aly.ctjpmb.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kvi.jinqigufen.top

Ruby: unless x            # nil 与 false 为假
来源：http://hwp.cheryme.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cho.wangshuangyany.cn

[A17] 位运算
来源：http://cjn.316326.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fkz.daxiang520.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zbc.bjfxy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aqd.shangyingyoupin.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://soh.wangshuangyany.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rkf.fengsongda.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://idi.gogol.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bcq.zycfv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dql.chenzaomai.com

[A18] 字符与 ASCII 码互转
来源：http://bme.pycfn.com

Py:   ord("A"); chr(65)
来源：http://jhx.zdqjudy.top

PHP:  ord("A"); chr(65)
来源：http://ybf.c1oappe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jli.jianghu66.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wou.ywan-chungtsiang.top

Java: (int) 'A'; (char) 65
来源：http://bdu.hysaishi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oop.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://cbc.xuetiantiany.cn

C#:   (int)'A'; (char)65
来源：http://lim.vqdsnc.cn

[A19] 交换两个变量
来源：http://kha.hesvh.cn

Py:   a, b = b, a
来源：http://pcj.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://njd.jianghu66.top

JS:   [a, b] = [b, a];
来源：http://zjz.epnwcf.com

TS:   [a, b] = [b, a];
来源：http://xhq.zhengqikj.top

Java: int t = a; a = b; b = t;
来源：http://uws.aizwys.cn

Go:   a, b = b, a
来源：http://hpp.hammf.cn

Ruby: a, b = b, a
来源：http://mys.jqgfzy.top

C#:   (a, b) = (b, a);
来源：http://str.316326.xyz

[A20] 读取标准输入
来源：http://bva.ctjpmb.com

Py:   name = input("请输入：")
来源：http://huq.hfpthk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xqi.xuanzx.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ygl.zhengqikj.top

TS:   // Node.js：readline 模块
来源：http://uti.fktsv.cn

Java: new Scanner(System.in).nextLine()
来源：http://nrn.tian-w.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://crx.yj202588.top

Ruby: gets.chomp
来源：http://ifa.cdnleiting.top

C#:   Console.ReadLine();
来源：http://evi.redwolf501.top

[A21] 保留指定小数位输出
来源：http://zhl.hesvh.cn

Py:   f"{3.14159:.2f}"
来源：http://yge.316326.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hjl.kuanghao11.cn

JS:   (3.14159).toFixed(2)
来源：http://sta.ctjpmb.com

TS:   (3.14159).toFixed(2)
来源：http://day.cashguo.top

Java: String.format("%.2f", 3.14159)
来源：http://soh.ydzc1.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uub.kuanghao11.cn

Ruby: format("%.2f", 3.14159)
来源：http://ixv.dashuyun.cn

C#:   3.14159.ToString("F2")
来源：http://rcs.hammf.cn

[A22] 获取字符串长度
来源：http://fat.cqqwz.cn

Py:   len(s)
来源：http://gka.chenjidiqi.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://szv.ybcxt.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nxp.xylfe.cn

TS:   s.length
来源：http://mjk.mhx1999.top

Java: s.length()
来源：http://yyr.aibaodan.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yak.andypj.xyz

Ruby: s.length
来源：http://rgv.shzxlz.cn

C#:   s.Length
来源：http://rke.jiagoushi.top

[A23] 大小写转换
来源：http://vpm.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://iaq.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bua.daria6918.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jsf.tianlin.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yod.hfpthk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ibw.52xcode.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qxw.jyoumei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qii.guowangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pom.xziqi.cn

[A24] 去除首尾空白
来源：http://ahu.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lwp.cdnleiting.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pjw.yongpay.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dhw.zhiwuduotai.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zxq.cdnleiting.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://igt.xziqi.cn

Go:   strings.TrimSpace(s)
来源：http://vme.gogol.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ksm.yanxiufei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vmm.xingfuxueyuan.xyz

[A25] 字符串比较
来源：http://hyu.chenjidiqi.icu

Py:   s1 == s2; s1 != s2
来源：http://zxt.nanxuanxn.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://khm.jiagoushi.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cxd.aibaodan.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qnr.fehbvm.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kip.pycfn.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vtd.yvedp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cqv.havefunace.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ice.sxryk.cn

[A26] 类型转换总览
来源：http://toy.guannengcc.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dmb.havefunace.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rrp.gzhubu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rih.shuidangran.top

TS:   Number() String() Boolean() x as number
来源：http://ntt.yuxming.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://due.fehbvm.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mua.guowangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://snt.aibaodan.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pzo.zdqjudy.top

================================================================================
来源：http://kgt.cqqwz.cn

B. 流程控制
来源：http://hvu.ybcxt.top

================================================================================
来源：http://bkj.zhoulong.xyz

[B01] 条件判断 if / else
来源：http://awc.tanke756.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bal.zhongyouzk.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cgq.jiagoushi.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zoj.svipenyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ruw.andypj.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://new.sysykeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zlh.dianchejie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eid.wangshuangyany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hop.hysaishi.cn

[B02] 多分支 else if / elif
来源：http://myb.tarul.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tgj.aizwys.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dnb.uphjek.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mbf.9152youxi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rrh.ybcxt.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ree.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sdl.vqdsnc.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jij.ppjwa.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ged.c1oappe.top

[B03] switch / match / case
来源：http://grn.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yqn.sweek.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uxg.ydzc1.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aww.chenzaomai.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qpf.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jtf.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://syk.ywan-chungtsiang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oyb.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pqk.epnwcf.com

[B04] for 计数循环
来源：http://nbs.jinqigfzy.top

Py:   for i in range(10): print(i)
来源：http://urb.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ysz.zhongyouzk.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rly.smart0.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mrx.sxryk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ooa.zhixingplan.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qzs.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://gsj.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fpg.hnqzz.top

[B05] 遍历数组 / 列表
来源：http://huq.redwolf501.top

Py:   for item in arr: print(item)
来源：http://www.ehwqpu.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dbe.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nxx.mhx1999.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rxw.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kxj.dashuyun.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zwi.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://voq.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uvq.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://reu.hesvh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xbv.sweek.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qqp.hongshengwenyu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ooo.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uen.havefunace.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xkn.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jzc.yuxming.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qbu.sxryk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xvc.bbcook.cn

[B07] while 循环
来源：http://rvy.yvedp.cn

Py:   while i < 10: i += 1
来源：http://mmw.guannengcc.top

PHP:  while ($i < 10) { $i++; }
来源：http://ifs.hesvh.cn

JS:   while (i < 10) { i++; }
来源：http://nuz.jinqigufen.top

TS:   while (i < 10) { i++; }
来源：http://qia.birdmap.top

Java: while (i < 10) { i++; }
来源：http://xpp.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pgz.sysykeji.top

Ruby: while i < 10; i += 1; end
来源：http://jlk.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://igh.fanxiaobao.xyz

[B08] do-while（至少执行一次）
来源：http://azx.shanyushiyangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://cfl.wangshuangyany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vkq.shuidangran.top

JS:   do { i++; } while (i < 10);
来源：http://cqd.zhixingplan.top

TS:   do { i++; } while (i < 10);
来源：http://uhu.chenlongwang.top

Java: do { i++; } while (i < 10);
来源：http://dki.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dam.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://yam.hcnkem.com

C#:   do { i++; } while (i < 10);
来源：http://qfc.sjlbkw.cn

[B09] break 与 continue
来源：http://aog.yj20258888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yht.aizwys.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://esl.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qoi.xuanzx.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ljy.zhijiandao.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nqa.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://atq.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hqr.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hgx.hongshengwenyu.top

[B10] 遍历同时拿索引
来源：http://fhl.chenlongwang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pih.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dhy.fehbvm.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wdr.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jlx.hfpthk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xox.yonumen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dcl.xuanzx.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zpe.hnxiangtu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zfb.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://ffg.aibaodan.cn

Py:   list(range(0, 10, 2))
来源：http://qwn.tian-w.cn

PHP:  range(0, 10, 2);
来源：http://jor.dianchejie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rpl.tianlin.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ynj.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dvg.nanxuanxn.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://say.xinyue.icu

Ruby: (0...10).step(2).to_a
来源：http://idl.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cax.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://bld.aizwys.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nvs.gotoacloud.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://psi.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uvf.birdmap.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cxy.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://utw.xingfuxueyuan.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mmq.sweek.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kmh.hfpthk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kvu.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://xzi.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://rac.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://azs.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iqk.tanke756.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ajm.yonumen.top

Java: x instanceof Number
来源：http://ema.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mks.zycfv.cn

Ruby: x.is_a?(Numeric)
来源：http://mwt.hesvh.cn

C#:   x is int or double or decimal
来源：http://gpl.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://xzl.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zpn.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hkc.cheryme.top

JS:   [1, 2, 3].includes(x)
来源：http://epd.yfazqb.com

TS:   [1, 2, 3].includes(x)
来源：http://ntn.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hsq.kuanghao11.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lgm.c1oappe.top

Ruby: [1, 2, 3].include?(x)
来源：http://oaa.yonumen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://myb.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://tbp.ywan-chungtsiang.top

Py:   a and b or not c
来源：http://miq.epnwcf.com

PHP:  $a && $b || !$c
来源：http://kib.jinqigufen.top

JS:   a && b || !c
来源：http://mds.zhongyouzk.top

TS:   a && b || !c
来源：http://ena.aizwys.cn

Java: a && b || !c
来源：http://deo.ydjk.org.cn

Go:   a && b || !c
来源：http://hfp.zhengqikj.top

Ruby: a && b || !c
来源：http://wpv.hammf.cn

C#:   a && b || !c
来源：http://xaf.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://epd.pengpengdd.cyou

Py:   if not data: return
来源：http://tnr.zdbjq.cn

PHP:  if (!$data) { return; }
来源：http://fqj.redwolf501.top

JS:   if (!data) return;
来源：http://hbh.shanyushiyangkeji.top

TS:   if (!data) return;
来源：http://fwt.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://sch.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://zed.zhixingplan.top

Ruby: return if data.nil?
来源：http://wuu.dianchejie.cn

C#:   if (data == null) return;
来源：http://yln.cucudq.cn

================================================================================
来源：http://atu.hywenlv.cn

C. 函数与作用域
来源：http://iki.shanyushiyangkeji.top

================================================================================
来源：http://eur.yonumen.top

[C01] 定义函数
来源：http://rfq.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://nml.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zvx.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://qrr.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mnr.guannengcc.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vrp.svipenyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sxo.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://pdg.shanyushiyangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gjx.ydzc1.top

[C02] 默认参数
来源：http://rnc.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://fac.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://aez.hnqzz.top

JS:   function greet(name = "World") { return name; }
来源：http://ojz.hongshengwenyu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pom.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ufl.fanxiaobao.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ikj.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://qne.52xcode.cn

C#:   string Greet(string name = "World") => name;
来源：http://ptd.cucudq.cn

[C03] 可变参数
来源：http://nyi.hcnkem.com

Py:   def total(*args): return sum(args)
来源：http://cgk.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mdo.9152youxi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rvs.wangshuangyany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://svs.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vur.hongshengwenyu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lkw.gogol.net.cn


<!-- 参考信息 -->