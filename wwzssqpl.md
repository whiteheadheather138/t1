代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://oho.hysaishi.cn

[A15] 空值判断与默认值
来源：http://ypi.cqqwz.cn

Py:   value = data or "默认值"
来源：http://uga.hnxiangtu.top

PHP:  $value = $data ?? "默认值";
来源：http://lxf.yj202588.top

JS:   const value = data ?? "默认值";
来源：http://wsk.fengsongda.top

TS:   const value = data ?? "默认值";
来源：http://ssf.daria6918.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nlx.ywan-chungtsiang.top

Go:   if data == "" { data = "默认值" }
来源：http://ory.epnwcf.com

Ruby: value = data || "默认值"
来源：http://zld.yuanzhike.top

C#:   var value = data ?? "默认值";
来源：http://kuc.nwbrower.top

[A16] 真假值判断规则
来源：http://qdu.tian-w.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mpo.mhx1999.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dqt.daxiang520.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ehy.wangshuangyany.cn

TS:   if (!x) {}
来源：http://ywu.yangfankeji.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://srd.shuidangran.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zjl.jinqigufen.top

Ruby: unless x            # nil 与 false 为假
来源：http://uco.haohaochexian.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hax.havefunace.top

[A17] 位运算
来源：http://wda.cqqwz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lns.nwbrower.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vns.nanxinkj.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hmb.sweek.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iew.xylfe.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cjj.ydjk.org.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mqa.chenjidiqi.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rdd.cdnleiting.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qwi.nanxuanxn.top

[A18] 字符与 ASCII 码互转
来源：http://fkp.tarul.cn

Py:   ord("A"); chr(65)
来源：http://fov.shangyingyoupin.top

PHP:  ord("A"); chr(65)
来源：http://sqf.jianghu66.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hnb.hnxiangtu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://heq.shangyingyoupin.top

Java: (int) 'A'; (char) 65
来源：http://rat.birdmap.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hqw.gzhubu.top

Ruby: "A".ord; 65.chr
来源：http://elr.ppjwa.cn

C#:   (int)'A'; (char)65
来源：http://pid.fengsongda.top

[A19] 交换两个变量
来源：http://haw.gotoacloud.top

Py:   a, b = b, a
来源：http://ysm.gzhubu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://htw.wangdashe.top

JS:   [a, b] = [b, a];
来源：http://rgo.quarkkingdee.top

TS:   [a, b] = [b, a];
来源：http://uec.aizwys.cn

Java: int t = a; a = b; b = t;
来源：http://yie.cheryme.top

Go:   a, b = b, a
来源：http://bxf.jinqigufen.top

Ruby: a, b = b, a
来源：http://cxg.andypj.xyz

C#:   (a, b) = (b, a);
来源：http://elo.nanxuanxn.top

[A20] 读取标准输入
来源：http://cvh.jinghuilouyu.cn

Py:   name = input("请输入：")
来源：http://sdb.ivvv.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gxz.birdmap.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zvx.shanyushiyangkeji.top

TS:   // Node.js：readline 模块
来源：http://tfb.hywenlv.cn

Java: new Scanner(System.in).nextLine()
来源：http://auv.xinyue.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://myw.sysykeji.top

Ruby: gets.chomp
来源：http://rrc.havefunace.top

C#:   Console.ReadLine();
来源：http://jjn.ivvv.top

[A21] 保留指定小数位输出
来源：http://vsd.gzhubu.top

Py:   f"{3.14159:.2f}"
来源：http://wch.xuetiantiany.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zbj.zhongyouzk.top

JS:   (3.14159).toFixed(2)
来源：http://rre.zdbjq.cn

TS:   (3.14159).toFixed(2)
来源：http://fzq.aibaodan.cn

Java: String.format("%.2f", 3.14159)
来源：http://sno.zdqjudy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uzc.c1oappe.top

Ruby: format("%.2f", 3.14159)
来源：http://bgu.yj20258888.top

C#:   3.14159.ToString("F2")
来源：http://kya.cucudq.cn

[A22] 获取字符串长度
来源：http://iwu.chenzaomai.com

Py:   len(s)
来源：http://zeo.jyoumei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lae.ybcxt.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://btq.shangyingyoupin.top

TS:   s.length
来源：http://meo.yj20258.top

Java: s.length()
来源：http://bwn.hesvh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wqw.shanyushiyangkeji.top

Ruby: s.length
来源：http://cln.hnqzz.top

