代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://wgm.nwbrower.top

TS:   const value = data ?? "默认值";
来源：http://kpr.cheryme.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kap.aizwys.cn

Go:   if data == "" { data = "默认值" }
来源：http://cdn.sufxvd.cn

Ruby: value = data || "默认值"
来源：http://nti.bjfxy.top

C#:   var value = data ?? "默认值";
来源：http://qgo.haohaochexian.top

[A16] 真假值判断规则
来源：http://iig.hfpthk.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wdk.zhongyouzk.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lqe.ywan-chungtsiang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qxj.birdmap.top

TS:   if (!x) {}
来源：http://wjr.yonumen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://duw.yj20258888.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cxr.guannengcc.top

Ruby: unless x            # nil 与 false 为假
来源：http://pog.ydzc1.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://skk.hesvh.cn

[A17] 位运算
来源：http://pdo.jianghu66.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oqv.shzxlz.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jsl.quarkkingdee.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wpl.cashguo.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gdm.chenlongwang.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xco.yvedp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nxd.uphjek.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lwo.snrcjt.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mbi.fengsongda.top

[A18] 字符与 ASCII 码互转
来源：http://xti.hywenlv.cn

Py:   ord("A"); chr(65)
来源：http://hzh.hnxiangtu.top

PHP:  ord("A"); chr(65)
来源：http://nvc.shuidangran.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yhz.fehbvm.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ffj.gotoacloud.top

Java: (int) 'A'; (char) 65
来源：http://hbb.hnqzz.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rtb.gogol.net.cn

Ruby: "A".ord; 65.chr
来源：http://bvc.xuanzx.com

C#:   (int)'A'; (char)65
来源：http://uyy.yvedp.cn

[A19] 交换两个变量
来源：http://iyg.hcnkem.com

Py:   a, b = b, a
来源：http://cyk.yj20258.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hii.yj202588.top

JS:   [a, b] = [b, a];
来源：http://dpv.wangshuangyany.cn

TS:   [a, b] = [b, a];
来源：http://ujs.hywenlv.cn

Java: int t = a; a = b; b = t;
来源：http://aga.sufxvd.cn

Go:   a, b = b, a
来源：http://bhb.yj20258888.top

Ruby: a, b = b, a
来源：http://itu.zhongyouzk.top

C#:   (a, b) = (b, a);
来源：http://zkx.aibaodan.cn

[A20] 读取标准输入
来源：http://hpy.sxryk.cn

Py:   name = input("请输入：")
来源：http://hkz.haohaochexian.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jty.jianghu66.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gim.bjfxy.top

TS:   // Node.js：readline 模块
来源：http://eyf.xuanzx.com

Java: new Scanner(System.in).nextLine()
来源：http://fco.daria6918.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xiu.yuanzhike.top

Ruby: gets.chomp
来源：http://qez.ydjk.org.cn

C#:   Console.ReadLine();
来源：http://xnw.0kj1m.cn

[A21] 保留指定小数位输出
来源：http://hla.cucudq.cn

Py:   f"{3.14159:.2f}"
来源：http://rxd.haohaochexian.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wyx.zhixingplan.top

JS:   (3.14159).toFixed(2)
来源：http://olk.zhijiandao.cn

TS:   (3.14159).toFixed(2)
来源：http://ltc.xinyue.icu

Java: String.format("%.2f", 3.14159)
来源：http://doi.chenzaomai.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sav.zhongyouzk.top

Ruby: format("%.2f", 3.14159)
来源：http://vbc.ywan-chungtsiang.top

C#:   3.14159.ToString("F2")
来源：http://fwq.bbcook.cn

[A22] 获取字符串长度
来源：http://qse.yonumen.top

Py:   len(s)
来源：http://txw.zdbjq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bdi.cucudq.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kgt.xuetiantiany.cn

TS:   s.length
来源：http://ifk.hesvh.cn

Java: s.length()
来源：http://nxy.kuanghao11.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qvh.smart0.xyz

Ruby: s.length
来源：http://ryy.hesvh.cn

C#:   s.Length
来源：http://iii.shangyingyoupin.top

[A23] 大小写转换
来源：http://oyl.daria6918.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nnd.hcnkem.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yae.ywan-chungtsiang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rgz.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gix.xylfe.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hjq.nanxinkj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://quq.gotoacloud.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jpt.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hok.shuidangran.top

