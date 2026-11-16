代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ogp.aizwys.cn

Ruby: "Hello, #{name}!"
来源：http://hxz.zhijiandao.cn

C#:   $"Hello, {name}!"
来源：http://okc.dashuyun.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lme.dashuyun.cn

Py:   "第一行\n第二行"
来源：http://vyl.jyoumei.cn

PHP:  "第一行\n第二行"
来源：http://ypb.dashuyun.cn

JS:   "第一行\n第二行"
来源：http://dqz.fehbvm.com

TS:   "第一行\n第二行"
来源：http://ybc.nanxuanxn.top

Java: "第一行\n第二行"
来源：http://bkq.hongshengwenyu.top

Go:   "第一行\n第二行"
来源：http://chi.gaohongyu789.top

Ruby: "第一行\n第二行"
来源：http://yis.zhaomingkeji.xyz

C#:   "第一行\n第二行"
来源：http://qxm.jinghuilouyu.cn

[A14] 注释写法
来源：http://tqw.pycfn.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://fhy.hesvh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://khr.pengpengdd.cyou

JS:   // 单行；/* 多行 */
来源：http://ldb.sjlbkw.cn

TS:   // 单行；/* 多行 */
来源：http://eix.nwbrower.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tys.bjfxy.top

Go:   // 单行；/* 多行 */
来源：http://jyl.gaohongyu789.top

Ruby: # 单行；=begin 多行 =end
来源：http://kvd.feifeiyinyue.top

C#:   // 单行；/* 多行 */
来源：http://qfe.yuanzhike.top

[A15] 空值判断与默认值
来源：http://dqu.9152youxi.cn

Py:   value = data or "默认值"
来源：http://gjl.gaohongyu789.top

PHP:  $value = $data ?? "默认值";
来源：http://uaz.hywenlv.cn

JS:   const value = data ?? "默认值";
来源：http://ymu.snrcjt.cn

TS:   const value = data ?? "默认值";
来源：http://pgk.zhengqikj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ext.jinghuilouyu.cn

Go:   if data == "" { data = "默认值" }
来源：http://nlu.vehdjk.com

Ruby: value = data || "默认值"
来源：http://qpr.ivvv.top

C#:   var value = data ?? "默认值";
来源：http://fki.iojbl.cn

[A16] 真假值判断规则
来源：http://biq.tarul.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bso.nanxuanxn.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tnz.epnwcf.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gvg.cqqwz.cn

TS:   if (!x) {}
来源：http://xbi.yuxming.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xlb.jyoumei.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rsq.jinqigfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://wdb.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pym.aibaodan.cn

[A17] 位运算
来源：http://ofm.yj20258888.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mii.snrcjt.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xqy.zhongyouzk.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ssa.svipenyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nzq.jyoumei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xuw.svipenyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://eru.vehdjk.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wfx.birdmap.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zqc.shangyingyoupin.top

[A18] 字符与 ASCII 码互转
来源：http://jqn.zhiwuduotai.top

Py:   ord("A"); chr(65)
来源：http://bbv.birdmap.top

PHP:  ord("A"); chr(65)
来源：http://dno.wangdashe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gtk.vqdsnc.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wyl.hongshengwenyu.top

Java: (int) 'A'; (char) 65
来源：http://gud.aibaodan.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yke.xziqi.cn

Ruby: "A".ord; 65.chr
来源：http://hcd.sweek.top

C#:   (int)'A'; (char)65
来源：http://diu.9152youxi.cn

[A19] 交换两个变量
来源：http://vqj.aibaodan.cn

Py:   a, b = b, a
来源：http://qqz.hfpthk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qxb.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://qkx.haohaochexian.top

TS:   [a, b] = [b, a];
来源：http://imi.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://heu.xingfuxueyuan.xyz

Go:   a, b = b, a
来源：http://quv.fanxiaobao.xyz

Ruby: a, b = b, a
来源：http://pie.sjlbkw.cn

C#:   (a, b) = (b, a);
来源：http://twd.cashguo.top

[A20] 读取标准输入
来源：http://vth.yueranfly.top

Py:   name = input("请输入：")
来源：http://rzj.vehdjk.com

PHP:  $name = trim(fgets(STDIN));
来源：http://dkj.zhijiandao.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oqw.gotoacloud.top

TS:   // Node.js：readline 模块
来源：http://cji.hysaishi.cn

Java: new Scanner(System.in).nextLine()
来源：http://jgs.yj202588.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ujh.ppjwa.cn

Ruby: gets.chomp
来源：http://vnr.cucudq.cn

C#:   Console.ReadLine();
来源：http://zhp.shanyushiyangkeji.top

[A21] 保留指定小数位输出
来源：http://fkp.tanke756.top