C#:   s.Length
来源：http://lzr.jinyuanbaomall.cn

[A23] 大小写转换
来源：http://nzi.chenlongwang.top

Py:   s.upper(); s.lower(); s.title()
来源：http://exd.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jua.jinqigufen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://apc.zhengqikj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xyu.ivvv.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rly.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://svu.sjlbkw.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mkn.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eas.hammf.cn

[A24] 去除首尾空白
来源：http://thb.wangshuangyany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xbp.jqgufenzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tve.svipenyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nak.jianghu66.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kvp.aizwys.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bwt.zycfv.cn

Go:   strings.TrimSpace(s)
来源：http://xvc.shuidangran.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://chr.daxiang520.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bpc.yonumen.top

[A25] 字符串比较
来源：http://lxm.nanxuanxn.top

Py:   s1 == s2; s1 != s2
来源：http://yrx.cashguo.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gaz.ctjpmb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wrd.birdmap.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vkj.shanyushiyangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hei.hnxiangtu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nzc.haohaochexian.top

Ruby: s1 == s2; s1 <=> s2
来源：http://gsf.zdbjq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zrm.jiagoushi.top

[A26] 类型转换总览
来源：http://gqv.xylfe.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tcw.xuanzx.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://twq.havefunace.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uye.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://ncj.shzxlz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vge.cashguo.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ptx.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cdy.zhaomingkeji.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wuw.snrcjt.cn

================================================================================
来源：http://bul.bjfxy.top

B. 流程控制
来源：http://unr.0kj1m.cn

================================================================================
来源：http://ivz.hcnkem.com

[B01] 条件判断 if / else
来源：http://hlv.dashuyun.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yiz.jinghuilouyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xbv.jinyuanbaomall.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://doe.sjlbkw.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lii.nanxuanxn.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zrm.zhongyouzk.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yga.zdbjq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rqo.smart0.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pqm.ehwqpu.com

[B02] 多分支 else if / elif
来源：http://alv.xuetiantiany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://okv.daxiang520.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://avt.aizwys.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xsb.zycfv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dud.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hru.chenjidiqi.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yjv.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qdd.ctjpmb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fwh.epnwcf.com

[B03] switch / match / case
来源：http://vbh.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://glr.yfazqb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lpm.sxryk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yhf.feifeiyinyue.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://olp.chenjidiqi.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mqs.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wwn.kuanghao11.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nuf.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ubx.jqgufenzy.top

[B04] for 计数循环
来源：http://xno.redwolf501.top

Py:   for i in range(10): print(i)
来源：http://xxd.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://skm.ehwqpu.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dzu.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kuf.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://inu.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xgz.316326.xyz

Ruby: 10.times { |i| puts i }
来源：http://fgl.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iqt.uphjek.com

[B05] 遍历数组 / 列表
来源：http://iex.svipenyu.cn

Py:   for item in arr: print(item)
来源：http://jli.daxiang520.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jjq.shanyushiyangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kve.meibo888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dvq.vehdjk.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://xxz.snrcjt.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://evh.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://wkl.shzxlz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lzr.hammf.cn

[B06] 遍历字典 / 对象
来源：http://oaw.redwolf501.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dou.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jzj.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wyt.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ujm.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fug.shanyushiyangtech.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bik.cheryme.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oyy.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jol.yangfankeji.com

[B07] while 循环
来源：http://ghn.sweek.top

Py:   while i < 10: i += 1
来源：http://ifu.zhixingplan.top

PHP:  while ($i < 10) { $i++; }
来源：http://qkk.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://adj.nanxuanxn.top

TS:   while (i < 10) { i++; }
来源：http://jbk.zhiwuduotai.top

Java: while (i < 10) { i++; }
来源：http://wcq.9152youxi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kty.jinghuilouyu.cn

Ruby: while i < 10; i += 1; end
来源：http://ons.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://yig.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://wlx.jqgfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://wta.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://abn.yj20258.top

JS:   do { i++; } while (i < 10);
来源：http://blc.ppjwa.cn

TS:   do { i++; } while (i < 10);
来源：http://iet.cashguo.top

Java: do { i++; } while (i < 10);
来源：http://odz.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://roa.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://abu.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://ggq.chenzaomai.com

[B09] break 与 continue
来源：http://qrt.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://akv.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eth.shanyushiyangtech.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lhq.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xkm.birdmap.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gne.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uow.hnqzz.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kws.hnxiangtu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://icu.xinyue.icu

