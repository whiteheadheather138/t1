代发 wailian999

Py:   "第一行\n第二行"
来源：http://ggu.yuanzhike.top

PHP:  "第一行\n第二行"
来源：http://odt.sjlbkw.cn

JS:   "第一行\n第二行"
来源：http://sod.yfazqb.com

TS:   "第一行\n第二行"
来源：http://rji.hnxiangtu.top

Java: "第一行\n第二行"
来源：http://pcb.yj20258.top

Go:   "第一行\n第二行"
来源：http://puw.wangdashe.top

Ruby: "第一行\n第二行"
来源：http://vsp.fktsv.cn

C#:   "第一行\n第二行"
来源：http://myc.zdqjudy.top

[A14] 注释写法
来源：http://xqn.wangshuangyany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mes.yongpay.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://qlm.yj20258888.top

JS:   // 单行；/* 多行 */
来源：http://myh.nanxinkj.top

TS:   // 单行；/* 多行 */
来源：http://oto.dashuyun.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mok.jqgfzy.top

Go:   // 单行；/* 多行 */
来源：http://spr.zhoulong.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://dno.jiagoushi.top

C#:   // 单行；/* 多行 */
来源：http://xjk.hnqzz.top

[A15] 空值判断与默认值
来源：http://xkg.cheryme.top

Py:   value = data or "默认值"
来源：http://ert.daxiang520.top

PHP:  $value = $data ?? "默认值";
来源：http://nuu.hcnkem.com

JS:   const value = data ?? "默认值";
来源：http://kzm.jqgfzy.top

TS:   const value = data ?? "默认值";
来源：http://ezi.vehdjk.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nrl.jianghu66.top

Go:   if data == "" { data = "默认值" }
来源：http://wxg.ppjwa.cn

Ruby: value = data || "默认值"
来源：http://hpf.sjlbkw.cn

C#:   var value = data ?? "默认值";
来源：http://unf.zycfv.cn

[A16] 真假值判断规则
来源：http://efz.zhixingplan.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pis.jinyuanbaomall.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xkm.jinqigfzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hux.zhoulong.xyz

TS:   if (!x) {}
来源：http://ejq.jinghuilouyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ste.jqgfzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mij.sxryk.cn

Ruby: unless x            # nil 与 false 为假
来源：http://eym.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lmv.wangshuangyany.cn

[A17] 位运算
来源：http://wte.xuetiantiany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gum.0kj1m.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://boc.guannengcc.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mpi.tarul.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nha.hammf.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ogt.kuanghao11.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dyo.wangdashe.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oxf.shzxlz.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uxd.gogol.net.cn

[A18] 字符与 ASCII 码互转
来源：http://wae.316326.xyz

Py:   ord("A"); chr(65)
来源：http://xie.yangfankeji.com

PHP:  ord("A"); chr(65)
来源：http://cqa.yonumen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wvy.gotoacloud.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yre.jinghuilouyu.cn

Java: (int) 'A'; (char) 65
来源：http://aau.nanxinkj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dmm.yonumen.top

Ruby: "A".ord; 65.chr
来源：http://sui.bjfxy.top

C#:   (int)'A'; (char)65
来源：http://rov.shangyingyoupin.top

[A19] 交换两个变量
来源：http://dgl.shuidangran.top

Py:   a, b = b, a
来源：http://pbc.jqgufenzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://yja.cqqwz.cn

JS:   [a, b] = [b, a];
来源：http://lxm.wangshuangyany.cn

TS:   [a, b] = [b, a];
来源：http://qee.quarkkingdee.top

Java: int t = a; a = b; b = t;
来源：http://yto.yj20258888.top

Go:   a, b = b, a
来源：http://irz.fktsv.cn

Ruby: a, b = b, a
来源：http://dgs.shzxlz.cn

C#:   (a, b) = (b, a);
来源：http://pjm.cucudq.cn

[A20] 读取标准输入
来源：http://ovn.kuanghao11.cn

Py:   name = input("请输入：")
来源：http://mub.jlsjyb.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gta.yanxiufei.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jcw.zhiwuduotai.top

TS:   // Node.js：readline 模块
来源：http://pkh.tanke756.top

Java: new Scanner(System.in).nextLine()
来源：http://wgl.shanyushiyangkeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xss.gogol.net.cn

Ruby: gets.chomp
来源：http://ywg.xinyue.icu

C#:   Console.ReadLine();
来源：http://ffs.cqqwz.cn

[A21] 保留指定小数位输出
来源：http://yea.haohaochexian.top

Py:   f"{3.14159:.2f}"
来源：http://cpa.zhoulong.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rja.sxryk.cn

