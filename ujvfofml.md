代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jai.ehwqpu.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nuh.jianghu66.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://inm.xinyue.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hae.yanxiufei.cn

[A18] 字符与 ASCII 码互转
来源：http://aot.sweek.top

Py:   ord("A"); chr(65)
来源：http://xyv.sweek.top

PHP:  ord("A"); chr(65)
来源：http://jea.tian-w.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://smz.xylfe.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cmw.yueranfly.top

Java: (int) 'A'; (char) 65
来源：http://zxb.nanxuanxn.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nep.kuanghao11.cn

Ruby: "A".ord; 65.chr
来源：http://zif.yuanzhike.top

C#:   (int)'A'; (char)65
来源：http://vfx.yvedp.cn

[A19] 交换两个变量
来源：http://pok.gzhubu.top

Py:   a, b = b, a
来源：http://ftv.hfpthk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://htz.zhengqikj.top

JS:   [a, b] = [b, a];
来源：http://znn.shzxlz.cn

TS:   [a, b] = [b, a];
来源：http://erz.fktsv.cn

Java: int t = a; a = b; b = t;
来源：http://ceo.zhixingplan.top

Go:   a, b = b, a
来源：http://jqs.vqdsnc.cn

Ruby: a, b = b, a
来源：http://chg.hongshengwenyu.top

C#:   (a, b) = (b, a);
来源：http://bev.nanxuanxn.top

[A20] 读取标准输入
来源：http://szj.wangshuangyany.cn

Py:   name = input("请输入：")
来源：http://upq.ehwqpu.com

PHP:  $name = trim(fgets(STDIN));
来源：http://svz.hesvh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wit.yonumen.top

TS:   // Node.js：readline 模块
来源：http://ydu.redwolf501.top

Java: new Scanner(System.in).nextLine()
来源：http://auy.hesvh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cmn.zhongyouzk.top

Ruby: gets.chomp
来源：http://gls.shzxlz.cn

C#:   Console.ReadLine();
来源：http://ssn.ctjpmb.com

[A21] 保留指定小数位输出
来源：http://kaq.zdbjq.cn

Py:   f"{3.14159:.2f}"
来源：http://qlj.aibaodan.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cmr.jiagoushi.top

JS:   (3.14159).toFixed(2)
来源：http://jqa.tanke756.top

TS:   (3.14159).toFixed(2)
来源：http://uum.haohaochexian.top

Java: String.format("%.2f", 3.14159)
来源：http://yls.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ioj.jqgfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://vuc.zdbjq.cn

C#:   3.14159.ToString("F2")
来源：http://zdw.jqgfzy.top

[A22] 获取字符串长度
来源：http://hzi.fktsv.cn

Py:   len(s)
来源：http://rye.cheryme.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ygi.xuetiantiany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lkf.wangdashe.top

TS:   s.length
来源：http://jjj.birdmap.top

Java: s.length()
来源：http://ouz.xinyue.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xcu.gogol.net.cn

Ruby: s.length
来源：http://avk.hnqzz.top

C#:   s.Length
来源：http://ilk.c1oappe.top

[A23] 大小写转换
来源：http://laq.guannengcc.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zgc.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ixi.52xcode.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gec.0kj1m.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ori.wangdashe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ezb.nanxuanxn.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dsa.nwbrower.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sga.ywan-chungtsiang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rhm.yangfankeji.com

[A24] 去除首尾空白
来源：http://aqn.hcnkem.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ctg.fktsv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vgq.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://adq.316326.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rgq.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cbl.pengpengdd.cyou

Go:   strings.TrimSpace(s)
来源：http://xow.c1oappe.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://apf.guowangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qfb.guannengcc.top

[A25] 字符串比较
来源：http://ipx.ywan-chungtsiang.top

Py:   s1 == s2; s1 != s2
来源：http://uiw.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rzf.yvedp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bpn.vqdsnc.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mju.daxiang520.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pre.yfazqb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ytc.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ago.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://atq.ehwqpu.com

[A26] 类型转换总览
来源：http://xoz.shanyushiyangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zlw.birdmap.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uap.cucudq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://srp.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://rjt.tarul.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qcn.jyoumei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hah.gaohongyu789.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mzp.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kcc.jinqigfzy.top

================================================================================
来源：http://hui.yuxming.cn

