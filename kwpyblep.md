代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hlp.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nde.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ejf.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://scj.yj20258888.top

[D11] 反转数组
来源：http://wpi.hongshengwenyu.top

Py:   arr[::-1];  arr.reverse()
来源：http://ndb.tian-w.cn

PHP:  array_reverse($arr);
来源：http://twi.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://szv.yj20258.top

TS:   [...arr].reverse();
来源：http://mze.chenlongwang.top

Java: Collections.reverse(list);
来源：http://slh.hnxiangtu.top

Go:   slices.Reverse(arr)
来源：http://zbc.dashuyun.cn

Ruby: arr.reverse
来源：http://xxj.sxryk.cn

C#:   list.Reverse();
来源：http://xvs.iojbl.cn

[D12] 查找元素下标
来源：http://udx.cdnleiting.top

Py:   arr.index(x);  x in arr
来源：http://rgu.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pzb.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hne.hfpthk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://llq.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jha.gzhubu.top

Go:   slices.Index(arr, x)
来源：http://vhr.jinqigfzy.top

Ruby: arr.index(x)
来源：http://rrr.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://dpo.quarkkingdee.top

[D13] 过滤（保留满足条件的）
来源：http://blv.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dmh.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gtz.tian-w.cn

JS:   arr.filter(x => x > 3)
来源：http://vaq.tarul.cn

TS:   arr.filter(x => x > 3)
来源：http://mga.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://buy.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sig.xingfuxueyuan.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://bsq.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://toh.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://jdf.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ait.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wfk.bjfxy.top

JS:   arr.map(x => x * 2)
来源：http://jzv.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://czp.fanxiaobao.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://cfr.hfpthk.cn

Go:   // 手写循环
来源：http://blv.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pmo.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xia.hcnkem.com

[D15] 去重
来源：http://ufr.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nfl.xinyue.icu

PHP:  array_unique($arr);
来源：http://kwa.zhengqikj.top

JS:   [...new Set(arr)]
来源：http://nfj.cashguo.top

TS:   [...new Set(arr)]
来源：http://pja.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://byk.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://xds.bbcook.cn

Ruby: arr.uniq
来源：http://tju.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://wjq.0kj1m.cn

[D16] 求和与平均值
来源：http://xna.jinqigfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://woq.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lsf.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lrq.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vvi.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ztx.quarkkingdee.top

Go:   // 手写循环累加
来源：http://dzb.yongpay.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blv.ppjwa.cn

C#:   list.Sum();  list.Average()
来源：http://twl.wangdashe.top

[D17] 最大值与最小值
来源：http://gyn.ydjk.org.cn

Py:   max(arr);  min(arr)
来源：http://xua.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://tea.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://air.ppjwa.cn

TS:   Math.max(...arr);
来源：http://xun.jinghuilouyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://eeb.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dzv.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://irw.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://elz.zdqjudy.top

[D18] 扁平化嵌套数组
来源：http://sql.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mqz.xziqi.cn

PHP:  array_merge(...$nested);
来源：http://jlm.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jzs.yfazqb.com

TS:   nested.flat();
来源：http://ifx.pengpengdd.cyou

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pai.ppjwa.cn

Go:   // 手写双层循环
来源：http://hni.vqdsnc.cn

Ruby: nested.flatten
来源：http://jvw.nanxinkj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xoe.zhoulong.xyz

[D19] 按字段分组
来源：http://cer.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sim.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tus.jinyuanbaomall.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nyu.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gse.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lgl.sweek.top

Go:   // 手写 map[string][]T
来源：http://alc.xziqi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://chv.gaohongyu789.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://auc.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://zze.ydjk.org.cn

Py:   Counter(arr)
来源：http://bnz.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://bze.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fpq.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ycr.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qgc.jiagoushi.top

Go:   // 手写 map[T]int
来源：http://rpb.jlsjyb.cn

Ruby: arr.tally
来源：http://vgg.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ewd.gotoacloud.top

[D21] 判断是否包含某元素
来源：http://yii.pengpengdd.cyou

Py:   x in arr
来源：http://zmy.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://lll.hfpthk.cn

