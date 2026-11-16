代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://quq.fehbvm.com

[A11] 条件表达式（三元）
来源：http://kmn.yj20258888.top

Py:   "yes" if x > 0 else "no"
来源：http://cfh.fanxiaobao.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://ttw.ydzc1.top

JS:   x > 0 ? "yes" : "no"
来源：http://din.yfazqb.com

TS:   x > 0 ? "yes" : "no"
来源：http://zhv.xuanzx.com

Java: x > 0 ? "yes" : "no"
来源：http://byq.quarkkingdee.top

Go:   // 无三元运算符，需用 if 语句
来源：http://nqs.ywan-chungtsiang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://pmb.shangyingyoupin.top

C#:   x > 0 ? "yes" : "no"
来源：http://ywr.sjlbkw.cn

[A12] 字符串插值 / 格式化
来源：http://wcm.feifeiyinyue.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cgo.epnwcf.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kle.jianghu66.top

JS:   `Hello, ${name}!`
来源：http://ngf.zycfv.cn

TS:   `Hello, ${name}!`
来源：http://nuh.shuidangran.top

Java: "Hello, %s!".formatted(name)
来源：http://ilv.316326.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jgl.guannengcc.top

Ruby: "Hello, #{name}!"
来源：http://ydu.redwolf501.top

C#:   $"Hello, {name}!"
来源：http://qql.cashguo.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gel.hnxiangtu.top

Py:   "第一行\n第二行"
来源：http://eia.sysykeji.top

PHP:  "第一行\n第二行"
来源：http://hkc.jinyuanbaomall.cn

JS:   "第一行\n第二行"
来源：http://rpn.haohaochexian.top

TS:   "第一行\n第二行"
来源：http://ndp.chenlongwang.top

Java: "第一行\n第二行"
来源：http://zpu.yuanzhike.top

Go:   "第一行\n第二行"
来源：http://ccu.sweek.top

Ruby: "第一行\n第二行"
来源：http://wzo.dianchejie.cn

C#:   "第一行\n第二行"
来源：http://igu.nwbrower.top

[A14] 注释写法
来源：http://eri.ydjk.org.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://byt.xziqi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pcd.wangshuangyany.cn

JS:   // 单行；/* 多行 */
来源：http://fzw.jianghu66.top

TS:   // 单行；/* 多行 */
来源：http://ryu.chenzaomai.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vwz.cqqwz.cn

Go:   // 单行；/* 多行 */
来源：http://iti.316326.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://scr.fengsongda.top

C#:   // 单行；/* 多行 */
来源：http://hff.ppjwa.cn

[A15] 空值判断与默认值
来源：http://yqw.yueranfly.top

Py:   value = data or "默认值"
来源：http://ztg.tanke756.top

PHP:  $value = $data ?? "默认值";
来源：http://hri.hongshengwenyu.top

JS:   const value = data ?? "默认值";
来源：http://tbi.sxryk.cn

TS:   const value = data ?? "默认值";
来源：http://xxg.iojbl.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://arq.yueranfly.top

Go:   if data == "" { data = "默认值" }
来源：http://kmf.yangfankeji.com

Ruby: value = data || "默认值"
来源：http://ifk.daxiang520.top

C#:   var value = data ?? "默认值";
来源：http://vzu.shuidangran.top

[A16] 真假值判断规则
来源：http://kxs.hammf.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lhn.xziqi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://krt.ywan-chungtsiang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sit.yvedp.cn

TS:   if (!x) {}
来源：http://pqz.quarkkingdee.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lfo.jinghuilouyu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xhf.guowangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://uub.yj20258.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uhi.xinyue.icu

[A17] 位运算
来源：http://hed.pengpengdd.cyou

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cep.hnxiangtu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://caa.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gsz.chenzaomai.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pys.aibaodan.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://imd.hammf.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rlm.fktsv.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://exi.daria6918.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mnd.smart0.xyz

[A18] 字符与 ASCII 码互转
来源：http://kve.cqqwz.cn

Py:   ord("A"); chr(65)
来源：http://mmj.pycfn.com

PHP:  ord("A"); chr(65)
来源：http://owm.sufxvd.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jzp.tianlin.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fzv.ydzc1.top

Java: (int) 'A'; (char) 65
来源：http://qry.bjfxy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rwq.iojbl.cn

Ruby: "A".ord; 65.chr
来源：http://our.shanyushiyangkeji.top

C#:   (int)'A'; (char)65
来源：http://lie.jinqigfzy.top

[A19] 交换两个变量
来源：http://obf.jyoumei.cn

Py:   a, b = b, a
来源：http://htr.cashguo.top

PHP:  [$a, $b] = [$b, $a];
来源：http://unp.chenlongwang.top

JS:   [a, b] = [b, a];
来源：http://gru.yongpay.top

TS:   [a, b] = [b, a];
来源：http://ytj.c1oappe.top