B. 流程控制
来源：http://ark.yvedp.cn

================================================================================
来源：http://kvv.gotoacloud.top

[B01] 条件判断 if / else
来源：http://kkg.nwbrower.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ift.yfazqb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://des.zhengqikj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://har.cucudq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dxi.yongpay.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tsx.jqgfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sqj.svipenyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vmv.sxryk.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yot.tian-w.cn

[B02] 多分支 else if / elif
来源：http://nkr.0kj1m.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lao.tarul.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://czf.chenlongwang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://unk.0kj1m.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xid.jqgfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vpt.hywenlv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vrc.zhaomingkeji.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tcw.zdqjudy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xhl.yanxiufei.cn

[B03] switch / match / case
来源：http://knl.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vrc.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xfq.yfazqb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zzw.yueranfly.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jqq.yangfankeji.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gbp.yanxiufei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bjb.zhengqikj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jpb.chenzaomai.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://smj.jinqigfzy.top

[B04] for 计数循环
来源：http://tps.smart0.xyz

Py:   for i in range(10): print(i)
来源：http://lak.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fhp.xuetiantiany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zil.ydzc1.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wji.gotoacloud.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wya.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wct.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://ijr.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://swr.jinqigufen.top

[B05] 遍历数组 / 列表
来源：http://iay.yonumen.top

Py:   for item in arr: print(item)
来源：http://wkt.9152youxi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iwb.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wtn.vehdjk.com

TS:   for (const item of arr) { console.log(item); }
来源：http://vtr.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vqa.ybcxt.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://env.uphjek.com

Ruby: arr.each { |item| puts item }
来源：http://yqz.ydzc1.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cvm.fengsongda.top

[B06] 遍历字典 / 对象
来源：http://kgu.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rut.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jeu.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lhf.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dny.sxryk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wdf.jinqigfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fbx.feifeiyinyue.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xet.daxiang520.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zvs.xuetiantiany.cn

[B07] while 循环
来源：http://npu.yonumen.top

Py:   while i < 10: i += 1
来源：http://lyd.9152youxi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://chz.jqgfzy.top

JS:   while (i < 10) { i++; }
来源：http://lxe.9152youxi.cn

TS:   while (i < 10) { i++; }
来源：http://osx.fktsv.cn

Java: while (i < 10) { i++; }
来源：http://unw.sysykeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dty.zhiwuduotai.top

Ruby: while i < 10; i += 1; end
来源：http://kzn.hfpthk.cn

C#:   while (i < 10) { i++; }
来源：http://wjz.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://bhg.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://moj.fengsongda.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yam.yj20258.top

JS:   do { i++; } while (i < 10);
来源：http://zqa.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://ddl.vehdjk.com

Java: do { i++; } while (i < 10);
来源：http://czx.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zsz.sweek.top

Ruby: begin; i += 1; end while i < 10
来源：http://gcf.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://ssq.gaohongyu789.top

[B09] break 与 continue
来源：http://qxu.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://crj.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gsd.aizwys.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dai.shuidangran.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fjs.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dks.xziqi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yun.tarul.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://apo.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tkq.ydzc1.top

[B10] 遍历同时拿索引
来源：http://hhs.yj202588.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ozd.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lzr.daxiang520.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xzm.zhiwuduotai.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ilz.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aju.yj20258888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ecx.zdbjq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pbv.jinqigufen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xsr.fanxiaobao.xyz

[B11] 生成数字序列 / 区间
来源：http://zwk.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://rop.zhixingplan.top

PHP:  range(0, 10, 2);
来源：http://oqo.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pzc.ywan-chungtsiang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ame.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kvm.snrcjt.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://enm.shangyingyoupin.top

Ruby: (0...10).step(2).to_a
来源：http://vbe.xingfuxueyuan.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fpy.yj202588.top

[B12] 跳出多层循环
来源：http://rul.hfpthk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tpc.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://kfx.feifeiyinyue.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tlt.iojbl.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lgr.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qpp.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zdz.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://obi.zycfv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bxb.yuanzhike.top

[B13] 判断是否为数字
来源：http://zbl.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://hdu.hcnkem.com

PHP:  is_numeric($x)
来源：http://wtw.havefunace.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ery.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zhq.xuetiantiany.cn

Java: x instanceof Number
来源：http://joo.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vju.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://atj.ctjpmb.com

