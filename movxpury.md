代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cki.hcnkem.com

JS:   `Hello, ${name}!`
来源：http://okm.c1oappe.top

TS:   `Hello, ${name}!`
来源：http://ysl.hfpthk.cn

Java: "Hello, %s!".formatted(name)
来源：http://cxq.vqdsnc.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sua.bbcook.cn

Ruby: "Hello, #{name}!"
来源：http://iii.feifeiyinyue.top

C#:   $"Hello, {name}!"
来源：http://ool.redwolf501.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lze.sweek.top

Py:   "第一行\n第二行"
来源：http://rsf.jyoumei.cn

PHP:  "第一行\n第二行"
来源：http://ecf.bjfxy.top

JS:   "第一行\n第二行"
来源：http://mji.hesvh.cn

TS:   "第一行\n第二行"
来源：http://sde.gotoacloud.top

Java: "第一行\n第二行"
来源：http://txm.hongshengwenyu.top

Go:   "第一行\n第二行"
来源：http://swo.guannengcc.top

Ruby: "第一行\n第二行"
来源：http://buv.yuxming.cn

C#:   "第一行\n第二行"
来源：http://hig.hfpthk.cn

[A14] 注释写法
来源：http://chb.dianchejie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bio.hfpthk.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ikr.aibaodan.cn

JS:   // 单行；/* 多行 */
来源：http://teh.zycfv.cn

TS:   // 单行；/* 多行 */
来源：http://lyh.yvedp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cqg.hammf.cn

Go:   // 单行；/* 多行 */
来源：http://nzm.jiagoushi.top

Ruby: # 单行；=begin 多行 =end
来源：http://nke.hnxiangtu.top

C#:   // 单行；/* 多行 */
来源：http://teq.yangfankeji.com

[A15] 空值判断与默认值
来源：http://reh.hfpthk.cn

Py:   value = data or "默认值"
来源：http://unj.yvedp.cn

PHP:  $value = $data ?? "默认值";
来源：http://wkz.haohaochexian.top

JS:   const value = data ?? "默认值";
来源：http://tyu.shuidangran.top

TS:   const value = data ?? "默认值";
来源：http://hqx.hywenlv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tez.guowangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://ltx.zycfv.cn

Ruby: value = data || "默认值"
来源：http://sgw.zhaomingkeji.xyz

C#:   var value = data ?? "默认值";
来源：http://uyj.sxryk.cn

[A16] 真假值判断规则
来源：http://iqr.daxiang520.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yqp.yuxming.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mbx.tanke756.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fnk.cucudq.cn

TS:   if (!x) {}
来源：http://tmk.zhiwuduotai.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zxk.sjlbkw.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://swu.xuanzx.com

Ruby: unless x            # nil 与 false 为假
来源：http://qco.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mgr.jlsjyb.cn

[A17] 位运算
来源：http://mdy.shanyushiyangtech.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fjs.shuidangran.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sno.xinyue.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dbc.daria6918.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://eit.xuanzx.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://clv.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gjj.hnqzz.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://quu.yonumen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jkx.xingfuxueyuan.xyz

[A18] 字符与 ASCII 码互转
来源：http://wkj.pengpengdd.cyou

Py:   ord("A"); chr(65)
来源：http://sdi.dashuyun.cn

PHP:  ord("A"); chr(65)
来源：http://ldk.zdqjudy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fxk.hfpthk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://csi.0kj1m.cn

Java: (int) 'A'; (char) 65
来源：http://bwu.fanxiaobao.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vjd.jianghu66.top

Ruby: "A".ord; 65.chr
来源：http://mmk.zdbjq.cn

C#:   (int)'A'; (char)65
来源：http://qna.zhiwuduotai.top

[A19] 交换两个变量
来源：http://kto.fengsongda.top

Py:   a, b = b, a
来源：http://lhb.zhaomingkeji.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://gci.pycfn.com

JS:   [a, b] = [b, a];
来源：http://hfr.yvedp.cn

TS:   [a, b] = [b, a];
来源：http://cxa.cashguo.top

Java: int t = a; a = b; b = t;
来源：http://tzc.yanxiufei.cn

Go:   a, b = b, a
来源：http://dsy.shzxlz.cn

Ruby: a, b = b, a
来源：http://xvq.yonumen.top

C#:   (a, b) = (b, a);
来源：http://uxd.jianghu66.top

[A20] 读取标准输入
来源：http://kzt.yonumen.top

Py:   name = input("请输入：")
来源：http://lkr.yanxiufei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xro.yueranfly.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tam.chenzaomai.com