Java: int t = a; a = b; b = t;
来源：http://aiu.xingfuxueyuan.xyz

Go:   a, b = b, a
来源：http://poe.hesvh.cn

Ruby: a, b = b, a
来源：http://chc.yj20258.top

C#:   (a, b) = (b, a);
来源：http://mtr.guowangkeji.top

[A20] 读取标准输入
来源：http://gfq.hnxiangtu.top

Py:   name = input("请输入：")
来源：http://sub.jinqigufen.top

PHP:  $name = trim(fgets(STDIN));
来源：http://omj.xziqi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://igq.52xcode.cn

TS:   // Node.js：readline 模块
来源：http://rdf.fanxiaobao.xyz

Java: new Scanner(System.in).nextLine()
来源：http://qik.dianchejie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kxe.xuanzx.com

Ruby: gets.chomp
来源：http://ydg.mhx1999.top

C#:   Console.ReadLine();
来源：http://ybd.zhaomingkeji.xyz

[A21] 保留指定小数位输出
来源：http://lze.meibo888.top

Py:   f"{3.14159:.2f}"
来源：http://upa.meibo888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tgn.jlsjyb.cn

JS:   (3.14159).toFixed(2)
来源：http://nsn.hongshengwenyu.top

TS:   (3.14159).toFixed(2)
来源：http://hmx.nwbrower.top

Java: String.format("%.2f", 3.14159)
来源：http://mro.hnxiangtu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://njv.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://cmi.haohaochexian.top

C#:   3.14159.ToString("F2")
来源：http://cdf.hammf.cn

[A22] 获取字符串长度
来源：http://ler.birdmap.top

Py:   len(s)
来源：http://ipo.tanke756.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://act.yj202588.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eny.zhengqikj.top

TS:   s.length
来源：http://fxh.bjfxy.top

Java: s.length()
来源：http://dsu.sufxvd.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ers.guannengcc.top

Ruby: s.length
来源：http://yro.yvedp.cn

C#:   s.Length
来源：http://gas.ydjk.org.cn

[A23] 大小写转换
来源：http://lyu.yueranfly.top

Py:   s.upper(); s.lower(); s.title()
来源：http://egc.uphjek.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://boy.hysaishi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cqu.cqqwz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ntz.yuxming.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mns.ppjwa.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://exg.ybcxt.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zcg.chenzaomai.com

C#:   s.ToUpper(); s.ToLower()
来源：http://dze.hfpthk.cn

[A24] 去除首尾空白
来源：http://xnz.aibaodan.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rna.xingfuxueyuan.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wkn.jinyuanbaomall.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://whs.xziqi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yyd.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zwi.yj20258888.top

Go:   strings.TrimSpace(s)
来源：http://rfx.gaohongyu789.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://twl.yonumen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cld.yonumen.top

[A25] 字符串比较
来源：http://gvg.0kj1m.cn

Py:   s1 == s2; s1 != s2
来源：http://fna.nanxuanxn.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://agc.zhiwuduotai.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://icf.yj202588.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cni.fanxiaobao.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wgy.chenzaomai.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fqp.kuanghao11.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oyh.andypj.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eex.andypj.xyz

[A26] 类型转换总览
来源：http://yyj.kuanghao11.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hrp.hesvh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vec.tarul.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vrl.ehwqpu.com

TS:   Number() String() Boolean() x as number
来源：http://tsn.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wgf.aibaodan.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://srf.bbcook.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sbk.ppjwa.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ovy.gotoacloud.top

================================================================================
来源：http://bmn.cheryme.top

B. 流程控制
来源：http://xqc.jianghu66.top

================================================================================
来源：http://jid.yueranfly.top

[B01] 条件判断 if / else
来源：http://xed.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bjk.havefunace.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wua.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nbl.yuanzhike.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rus.cashguo.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zmk.iojbl.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ulh.zdqjudy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://efp.fktsv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://krf.ydjk.org.cn

[B02] 多分支 else if / elif
来源：http://nev.9152youxi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vfd.jqgfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rdq.aibaodan.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zwp.bbcook.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iqe.zhaomingkeji.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://agy.uphjek.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yqg.bjfxy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nys.tian-w.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://emy.hywenlv.cn

[B03] switch / match / case
来源：http://lot.zhongyouzk.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://swn.shuidangran.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xbg.sjlbkw.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vom.snrcjt.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vcm.gaohongyu789.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ato.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wal.meibo888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://crr.zycfv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://djy.sxryk.cn

[B04] for 计数循环
来源：http://nlq.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://hvh.jinqigfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gyn.hfpthk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dbx.sweek.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qbi.hesvh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iao.tanke756.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qfn.gotoacloud.top

Ruby: 10.times { |i| puts i }
来源：http://ham.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zdu.gaohongyu789.top

