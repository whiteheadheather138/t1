代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://izl.gzhubu.top

Ruby: "Hello, #{name}!"
来源：http://cgi.shanyushiyangkeji.top

C#:   $"Hello, {name}!"
来源：http://epq.c1oappe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dew.aizwys.cn

Py:   "第一行\n第二行"
来源：http://idq.svipenyu.cn

PHP:  "第一行\n第二行"
来源：http://aoe.zycfv.cn

JS:   "第一行\n第二行"
来源：http://dir.uphjek.com

TS:   "第一行\n第二行"
来源：http://tyq.dashuyun.cn

Java: "第一行\n第二行"
来源：http://yxi.jqgfzy.top

Go:   "第一行\n第二行"
来源：http://kgx.nanxinkj.top

Ruby: "第一行\n第二行"
来源：http://xys.cheryme.top

C#:   "第一行\n第二行"
来源：http://qja.hongshengwenyu.top

[A14] 注释写法
来源：http://jtk.shuidangran.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://msl.gzhubu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pcb.shanyushiyangkeji.top

JS:   // 单行；/* 多行 */
来源：http://qap.cdnleiting.top

TS:   // 单行；/* 多行 */
来源：http://eoe.yongpay.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zza.kuanghao11.cn

Go:   // 单行；/* 多行 */
来源：http://upe.yongpay.top

Ruby: # 单行；=begin 多行 =end
来源：http://jqi.birdmap.top

C#:   // 单行；/* 多行 */
来源：http://hdi.yfazqb.com

[A15] 空值判断与默认值
来源：http://pfy.316326.xyz

Py:   value = data or "默认值"
来源：http://uqn.aizwys.cn

PHP:  $value = $data ?? "默认值";
来源：http://evz.yj202588.top

JS:   const value = data ?? "默认值";
来源：http://eiq.chenjidiqi.icu

TS:   const value = data ?? "默认值";
来源：http://hyg.ctjpmb.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rwl.hnqzz.top

Go:   if data == "" { data = "默认值" }
来源：http://mzm.snrcjt.cn

Ruby: value = data || "默认值"
来源：http://obm.ybcxt.top

C#:   var value = data ?? "默认值";
来源：http://cmq.haohaochexian.top

[A16] 真假值判断规则
来源：http://oai.aizwys.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wnm.yuxming.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://avn.cdnleiting.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qak.redwolf501.top

TS:   if (!x) {}
来源：http://gcq.xinyue.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://iyb.0kj1m.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qlp.ivvv.top

Ruby: unless x            # nil 与 false 为假
来源：http://zsg.52xcode.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eyh.tarul.cn

[A17] 位运算
来源：http://oyg.meibo888.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lpn.jinqigufen.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uhz.zdqjudy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gxs.jinqigufen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://msk.xziqi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://msz.wangshuangyany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hyq.aizwys.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ckd.yj20258.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bff.dianchejie.cn

[A18] 字符与 ASCII 码互转
来源：http://vim.xylfe.cn

Py:   ord("A"); chr(65)
来源：http://whp.dashuyun.cn

PHP:  ord("A"); chr(65)
来源：http://ngu.daxiang520.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zcp.shangyingyoupin.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fel.hcnkem.com

Java: (int) 'A'; (char) 65
来源：http://dxj.nwbrower.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nbz.nanxinkj.top

Ruby: "A".ord; 65.chr
来源：http://tbz.hnqzz.top

C#:   (int)'A'; (char)65
来源：http://rvm.hywenlv.cn

[A19] 交换两个变量
来源：http://ajs.hammf.cn

Py:   a, b = b, a
来源：http://qmh.guowangkeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://lkn.ydzc1.top

JS:   [a, b] = [b, a];
来源：http://gbo.pycfn.com

TS:   [a, b] = [b, a];
来源：http://vpp.yuanzhike.top

Java: int t = a; a = b; b = t;
来源：http://jty.chenzaomai.com

Go:   a, b = b, a
来源：http://axn.svipenyu.cn

Ruby: a, b = b, a
来源：http://xzc.ctjpmb.com

C#:   (a, b) = (b, a);
来源：http://cba.quarkkingdee.top

[A20] 读取标准输入
来源：http://bcf.xuetiantiany.cn

Py:   name = input("请输入：")
来源：http://fgl.daxiang520.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zrt.quarkkingdee.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gkx.zdbjq.cn

TS:   // Node.js：readline 模块
来源：http://aun.chenjidiqi.icu

Java: new Scanner(System.in).nextLine()
来源：http://ftw.fktsv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sra.cdnleiting.top

Ruby: gets.chomp
来源：http://gkf.vqdsnc.cn