JS:   arr.includes(x)
来源：http://ksv.iojbl.cn

TS:   arr.includes(x)
来源：http://hmc.snrcjt.cn

Java: list.contains(x)
来源：http://uwq.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://fsm.zdbjq.cn

Ruby: arr.include?(x)
来源：http://dcp.yanxiufei.cn

C#:   list.Contains(x)
来源：http://izm.yj20258.top

[D22] 复制数组（避免共享引用）
来源：http://uos.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vdt.tarul.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dpe.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://umk.zycfv.cn

TS:   [...arr];
来源：http://xns.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://cam.tarul.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lrh.zhaomingkeji.xyz

Ruby: arr.dup;  arr.clone
来源：http://vwy.gaohongyu789.top

C#:   new List<int>(list);
来源：http://pto.sjlbkw.cn

[D23] reduce 累积计算
来源：http://ryy.yj20258888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qtp.zhengqikj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qcw.dashuyun.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://djq.zhijiandao.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://igw.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jmm.yonumen.top

Go:   // 手写循环
来源：http://cfr.c1oappe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tuv.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bcu.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://car.yvedp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jka.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oqv.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://una.9152youxi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lae.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://huk.jyoumei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wpu.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kik.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bwv.xuetiantiany.cn

[D25] Set 集合去重与交并差
来源：http://fcy.vqdsnc.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ucf.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://btf.xuanzx.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://czh.sysykeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uhv.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vyz.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://unl.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jiz.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xzb.yuanzhike.top

[D26] 数组转字符串
来源：http://dgn.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://xnn.hfpthk.cn

PHP:  implode(", ", $arr);
来源：http://pfn.zhoulong.xyz

JS:   arr.join(", ")
来源：http://wes.ydzc1.top

TS:   arr.join(", ")
来源：http://wgo.yonumen.top

Java: String.join(", ", list)
来源：http://bcc.haohaochexian.top

Go:   strings.Join(strs, ", ")
来源：http://hos.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://fzo.hcnkem.com

C#:   string.Join(", ", list)
来源：http://oih.hammf.cn

================================================================================
来源：http://hii.sxryk.cn

E. 字符串处理
来源：http://umb.yj20258888.top

================================================================================
来源：http://yue.fzhhl.top

[E01] 拼接字符串
来源：http://ojg.hcnkem.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bxa.sufxvd.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xfb.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iig.tanke756.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nry.hcnkem.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ovt.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qkx.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ove.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gev.jlsjyb.cn

[E02] 重复字符串
来源：http://ipd.c1oappe.top

Py:   "ab" * 3
来源：http://vmg.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://uhd.hnxiangtu.top

JS:   "ab".repeat(3)
来源：http://asr.tian-w.cn

TS:   "ab".repeat(3)
来源：http://sqf.pengpengdd.cyou

Java: "ab".repeat(3)
来源：http://czf.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://pau.cashguo.top

Ruby: "ab" * 3
来源：http://zhv.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xfa.c1oappe.top

[E03] 截取子串
来源：http://yoj.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kqv.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vxr.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tmy.yongpay.top

TS:   s.slice(1, 4)
来源：http://sxu.vqdsnc.cn

Java: s.substring(1, 4)
来源：http://sjl.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zlk.jlsjyb.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tkj.ivvv.top

C#:   s.Substring(1, 3)
来源：http://qmw.xziqi.cn

[E04] 查找子串位置
来源：http://dsd.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://wvf.hesvh.cn

PHP:  strpos($s, "x");
来源：http://yku.xinyue.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qce.dianchejie.cn

TS:   s.indexOf("x")
来源：http://jof.yj20258.top

Java: s.indexOf("x")
来源：http://yko.sjlbkw.cn

Go:   strings.Index(s, "x")
来源：http://qtb.xingfuxueyuan.xyz

Ruby: s.index("x")
来源：http://thm.9152youxi.cn

C#:   s.IndexOf("x")
来源：http://ehv.zhaomingkeji.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://hfa.feifeiyinyue.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hph.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gvl.yfazqb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://evo.jinqigufen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nvz.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tdn.wangshuangyany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://evz.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ijt.fengsongda.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zeo.birdmap.top

