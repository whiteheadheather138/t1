代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://niq.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://eph.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://gbr.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wwu.redwolf501.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hlt.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://mzv.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qnw.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://ixp.zdqjudy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qlp.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fkv.snrcjt.cn

JS:   arr.map(x => x * 2)
来源：http://zlr.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://hfk.zhiwuduotai.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pnm.jqgufenzy.top

Go:   // 手写循环
来源：http://sfc.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://ijt.bbcook.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://orx.yvedp.cn

[D15] 去重
来源：http://edt.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hbj.0kj1m.cn

PHP:  array_unique($arr);
来源：http://ozs.xuanzx.com

JS:   [...new Set(arr)]
来源：http://bny.xziqi.cn

TS:   [...new Set(arr)]
来源：http://zvc.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fzl.wangshuangyany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://osh.nwbrower.top

Ruby: arr.uniq
来源：http://rli.ctjpmb.com

C#:   list.Distinct().ToList()
来源：http://kxf.cheryme.top

[D16] 求和与平均值
来源：http://eqj.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uqe.zhiwuduotai.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kdh.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bni.yangfankeji.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iqa.cucudq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mnh.cheryme.top

Go:   // 手写循环累加
来源：http://uqd.52xcode.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://clk.52xcode.cn

C#:   list.Sum();  list.Average()
来源：http://mbe.aibaodan.cn

[D17] 最大值与最小值
来源：http://fkf.daxiang520.top

Py:   max(arr);  min(arr)
来源：http://ocd.316326.xyz

PHP:  max($arr);  min($arr);
来源：http://owu.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rrc.meibo888.top

TS:   Math.max(...arr);
来源：http://gnl.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dyo.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nue.hysaishi.cn

Ruby: arr.max;  arr.min
来源：http://dlo.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://boh.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://rwt.hongshengwenyu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fuc.wangshuangyany.cn

PHP:  array_merge(...$nested);
来源：http://avr.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dzv.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://dxn.yonumen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ndf.yuxming.cn

Go:   // 手写双层循环
来源：http://xrc.316326.xyz

Ruby: nested.flatten
来源：http://mjm.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lau.hongshengwenyu.top

[D19] 按字段分组
来源：http://dlr.shuidangran.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vof.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://syp.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://efn.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vqi.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aud.cashguo.top

Go:   // 手写 map[string][]T
来源：http://aqo.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tno.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://awf.sweek.top

[D20] 统计每个元素出现次数
来源：http://xmv.zhiwuduotai.top

Py:   Counter(arr)
来源：http://kum.hnxiangtu.top

PHP:  array_count_values($arr);
来源：http://yzm.fktsv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fev.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zye.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cnk.nanxinkj.top

Go:   // 手写 map[T]int
来源：http://qmv.tian-w.cn

Ruby: arr.tally
来源：http://kfs.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mwk.sxryk.cn

[D21] 判断是否包含某元素
来源：http://fab.gaohongyu789.top

Py:   x in arr
来源：http://thy.iojbl.cn

PHP:  in_array($x, $arr, true);
来源：http://zfd.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://ifj.zhoulong.xyz

TS:   arr.includes(x)
来源：http://ycd.cheryme.top

Java: list.contains(x)
来源：http://wuz.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://kbz.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://hrx.yvedp.cn

C#:   list.Contains(x)
来源：http://lsn.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://dyc.jqgfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://leo.hysaishi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aqw.hnqzz.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://otl.fengsongda.top

TS:   [...arr];
来源：http://izc.ctjpmb.com

Java: new ArrayList<>(list);
来源：http://mhh.yangfankeji.com

Go:   copied := append([]int(nil), arr...)
来源：http://fxj.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://szf.smart0.xyz

C#:   new List<int>(list);
来源：http://xme.hysaishi.cn

[D23] reduce 累积计算
来源：http://oyq.fengsongda.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eps.zhengqikj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iqv.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xgv.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ynm.shuidangran.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ybs.mhx1999.top

Go:   // 手写循环
来源：http://vfq.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://egj.hywenlv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rfj.hywenlv.cn