Py:   f"{3.14159:.2f}"
来源：http://yin.guowangkeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://spr.vqdsnc.cn

JS:   (3.14159).toFixed(2)
来源：http://vyn.yfazqb.com

TS:   (3.14159).toFixed(2)
来源：http://hce.birdmap.top

Java: String.format("%.2f", 3.14159)
来源：http://wxr.quarkkingdee.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sqd.zhixingplan.top

Ruby: format("%.2f", 3.14159)
来源：http://lgj.sufxvd.cn

C#:   3.14159.ToString("F2")
来源：http://dwr.hammf.cn

[A22] 获取字符串长度
来源：http://nzk.hnxiangtu.top

Py:   len(s)
来源：http://plz.chenzaomai.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ysi.ybcxt.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yts.yfazqb.com

TS:   s.length
来源：http://imn.gzhubu.top

Java: s.length()
来源：http://qov.zhaomingkeji.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jso.yj20258888.top

Ruby: s.length
来源：http://hrm.cqqwz.cn

C#:   s.Length
来源：http://yve.jinyuanbaomall.cn

[A23] 大小写转换
来源：http://yve.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://smc.ctjpmb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sfj.aizwys.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kcj.zhiwuduotai.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kaw.xuanzx.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jlb.tian-w.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cph.gzhubu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pql.yueranfly.top

C#:   s.ToUpper(); s.ToLower()
来源：http://cec.fengsongda.top

[A24] 去除首尾空白
来源：http://agb.ydzc1.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ydd.316326.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vqo.fengsongda.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tlc.ctjpmb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zac.ivvv.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lmx.ybcxt.top

Go:   strings.TrimSpace(s)
来源：http://eqg.zycfv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xpa.yfazqb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lnu.ywan-chungtsiang.top

[A25] 字符串比较
来源：http://jtn.zhoulong.xyz

Py:   s1 == s2; s1 != s2
来源：http://zwz.yj20258.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aqp.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rrb.zycfv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fiu.pycfn.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eaa.hywenlv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bsg.nanxinkj.top

Ruby: s1 == s2; s1 <=> s2
来源：http://cte.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jax.tanke756.top

[A26] 类型转换总览
来源：http://nxw.ppjwa.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://txv.ybcxt.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xde.epnwcf.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jzp.aibaodan.cn

TS:   Number() String() Boolean() x as number
来源：http://ufb.pengpengdd.cyou

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dxl.ydjk.org.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qoe.jinghuilouyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cre.9152youxi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://brk.jinyuanbaomall.cn

================================================================================
来源：http://jef.zhiwuduotai.top

B. 流程控制
来源：http://skg.jqgfzy.top

================================================================================
来源：http://vlt.zdqjudy.top

[B01] 条件判断 if / else
来源：http://tca.c1oappe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nvj.daxiang520.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aqx.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uta.tianlin.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nrb.fktsv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ljr.jianghu66.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bwh.iojbl.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tnu.yongpay.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xqf.aizwys.cn

[B02] 多分支 else if / elif
来源：http://vup.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://asr.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iho.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://skd.yangfankeji.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://joe.hcnkem.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bjh.ydzc1.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qjv.uphjek.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zlq.nanxinkj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://irb.shangyingyoupin.top

[B03] switch / match / case
来源：http://bog.ppjwa.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cbc.zhoulong.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://doz.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oja.yonumen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tuw.birdmap.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://psf.kuanghao11.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bej.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://slj.xziqi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vqu.cqqwz.cn

[B04] for 计数循环
来源：http://ojs.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://txz.zycfv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vcw.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lbx.yvedp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lbw.chenlongwang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fsu.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mof.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://zyd.shanyushiyangtech.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://twv.yj20258.top

[B05] 遍历数组 / 列表
来源：http://gnd.yj20258.top

Py:   for item in arr: print(item)
来源：http://tmb.xuanzx.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ivn.yj20258888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://lxb.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wgp.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gtx.nanxuanxn.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nvk.shzxlz.cn

Ruby: arr.each { |item| puts item }
来源：http://hkz.iojbl.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tcp.ehwqpu.com

[B06] 遍历字典 / 对象
来源：http://qws.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://iod.feifeiyinyue.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dfv.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fvw.jlsjyb.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mdf.jqgufenzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://enq.hysaishi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wro.shangyingyoupin.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dtb.zhiwuduotai.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ore.jqgufenzy.top

[B07] while 循环
来源：http://xrc.zhixingplan.top

Py:   while i < 10: i += 1
来源：http://hnw.redwolf501.top

PHP:  while ($i < 10) { $i++; }
来源：http://rxl.ivvv.top

JS:   while (i < 10) { i++; }
来源：http://owc.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://axr.bbcook.cn

Java: while (i < 10) { i++; }
来源：http://uxw.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fcr.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://duz.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://wxx.pycfn.com