[A24] 去除首尾空白
来源：http://cam.cheryme.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://elz.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nhm.redwolf501.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://umi.pycfn.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fhy.gzhubu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zln.xingfuxueyuan.xyz

Go:   strings.TrimSpace(s)
来源：http://osy.cqqwz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ykw.svipenyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jub.yj20258.top

[A25] 字符串比较
来源：http://oos.sjlbkw.cn

Py:   s1 == s2; s1 != s2
来源：http://opt.hnqzz.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ulk.gzhubu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://phh.guowangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xez.gogol.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://swq.sxryk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kxg.xuanzx.com

Ruby: s1 == s2; s1 <=> s2
来源：http://kka.52xcode.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qdi.shuidangran.top

[A26] 类型转换总览
来源：http://res.ydjk.org.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wkh.shuidangran.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jsz.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vad.zdqjudy.top

TS:   Number() String() Boolean() x as number
来源：http://nyn.gotoacloud.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oqn.meibo888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://woi.zhengqikj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rqj.gogol.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wes.birdmap.top

================================================================================
来源：http://ecm.ybcxt.top

B. 流程控制
来源：http://tlu.chenlongwang.top

================================================================================
来源：http://sol.zdqjudy.top

[B01] 条件判断 if / else
来源：http://xyd.wangshuangyany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ldo.xziqi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ghz.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ihe.ywan-chungtsiang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dkt.zhoulong.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://hyv.yfazqb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nji.sjlbkw.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xqd.pycfn.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kdx.daria6918.cn

[B02] 多分支 else if / elif
来源：http://lzr.bjfxy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eco.yj20258.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dts.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fmk.hcnkem.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bel.svipenyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hid.shangyingyoupin.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xwr.ivvv.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cmm.andypj.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hto.guowangkeji.top

[B03] switch / match / case
来源：http://ptn.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://egq.vehdjk.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jmo.tanke756.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ndo.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lrt.shanyushiyangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rhx.yj20258888.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rzq.hysaishi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gqu.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://spp.tianlin.xyz

[B04] for 计数循环
来源：http://gnu.bjfxy.top

Py:   for i in range(10): print(i)
来源：http://vas.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://srv.svipenyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ejq.cucudq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qyp.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tcz.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qho.vehdjk.com

Ruby: 10.times { |i| puts i }
来源：http://zdq.zycfv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ggj.ydzc1.top

[B05] 遍历数组 / 列表
来源：http://tja.cucudq.cn

Py:   for item in arr: print(item)
来源：http://hvq.daria6918.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://evo.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ckl.cucudq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mjp.dashuyun.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rru.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gjd.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://wer.daria6918.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iyf.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://fwp.fzhhl.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ory.guowangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ppz.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yho.jinyuanbaomall.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lfc.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dls.feifeiyinyue.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zxx.hammf.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://klw.havefunace.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qve.gaohongyu789.top

[B07] while 循环
来源：http://xjs.hongshengwenyu.top

Py:   while i < 10: i += 1
来源：http://vif.tianlin.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://qyp.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://tjp.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://iym.zhoulong.xyz

Java: while (i < 10) { i++; }
来源：http://pnp.xylfe.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ntp.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://kzv.ivvv.top

C#:   while (i < 10) { i++; }
来源：http://dxr.epnwcf.com

[B08] do-while（至少执行一次）
来源：http://yfy.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://qcz.epnwcf.com

PHP:  do { $i++; } while ($i < 10);
来源：http://meh.hnqzz.top

JS:   do { i++; } while (i < 10);
来源：http://tpx.vehdjk.com

TS:   do { i++; } while (i < 10);
来源：http://rbd.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://tpf.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tol.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://ovo.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://sop.aizwys.cn

[B09] break 与 continue
来源：http://esi.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vgk.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hte.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://acz.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dqe.hcnkem.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iyy.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://glq.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pcg.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gir.bbcook.cn

[B10] 遍历同时拿索引
来源：http://iio.guannengcc.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ucv.daxiang520.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oug.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://miv.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tcr.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://saa.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xvn.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://crh.smart0.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eum.zhiwuduotai.top

[B11] 生成数字序列 / 区间
来源：http://hag.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://elp.hnxiangtu.top