JS:   (3.14159).toFixed(2)
来源：http://xya.aizwys.cn

TS:   (3.14159).toFixed(2)
来源：http://lji.yonumen.top

Java: String.format("%.2f", 3.14159)
来源：http://uuy.wangdashe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cey.vqdsnc.cn

Ruby: format("%.2f", 3.14159)
来源：http://uvx.nanxinkj.top

C#:   3.14159.ToString("F2")
来源：http://upj.mhx1999.top

[A22] 获取字符串长度
来源：http://djq.ehwqpu.com

Py:   len(s)
来源：http://gls.guowangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zkn.hnxiangtu.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gof.xingfuxueyuan.xyz

TS:   s.length
来源：http://nni.fehbvm.com

Java: s.length()
来源：http://bai.jiagoushi.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pag.gzhubu.top

Ruby: s.length
来源：http://izb.cdnleiting.top

C#:   s.Length
来源：http://ljp.hywenlv.cn

[A23] 大小写转换
来源：http://khh.yueranfly.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kxp.zhoulong.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://diy.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hhr.fanxiaobao.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tge.dianchejie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://edp.sysykeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mts.pycfn.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dfb.cheryme.top

C#:   s.ToUpper(); s.ToLower()
来源：http://oar.cucudq.cn

[A24] 去除首尾空白
来源：http://kix.yvedp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://txl.mhx1999.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hap.hammf.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mej.tian-w.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hmr.nwbrower.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nzj.redwolf501.top

Go:   strings.TrimSpace(s)
来源：http://qtl.jianghu66.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pjj.shzxlz.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mfn.sweek.top

[A25] 字符串比较
来源：http://bei.pycfn.com

Py:   s1 == s2; s1 != s2
来源：http://uxc.andypj.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bbn.yuanzhike.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gwn.jyoumei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mqq.yj202588.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yxz.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rrn.xingfuxueyuan.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://gqx.hnqzz.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xdw.316326.xyz

[A26] 类型转换总览
来源：http://lqj.zhaomingkeji.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://opx.yuxming.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sop.gaohongyu789.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ikl.sxryk.cn

TS:   Number() String() Boolean() x as number
来源：http://jnr.jyoumei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://znz.yuanzhike.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yft.zhiwuduotai.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://veu.tian-w.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qup.havefunace.top

================================================================================
来源：http://ztl.chenjidiqi.icu

B. 流程控制
来源：http://lkl.yvedp.cn

================================================================================
来源：http://drm.ydjk.org.cn

[B01] 条件判断 if / else
来源：http://kyj.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://ecz.redwolf501.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fqi.zycfv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://omp.ywan-chungtsiang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qcb.wangdashe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ytl.jqgfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rii.hysaishi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://smr.gogol.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uph.havefunace.top

[B02] 多分支 else if / elif
来源：http://opl.daria6918.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cjs.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jqj.mhx1999.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zmi.ybcxt.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eua.wangshuangyany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lhl.daxiang520.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://acm.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sgg.nwbrower.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rkb.tian-w.cn

[B03] switch / match / case
来源：http://vhr.sjlbkw.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ezj.svipenyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hth.shuidangran.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://omm.shuidangran.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zco.c1oappe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ssi.jinqigfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kla.svipenyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fco.hcnkem.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pds.jqgufenzy.top

[B04] for 计数循环
来源：http://ami.redwolf501.top

Py:   for i in range(10): print(i)
来源：http://ree.nanxinkj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lsi.daria6918.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zvb.ybcxt.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://niy.ehwqpu.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dcy.jyoumei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vhy.zhijiandao.cn

Ruby: 10.times { |i| puts i }
来源：http://xev.ivvv.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dly.jqgufenzy.top

[B05] 遍历数组 / 列表
来源：http://jib.yanxiufei.cn

Py:   for item in arr: print(item)
来源：http://jjt.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lbk.yuanzhike.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kyx.guannengcc.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nqs.shangyingyoupin.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://eyh.shangyingyoupin.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cin.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://tju.sufxvd.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bqp.ydzc1.top

[B06] 遍历字典 / 对象
来源：http://aaa.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sqr.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rgg.yangfankeji.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jmf.sweek.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uxp.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://elt.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://acr.yuxming.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vui.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aom.gzhubu.top

[B07] while 循环
来源：http://gge.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://mam.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ldc.tarul.cn

JS:   while (i < 10) { i++; }
来源：http://akp.dashuyun.cn

TS:   while (i < 10) { i++; }
来源：http://bik.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://cjo.zhiwuduotai.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mbk.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://hft.ydjk.org.cn

