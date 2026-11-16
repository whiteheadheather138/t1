代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mlf.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fte.zhengqikj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mdw.tianlin.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hrg.redwolf501.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://soa.jinqigfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sps.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dyk.iojbl.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vnv.hesvh.cn

[D11] 反转数组
来源：http://jpy.mhx1999.top

Py:   arr[::-1];  arr.reverse()
来源：http://fkv.nanxuanxn.top

PHP:  array_reverse($arr);
来源：http://hik.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lgy.pengpengdd.cyou

TS:   [...arr].reverse();
来源：http://oli.0kj1m.cn

Java: Collections.reverse(list);
来源：http://wrp.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://vzf.xuanzx.com

Ruby: arr.reverse
来源：http://hxx.guowangkeji.top

C#:   list.Reverse();
来源：http://ahh.fktsv.cn

[D12] 查找元素下标
来源：http://wfr.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://cns.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zcf.hammf.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qal.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pky.yj202588.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ezs.cashguo.top

Go:   slices.Index(arr, x)
来源：http://vnp.tianlin.xyz

Ruby: arr.index(x)
来源：http://sbn.shuidangran.top

C#:   list.IndexOf(x);
来源：http://qay.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://bdc.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tkj.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nxa.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://ebz.cheryme.top

TS:   arr.filter(x => x > 3)
来源：http://zaf.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nir.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ozn.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://ddd.hywenlv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dlr.shangyingyoupin.top

[D14] 映射转换（每个元素变形）
来源：http://spq.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://geg.yfazqb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jbo.jinqigufen.top

JS:   arr.map(x => x * 2)
来源：http://auc.cheryme.top

TS:   arr.map(x => x * 2)
来源：http://hbr.hnxiangtu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ufq.ctjpmb.com

Go:   // 手写循环
来源：http://qfq.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://eml.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://bkw.yj202588.top

[D15] 去重
来源：http://uvw.hnqzz.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vwl.ywan-chungtsiang.top

PHP:  array_unique($arr);
来源：http://irj.shuidangran.top

JS:   [...new Set(arr)]
来源：http://lpe.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://got.zhixingplan.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ony.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://gao.chenlongwang.top

Ruby: arr.uniq
来源：http://ogp.tian-w.cn

C#:   list.Distinct().ToList()
来源：http://yho.guowangkeji.top

[D16] 求和与平均值
来源：http://bmp.jinyuanbaomall.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tvq.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eop.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ybo.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mma.hywenlv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zlv.aibaodan.cn

Go:   // 手写循环累加
来源：http://mne.zhixingplan.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ihb.ctjpmb.com

C#:   list.Sum();  list.Average()
来源：http://giq.guowangkeji.top

[D17] 最大值与最小值
来源：http://gge.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://kbb.ppjwa.cn

PHP:  max($arr);  min($arr);
来源：http://qlf.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vqa.ydzc1.top

TS:   Math.max(...arr);
来源：http://hac.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ius.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cia.nanxuanxn.top

Ruby: arr.max;  arr.min
来源：http://uzm.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://mpq.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://aua.gogol.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ozv.hammf.cn

PHP:  array_merge(...$nested);
来源：http://hps.tanke756.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ugt.cqqwz.cn

TS:   nested.flat();
来源：http://sln.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sfl.sjlbkw.cn

Go:   // 手写双层循环
来源：http://ygc.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://yxj.tanke756.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fhd.snrcjt.cn

[D19] 按字段分组
来源：http://nrh.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://try.yanxiufei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aiu.gogol.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vhw.jinqigufen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dxa.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dig.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://tdr.hnxiangtu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dve.shanyushiyangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rne.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://vvb.zhijiandao.cn

Py:   Counter(arr)
来源：http://kiu.bjfxy.top

PHP:  array_count_values($arr);
来源：http://gae.wangdashe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zwm.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dya.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lwq.yuxming.cn

Go:   // 手写 map[T]int
来源：http://wic.cashguo.top

Ruby: arr.tally
来源：http://sde.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ssg.shzxlz.cn

[D21] 判断是否包含某元素
来源：http://rtv.xinyue.icu

Py:   x in arr
来源：http://pcs.sjlbkw.cn