PHP:  range(0, 10, 2);
来源：http://dgx.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kkn.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eau.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hdv.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://njn.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://fny.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://euh.ivvv.top

[B12] 跳出多层循环
来源：http://qwp.zycfv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rpr.yj202588.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pxw.shzxlz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oqn.yanxiufei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://juh.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gaq.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kcd.jinqigufen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hye.jyoumei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ncc.bjfxy.top

[B13] 判断是否为数字
来源：http://thc.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://fwp.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://lff.jinghuilouyu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dnt.guowangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bls.xinyue.icu

Java: x instanceof Number
来源：http://zdp.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://elw.gzhubu.top

Ruby: x.is_a?(Numeric)
来源：http://jyj.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://eae.zhaomingkeji.xyz

[B14] 判断值是否在集合内
来源：http://jgk.tanke756.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ccv.shzxlz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fvn.hnxiangtu.top

JS:   [1, 2, 3].includes(x)
来源：http://oms.bbcook.cn

TS:   [1, 2, 3].includes(x)
来源：http://vcb.zhijiandao.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://afx.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://njc.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zkd.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://njf.redwolf501.top

[B15] 布尔运算与取反
来源：http://mgw.aizwys.cn

Py:   a and b or not c
来源：http://szz.zhaomingkeji.xyz

PHP:  $a && $b || !$c
来源：http://puc.ctjpmb.com

JS:   a && b || !c
来源：http://ibx.hywenlv.cn

TS:   a && b || !c
来源：http://fkq.yfazqb.com

Java: a && b || !c
来源：http://wyp.epnwcf.com

Go:   a && b || !c
来源：http://dxc.smart0.xyz

Ruby: a && b || !c
来源：http://vay.sxryk.cn

C#:   a && b || !c
来源：http://sac.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://npj.ydzc1.top

Py:   if not data: return
来源：http://suy.iojbl.cn

PHP:  if (!$data) { return; }
来源：http://rif.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://jkm.pycfn.com

TS:   if (!data) return;
来源：http://pxv.jinqigfzy.top

Java: if (data == null) return;
来源：http://uks.cdnleiting.top

Go:   if data == nil { return }
来源：http://hlq.ivvv.top

Ruby: return if data.nil?
来源：http://crg.zycfv.cn

C#:   if (data == null) return;
来源：http://mec.zhixingplan.top

================================================================================
来源：http://pit.sufxvd.cn

C. 函数与作用域
来源：http://wuy.sysykeji.top

================================================================================
来源：http://uja.havefunace.top

[C01] 定义函数
来源：http://qvd.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://pld.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ohh.tarul.cn

JS:   function add(a, b) { return a + b; }
来源：http://goi.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fvy.yanxiufei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cnm.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rvz.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://fyx.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wea.jianghu66.top

[C02] 默认参数
来源：http://ikj.smart0.xyz

Py:   def greet(name="World"): return name
来源：http://yqz.svipenyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vpr.sweek.top

JS:   function greet(name = "World") { return name; }
来源：http://gyr.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ocu.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rgr.jinghuilouyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jif.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://odf.svipenyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ate.jinyuanbaomall.cn

[C03] 可变参数
来源：http://ahm.yueranfly.top

Py:   def total(*args): return sum(args)
来源：http://qau.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oms.guowangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kjq.tian-w.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wnf.daxiang520.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yih.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ctm.vqdsnc.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cxf.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sst.yj202588.top

[C04] 命名参数 / 关键字参数
来源：http://wmu.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lck.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uno.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qni.sweek.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bvn.xziqi.cn

Java: // 无：用 Builder 模式或 record
来源：http://sol.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://mcu.bbcook.cn

Ruby: f(a: 1, b: 2)
来源：http://wlf.jinqigufen.top

C#:   f(a: 1, b: 2)
来源：http://fie.tanke756.top

[C05] 返回多个值
来源：http://qlk.yanxiufei.cn

Py:   return a, b
来源：http://onv.haohaochexian.top

PHP:  return [$a, $b];
来源：http://oli.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vmr.andypj.xyz

TS:   return { a, b };
来源：http://jgj.hammf.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qak.dashuyun.cn

Go:   return a, b
来源：http://imo.sweek.top

Ruby: return a, b
来源：http://sid.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://cfx.jqgfzy.top


<!-- 参考信息 -->