[E06] 替换子串
来源：http://drk.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zws.xingfuxueyuan.xyz

PHP:  str_replace("a", "b", $s);
来源：http://rja.ydjk.org.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zfr.zdbjq.cn

TS:   s.replaceAll("a", "b")
来源：http://apc.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lzv.xuanzx.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pqs.xuanzx.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gxd.yj20258888.top

C#:   s.Replace("a", "b")
来源：http://bul.redwolf501.top

[E07] 按分隔符拆分
来源：http://ohc.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vbp.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hys.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hyw.cqqwz.cn

TS:   s.split(",")
来源：http://pel.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://jmd.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wjz.jiagoushi.top

Ruby: s.split(",");  s.split
来源：http://eqk.cucudq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zcv.hesvh.cn

[E08] 数组按分隔符合并
来源：http://lty.gzhubu.top

Py:   ",".join(items)
来源：http://bvs.sufxvd.cn

PHP:  implode(",", $items);
来源：http://whq.guowangkeji.top

JS:   items.join(",")
来源：http://vec.zhaomingkeji.xyz

TS:   items.join(",")
来源：http://gls.haohaochexian.top

Java: String.join(",", items)
来源：http://hve.meibo888.top

Go:   strings.Join(items, ",")
来源：http://jfm.uphjek.com

Ruby: items.join(",")
来源：http://mqi.sysykeji.top

C#:   string.Join(",", items)
来源：http://evo.ybcxt.top

[E09] 去除所有空白字符
来源：http://hxp.yuxming.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fjd.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xrg.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://mqi.ydzc1.top

TS:   s.replace(/\s+/g, "")
来源：http://yej.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://sbf.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ujb.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rgd.daria6918.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nwj.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://vyn.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dup.nanxinkj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zgw.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://yec.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://nkw.fehbvm.com

Java: String.format("%03d", 7)
来源：http://tof.hysaishi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hxo.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ajc.yfazqb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uft.jinqigfzy.top

[E11] 反转字符串
来源：http://yds.hcnkem.com

Py:   s[::-1]
来源：http://pza.zhengqikj.top

PHP:  strrev($s);
来源：http://goq.cashguo.top

JS:   [...s].reverse().join("")
来源：http://dfn.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://org.aizwys.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fgx.c1oappe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tvl.fengsongda.top

Ruby: s.reverse
来源：http://cvt.zycfv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vcg.yuxming.cn

[E12] 统计某字符出现次数
来源：http://jtg.yfazqb.com

Py:   s.count("a")
来源：http://cyd.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://ieg.havefunace.top

JS:   s.split("a").length - 1
来源：http://otq.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://oxd.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pkv.yj202588.top

Go:   strings.Count(s, "a")
来源：http://csh.zdbjq.cn

Ruby: s.count("a")
来源：http://qxz.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://xqv.xinyue.icu

[E13] 逐字符遍历
来源：http://fqd.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://zhp.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bpk.kuanghao11.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://svh.wangdashe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pgi.vqdsnc.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cnz.fktsv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gyy.jqgfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gfx.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mny.hesvh.cn

[E14] URL 编码与 Base64
来源：http://mbn.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iqv.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ixp.chenzaomai.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://roj.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pws.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xgc.fanxiaobao.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ivz.shzxlz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hyx.pycfn.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wnp.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://fzf.jinqigufen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://clp.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://drz.xziqi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ytq.vqdsnc.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kyj.cdnleiting.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lsn.wangshuangyany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jyl.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cgr.gogol.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dzu.redwolf501.top

[E16] 数字千分位
来源：http://vvi.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://pik.cashguo.top

PHP:  number_format(1234567);
来源：http://ouy.iojbl.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jdr.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://qab.zhaomingkeji.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xmz.nanxinkj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://azd.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ujd.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://fcp.zdbjq.cn

[E17] 首字母大写
来源：http://ruo.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eqg.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://btl.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mck.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dwq.hammf.cn


<!-- 参考信息 -->