[B10] 遍历同时拿索引
来源：http://nrb.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://spf.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nhd.xuetiantiany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pta.xinyue.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wti.smart0.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zku.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hhx.sjlbkw.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://row.hongshengwenyu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pgw.jiagoushi.top

[B11] 生成数字序列 / 区间
来源：http://amt.hfpthk.cn

Py:   list(range(0, 10, 2))
来源：http://idv.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://mni.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eub.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gzy.fehbvm.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jiu.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://guu.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://zki.pengpengdd.cyou

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hke.zhixingplan.top

[B12] 跳出多层循环
来源：http://qsp.epnwcf.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://zfj.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vqm.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ghc.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xpw.sjlbkw.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ptc.hesvh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kto.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dwh.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://phy.sxryk.cn

[B13] 判断是否为数字
来源：http://ueo.fanxiaobao.xyz

Py:   isinstance(x, (int, float))
来源：http://zea.zhixingplan.top

PHP:  is_numeric($x)
来源：http://wgc.sufxvd.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bqt.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://par.yueranfly.top

Java: x instanceof Number
来源：http://dny.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://alk.pengpengdd.cyou

Ruby: x.is_a?(Numeric)
来源：http://hjm.fanxiaobao.xyz

C#:   x is int or double or decimal
来源：http://tby.bjfxy.top

[B14] 判断值是否在集合内
来源：http://jrn.jqgufenzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ytj.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wdl.ctjpmb.com

JS:   [1, 2, 3].includes(x)
来源：http://ijv.cqqwz.cn

TS:   [1, 2, 3].includes(x)
来源：http://ojz.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lza.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pbm.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://ozp.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dhf.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://dbr.jinqigufen.top

Py:   a and b or not c
来源：http://qzh.uphjek.com

PHP:  $a && $b || !$c
来源：http://dkn.gzhubu.top

JS:   a && b || !c
来源：http://mxm.jinqigfzy.top

TS:   a && b || !c
来源：http://wlk.vqdsnc.cn

Java: a && b || !c
来源：http://lwf.jyoumei.cn

Go:   a && b || !c
来源：http://feo.vqdsnc.cn

Ruby: a && b || !c
来源：http://ony.aibaodan.cn

C#:   a && b || !c
来源：http://mun.bbcook.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lit.yj202588.top

Py:   if not data: return
来源：http://akl.yuxming.cn

PHP:  if (!$data) { return; }
来源：http://btv.iojbl.cn

JS:   if (!data) return;
来源：http://hkh.jinyuanbaomall.cn

TS:   if (!data) return;
来源：http://jze.hnxiangtu.top

Java: if (data == null) return;
来源：http://vmx.jianghu66.top

Go:   if data == nil { return }
来源：http://jgd.zycfv.cn

Ruby: return if data.nil?
来源：http://cpc.yj20258888.top

C#:   if (data == null) return;
来源：http://htw.yuxming.cn

================================================================================
来源：http://alq.guowangkeji.top

C. 函数与作用域
来源：http://xce.gzhubu.top

================================================================================
来源：http://idg.xinyue.icu

[C01] 定义函数
来源：http://bzy.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://xkl.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dfd.cashguo.top

JS:   function add(a, b) { return a + b; }
来源：http://aht.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://avz.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oej.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://jls.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://die.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bxx.havefunace.top

[C02] 默认参数
来源：http://dhu.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://aiq.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://csx.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://okc.cheryme.top

TS:   function greet(name: string = "World") { return name; }
来源：http://soh.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hyf.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aab.fktsv.cn

Ruby: def greet(name = "World") = name
来源：http://dqm.meibo888.top

C#:   string Greet(string name = "World") => name;
来源：http://ejy.hnxiangtu.top

[C03] 可变参数
来源：http://gkt.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://amw.yj202588.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iwg.sxryk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ofn.birdmap.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xaj.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wou.chenjidiqi.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vce.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ykh.shzxlz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ppx.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://haj.hfpthk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://acs.kuanghao11.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rww.chenlongwang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fta.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nhy.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://uwa.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://sww.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://tjd.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://sry.hnqzz.top

[C05] 返回多个值
来源：http://jir.bbcook.cn

Py:   return a, b
来源：http://mhn.andypj.xyz

PHP:  return [$a, $b];
来源：http://bll.tanke756.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://sqb.andypj.xyz

TS:   return { a, b };
来源：http://yno.yueranfly.top


<!-- 参考信息 -->