[D24] 字典 / Map 基本操作
来源：http://ahr.birdmap.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sns.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aak.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fiw.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gct.fengsongda.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://buz.hongshengwenyu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fhy.haohaochexian.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wkr.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aqr.tarul.cn

[D25] Set 集合去重与交并差
来源：http://rxg.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nan.gotoacloud.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xqy.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xjk.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vfk.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://udp.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lze.yongpay.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gcw.ppjwa.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wfb.tian-w.cn

[D26] 数组转字符串
来源：http://hdp.chenjidiqi.icu

Py:   ", ".join(map(str, arr))
来源：http://yaz.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://qsk.sufxvd.cn

JS:   arr.join(", ")
来源：http://xga.ctjpmb.com

TS:   arr.join(", ")
来源：http://vac.xuanzx.com

Java: String.join(", ", list)
来源：http://enp.epnwcf.com

Go:   strings.Join(strs, ", ")
来源：http://nol.hnqzz.top

Ruby: arr.join(", ")
来源：http://xjq.cheryme.top

C#:   string.Join(", ", list)
来源：http://qqq.xziqi.cn

================================================================================
来源：http://rbg.yongpay.top

E. 字符串处理
来源：http://lum.chenlongwang.top

================================================================================
来源：http://pvs.jyoumei.cn

[E01] 拼接字符串
来源：http://cpi.tanke756.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://imy.snrcjt.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cck.cqqwz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nnv.jqgfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aya.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hea.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nje.tian-w.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vtp.yongpay.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gfp.zdqjudy.top

[E02] 重复字符串
来源：http://nkn.zhengqikj.top

Py:   "ab" * 3
来源：http://sms.yueranfly.top

PHP:  str_repeat("ab", 3);
来源：http://nrv.zhoulong.xyz

JS:   "ab".repeat(3)
来源：http://cev.xylfe.cn

TS:   "ab".repeat(3)
来源：http://qwt.tianlin.xyz

Java: "ab".repeat(3)
来源：http://qgn.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://xvx.shzxlz.cn

Ruby: "ab" * 3
来源：http://bsl.meibo888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fqg.dashuyun.cn

[E03] 截取子串
来源：http://sjc.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ran.316326.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qjt.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cob.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://gpg.sufxvd.cn

Java: s.substring(1, 4)
来源：http://wvi.iojbl.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://epn.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://obe.zdbjq.cn

C#:   s.Substring(1, 3)
来源：http://moa.zdqjudy.top

[E04] 查找子串位置
来源：http://ztx.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://syb.nwbrower.top

PHP:  strpos($s, "x");
来源：http://drn.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dta.ppjwa.cn

TS:   s.indexOf("x")
来源：http://lij.cheryme.top

Java: s.indexOf("x")
来源：http://kgn.mhx1999.top

Go:   strings.Index(s, "x")
来源：http://rrh.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://nzb.yvedp.cn

C#:   s.IndexOf("x")
来源：http://ulz.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zkw.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jjw.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://miy.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yox.yj20258888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jjv.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zac.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vls.zhiwuduotai.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hab.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fjr.yfazqb.com

[E06] 替换子串
来源：http://afz.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tzd.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://lvo.guowangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lzf.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://lke.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mon.cdnleiting.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dkn.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hhp.tanke756.top

C#:   s.Replace("a", "b")
来源：http://lxs.uphjek.com

[E07] 按分隔符拆分
来源：http://qrx.xziqi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iuo.xuanzx.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nhd.vehdjk.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://frn.chenjidiqi.icu

TS:   s.split(",")
来源：http://nqu.gaohongyu789.top

Java: s.split(",");  s.split("\\s+")
来源：http://ihp.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ydz.shzxlz.cn

Ruby: s.split(",");  s.split
来源：http://gdi.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://utz.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://xkr.smart0.xyz

Py:   ",".join(items)
来源：http://cmu.epnwcf.com

PHP:  implode(",", $items);
来源：http://gln.gaohongyu789.top

JS:   items.join(",")
来源：http://xza.quarkkingdee.top

TS:   items.join(",")
来源：http://fgl.uphjek.com

Java: String.join(",", items)
来源：http://qhe.feifeiyinyue.top

Go:   strings.Join(items, ",")
来源：http://ugw.yj20258.top