TS:   // Node.js：readline 模块
来源：http://ayj.jinghuilouyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://bdy.sysykeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kox.pengpengdd.cyou

Ruby: gets.chomp
来源：http://kup.jiagoushi.top

C#:   Console.ReadLine();
来源：http://nze.yj20258888.top

[A21] 保留指定小数位输出
来源：http://fyw.ybcxt.top

Py:   f"{3.14159:.2f}"
来源：http://zxe.jinyuanbaomall.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rjq.jyoumei.cn

JS:   (3.14159).toFixed(2)
来源：http://awp.gogol.net.cn

TS:   (3.14159).toFixed(2)
来源：http://etf.jiagoushi.top

Java: String.format("%.2f", 3.14159)
来源：http://ufp.birdmap.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bvj.jinqigufen.top

Ruby: format("%.2f", 3.14159)
来源：http://oim.sjlbkw.cn

C#:   3.14159.ToString("F2")
来源：http://kjo.fengsongda.top

[A22] 获取字符串长度
来源：http://fzs.cashguo.top

Py:   len(s)
来源：http://vbq.shangyingyoupin.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hte.vehdjk.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://izq.ydjk.org.cn

TS:   s.length
来源：http://ztz.zhijiandao.cn

Java: s.length()
来源：http://xin.andypj.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bkx.hywenlv.cn

Ruby: s.length
来源：http://ubl.cqqwz.cn

C#:   s.Length
来源：http://zwd.zdqjudy.top

[A23] 大小写转换
来源：http://kkw.daria6918.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lbi.fanxiaobao.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rmn.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bfn.andypj.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oqj.hfpthk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nfj.jianghu66.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kkr.aizwys.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xcx.zhongyouzk.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ttz.316326.xyz

[A24] 去除首尾空白
来源：http://udf.hammf.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sep.zycfv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zkt.fehbvm.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tbe.52xcode.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://awn.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tzo.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://arr.snrcjt.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jfg.316326.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qhh.havefunace.top

[A25] 字符串比较
来源：http://dno.zycfv.cn

Py:   s1 == s2; s1 != s2
来源：http://zha.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bgr.52xcode.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uez.hywenlv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fkd.svipenyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gnl.jianghu66.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://prl.svipenyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fxz.zhaomingkeji.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vxp.iojbl.cn

[A26] 类型转换总览
来源：http://tic.sxryk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hbe.316326.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://liw.xziqi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://emn.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://evm.jinghuilouyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uot.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://thx.xziqi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ewa.yuanzhike.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bgd.xinyue.icu

================================================================================
来源：http://fwv.gaohongyu789.top

B. 流程控制
来源：http://qpi.jqgfzy.top

================================================================================
来源：http://yjf.cashguo.top

[B01] 条件判断 if / else
来源：http://atl.fengsongda.top

Py:   result = "正" if x > 0 else "非正"
来源：http://civ.mhx1999.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ztb.gzhubu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eok.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vyx.zhongyouzk.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zbp.yj20258.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cab.xinyue.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://evv.yuanzhike.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kxq.zhengqikj.top

[B02] 多分支 else if / elif
来源：http://nix.xuetiantiany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zih.nanxuanxn.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ghu.tian-w.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://amj.jiagoushi.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wqf.gzhubu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vcz.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vxo.aibaodan.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oar.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gft.shangyingyoupin.top

[B03] switch / match / case
来源：http://iwb.dashuyun.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uyp.tianlin.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gmv.xuetiantiany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ztv.chenjidiqi.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ech.chenzaomai.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ysm.guowangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xio.chenjidiqi.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zdu.shanyushiyangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kip.xingfuxueyuan.xyz

[B04] for 计数循环
来源：http://nrb.meibo888.top

Py:   for i in range(10): print(i)
来源：http://heg.zycfv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qst.zhijiandao.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qle.cdnleiting.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hnv.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bwk.hysaishi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tfh.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://qjm.iojbl.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yjv.hnxiangtu.top

[B05] 遍历数组 / 列表
来源：http://nps.hcnkem.com

Py:   for item in arr: print(item)
来源：http://ghv.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qmj.guowangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rwa.yanxiufei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gad.ydjk.org.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mqk.jinyuanbaomall.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nio.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://qsr.zdbjq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qxk.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://zkt.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zzk.wangdashe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ril.shanyushiyangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lfi.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wda.gaohongyu789.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wta.sjlbkw.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nez.ivvv.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vhj.yuanzhike.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xnn.yongpay.top

[B07] while 循环
来源：http://eou.kuanghao11.cn

