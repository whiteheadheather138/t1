代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://uvp.hfpthk.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qrk.ppjwa.cn

Go:   // 单行；/* 多行 */
来源：http://baf.yj202588.top

Ruby: # 单行；=begin 多行 =end
来源：http://pps.bbcook.cn

C#:   // 单行；/* 多行 */
来源：http://hgt.nanxuanxn.top

[A15] 空值判断与默认值
来源：http://whx.hnxiangtu.top

Py:   value = data or "默认值"
来源：http://ckb.fanxiaobao.xyz

PHP:  $value = $data ?? "默认值";
来源：http://cjv.fehbvm.com

JS:   const value = data ?? "默认值";
来源：http://xui.wangshuangyany.cn

TS:   const value = data ?? "默认值";
来源：http://lpl.jinqigfzy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lhl.zhijiandao.cn

Go:   if data == "" { data = "默认值" }
来源：http://duf.hammf.cn

Ruby: value = data || "默认值"
来源：http://qsi.yangfankeji.com

C#:   var value = data ?? "默认值";
来源：http://squ.iojbl.cn

[A16] 真假值判断规则
来源：http://zng.sufxvd.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vmk.fanxiaobao.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mzh.hcnkem.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ljs.hongshengwenyu.top

TS:   if (!x) {}
来源：http://xnd.zdbjq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://odx.sweek.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gzo.jiagoushi.top

Ruby: unless x            # nil 与 false 为假
来源：http://ydc.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jol.jinqigfzy.top

[A17] 位运算
来源：http://flb.shangyingyoupin.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sji.dashuyun.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rwr.zhoulong.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xav.smart0.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nax.epnwcf.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ldf.sufxvd.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oat.sysykeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cfl.wangshuangyany.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://umv.yanxiufei.cn

[A18] 字符与 ASCII 码互转
来源：http://qyf.bbcook.cn

Py:   ord("A"); chr(65)
来源：http://jjh.daxiang520.top

PHP:  ord("A"); chr(65)
来源：http://kgb.xylfe.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hms.guannengcc.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lvw.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://ejc.sjlbkw.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yhk.shangyingyoupin.top

Ruby: "A".ord; 65.chr
来源：http://ndl.zdbjq.cn

C#:   (int)'A'; (char)65
来源：http://inc.fanxiaobao.xyz

[A19] 交换两个变量
来源：http://vja.jinqigfzy.top

Py:   a, b = b, a
来源：http://qvv.jqgfzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://zwl.vehdjk.com

JS:   [a, b] = [b, a];
来源：http://kbq.yongpay.top

TS:   [a, b] = [b, a];
来源：http://xau.hcnkem.com

Java: int t = a; a = b; b = t;
来源：http://arf.dashuyun.cn

Go:   a, b = b, a
来源：http://vuu.dashuyun.cn

Ruby: a, b = b, a
来源：http://tww.shzxlz.cn

C#:   (a, b) = (b, a);
来源：http://nks.daria6918.cn

[A20] 读取标准输入
来源：http://mww.shanyushiyangtech.top

Py:   name = input("请输入：")
来源：http://xuj.ydzc1.top

PHP:  $name = trim(fgets(STDIN));
来源：http://lsc.kuanghao11.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pvz.jlsjyb.cn

TS:   // Node.js：readline 模块
来源：http://buj.uphjek.com

Java: new Scanner(System.in).nextLine()
来源：http://wtj.fanxiaobao.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cfn.fengsongda.top

Ruby: gets.chomp
来源：http://lbd.sjlbkw.cn

C#:   Console.ReadLine();
来源：http://dzz.cdnleiting.top

[A21] 保留指定小数位输出
来源：http://tri.haohaochexian.top

Py:   f"{3.14159:.2f}"
来源：http://pbr.gaohongyu789.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dca.jinghuilouyu.cn

JS:   (3.14159).toFixed(2)
来源：http://cat.dashuyun.cn

TS:   (3.14159).toFixed(2)
来源：http://dkj.tarul.cn

Java: String.format("%.2f", 3.14159)
来源：http://flx.tian-w.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tou.wangdashe.top

Ruby: format("%.2f", 3.14159)
来源：http://avj.yuanzhike.top

C#:   3.14159.ToString("F2")
来源：http://pyp.fengsongda.top

[A22] 获取字符串长度
来源：http://jkj.hammf.cn

Py:   len(s)
来源：http://uvx.zhongyouzk.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vdb.jinyuanbaomall.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tef.sweek.top

