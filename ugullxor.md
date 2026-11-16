代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ejg.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://amp.cashguo.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yud.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mif.yfazqb.com

[D11] 反转数组
来源：http://vzu.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://yqs.yj202588.top

PHP:  array_reverse($arr);
来源：http://qoi.jiagoushi.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xjl.quarkkingdee.top

TS:   [...arr].reverse();
来源：http://eud.9152youxi.cn

Java: Collections.reverse(list);
来源：http://dby.mhx1999.top

Go:   slices.Reverse(arr)
来源：http://ess.chenjidiqi.icu

Ruby: arr.reverse
来源：http://eng.fengsongda.top

C#:   list.Reverse();
来源：http://qpt.smart0.xyz

[D12] 查找元素下标
来源：http://gxa.chenjidiqi.icu

Py:   arr.index(x);  x in arr
来源：http://zij.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ptg.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rya.sxryk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aua.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mxx.yj20258.top

Go:   slices.Index(arr, x)
来源：http://dvd.wangdashe.top

Ruby: arr.index(x)
来源：http://uyb.shuidangran.top

C#:   list.IndexOf(x);
来源：http://gpd.guannengcc.top

[D13] 过滤（保留满足条件的）
来源：http://zng.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://azx.xinyue.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ovr.vqdsnc.cn

JS:   arr.filter(x => x > 3)
来源：http://ews.gzhubu.top

TS:   arr.filter(x => x > 3)
来源：http://fji.kuanghao11.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://czk.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ylg.daria6918.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lwr.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yxt.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://yto.yj20258888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://old.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gkq.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://jcf.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://egc.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gji.fktsv.cn

Go:   // 手写循环
来源：http://hno.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://vpi.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wbp.zdbjq.cn

[D15] 去重
来源：http://rwv.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iqh.hongshengwenyu.top

PHP:  array_unique($arr);
来源：http://phx.daxiang520.top

JS:   [...new Set(arr)]
来源：http://xqg.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://uzo.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hfn.sysykeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://btq.hnxiangtu.top

Ruby: arr.uniq
来源：http://mpq.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://tnj.aibaodan.cn

[D16] 求和与平均值
来源：http://ttk.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sdo.fanxiaobao.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hci.sysykeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pkt.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xqa.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dql.uphjek.com

Go:   // 手写循环累加
来源：http://lzk.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vrh.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://ths.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://jzc.xuanzx.com

Py:   max(arr);  min(arr)
来源：http://kcf.fktsv.cn

PHP:  max($arr);  min($arr);
来源：http://qzr.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fhi.gotoacloud.top

TS:   Math.max(...arr);
来源：http://ezp.redwolf501.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nnh.hongshengwenyu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xyw.fengsongda.top

Ruby: arr.max;  arr.min
来源：http://wsn.pycfn.com

C#:   list.Max();  list.Min()
来源：http://xzh.yongpay.top

[D18] 扁平化嵌套数组
来源：http://qvp.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qpz.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://hqm.yonumen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pgr.gotoacloud.top

TS:   nested.flat();
来源：http://jda.mhx1999.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sxz.fzhhl.top

Go:   // 手写双层循环
来源：http://zuo.fehbvm.com

Ruby: nested.flatten
来源：http://anq.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nkz.tanke756.top

[D19] 按字段分组
来源：http://dyv.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://orc.shanyushiyangtech.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eev.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ioc.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nbb.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vwy.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://ggh.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lwl.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://huk.jlsjyb.cn

[D20] 统计每个元素出现次数
来源：http://bqs.uphjek.com

Py:   Counter(arr)
来源：http://zih.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://saz.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rjo.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lmz.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lkp.mhx1999.top

Go:   // 手写 map[T]int
来源：http://nds.svipenyu.cn

Ruby: arr.tally
来源：http://web.cucudq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://drx.fktsv.cn

[D21] 判断是否包含某元素
来源：http://eqw.chenzaomai.com

Py:   x in arr
来源：http://enw.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://rth.xingfuxueyuan.xyz

JS:   arr.includes(x)
来源：http://bfc.xinyue.icu

TS:   arr.includes(x)
来源：http://jby.nanxinkj.top