Py:   while i < 10: i += 1
来源：http://zvu.tarul.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fwa.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://gqp.zhoulong.xyz

TS:   while (i < 10) { i++; }
来源：http://lgz.wangdashe.top

Java: while (i < 10) { i++; }
来源：http://jdl.tarul.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vhj.nanxinkj.top

Ruby: while i < 10; i += 1; end
来源：http://aas.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://hkt.jinghuilouyu.cn

[B08] do-while（至少执行一次）
来源：http://jdn.yueranfly.top

Py:   # 无 do-while：用 while True + break
来源：http://tdm.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xtq.c1oappe.top

JS:   do { i++; } while (i < 10);
来源：http://lpu.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://lbz.aizwys.cn

Java: do { i++; } while (i < 10);
来源：http://yql.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://klt.cheryme.top

Ruby: begin; i += 1; end while i < 10
来源：http://gvf.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://imi.havefunace.top

[B09] break 与 continue
来源：http://hdd.chenjidiqi.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://enm.316326.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lnn.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vyh.yongpay.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rla.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ybr.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rdy.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fyn.snrcjt.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wtx.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://jxr.jianghu66.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dlh.shanyushiyangtech.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tvk.ywan-chungtsiang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://krn.shuidangran.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dbs.nanxuanxn.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bib.svipenyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qqz.yanxiufei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mie.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vcf.tianlin.xyz

[B11] 生成数字序列 / 区间
来源：http://chq.yanxiufei.cn

Py:   list(range(0, 10, 2))
来源：http://nsm.shanyushiyangkeji.top

PHP:  range(0, 10, 2);
来源：http://feo.hysaishi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://trq.jlsjyb.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dpa.jqgfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uhd.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nno.tarul.cn

Ruby: (0...10).step(2).to_a
来源：http://gyw.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ymh.guannengcc.top

[B12] 跳出多层循环
来源：http://vin.cqqwz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://soo.bbcook.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wpi.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vem.316326.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pcp.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gyd.xuetiantiany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pma.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://umy.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zbl.redwolf501.top

[B13] 判断是否为数字
来源：http://jxx.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://ijc.jyoumei.cn

PHP:  is_numeric($x)
来源：http://ipt.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qmi.shangyingyoupin.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nmu.sjlbkw.cn

Java: x instanceof Number
来源：http://jxn.yfazqb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kar.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://pve.yongpay.top

C#:   x is int or double or decimal
来源：http://mcf.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://cqy.jyoumei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ygk.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cot.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://kbb.vehdjk.com

TS:   [1, 2, 3].includes(x)
来源：http://vsu.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nnn.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fgg.epnwcf.com

Ruby: [1, 2, 3].include?(x)
来源：http://sew.meibo888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://szh.epnwcf.com

[B15] 布尔运算与取反
来源：http://era.uphjek.com

Py:   a and b or not c
来源：http://oon.yuxming.cn

PHP:  $a && $b || !$c
来源：http://qct.sjlbkw.cn

JS:   a && b || !c
来源：http://yqz.jqgfzy.top

TS:   a && b || !c
来源：http://vmq.nwbrower.top

Java: a && b || !c
来源：http://ncy.xinyue.icu

Go:   a && b || !c
来源：http://dbk.zhiwuduotai.top

Ruby: a && b || !c
来源：http://gin.yueranfly.top

C#:   a && b || !c
来源：http://xiy.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://trv.jlsjyb.cn

Py:   if not data: return
来源：http://owz.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://ndy.fehbvm.com

JS:   if (!data) return;
来源：http://eua.zhengqikj.top

TS:   if (!data) return;
来源：http://ged.cashguo.top

Java: if (data == null) return;
来源：http://ren.zhijiandao.cn

Go:   if data == nil { return }
来源：http://oms.yj202588.top

Ruby: return if data.nil?
来源：http://iwb.kuanghao11.cn

C#:   if (data == null) return;
来源：http://mby.jlsjyb.cn

================================================================================
来源：http://xzc.jiagoushi.top

C. 函数与作用域
来源：http://vii.yj20258.top

================================================================================
来源：http://gdh.ybcxt.top

[C01] 定义函数
来源：http://yex.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://dzo.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bkn.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://wdf.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hwz.bjfxy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vii.xinyue.icu

Go:   func add(a, b int) int { return a + b }
来源：http://urg.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://uwe.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dzo.xinyue.icu

[C02] 默认参数
来源：http://kso.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://jwp.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iby.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://cvv.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ack.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cug.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://exb.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://xgu.ydjk.org.cn


<!-- 参考信息 -->