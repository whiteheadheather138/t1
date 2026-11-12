代发 wailian999

Ruby: arr.index(x)
来源：http://poj.jianghu66.top

C#:   list.IndexOf(x);
来源：http://len.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://ffo.ywan-chungtsiang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mem.zhixingplan.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tpy.nanxuanxn.top

JS:   arr.filter(x => x > 3)
来源：http://bfl.jinyuanbaomall.cn

TS:   arr.filter(x => x > 3)
来源：http://huw.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://goy.gaohongyu789.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tbw.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://vij.ehwqpu.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ape.fktsv.cn

[D14] 映射转换（每个元素变形）
来源：http://cqe.jqgufenzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tii.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gqm.iojbl.cn

JS:   arr.map(x => x * 2)
来源：http://wfl.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://ala.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rni.ivvv.top

Go:   // 手写循环
来源：http://hlv.tanke756.top

Ruby: arr.map { |x| x * 2 }
来源：http://ely.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kwk.cashguo.top

[D15] 去重
来源：http://ogy.hongshengwenyu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iok.jqgfzy.top

PHP:  array_unique($arr);
来源：http://uix.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://fxm.dashuyun.cn

TS:   [...new Set(arr)]
来源：http://axu.shanyushiyangtech.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ddx.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://apf.cucudq.cn

Ruby: arr.uniq
来源：http://yys.fehbvm.com

C#:   list.Distinct().ToList()
来源：http://fgz.zycfv.cn

[D16] 求和与平均值
来源：http://mtf.fktsv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ksp.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mai.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vdy.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://htd.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mig.zhengqikj.top

Go:   // 手写循环累加
来源：http://nwj.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pmh.uphjek.com

C#:   list.Sum();  list.Average()
来源：http://ztm.hesvh.cn

[D17] 最大值与最小值
来源：http://owh.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://elh.fzhhl.top

PHP:  max($arr);  min($arr);
来源：http://wmh.fktsv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lol.hesvh.cn

TS:   Math.max(...arr);
来源：http://rfk.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://rut.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fur.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://tlq.xuetiantiany.cn

C#:   list.Max();  list.Min()
来源：http://xtx.birdmap.top

[D18] 扁平化嵌套数组
来源：http://fbs.shuidangran.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://duv.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://jbl.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ika.zycfv.cn

TS:   nested.flat();
来源：http://olz.jiagoushi.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fdj.ydzc1.top

Go:   // 手写双层循环
来源：http://zhm.gzhubu.top

Ruby: nested.flatten
来源：http://doi.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://blk.jinghuilouyu.cn

[D19] 按字段分组
来源：http://qmu.hcnkem.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cfx.yanxiufei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wld.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://idi.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://req.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uke.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://hsl.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ufe.cqqwz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://opz.gaohongyu789.top

[D20] 统计每个元素出现次数
来源：http://uge.yonumen.top

Py:   Counter(arr)
来源：http://oaz.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://oqf.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vej.pycfn.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lsm.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xes.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://pbb.hnqzz.top

Ruby: arr.tally
来源：http://pfo.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aaa.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://twy.ydjk.org.cn

Py:   x in arr
来源：http://urd.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://bwx.hcnkem.com

JS:   arr.includes(x)
来源：http://eac.xinyue.icu

TS:   arr.includes(x)
来源：http://hyh.cucudq.cn

Java: list.contains(x)
来源：http://qlk.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://cug.aibaodan.cn

Ruby: arr.include?(x)
来源：http://wll.yj20258.top

C#:   list.Contains(x)
来源：http://bxi.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://jzm.jinghuilouyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://niz.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aoy.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vbc.yuanzhike.top

TS:   [...arr];
来源：http://wio.kuanghao11.cn

Java: new ArrayList<>(list);
来源：http://wps.hfpthk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qro.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://xbr.guowangkeji.top

C#:   new List<int>(list);
来源：http://iwc.dianchejie.cn

[D23] reduce 累积计算
来源：http://env.xingfuxueyuan.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://acl.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://krh.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://azg.sysykeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ovu.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pdj.hywenlv.cn

