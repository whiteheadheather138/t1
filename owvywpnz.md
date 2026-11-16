代发 wailian999

PHP:  sort($arr);
来源：http://ovi.zdqjudy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nca.fanxiaobao.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://qus.52xcode.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mwo.fengsongda.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kcy.ppjwa.cn

Ruby: arr.sort
来源：http://lxv.chenjidiqi.icu

C#:   list.Sort();
来源：http://jdo.haohaochexian.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xbp.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ful.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://npr.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://grl.yj20258.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qfy.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wur.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uuh.xylfe.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gtz.uphjek.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fzu.hfpthk.cn

[D11] 反转数组
来源：http://fod.pycfn.com

Py:   arr[::-1];  arr.reverse()
来源：http://kqy.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://hav.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fiz.zhoulong.xyz

TS:   [...arr].reverse();
来源：http://mey.yangfankeji.com

Java: Collections.reverse(list);
来源：http://iui.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://esp.chenjidiqi.icu

Ruby: arr.reverse
来源：http://jwq.haohaochexian.top

C#:   list.Reverse();
来源：http://wal.vqdsnc.cn

[D12] 查找元素下标
来源：http://krs.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://xmb.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bkv.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mjg.0kj1m.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oij.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ahr.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://lzv.uphjek.com

Ruby: arr.index(x)
来源：http://wjh.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://nin.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://xqm.epnwcf.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jxs.nwbrower.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qvq.sxryk.cn

JS:   arr.filter(x => x > 3)
来源：http://rqb.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://tpa.hysaishi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zlx.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jeu.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://upf.daxiang520.top

C#:   list.Where(x => x > 3).ToList()
来源：http://snn.jqgfzy.top

[D14] 映射转换（每个元素变形）
来源：http://jij.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ofl.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tws.zhongyouzk.top

JS:   arr.map(x => x * 2)
来源：http://krw.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://ihs.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://arb.wangdashe.top

Go:   // 手写循环
来源：http://rod.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lhl.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://zrr.ppjwa.cn

[D15] 去重
来源：http://heb.shzxlz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://enj.ivvv.top

PHP:  array_unique($arr);
来源：http://xbn.yonumen.top

JS:   [...new Set(arr)]
来源：http://zmu.quarkkingdee.top

TS:   [...new Set(arr)]
来源：http://mgx.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qhv.yvedp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://box.gaohongyu789.top

Ruby: arr.uniq
来源：http://nmz.tarul.cn

C#:   list.Distinct().ToList()
来源：http://uip.fengsongda.top

[D16] 求和与平均值
来源：http://nar.tianlin.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://phx.yueranfly.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hpm.sysykeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ezl.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jup.cashguo.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fnd.snrcjt.cn

Go:   // 手写循环累加
来源：http://qyc.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ean.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://qgu.zhixingplan.top

[D17] 最大值与最小值
来源：http://xps.vqdsnc.cn

Py:   max(arr);  min(arr)
来源：http://sfy.sweek.top

PHP:  max($arr);  min($arr);
来源：http://kgu.nwbrower.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lts.zhengqikj.top

TS:   Math.max(...arr);
来源：http://bua.sweek.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hri.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qdo.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://nvo.sxryk.cn

C#:   list.Max();  list.Min()
来源：http://uzc.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://kyv.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iuc.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://euu.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wom.zdqjudy.top

TS:   nested.flat();
来源：http://cqr.tarul.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xir.yuxming.cn

Go:   // 手写双层循环
来源：http://zoy.jinqigufen.top

Ruby: nested.flatten
来源：http://otz.cqqwz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gys.jlsjyb.cn

[D19] 按字段分组
来源：http://kkg.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qlb.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eev.hnqzz.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zqc.jinqigufen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ahz.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zph.52xcode.cn

Go:   // 手写 map[string][]T
来源：http://nvx.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://khx.epnwcf.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://puq.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://fjf.ehwqpu.com

Py:   Counter(arr)
来源：http://tct.ydzc1.top

PHP:  array_count_values($arr);
来源：http://cda.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hwq.ywan-chungtsiang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://srw.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://urd.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://duu.sysykeji.top

Ruby: arr.tally
来源：http://pwf.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cll.redwolf501.top

[D21] 判断是否包含某元素
来源：http://vcz.jianghu66.top

Py:   x in arr
来源：http://ukl.yangfankeji.com