C#:   x is int or double or decimal
来源：http://faz.iojbl.cn

[B14] 判断值是否在集合内
来源：http://noi.cashguo.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vaw.yj20258888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xtu.jinqigufen.top

JS:   [1, 2, 3].includes(x)
来源：http://tgq.gaohongyu789.top

TS:   [1, 2, 3].includes(x)
来源：http://fif.andypj.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://ooh.jqgfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fjt.kuanghao11.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dsi.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wic.dashuyun.cn

[B15] 布尔运算与取反
来源：http://dcj.aizwys.cn

Py:   a and b or not c
来源：http://kni.hammf.cn

PHP:  $a && $b || !$c
来源：http://uvz.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://ryu.tanke756.top

TS:   a && b || !c
来源：http://jlg.chenlongwang.top

Java: a && b || !c
来源：http://eem.yj20258.top

Go:   a && b || !c
来源：http://zuo.hammf.cn

Ruby: a && b || !c
来源：http://smz.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://gjy.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://zll.dianchejie.cn

Py:   if not data: return
来源：http://geh.yj20258.top

PHP:  if (!$data) { return; }
来源：http://dns.yanxiufei.cn

JS:   if (!data) return;
来源：http://ten.sysykeji.top

TS:   if (!data) return;
来源：http://hke.gotoacloud.top

Java: if (data == null) return;
来源：http://rcp.zhixingplan.top

Go:   if data == nil { return }
来源：http://hjd.daria6918.cn

Ruby: return if data.nil?
来源：http://lds.zhoulong.xyz

C#:   if (data == null) return;
来源：http://odo.0kj1m.cn

================================================================================
来源：http://ois.chenlongwang.top

C. 函数与作用域
来源：http://mgt.daxiang520.top

================================================================================
来源：http://xeh.nwbrower.top

[C01] 定义函数
来源：http://lky.havefunace.top

Py:   def add(a, b): return a + b
来源：http://mzk.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gob.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://myr.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zff.ppjwa.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://poh.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://jyq.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://saf.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gph.316326.xyz

[C02] 默认参数
来源：http://vha.yonumen.top

Py:   def greet(name="World"): return name
来源：http://syd.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://byy.zhoulong.xyz

JS:   function greet(name = "World") { return name; }
来源：http://cxl.tarul.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hjl.daria6918.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rdt.yonumen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aop.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://gvi.guannengcc.top

C#:   string Greet(string name = "World") => name;
来源：http://cks.zhijiandao.cn

[C03] 可变参数
来源：http://vcw.hfpthk.cn

Py:   def total(*args): return sum(args)
来源：http://jio.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bxi.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tud.zhijiandao.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yxg.tarul.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kdo.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ubl.52xcode.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cfc.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xuj.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://ddy.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vxo.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lcx.0kj1m.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wle.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ydd.yangfankeji.com

Java: // 无：用 Builder 模式或 record
来源：http://dpt.xylfe.cn

Go:   // 无：用配置结构体参数
来源：http://iik.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://qpi.jinqigufen.top

C#:   f(a: 1, b: 2)
来源：http://wfz.yj20258.top

[C05] 返回多个值
来源：http://cgk.shuidangran.top

Py:   return a, b
来源：http://hrk.svipenyu.cn

PHP:  return [$a, $b];
来源：http://elo.andypj.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://nrv.guannengcc.top

TS:   return { a, b };
来源：http://vqy.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yzv.52xcode.cn

Go:   return a, b
来源：http://bmy.9152youxi.cn

Ruby: return a, b
来源：http://dxw.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://uxf.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://hqs.fehbvm.com

Py:   square = lambda x: x * x
来源：http://wfk.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kjt.sweek.top

JS:   const square = x => x * x;
来源：http://hop.zhaomingkeji.xyz

TS:   const square = (x: number): number => x * x;
来源：http://vzp.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://goa.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cea.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://ovs.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://rig.aibaodan.cn

[C07] 把函数作为参数传入
来源：http://nsx.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lei.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://aqy.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vzk.chenlongwang.top

TS:   arr.map(String)
来源：http://mmd.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jud.xingfuxueyuan.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dyw.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://wwi.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ixn.sweek.top

[C08] 闭包
来源：http://xmx.daxiang520.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kbk.vehdjk.com


<!-- 参考信息 -->