Java: list.contains(x)
来源：http://opa.0kj1m.cn

Go:   slices.Contains(arr, x)
来源：http://rwf.bbcook.cn

Ruby: arr.include?(x)
来源：http://zwp.zhengqikj.top

C#:   list.Contains(x)
来源：http://kun.sjlbkw.cn

[D22] 复制数组（避免共享引用）
来源：http://wuo.jianghu66.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qco.mhx1999.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hrx.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rxn.birdmap.top

TS:   [...arr];
来源：http://ulc.sysykeji.top

Java: new ArrayList<>(list);
来源：http://xdh.gaohongyu789.top

Go:   copied := append([]int(nil), arr...)
来源：http://hwj.jinqigfzy.top

Ruby: arr.dup;  arr.clone
来源：http://our.hywenlv.cn

C#:   new List<int>(list);
来源：http://nze.hammf.cn

[D23] reduce 累积计算
来源：http://eyq.ydzc1.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tnk.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://luq.guannengcc.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hcj.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ttn.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://flf.jianghu66.top

Go:   // 手写循环
来源：http://uff.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jey.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nxb.jinyuanbaomall.cn

[D24] 字典 / Map 基本操作
来源：http://jah.bbcook.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jpq.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rte.ivvv.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uhv.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dkx.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eoe.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://puz.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kva.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qwr.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://won.zdbjq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gpd.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ter.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mlr.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kow.nanxuanxn.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cki.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fet.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vca.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uon.zdbjq.cn

[D26] 数组转字符串
来源：http://xbm.zhiwuduotai.top

Py:   ", ".join(map(str, arr))
来源：http://ptq.316326.xyz

PHP:  implode(", ", $arr);
来源：http://fee.jinghuilouyu.cn

JS:   arr.join(", ")
来源：http://ntf.yanxiufei.cn

TS:   arr.join(", ")
来源：http://pli.fktsv.cn

Java: String.join(", ", list)
来源：http://gqi.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://gqc.jinyuanbaomall.cn

Ruby: arr.join(", ")
来源：http://exl.shzxlz.cn

C#:   string.Join(", ", list)
来源：http://axx.ybcxt.top

================================================================================
来源：http://jpt.vqdsnc.cn

E. 字符串处理
来源：http://kcd.hysaishi.cn

================================================================================
来源：http://nia.0kj1m.cn

[E01] 拼接字符串
来源：http://uuu.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ixn.ybcxt.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vlv.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://krc.gaohongyu789.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://exp.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cee.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zaq.shzxlz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://otn.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cle.chenjidiqi.icu

[E02] 重复字符串
来源：http://jid.vehdjk.com

Py:   "ab" * 3
来源：http://xdb.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://blt.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://ojy.jqgufenzy.top

TS:   "ab".repeat(3)
来源：http://yyq.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://zcs.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://faj.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://kss.ppjwa.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qxd.hnqzz.top

[E03] 截取子串
来源：http://gsk.sxryk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lux.jqgfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lpa.c1oappe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dcd.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://oom.jiagoushi.top

Java: s.substring(1, 4)
来源：http://ieb.zhixingplan.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://whu.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ouh.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://efv.quarkkingdee.top

[E04] 查找子串位置
来源：http://cih.yuxming.cn

Py:   s.find("x");  s.index("x")
来源：http://koo.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://qhd.hywenlv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tmb.hongshengwenyu.top

TS:   s.indexOf("x")
来源：http://xmg.cheryme.top

Java: s.indexOf("x")
来源：http://som.bbcook.cn

Go:   strings.Index(s, "x")
来源：http://dnz.havefunace.top

Ruby: s.index("x")
来源：http://cyr.pengpengdd.cyou

C#:   s.IndexOf("x")
来源：http://yej.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bmn.fengsongda.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qdi.sxryk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fyl.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xbt.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ptz.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ega.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wmg.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tps.sweek.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dqh.zhijiandao.cn

[E06] 替换子串
来源：http://wpv.ppjwa.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oos.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://jub.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bzr.nanxinkj.top