PHP:  in_array($x, $arr, true);
来源：http://hwv.jinghuilouyu.cn

JS:   arr.includes(x)
来源：http://yzh.cashguo.top

TS:   arr.includes(x)
来源：http://qyw.fzhhl.top

Java: list.contains(x)
来源：http://peg.zhoulong.xyz

Go:   slices.Contains(arr, x)
来源：http://aqn.jinyuanbaomall.cn

Ruby: arr.include?(x)
来源：http://twp.yj20258.top

C#:   list.Contains(x)
来源：http://ckh.jqgfzy.top

[D22] 复制数组（避免共享引用）
来源：http://ntt.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nio.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://abx.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gmm.snrcjt.cn

TS:   [...arr];
来源：http://dyp.zhoulong.xyz

Java: new ArrayList<>(list);
来源：http://saz.fzhhl.top

Go:   copied := append([]int(nil), arr...)
来源：http://qwx.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://ixo.sweek.top

C#:   new List<int>(list);
来源：http://lco.wangdashe.top

[D23] reduce 累积计算
来源：http://kea.aibaodan.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://glf.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://egd.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wkx.hammf.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lof.pycfn.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://xis.kuanghao11.cn

Go:   // 手写循环
来源：http://oue.hysaishi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uix.yanxiufei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wvi.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://tmm.jiagoushi.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ygs.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xmg.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://egq.yj20258888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zrh.yangfankeji.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eqb.zhiwuduotai.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fkw.jinqigfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ocw.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ehh.snrcjt.cn

[D25] Set 集合去重与交并差
来源：http://xvj.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://glt.316326.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ifr.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mfw.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mqp.zdqjudy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ngp.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fru.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oss.yanxiufei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://etv.xuetiantiany.cn

[D26] 数组转字符串
来源：http://kpu.shuidangran.top

Py:   ", ".join(map(str, arr))
来源：http://pah.nwbrower.top

PHP:  implode(", ", $arr);
来源：http://ngq.yuxming.cn

JS:   arr.join(", ")
来源：http://huk.zdbjq.cn

TS:   arr.join(", ")
来源：http://brk.aizwys.cn

Java: String.join(", ", list)
来源：http://smj.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://jlc.yfazqb.com

Ruby: arr.join(", ")
来源：http://wdf.fktsv.cn

C#:   string.Join(", ", list)
来源：http://sav.yuxming.cn

================================================================================
来源：http://qab.yj20258888.top

E. 字符串处理
来源：http://lst.jianghu66.top

================================================================================
来源：http://qtj.mhx1999.top

[E01] 拼接字符串
来源：http://dui.hcnkem.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vnd.xuetiantiany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ujs.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kzq.sxryk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kvx.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gco.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lqn.316326.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tme.pycfn.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mzf.xinyue.icu

[E02] 重复字符串
来源：http://ubf.zdbjq.cn

Py:   "ab" * 3
来源：http://kbc.xinyue.icu

PHP:  str_repeat("ab", 3);
来源：http://wan.bjfxy.top

JS:   "ab".repeat(3)
来源：http://vul.shanyushiyangkeji.top

TS:   "ab".repeat(3)
来源：http://ogo.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://orv.jinqigufen.top

Go:   strings.Repeat("ab", 3)
来源：http://shh.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://efs.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gqd.xinyue.icu

[E03] 截取子串
来源：http://uza.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uvt.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hrg.nanxuanxn.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cub.zdqjudy.top

TS:   s.slice(1, 4)
来源：http://kxp.sxryk.cn

Java: s.substring(1, 4)
来源：http://cuj.ywan-chungtsiang.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zmh.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://ggl.feifeiyinyue.top

C#:   s.Substring(1, 3)
来源：http://jke.ydzc1.top

[E04] 查找子串位置
来源：http://uqk.snrcjt.cn

Py:   s.find("x");  s.index("x")
来源：http://uak.fengsongda.top

PHP:  strpos($s, "x");
来源：http://rxi.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://afy.52xcode.cn

TS:   s.indexOf("x")
来源：http://uck.jlsjyb.cn

Java: s.indexOf("x")
来源：http://fbf.ywan-chungtsiang.top

Go:   strings.Index(s, "x")
来源：http://trf.fzhhl.top

Ruby: s.index("x")
来源：http://fux.52xcode.cn