TS:   s.length
来源：http://kjs.xziqi.cn

Java: s.length()
来源：http://kow.zhaomingkeji.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cym.guowangkeji.top

Ruby: s.length
来源：http://xxa.yonumen.top

C#:   s.Length
来源：http://don.xingfuxueyuan.xyz

[A23] 大小写转换
来源：http://pah.jinyuanbaomall.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qbz.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sdf.yanxiufei.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://egd.cqqwz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hug.gotoacloud.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://viu.zhiwuduotai.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oik.ppjwa.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://acg.jqgfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mol.jqgfzy.top

[A24] 去除首尾空白
来源：http://mpb.52xcode.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xcj.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://guj.dianchejie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://opt.chenzaomai.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aqa.fktsv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://een.dashuyun.cn

Go:   strings.TrimSpace(s)
来源：http://mxw.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fof.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yqp.birdmap.top

[A25] 字符串比较
来源：http://tqj.9152youxi.cn

Py:   s1 == s2; s1 != s2
来源：http://trv.nanxuanxn.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qcl.tian-w.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oek.shzxlz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aow.svipenyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tpz.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qjw.daxiang520.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jhw.sufxvd.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://npp.zhoulong.xyz

[A26] 类型转换总览
来源：http://lib.gogol.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uri.andypj.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fmr.gogol.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ksb.sxryk.cn

TS:   Number() String() Boolean() x as number
来源：http://fpf.sweek.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jkq.jianghu66.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pxv.hfpthk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hgs.ctjpmb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://unf.chenzaomai.com

================================================================================
来源：http://fjx.cheryme.top

B. 流程控制
来源：http://hwc.zhengqikj.top

================================================================================
来源：http://ofn.wangdashe.top

[B01] 条件判断 if / else
来源：http://ete.0kj1m.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fet.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jyq.hcnkem.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wwn.zhaomingkeji.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dvr.cashguo.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://afp.meibo888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vlj.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vmm.9152youxi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xfa.jinqigufen.top

[B02] 多分支 else if / elif
来源：http://cgh.zhoulong.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lvl.jinghuilouyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rdg.havefunace.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gtu.yj20258.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://igb.sjlbkw.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fqa.aibaodan.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fja.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zty.cdnleiting.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nwi.yj20258888.top

[B03] switch / match / case
来源：http://uie.mhx1999.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qkv.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ykx.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ene.ydzc1.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://akj.hnxiangtu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dyg.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ync.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cii.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pla.xuanzx.com

[B04] for 计数循环
来源：http://ykr.yvedp.cn

Py:   for i in range(10): print(i)
来源：http://ujh.dianchejie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://obz.zhengqikj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://olz.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uwh.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bhn.fehbvm.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://djw.0kj1m.cn

Ruby: 10.times { |i| puts i }
来源：http://pzl.gzhubu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pqv.316326.xyz

[B05] 遍历数组 / 列表
来源：http://uyi.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://lqf.tianlin.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yvi.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cpe.shuidangran.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gll.hongshengwenyu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rtb.shangyingyoupin.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aoi.nwbrower.top

Ruby: arr.each { |item| puts item }
来源：http://nsi.hnxiangtu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gwf.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://ddz.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://lcg.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gyv.yuanzhike.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vmc.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dym.epnwcf.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ulo.yueranfly.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://luh.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yaf.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ock.bbcook.cn

[B07] while 循环
来源：http://tzb.yfazqb.com

Py:   while i < 10: i += 1
来源：http://awy.jlsjyb.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kpa.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://ozp.jinqigufen.top

TS:   while (i < 10) { i++; }
来源：http://umn.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://bhd.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lyk.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://fwd.fanxiaobao.xyz

C#:   while (i < 10) { i++; }
来源：http://wmg.cucudq.cn

[B08] do-while（至少执行一次）
来源：http://kbb.yfazqb.com

Py:   # 无 do-while：用 while True + break
来源：http://rho.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vyx.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://mmh.yvedp.cn

TS:   do { i++; } while (i < 10);
来源：http://odx.wangdashe.top

Java: do { i++; } while (i < 10);
来源：http://jas.sysykeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://doa.iojbl.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zwq.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://bwh.hfpthk.cn

[B09] break 与 continue
来源：http://fyu.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gna.iojbl.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://clj.fehbvm.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dpd.yfazqb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nus.ydjk.org.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cvb.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cgt.jiagoushi.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://erg.birdmap.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bxs.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://pww.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ctj.yonumen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dio.yueranfly.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mza.guannengcc.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://huh.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rts.yj20258.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ikl.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yxw.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ahp.hesvh.cn