C#:   Console.ReadLine();
来源：http://fma.sjlbkw.cn

[A21] 保留指定小数位输出
来源：http://pqu.sxryk.cn

Py:   f"{3.14159:.2f}"
来源：http://aza.pengpengdd.cyou

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eme.yuanzhike.top

JS:   (3.14159).toFixed(2)
来源：http://egn.shzxlz.cn

TS:   (3.14159).toFixed(2)
来源：http://xow.sysykeji.top

Java: String.format("%.2f", 3.14159)
来源：http://vne.andypj.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kgj.hesvh.cn

Ruby: format("%.2f", 3.14159)
来源：http://zkp.fanxiaobao.xyz

C#:   3.14159.ToString("F2")
来源：http://jyg.wangdashe.top

[A22] 获取字符串长度
来源：http://jmi.zhixingplan.top

Py:   len(s)
来源：http://ule.jlsjyb.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dvz.nwbrower.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://suc.yueranfly.top

TS:   s.length
来源：http://psl.hnxiangtu.top

Java: s.length()
来源：http://wnq.ppjwa.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ghp.daxiang520.top

Ruby: s.length
来源：http://xho.zhoulong.xyz

C#:   s.Length
来源：http://ono.fehbvm.com

[A23] 大小写转换
来源：http://dpq.cdnleiting.top

Py:   s.upper(); s.lower(); s.title()
来源：http://tfg.hesvh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ayo.hfpthk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wkb.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rsg.c1oappe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xdd.ydjk.org.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qyv.zhaomingkeji.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wxd.sufxvd.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dse.hfpthk.cn

[A24] 去除首尾空白
来源：http://jcv.fanxiaobao.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mus.zhixingplan.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://edk.chenzaomai.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ifu.cheryme.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yis.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://evm.iojbl.cn

Go:   strings.TrimSpace(s)
来源：http://wbk.ydjk.org.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uml.hnqzz.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ryk.sysykeji.top

[A25] 字符串比较
来源：http://ybq.ppjwa.cn

Py:   s1 == s2; s1 != s2
来源：http://gsc.hesvh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://krn.yuxming.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oii.aibaodan.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yhz.yfazqb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xcw.zdqjudy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ilc.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vwi.shanyushiyangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://apg.sufxvd.cn

[A26] 类型转换总览
来源：http://stj.mhx1999.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tpt.hnqzz.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gwg.ydjk.org.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tus.tianlin.xyz

TS:   Number() String() Boolean() x as number
来源：http://hfy.yongpay.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fgj.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jxi.yvedp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oli.birdmap.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lar.yonumen.top

================================================================================
来源：http://vzy.xinyue.icu

B. 流程控制
来源：http://dpc.iojbl.cn

================================================================================
来源：http://jyo.jqgufenzy.top

[B01] 条件判断 if / else
来源：http://vgj.vehdjk.com

Py:   result = "正" if x > 0 else "非正"
来源：http://iwu.zhaomingkeji.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hiz.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eya.jqgfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iwe.ivvv.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cze.ydjk.org.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gsl.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yol.yongpay.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dhi.aibaodan.cn

[B02] 多分支 else if / elif
来源：http://qpr.jinqigfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xtk.guannengcc.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yem.bjfxy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qcg.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://idv.shanyushiyangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jig.uphjek.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qio.kuanghao11.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wnb.zhaomingkeji.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nju.zhongyouzk.top

[B03] switch / match / case
来源：http://sbu.xingfuxueyuan.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nnt.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gmp.chenzaomai.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://efy.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nel.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wjd.shzxlz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tab.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://csf.guannengcc.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qnx.pycfn.com

[B04] for 计数循环
来源：http://hgj.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://snz.xinyue.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cvv.shzxlz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dlo.gzhubu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xdg.xuetiantiany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gkt.bjfxy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ihr.yanxiufei.cn

Ruby: 10.times { |i| puts i }
来源：http://oap.zhiwuduotai.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://onh.wangdashe.top

[B05] 遍历数组 / 列表
来源：http://itf.gogol.net.cn

Py:   for item in arr: print(item)
来源：http://nwq.tanke756.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qts.ppjwa.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://une.ybcxt.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zjg.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cno.aibaodan.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tmn.hnqzz.top

Ruby: arr.each { |item| puts item }
来源：http://oub.tarul.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rxe.nanxuanxn.top

[B06] 遍历字典 / 对象
来源：http://pzt.c1oappe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zcm.jianghu66.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aze.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qji.zhijiandao.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oux.ydjk.org.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://owo.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tgj.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://prq.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kiu.yonumen.top

[B07] while 循环
来源：http://lyq.xuetiantiany.cn