Ruby: items.join(",")
来源：http://crq.hcnkem.com

C#:   string.Join(",", items)
来源：http://gba.jyoumei.cn

[E09] 去除所有空白字符
来源：http://gsy.ydzc1.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dbj.jinghuilouyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://elz.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://ukw.daxiang520.top

TS:   s.replace(/\s+/g, "")
来源：http://tfs.gotoacloud.top

Java: s.replaceAll("\\s+", "")
来源：http://sud.cheryme.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://sxc.zhixingplan.top

Ruby: s.gsub(/\s+/, "")
来源：http://tkt.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jcb.yongpay.top

[E10] 左侧补零 / 定长填充
来源：http://jje.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://thr.sjlbkw.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zky.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://jgy.birdmap.top

TS:   "7".padStart(3, "0")
来源：http://lcc.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://axx.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xig.andypj.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rsl.jinyuanbaomall.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yjh.fzhhl.top

[E11] 反转字符串
来源：http://pco.yonumen.top

Py:   s[::-1]
来源：http://xsy.yanxiufei.cn

PHP:  strrev($s);
来源：http://lcw.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://vzr.uphjek.com

TS:   [...s].reverse().join("")
来源：http://hwg.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lxd.shangyingyoupin.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://bkb.jyoumei.cn

Ruby: s.reverse
来源：http://fgj.xuetiantiany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ulm.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://uxu.daria6918.cn

Py:   s.count("a")
来源：http://svd.fengsongda.top

PHP:  substr_count($s, "a");
来源：http://pxp.ywan-chungtsiang.top

JS:   s.split("a").length - 1
来源：http://stw.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://rmc.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hvp.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://fup.cheryme.top

Ruby: s.count("a")
来源：http://ett.chenzaomai.com

C#:   s.Count(c => c == 'a')
来源：http://jdc.gogol.net.cn

[E13] 逐字符遍历
来源：http://psu.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://xui.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://esy.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wnc.zhaomingkeji.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://zre.zycfv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cby.hesvh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://upc.yj20258.top

Ruby: s.each_char { |ch| puts ch }
来源：http://voe.jiagoushi.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pon.feifeiyinyue.top

[E14] URL 编码与 Base64
来源：http://ogs.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ffg.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yyd.sxryk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mvg.jqgufenzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://svo.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://otg.yuxming.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uvq.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ulr.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cqj.yfazqb.com

[E15] HTML 转义 / 反转义
来源：http://gtv.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bai.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://szo.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pxa.wangdashe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dcu.aizwys.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iln.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rif.fehbvm.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mbu.zhongyouzk.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mkv.feifeiyinyue.top

[E16] 数字千分位
来源：http://ixm.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://not.ehwqpu.com

PHP:  number_format(1234567);
来源：http://aso.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cly.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yaf.redwolf501.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dsd.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cag.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jgk.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://fqa.epnwcf.com

[E17] 首字母大写
来源：http://hqn.chenlongwang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lxr.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zto.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bhk.c1oappe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ybh.jqgufenzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qpu.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tym.feifeiyinyue.top

Ruby: s.capitalize
来源：http://zjg.feifeiyinyue.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qrx.hywenlv.cn

[E18] 模板占位符替换
来源：http://mxd.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yax.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jhy.andypj.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://fky.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oob.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ftv.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gyo.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tmf.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pec.guannengcc.top

[E19] 多行文本按行拆分
来源：http://biz.dianchejie.cn

Py:   s.splitlines()
来源：http://ldb.hywenlv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://las.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://rkz.dianchejie.cn

TS:   s.split(/\r?\n/)
来源：http://lav.wangdashe.top

Java: s.lines().toList()
来源：http://jiv.ehwqpu.com

Go:   strings.Split(s, "\n")
来源：http://wfj.0kj1m.cn

Ruby: s.lines
来源：http://qib.yangfankeji.com

C#:   s.Split('\n')
来源：http://lnh.xuanzx.com

[E20] 判断字符串是否为空
来源：http://pfx.guowangkeji.top

Py:   if not s:
来源：http://ihy.andypj.xyz


<!-- 参考信息 -->