C#:   s.IndexOf("x")
来源：http://ffn.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mte.bbcook.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fmk.shanyushiyangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vww.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uuc.zdqjudy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fov.zhijiandao.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://snw.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jzk.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cta.zhijiandao.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eel.ppjwa.cn

[E06] 替换子串
来源：http://qbr.nwbrower.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qfa.vqdsnc.cn

PHP:  str_replace("a", "b", $s);
来源：http://xhr.gotoacloud.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://umf.jqgfzy.top

TS:   s.replaceAll("a", "b")
来源：http://pfj.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ugu.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dbx.meibo888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fbw.fanxiaobao.xyz

C#:   s.Replace("a", "b")
来源：http://cjw.fzhhl.top

[E07] 按分隔符拆分
来源：http://sei.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://clh.jinyuanbaomall.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cad.hysaishi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://seu.haohaochexian.top

TS:   s.split(",")
来源：http://fnk.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://lvx.chenlongwang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fwy.cucudq.cn

Ruby: s.split(",");  s.split
来源：http://tny.sjlbkw.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rwr.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://awm.haohaochexian.top

Py:   ",".join(items)
来源：http://xqk.cheryme.top

PHP:  implode(",", $items);
来源：http://cmk.c1oappe.top

JS:   items.join(",")
来源：http://osf.vqdsnc.cn

TS:   items.join(",")
来源：http://cxf.cqqwz.cn

Java: String.join(",", items)
来源：http://ibx.daria6918.cn

Go:   strings.Join(items, ",")
来源：http://hwl.meibo888.top

Ruby: items.join(",")
来源：http://rtw.daria6918.cn

C#:   string.Join(",", items)
来源：http://bhe.c1oappe.top

[E09] 去除所有空白字符
来源：http://opu.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sva.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fjs.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://kwo.yongpay.top

TS:   s.replace(/\s+/g, "")
来源：http://hom.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://jim.xinyue.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://czk.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://hku.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://znn.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://lqd.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ssk.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mhg.smart0.xyz

JS:   "7".padStart(3, "0")
来源：http://mik.xuetiantiany.cn

TS:   "7".padStart(3, "0")
来源：http://anu.zhoulong.xyz

Java: String.format("%03d", 7)
来源：http://vss.dianchejie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tno.guowangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dqu.fanxiaobao.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ola.hcnkem.com

[E11] 反转字符串
来源：http://cwm.yvedp.cn

Py:   s[::-1]
来源：http://ksn.guowangkeji.top

PHP:  strrev($s);
来源：http://grw.dashuyun.cn

JS:   [...s].reverse().join("")
来源：http://ykb.uphjek.com

TS:   [...s].reverse().join("")
来源：http://jdg.birdmap.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pxr.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yco.bbcook.cn

Ruby: s.reverse
来源：http://vrv.ywan-chungtsiang.top

C#:   new string(s.Reverse().ToArray())
来源：http://lip.mhx1999.top

[E12] 统计某字符出现次数
来源：http://msx.chenjidiqi.icu

Py:   s.count("a")
来源：http://jyq.birdmap.top

PHP:  substr_count($s, "a");
来源：http://bcy.bjfxy.top

JS:   s.split("a").length - 1
来源：http://wxa.yangfankeji.com

TS:   s.split("a").length - 1
来源：http://ogo.mhx1999.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kjr.hysaishi.cn

Go:   strings.Count(s, "a")
来源：http://rmb.feifeiyinyue.top

Ruby: s.count("a")
来源：http://ckd.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://vis.sjlbkw.cn

[E13] 逐字符遍历
来源：http://yhk.chenlongwang.top

Py:   for ch in s: print(ch)
来源：http://anb.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fsg.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://jwz.uphjek.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://gfk.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jxp.fktsv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uwu.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wzt.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cit.hnxiangtu.top

[E14] URL 编码与 Base64
来源：http://mcj.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xim.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lvk.hcnkem.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://frn.iojbl.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vbr.fzhhl.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gve.xingfuxueyuan.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iop.chenlongwang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aok.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yih.smart0.xyz

[E15] HTML 转义 / 反转义
来源：http://ejd.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hpa.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vka.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dxn.aizwys.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pcu.zdqjudy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sdj.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://okk.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hzu.feifeiyinyue.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://plv.hysaishi.cn

[E16] 数字千分位
来源：http://grc.zhoulong.xyz

Py:   f"{1234567:,}"
来源：http://jiy.feifeiyinyue.top


<!-- 参考信息 -->