Py:   while i < 10: i += 1
来源：http://srl.zhaomingkeji.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ppq.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://dfo.ivvv.top

TS:   while (i < 10) { i++; }
来源：http://gai.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://grf.guowangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mfo.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://srq.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://qxe.xziqi.cn

[B08] do-while（至少执行一次）
来源：http://xuo.hammf.cn

Py:   # 无 do-while：用 while True + break
来源：http://wqj.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fsh.cheryme.top

JS:   do { i++; } while (i < 10);
来源：http://hwx.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://wgr.jyoumei.cn

Java: do { i++; } while (i < 10);
来源：http://ggs.guannengcc.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tlu.jlsjyb.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ylb.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://uzr.gotoacloud.top

[B09] break 与 continue
来源：http://ely.ppjwa.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wja.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vgf.hammf.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zbf.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oin.dashuyun.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ahx.ywan-chungtsiang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wpo.xylfe.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dyo.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://irk.yuxming.cn

[B10] 遍历同时拿索引
来源：http://thc.yuanzhike.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ytu.shuidangran.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vof.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lmm.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ldr.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ejg.shanyushiyangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nuy.bbcook.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ykn.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jvg.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://jhz.shanyushiyangkeji.top

Py:   list(range(0, 10, 2))
来源：http://vqm.jqgfzy.top

PHP:  range(0, 10, 2);
来源：http://ter.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gja.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://scf.yuxming.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lnd.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nvg.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://ygi.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zbz.daria6918.cn

[B12] 跳出多层循环
来源：http://opo.chenzaomai.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://tgm.zhongyouzk.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://voi.tianlin.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://grw.chenlongwang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ytv.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xrc.zhengqikj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ohg.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rhi.9152youxi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://abx.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://rsu.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://yyd.9152youxi.cn

PHP:  is_numeric($x)
来源：http://hbo.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ynh.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jsr.jinyuanbaomall.cn

Java: x instanceof Number
来源：http://zei.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ezq.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://zir.shzxlz.cn

C#:   x is int or double or decimal
来源：http://zbk.ydzc1.top

[B14] 判断值是否在集合内
来源：http://ktt.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xqj.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ftl.zdqjudy.top

JS:   [1, 2, 3].includes(x)
来源：http://nlq.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://zjm.jlsjyb.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xkl.sufxvd.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://stc.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qok.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qly.daria6918.cn

[B15] 布尔运算与取反
来源：http://llv.52xcode.cn

Py:   a and b or not c
来源：http://luy.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://gtl.hongshengwenyu.top

JS:   a && b || !c
来源：http://sby.cqqwz.cn

TS:   a && b || !c
来源：http://rnu.yonumen.top

Java: a && b || !c
来源：http://stb.fehbvm.com

Go:   a && b || !c
来源：http://qvc.9152youxi.cn

Ruby: a && b || !c
来源：http://xsi.yj20258888.top

C#:   a && b || !c
来源：http://mrv.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://coq.ybcxt.top

Py:   if not data: return
来源：http://nud.sxryk.cn

PHP:  if (!$data) { return; }
来源：http://tcm.yueranfly.top

JS:   if (!data) return;
来源：http://obr.yj20258888.top

TS:   if (!data) return;
来源：http://tim.redwolf501.top

Java: if (data == null) return;
来源：http://znl.guannengcc.top

Go:   if data == nil { return }
来源：http://mek.yj202588.top

Ruby: return if data.nil?
来源：http://sah.jqgfzy.top

C#:   if (data == null) return;
来源：http://phu.cheryme.top

================================================================================
来源：http://hxy.wangshuangyany.cn

C. 函数与作用域
来源：http://tmq.cqqwz.cn

================================================================================
来源：http://vsd.wangdashe.top

[C01] 定义函数
来源：http://smn.yanxiufei.cn

Py:   def add(a, b): return a + b
来源：http://ooy.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eco.fehbvm.com

JS:   function add(a, b) { return a + b; }
来源：http://rll.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jlf.guannengcc.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fwf.pycfn.com

Go:   func add(a, b int) int { return a + b }
来源：http://zqw.zdqjudy.top

Ruby: def add(a, b); a + b; end
来源：http://hfe.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://psd.vehdjk.com

[C02] 默认参数
来源：http://hbq.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://fod.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://xrh.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://czw.ybcxt.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jpo.cdnleiting.top

Java: // 无默认参数：方法重载或 Optional
来源：http://obr.c1oappe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ssc.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://sks.tanke756.top

C#:   string Greet(string name = "World") => name;
来源：http://vrb.yuanzhike.top

[C03] 可变参数
来源：http://zzo.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://atg.jianghu66.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://anv.yonumen.top


<!-- 参考信息 -->