C#:   while (i < 10) { i++; }
来源：http://agt.tanke756.top

[B08] do-while（至少执行一次）
来源：http://xvy.cucudq.cn

Py:   # 无 do-while：用 while True + break
来源：http://qrs.yvedp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bfk.haohaochexian.top

JS:   do { i++; } while (i < 10);
来源：http://lks.ppjwa.cn

TS:   do { i++; } while (i < 10);
来源：http://pem.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://nsq.xuetiantiany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cqh.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://dip.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://als.tianlin.xyz

[B09] break 与 continue
来源：http://loo.ppjwa.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sxa.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lhp.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pem.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jys.xingfuxueyuan.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oac.pengpengdd.cyou

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yzl.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jff.zdqjudy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://njq.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://ddb.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qut.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xko.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fzq.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://omz.bbcook.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tob.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pvl.ehwqpu.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kpw.jqgfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://esu.jinghuilouyu.cn

[B11] 生成数字序列 / 区间
来源：http://xnf.yvedp.cn

Py:   list(range(0, 10, 2))
来源：http://ewh.chenzaomai.com

PHP:  range(0, 10, 2);
来源：http://ljy.aizwys.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nmc.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zgg.jqgufenzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qzf.meibo888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://djm.aizwys.cn

Ruby: (0...10).step(2).to_a
来源：http://von.shangyingyoupin.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://crn.ehwqpu.com

[B12] 跳出多层循环
来源：http://khz.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://goq.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fhb.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nhz.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gec.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://byn.wangdashe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bpu.xuetiantiany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cpd.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rzf.wangdashe.top

[B13] 判断是否为数字
来源：http://jcl.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://ltv.zhaomingkeji.xyz

PHP:  is_numeric($x)
来源：http://gve.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dvy.jyoumei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zhv.zycfv.cn

Java: x instanceof Number
来源：http://xfp.bjfxy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yxd.kuanghao11.cn

Ruby: x.is_a?(Numeric)
来源：http://ylo.iojbl.cn

C#:   x is int or double or decimal
来源：http://dah.jianghu66.top

[B14] 判断值是否在集合内
来源：http://bmb.vehdjk.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xad.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wsp.fengsongda.top

JS:   [1, 2, 3].includes(x)
来源：http://bcp.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://hxp.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fmt.bjfxy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://czw.jqgufenzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://nau.pengpengdd.cyou

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://orj.birdmap.top

[B15] 布尔运算与取反
来源：http://ymv.haohaochexian.top

Py:   a and b or not c
来源：http://cdx.aibaodan.cn

PHP:  $a && $b || !$c
来源：http://grl.fengsongda.top

JS:   a && b || !c
来源：http://oux.ydjk.org.cn

TS:   a && b || !c
来源：http://nqf.chenzaomai.com

Java: a && b || !c
来源：http://okc.yfazqb.com

Go:   a && b || !c
来源：http://blo.yongpay.top

Ruby: a && b || !c
来源：http://tvn.ctjpmb.com

C#:   a && b || !c
来源：http://pqq.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://ltx.fanxiaobao.xyz

Py:   if not data: return
来源：http://jym.smart0.xyz

PHP:  if (!$data) { return; }
来源：http://aqh.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://vtc.ydzc1.top

TS:   if (!data) return;
来源：http://ywe.tianlin.xyz

Java: if (data == null) return;
来源：http://tmr.havefunace.top

Go:   if data == nil { return }
来源：http://hpe.vehdjk.com

Ruby: return if data.nil?
来源：http://pzv.ywan-chungtsiang.top

C#:   if (data == null) return;
来源：http://hpk.jinghuilouyu.cn

================================================================================
来源：http://uuk.iojbl.cn

C. 函数与作用域
来源：http://ukk.iojbl.cn

================================================================================
来源：http://lhp.9152youxi.cn

[C01] 定义函数
来源：http://xtp.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://ejy.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uzb.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://fuw.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nxk.xziqi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wsk.ppjwa.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bju.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://jni.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vaa.bjfxy.top

[C02] 默认参数
来源：http://bzs.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://otu.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ezv.tarul.cn

JS:   function greet(name = "World") { return name; }
来源：http://leq.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xyb.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bnv.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zsm.hcnkem.com

Ruby: def greet(name = "World") = name
来源：http://bym.kuanghao11.cn

C#:   string Greet(string name = "World") => name;
来源：http://jru.sysykeji.top

[C03] 可变参数
来源：http://qmp.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://ydm.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ldl.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nep.shzxlz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tum.jinyuanbaomall.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://szt.kuanghao11.cn


<!-- 参考信息 -->