PHP:  in_array($x, $arr, true);
来源：http://fzq.wangshuangyany.cn

JS:   arr.includes(x)
来源：http://uso.shzxlz.cn

TS:   arr.includes(x)
来源：http://mtb.yuxming.cn

Java: list.contains(x)
来源：http://emy.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://lqp.9152youxi.cn

Ruby: arr.include?(x)
来源：http://njg.birdmap.top

C#:   list.Contains(x)
来源：http://vtj.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://lsr.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ipj.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://foh.sufxvd.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zyl.chenzaomai.com

TS:   [...arr];
来源：http://vid.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://cnu.yj202588.top

Go:   copied := append([]int(nil), arr...)
来源：http://fic.shanyushiyangtech.top

Ruby: arr.dup;  arr.clone
来源：http://bda.sweek.top

C#:   new List<int>(list);
来源：http://wxl.jiagoushi.top

[D23] reduce 累积计算
来源：http://bfn.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lwa.hfpthk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gta.pengpengdd.cyou

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://llu.sufxvd.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nzs.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ecb.sjlbkw.cn

Go:   // 手写循环
来源：http://ikz.ppjwa.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zlf.jinqigfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cqm.cqqwz.cn

[D24] 字典 / Map 基本操作
来源：http://kbk.yj20258.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ojl.daxiang520.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wrr.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xcg.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dii.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zrt.wangdashe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fhf.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pqe.0kj1m.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zts.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://nhs.pycfn.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xkn.yongpay.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qbx.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kcq.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gyq.tarul.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eyk.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://boa.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dcg.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rix.vehdjk.com

[D26] 数组转字符串
来源：http://mle.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://xot.yj202588.top

PHP:  implode(", ", $arr);
来源：http://nhr.chenjidiqi.icu

JS:   arr.join(", ")
来源：http://jtt.vqdsnc.cn

TS:   arr.join(", ")
来源：http://ibp.tian-w.cn

Java: String.join(", ", list)
来源：http://noq.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://ibp.fzhhl.top

Ruby: arr.join(", ")
来源：http://gbf.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://mgc.hesvh.cn

================================================================================
来源：http://gce.ctjpmb.com

E. 字符串处理
来源：http://jbd.zdqjudy.top

================================================================================
来源：http://lpb.gaohongyu789.top

[E01] 拼接字符串
来源：http://vbr.yuxming.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eku.zhiwuduotai.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bet.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cch.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://agc.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vzu.ywan-chungtsiang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nhm.yangfankeji.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tud.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://owa.fanxiaobao.xyz

[E02] 重复字符串
来源：http://hfj.jqgfzy.top

Py:   "ab" * 3
来源：http://bcd.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://yta.xuanzx.com

JS:   "ab".repeat(3)
来源：http://maf.andypj.xyz

TS:   "ab".repeat(3)
来源：http://qmz.ybcxt.top

Java: "ab".repeat(3)
来源：http://ywh.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://cfu.zhoulong.xyz

Ruby: "ab" * 3
来源：http://poo.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qyq.ppjwa.cn

[E03] 截取子串
来源：http://tii.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rla.yongpay.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qlz.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pki.birdmap.top

TS:   s.slice(1, 4)
来源：http://fdy.guannengcc.top

Java: s.substring(1, 4)
来源：http://xzv.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zfb.aizwys.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lqi.pycfn.com

C#:   s.Substring(1, 3)
来源：http://ive.bjfxy.top

[E04] 查找子串位置
来源：http://lrr.ybcxt.top

Py:   s.find("x");  s.index("x")
来源：http://tib.sjlbkw.cn

PHP:  strpos($s, "x");
来源：http://vjr.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bho.cashguo.top

TS:   s.indexOf("x")
来源：http://plm.fktsv.cn

Java: s.indexOf("x")
来源：http://qgh.hcnkem.com

Go:   strings.Index(s, "x")
来源：http://idv.vqdsnc.cn

Ruby: s.index("x")
来源：http://gdc.yfazqb.com

C#:   s.IndexOf("x")
来源：http://sse.vehdjk.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://zcu.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://alp.hongshengwenyu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://teb.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zgi.xuanzx.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://nfv.aizwys.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jsq.chenzaomai.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xxv.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://chl.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xar.zhoulong.xyz