Go:   // 手写循环
来源：http://fjj.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nue.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jca.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://nvd.zhengqikj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tfi.gogol.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zwg.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://skn.sxryk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xlu.c1oappe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iim.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cto.gogol.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ovw.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vvv.jqgfzy.top

[D25] Set 集合去重与交并差
来源：http://fan.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://chr.xuetiantiany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xlc.ydjk.org.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pbo.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qso.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://anq.fktsv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ekj.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fuw.zycfv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fzo.sxryk.cn

[D26] 数组转字符串
来源：http://xir.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://lew.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://ulc.shzxlz.cn

JS:   arr.join(", ")
来源：http://gov.gogol.net.cn

TS:   arr.join(", ")
来源：http://cvb.9152youxi.cn

Java: String.join(", ", list)
来源：http://ctg.316326.xyz

Go:   strings.Join(strs, ", ")
来源：http://rqq.zdbjq.cn

Ruby: arr.join(", ")
来源：http://xbp.hammf.cn

C#:   string.Join(", ", list)
来源：http://pjc.jinqigufen.top

================================================================================
来源：http://sor.xingfuxueyuan.xyz

E. 字符串处理
来源：http://xdo.ywan-chungtsiang.top

================================================================================
来源：http://abg.yuxming.cn

[E01] 拼接字符串
来源：http://eih.cheryme.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aav.dashuyun.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://apz.zdbjq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hxd.kuanghao11.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eqx.sjlbkw.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nmx.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://owm.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ypz.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mop.feifeiyinyue.top

[E02] 重复字符串
来源：http://ril.fktsv.cn

Py:   "ab" * 3
来源：http://zlg.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://tyy.hesvh.cn

JS:   "ab".repeat(3)
来源：http://kvc.yuxming.cn

TS:   "ab".repeat(3)
来源：http://ogw.hfpthk.cn

Java: "ab".repeat(3)
来源：http://rrs.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://whd.gaohongyu789.top

Ruby: "ab" * 3
来源：http://err.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://apu.shzxlz.cn

[E03] 截取子串
来源：http://pxb.zhengqikj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://msh.gzhubu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wam.sufxvd.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wor.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://xnn.gotoacloud.top

Java: s.substring(1, 4)
来源：http://wxo.jinyuanbaomall.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nat.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://lsn.meibo888.top

C#:   s.Substring(1, 3)
来源：http://jex.chenlongwang.top

[E04] 查找子串位置
来源：http://wms.hammf.cn

Py:   s.find("x");  s.index("x")
来源：http://wpu.52xcode.cn

PHP:  strpos($s, "x");
来源：http://jgy.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://veu.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://jvq.jinqigufen.top

Java: s.indexOf("x")
来源：http://wvf.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://vbj.ydzc1.top

Ruby: s.index("x")
来源：http://lym.smart0.xyz

C#:   s.IndexOf("x")
来源：http://zil.hnqzz.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ukt.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cwx.fktsv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vpt.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qza.havefunace.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jnp.bjfxy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wvb.mhx1999.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ltd.tian-w.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ozi.chenjidiqi.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xrq.9152youxi.cn

[E06] 替换子串
来源：http://mso.nanxuanxn.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tnp.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://kxa.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yhj.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://pgr.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ymu.zhiwuduotai.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vyh.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kxs.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://lhc.nanxuanxn.top

[E07] 按分隔符拆分
来源：http://zeu.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zvw.tanke756.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bkh.bjfxy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gbo.zhiwuduotai.top

TS:   s.split(",")
来源：http://ovb.hesvh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zdl.cheryme.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yvs.xuetiantiany.cn

Ruby: s.split(",");  s.split
来源：http://ykd.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kds.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://usg.cashguo.top

Py:   ",".join(items)
来源：http://wid.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://eik.tanke756.top

JS:   items.join(",")
来源：http://lmw.snrcjt.cn

TS:   items.join(",")
来源：http://esq.ehwqpu.com

Java: String.join(",", items)
来源：http://sfd.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://bco.daria6918.cn