[B05] 遍历数组 / 列表
来源：http://ubq.redwolf501.top

Py:   for item in arr: print(item)
来源：http://frb.sweek.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ngf.zdbjq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://frm.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://ruy.ivvv.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ybx.nwbrower.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://prm.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://tvz.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ggg.tarul.cn

[B06] 遍历字典 / 对象
来源：http://rkx.ivvv.top

Py:   for k, v in d.items(): print(k, v)
来源：http://niu.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tfy.yonumen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eif.hnqzz.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wgw.cdnleiting.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vep.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wal.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://toj.jqgfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vrz.tarul.cn

[B07] while 循环
来源：http://obe.fengsongda.top

Py:   while i < 10: i += 1
来源：http://imt.sxryk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qgy.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://njl.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://pqx.zhoulong.xyz

Java: while (i < 10) { i++; }
来源：http://ins.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ogg.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://rhc.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://jnj.hesvh.cn

[B08] do-while（至少执行一次）
来源：http://enx.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://lyz.hammf.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lna.chenlongwang.top

JS:   do { i++; } while (i < 10);
来源：http://fca.gaohongyu789.top

TS:   do { i++; } while (i < 10);
来源：http://ipm.xinyue.icu

Java: do { i++; } while (i < 10);
来源：http://wye.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mst.fehbvm.com

Ruby: begin; i += 1; end while i < 10
来源：http://axf.jqgfzy.top

C#:   do { i++; } while (i < 10);
来源：http://nvd.yj20258.top

[B09] break 与 continue
来源：http://fxe.shuidangran.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lcs.hcnkem.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jqv.sjlbkw.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ktw.jlsjyb.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gpm.hcnkem.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zfi.yfazqb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wms.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zff.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ldu.wangdashe.top

[B10] 遍历同时拿索引
来源：http://mpl.sufxvd.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lmm.chenlongwang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xfb.guannengcc.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iuo.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bnh.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xml.vqdsnc.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rfb.yuanzhike.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ipb.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rca.yueranfly.top

[B11] 生成数字序列 / 区间
来源：http://ith.gotoacloud.top

Py:   list(range(0, 10, 2))
来源：http://aoh.zhixingplan.top

PHP:  range(0, 10, 2);
来源：http://frt.shanyushiyangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gnj.hongshengwenyu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://djc.guannengcc.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ztj.guannengcc.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zdf.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://pdn.chenjidiqi.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bsv.52xcode.cn

[B12] 跳出多层循环
来源：http://fnz.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qqz.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://jeq.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ojs.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vns.yj20258888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ccm.hfpthk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oaa.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tpw.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wmr.ivvv.top

[B13] 判断是否为数字
来源：http://hxt.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://eor.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://lhu.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dgo.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vqm.yueranfly.top

Java: x instanceof Number
来源：http://ozj.tarul.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://obl.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://diy.sjlbkw.cn

C#:   x is int or double or decimal
来源：http://ywm.vqdsnc.cn

[B14] 判断值是否在集合内
来源：http://rxh.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ltq.316326.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://guo.yj20258.top

JS:   [1, 2, 3].includes(x)
来源：http://kvo.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://azu.smart0.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://mrd.chenzaomai.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://klk.yj20258.top

Ruby: [1, 2, 3].include?(x)
来源：http://pbe.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ndi.hesvh.cn

[B15] 布尔运算与取反
来源：http://jbn.andypj.xyz

Py:   a and b or not c
来源：http://iuq.vehdjk.com

PHP:  $a && $b || !$c
来源：http://mqr.hongshengwenyu.top

JS:   a && b || !c
来源：http://ezy.havefunace.top

TS:   a && b || !c
来源：http://lbg.yuanzhike.top

Java: a && b || !c
来源：http://cwo.tianlin.xyz

Go:   a && b || !c
来源：http://zkf.gaohongyu789.top

Ruby: a && b || !c
来源：http://fcl.zycfv.cn

C#:   a && b || !c
来源：http://plu.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://iiv.jinghuilouyu.cn

Py:   if not data: return
来源：http://tws.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://igw.sweek.top

JS:   if (!data) return;
来源：http://mlg.yanxiufei.cn

TS:   if (!data) return;
来源：http://zbv.zhixingplan.top

Java: if (data == null) return;
来源：http://eop.aibaodan.cn

Go:   if data == nil { return }
来源：http://uqd.hcnkem.com

Ruby: return if data.nil?
来源：http://tsd.yfazqb.com

C#:   if (data == null) return;
来源：http://pbk.zdqjudy.top

================================================================================
来源：http://aqn.guowangkeji.top

C. 函数与作用域
来源：http://tet.xziqi.cn

================================================================================
来源：http://wye.sweek.top

[C01] 定义函数
来源：http://wvy.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://nta.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wzd.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://zak.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tjt.pycfn.com


<!-- 参考信息 -->