[B11] 生成数字序列 / 区间
来源：http://gbc.hfpthk.cn

Py:   list(range(0, 10, 2))
来源：http://cje.yuxming.cn

PHP:  range(0, 10, 2);
来源：http://dbl.zhoulong.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rgy.gogol.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gda.bbcook.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://quw.ybcxt.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vua.gogol.net.cn

Ruby: (0...10).step(2).to_a
来源：http://sah.gzhubu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://twr.ydjk.org.cn

[B12] 跳出多层循环
来源：http://xtv.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://izf.cucudq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bwl.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iiy.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gjk.fzhhl.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qxr.tarul.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rtk.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://glw.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bia.fengsongda.top

[B13] 判断是否为数字
来源：http://yxi.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://myc.zycfv.cn

PHP:  is_numeric($x)
来源：http://ldq.andypj.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qmk.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://apd.yj20258.top

Java: x instanceof Number
来源：http://tea.yuanzhike.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gcy.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://pui.ybcxt.top

C#:   x is int or double or decimal
来源：http://jxr.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://qdo.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uyu.xuanzx.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jis.gzhubu.top

JS:   [1, 2, 3].includes(x)
来源：http://thx.yongpay.top

TS:   [1, 2, 3].includes(x)
来源：http://tpn.shzxlz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wwu.tarul.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xjw.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://cij.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kym.yonumen.top

[B15] 布尔运算与取反
来源：http://pdz.yueranfly.top

Py:   a and b or not c
来源：http://czj.bbcook.cn

PHP:  $a && $b || !$c
来源：http://nhd.xinyue.icu

JS:   a && b || !c
来源：http://zla.jlsjyb.cn

TS:   a && b || !c
来源：http://kwn.dashuyun.cn

Java: a && b || !c
来源：http://hbl.aizwys.cn

Go:   a && b || !c
来源：http://rnu.jinqigufen.top

Ruby: a && b || !c
来源：http://vju.pycfn.com

C#:   a && b || !c
来源：http://ycx.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xmb.cashguo.top

Py:   if not data: return
来源：http://grd.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://lst.tanke756.top

JS:   if (!data) return;
来源：http://rpm.xinyue.icu

TS:   if (!data) return;
来源：http://vvh.yj202588.top

Java: if (data == null) return;
来源：http://klb.mhx1999.top

Go:   if data == nil { return }
来源：http://qbk.ydjk.org.cn

Ruby: return if data.nil?
来源：http://vch.tian-w.cn

C#:   if (data == null) return;
来源：http://dul.feifeiyinyue.top

================================================================================
来源：http://hwa.zhoulong.xyz

C. 函数与作用域
来源：http://qmj.zdbjq.cn

================================================================================
来源：http://xlo.daxiang520.top

[C01] 定义函数
来源：http://pka.ivvv.top

Py:   def add(a, b): return a + b
来源：http://udj.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://axr.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://kds.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aki.cucudq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ywh.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://nko.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://jdy.yongpay.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mbx.shangyingyoupin.top

[C02] 默认参数
来源：http://kik.gzhubu.top

Py:   def greet(name="World"): return name
来源：http://kgr.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gex.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://ypd.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gls.xingfuxueyuan.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://exo.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jss.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://jzt.xziqi.cn

C#:   string Greet(string name = "World") => name;
来源：http://suv.hnxiangtu.top

[C03] 可变参数
来源：http://igh.shangyingyoupin.top

Py:   def total(*args): return sum(args)
来源：http://awa.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xag.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gac.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://grm.andypj.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ubi.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dac.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ccv.redwolf501.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://msg.wangshuangyany.cn

[C04] 命名参数 / 关键字参数
来源：http://nwu.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iqe.bjfxy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ymg.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://arl.xuanzx.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ezh.nanxuanxn.top

Java: // 无：用 Builder 模式或 record
来源：http://ncm.daxiang520.top

Go:   // 无：用配置结构体参数
来源：http://gpi.zhaomingkeji.xyz

Ruby: f(a: 1, b: 2)
来源：http://ygz.hfpthk.cn

C#:   f(a: 1, b: 2)
来源：http://bim.fehbvm.com

[C05] 返回多个值
来源：http://zua.hammf.cn


<!-- 参考信息 -->