Ruby: items.join(",")
来源：http://gxz.yonumen.top

C#:   string.Join(",", items)
来源：http://zzo.jyoumei.cn

[E09] 去除所有空白字符
来源：http://dzh.jinyuanbaomall.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yvc.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bib.jiagoushi.top

JS:   s.replace(/\s+/g, "")
来源：http://pjp.gogol.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://pgz.tianlin.xyz

Java: s.replaceAll("\\s+", "")
来源：http://ncm.xuetiantiany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://muf.ehwqpu.com

Ruby: s.gsub(/\s+/, "")
来源：http://uzv.sweek.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ldj.yuanzhike.top

[E10] 左侧补零 / 定长填充
来源：http://jbx.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hof.sjlbkw.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rtk.fktsv.cn

JS:   "7".padStart(3, "0")
来源：http://uts.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://xbb.316326.xyz

Java: String.format("%03d", 7)
来源：http://vqi.hnqzz.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gqf.svipenyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wjr.svipenyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hnr.havefunace.top

[E11] 反转字符串
来源：http://dsw.nanxinkj.top

Py:   s[::-1]
来源：http://oas.hesvh.cn

PHP:  strrev($s);
来源：http://stg.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://jay.pycfn.com

TS:   [...s].reverse().join("")
来源：http://kth.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://maq.zhixingplan.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jhw.zhixingplan.top

Ruby: s.reverse
来源：http://qms.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://imd.cucudq.cn

[E12] 统计某字符出现次数
来源：http://bkg.cucudq.cn

Py:   s.count("a")
来源：http://mlj.316326.xyz

PHP:  substr_count($s, "a");
来源：http://vnx.ivvv.top

JS:   s.split("a").length - 1
来源：http://ukz.zhiwuduotai.top

TS:   s.split("a").length - 1
来源：http://jkj.hongshengwenyu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://plm.aibaodan.cn

Go:   strings.Count(s, "a")
来源：http://ric.sufxvd.cn

Ruby: s.count("a")
来源：http://hhs.sjlbkw.cn

C#:   s.Count(c => c == 'a')
来源：http://vys.tarul.cn

[E13] 逐字符遍历
来源：http://cme.nanxuanxn.top

Py:   for ch in s: print(ch)
来源：http://ikj.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cpi.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fdk.ppjwa.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ccz.hongshengwenyu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zfl.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qnr.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fje.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wfx.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://vvk.jianghu66.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iys.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ncb.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ese.shanyushiyangtech.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ejm.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://khj.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xgj.aizwys.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xtl.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blc.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://hhu.gotoacloud.top

Py:   html.escape(s);  html.unescape(s)
来源：http://daj.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ydf.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fuk.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wgs.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jvd.cdnleiting.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://onf.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hgf.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cma.fktsv.cn

[E16] 数字千分位
来源：http://gnp.ybcxt.top

Py:   f"{1234567:,}"
来源：http://rhq.yueranfly.top

PHP:  number_format(1234567);
来源：http://cnj.uphjek.com

JS:   (1234567).toLocaleString("en-US")
来源：http://juo.vehdjk.com

TS:   (1234567).toLocaleString("en-US")
来源：http://onq.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://udo.quarkkingdee.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hly.hnqzz.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nhy.c1oappe.top

C#:   1234567.ToString("N0")
来源：http://pcb.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://fxf.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://siq.jinqigufen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://swb.wangdashe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wze.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ryo.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bty.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wsc.yuanzhike.top

Ruby: s.capitalize
来源：http://kre.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pam.yvedp.cn

[E18] 模板占位符替换
来源：http://bfd.nanxuanxn.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bkr.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://udv.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://caj.jyoumei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jai.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://und.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://htt.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iuc.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oih.cashguo.top

[E19] 多行文本按行拆分
来源：http://hwj.zhoulong.xyz

Py:   s.splitlines()
来源：http://bvo.tian-w.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dhr.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://pfh.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://ujf.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://bnz.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://fdr.0kj1m.cn


<!-- 参考信息 -->