[E06] 替换子串
来源：http://lol.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qql.chenjidiqi.icu

PHP:  str_replace("a", "b", $s);
来源：http://jzl.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ckp.ppjwa.cn

TS:   s.replaceAll("a", "b")
来源：http://ojb.xingfuxueyuan.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wqj.ybcxt.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zqt.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jeu.fengsongda.top

C#:   s.Replace("a", "b")
来源：http://pip.jyoumei.cn

[E07] 按分隔符拆分
来源：http://knm.zhoulong.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aql.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vnw.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lrj.tanke756.top

TS:   s.split(",")
来源：http://afw.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pmb.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uuk.jinqigfzy.top

Ruby: s.split(",");  s.split
来源：http://rgl.ppjwa.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tex.daxiang520.top

[E08] 数组按分隔符合并
来源：http://fhv.cdnleiting.top

Py:   ",".join(items)
来源：http://htt.snrcjt.cn

PHP:  implode(",", $items);
来源：http://ywv.ydjk.org.cn

JS:   items.join(",")
来源：http://pty.yuxming.cn

TS:   items.join(",")
来源：http://zln.zhaomingkeji.xyz

Java: String.join(",", items)
来源：http://idt.bjfxy.top

Go:   strings.Join(items, ",")
来源：http://jma.hfpthk.cn

Ruby: items.join(",")
来源：http://xzk.wangdashe.top

C#:   string.Join(",", items)
来源：http://zyi.birdmap.top

[E09] 去除所有空白字符
来源：http://ihc.xingfuxueyuan.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://czw.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ady.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://wui.hesvh.cn

TS:   s.replace(/\s+/g, "")
来源：http://bjq.yueranfly.top

Java: s.replaceAll("\\s+", "")
来源：http://qnu.jinqigfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bty.aibaodan.cn

Ruby: s.gsub(/\s+/, "")
来源：http://knq.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rst.hcnkem.com

[E10] 左侧补零 / 定长填充
来源：http://djl.zhijiandao.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gde.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mwg.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://jrc.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://sez.chenjidiqi.icu

Java: String.format("%03d", 7)
来源：http://psj.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mku.sufxvd.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nub.cashguo.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zwq.sxryk.cn

[E11] 反转字符串
来源：http://lsf.kuanghao11.cn

Py:   s[::-1]
来源：http://pzc.gotoacloud.top

PHP:  strrev($s);
来源：http://zfr.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://yxt.hnqzz.top

TS:   [...s].reverse().join("")
来源：http://hxf.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oyv.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kvm.havefunace.top

Ruby: s.reverse
来源：http://qvx.aibaodan.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wxo.vqdsnc.cn

[E12] 统计某字符出现次数
来源：http://yaa.sysykeji.top

Py:   s.count("a")
来源：http://tnz.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://sds.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://jfo.zdqjudy.top

TS:   s.split("a").length - 1
来源：http://jam.gogol.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zsl.xuetiantiany.cn

Go:   strings.Count(s, "a")
来源：http://hmj.ppjwa.cn

Ruby: s.count("a")
来源：http://osz.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://jgl.yuanzhike.top

[E13] 逐字符遍历
来源：http://qcw.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://mna.andypj.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cbe.yuxming.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://osr.gzhubu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hfa.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dmg.birdmap.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://obq.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://trr.yanxiufei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lbj.haohaochexian.top

[E14] URL 编码与 Base64
来源：http://auf.fzhhl.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://izy.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://xwc.ivvv.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uue.jinyuanbaomall.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rvp.jinqigufen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zrn.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bbc.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ole.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://imv.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://ttb.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yxi.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://huh.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bcb.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://iaf.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ktn.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nam.chenjidiqi.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eif.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ytw.jinghuilouyu.cn

[E16] 数字千分位
来源：http://bru.hongshengwenyu.top

Py:   f"{1234567:,}"
来源：http://fex.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://ezr.yj20258.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mnd.tian-w.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zcl.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://huj.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qhb.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jfz.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://opc.ehwqpu.com

[E17] 首字母大写
来源：http://zjb.hammf.cn


<!-- 参考信息 -->