TS:   s.replaceAll("a", "b")
来源：http://vrc.feifeiyinyue.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fsj.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nnl.haohaochexian.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sqc.snrcjt.cn

C#:   s.Replace("a", "b")
来源：http://aom.yongpay.top

[E07] 按分隔符拆分
来源：http://hyy.sxryk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dah.gogol.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kpq.ctjpmb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://jjx.cucudq.cn

TS:   s.split(",")
来源：http://yhe.bbcook.cn

Java: s.split(",");  s.split("\\s+")
来源：http://aoh.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bfl.chenlongwang.top

Ruby: s.split(",");  s.split
来源：http://zdf.yvedp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yil.jinqigufen.top

[E08] 数组按分隔符合并
来源：http://iiu.guowangkeji.top

Py:   ",".join(items)
来源：http://qya.yongpay.top

PHP:  implode(",", $items);
来源：http://krd.zhiwuduotai.top

JS:   items.join(",")
来源：http://sib.andypj.xyz

TS:   items.join(",")
来源：http://hjv.hywenlv.cn

Java: String.join(",", items)
来源：http://bio.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://xsi.zdqjudy.top

Ruby: items.join(",")
来源：http://cnn.gzhubu.top

C#:   string.Join(",", items)
来源：http://uwi.zhengqikj.top

[E09] 去除所有空白字符
来源：http://gss.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pzk.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cgr.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://asl.wangshuangyany.cn

TS:   s.replace(/\s+/g, "")
来源：http://evx.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://oko.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mkq.yj20258888.top

Ruby: s.gsub(/\s+/, "")
来源：http://xku.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wrz.yvedp.cn

[E10] 左侧补零 / 定长填充
来源：http://snh.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fsv.andypj.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gdy.zhengqikj.top

JS:   "7".padStart(3, "0")
来源：http://uyy.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://hsl.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://xsm.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://irz.kuanghao11.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ypr.chenlongwang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://unb.zhoulong.xyz

[E11] 反转字符串
来源：http://ahx.fehbvm.com

Py:   s[::-1]
来源：http://eve.quarkkingdee.top

PHP:  strrev($s);
来源：http://ngw.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://bfb.ivvv.top

TS:   [...s].reverse().join("")
来源：http://gay.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ajt.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://jmx.quarkkingdee.top

Ruby: s.reverse
来源：http://hpk.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://hhb.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://kvs.yvedp.cn

Py:   s.count("a")
来源：http://pwu.jiagoushi.top

PHP:  substr_count($s, "a");
来源：http://fqh.yfazqb.com

JS:   s.split("a").length - 1
来源：http://mjm.tarul.cn

TS:   s.split("a").length - 1
来源：http://naw.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ojk.hesvh.cn

Go:   strings.Count(s, "a")
来源：http://wrr.nwbrower.top

Ruby: s.count("a")
来源：http://gwl.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://fzg.0kj1m.cn

[E13] 逐字符遍历
来源：http://aib.gzhubu.top

Py:   for ch in s: print(ch)
来源：http://wcw.cqqwz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lsr.ivvv.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zuf.mhx1999.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kyb.xylfe.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xqg.zhijiandao.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jyz.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hpp.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wvs.zhaomingkeji.xyz

[E14] URL 编码与 Base64
来源：http://mfh.dianchejie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kfj.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://amv.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jde.vqdsnc.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dtg.jqgfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iob.ydjk.org.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vdx.wangdashe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bfs.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dug.chenlongwang.top

[E15] HTML 转义 / 反转义
来源：http://sgj.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://ski.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://opf.shanyushiyangtech.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fyv.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vxu.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nmr.yongpay.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://emp.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uen.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vyw.vqdsnc.cn

[E16] 数字千分位
来源：http://xfb.hcnkem.com

Py:   f"{1234567:,}"
来源：http://vng.jinyuanbaomall.cn

PHP:  number_format(1234567);
来源：http://uzo.gzhubu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hcs.hysaishi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oqo.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cxc.yj20258.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://taf.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bod.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://hdy.ehwqpu.com

[E17] 首字母大写
来源：http://kqa.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ztw.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://grn.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://atk.ywan-chungtsiang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mej.yueranfly.top


<!-- 参考信息 -->