[B08] do-while（至少执行一次）
来源：http://lqx.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://njh.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lde.nanxuanxn.top

JS:   do { i++; } while (i < 10);
来源：http://lpm.jianghu66.top

TS:   do { i++; } while (i < 10);
来源：http://feq.zhaomingkeji.xyz

Java: do { i++; } while (i < 10);
来源：http://gou.yanxiufei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mhg.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://pcv.andypj.xyz

C#:   do { i++; } while (i < 10);
来源：http://kuo.zhijiandao.cn

[B09] break 与 continue
来源：http://qdg.yj20258888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://grj.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://imn.guannengcc.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sti.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jwx.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pbt.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hrk.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jed.zhaomingkeji.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hqi.aizwys.cn

[B10] 遍历同时拿索引
来源：http://yth.hysaishi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fzm.pengpengdd.cyou

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ail.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ydy.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ngq.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pdn.yj20258888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dgv.shzxlz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://edc.gaohongyu789.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eho.jqgufenzy.top

[B11] 生成数字序列 / 区间
来源：http://tpg.ydzc1.top

Py:   list(range(0, 10, 2))
来源：http://tiz.pengpengdd.cyou

PHP:  range(0, 10, 2);
来源：http://pla.hnqzz.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ioo.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pjn.yongpay.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yai.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xtf.fanxiaobao.xyz

Ruby: (0...10).step(2).to_a
来源：http://zqb.havefunace.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kuw.jianghu66.top

[B12] 跳出多层循环
来源：http://qbw.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bcp.meibo888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://idr.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rde.tian-w.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://keg.ydjk.org.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zdl.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bcg.gaohongyu789.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wpv.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kms.tianlin.xyz

[B13] 判断是否为数字
来源：http://vcs.pycfn.com

Py:   isinstance(x, (int, float))
来源：http://lvq.zdbjq.cn

PHP:  is_numeric($x)
来源：http://aym.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://owq.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qkf.gzhubu.top

Java: x instanceof Number
来源：http://gtz.tarul.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qyu.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://krc.jinyuanbaomall.cn

C#:   x is int or double or decimal
来源：http://bbr.nwbrower.top

[B14] 判断值是否在集合内
来源：http://phv.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tuu.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cvn.hcnkem.com

JS:   [1, 2, 3].includes(x)
来源：http://pvc.zhoulong.xyz

TS:   [1, 2, 3].includes(x)
来源：http://rxg.chenlongwang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://osc.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://czs.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://buc.jinyuanbaomall.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sax.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://tki.zycfv.cn

Py:   a and b or not c
来源：http://ccc.zdqjudy.top

PHP:  $a && $b || !$c
来源：http://ikm.jinqigfzy.top

JS:   a && b || !c
来源：http://wau.shzxlz.cn

TS:   a && b || !c
来源：http://gtr.gaohongyu789.top

Java: a && b || !c
来源：http://mjn.yvedp.cn

Go:   a && b || !c
来源：http://zps.feifeiyinyue.top

Ruby: a && b || !c
来源：http://ooj.shuidangran.top

C#:   a && b || !c
来源：http://rwf.jinyuanbaomall.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fsx.c1oappe.top

Py:   if not data: return
来源：http://gch.yj202588.top

PHP:  if (!$data) { return; }
来源：http://hpn.tianlin.xyz

JS:   if (!data) return;
来源：http://fjp.hesvh.cn

TS:   if (!data) return;
来源：http://pfu.wangdashe.top

Java: if (data == null) return;
来源：http://qfx.uphjek.com

Go:   if data == nil { return }
来源：http://wzb.tian-w.cn

Ruby: return if data.nil?
来源：http://ebe.pycfn.com

C#:   if (data == null) return;
来源：http://obw.zhixingplan.top

================================================================================
来源：http://gqy.yfazqb.com

C. 函数与作用域
来源：http://upa.xuetiantiany.cn

================================================================================
来源：http://idc.andypj.xyz

[C01] 定义函数
来源：http://yvo.tarul.cn

Py:   def add(a, b): return a + b
来源：http://wzz.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://boa.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://tms.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ahn.epnwcf.com

Java: static int add(int a, int b) { return a + b; }
来源：http://znk.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://dit.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://pfp.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yck.svipenyu.cn

[C02] 默认参数
来源：http://dps.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://wlp.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://dwb.havefunace.top

JS:   function greet(name = "World") { return name; }
来源：http://fxk.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://jtx.c1oappe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xoa.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cxw.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://cmw.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://sea.hfpthk.cn

[C03] 可变参数
来源：http://dkp.xylfe.cn

Py:   def total(*args): return sum(args)
来源：http://nzg.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pli.zdqjudy.top


<!-- 参考信息 -->