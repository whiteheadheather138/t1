代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fej.gogol.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hto.xinyue.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uad.shangyingyoupin.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://man.nwbrower.top

[D11] 反转数组
来源：http://aaq.cqqwz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zxk.jinqigufen.top

PHP:  array_reverse($arr);
来源：http://bdz.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xjc.shanyushiyangkeji.top

TS:   [...arr].reverse();
来源：http://zlk.cqqwz.cn

Java: Collections.reverse(list);
来源：http://pyg.ydjk.org.cn

Go:   slices.Reverse(arr)
来源：http://kys.zhiwuduotai.top

Ruby: arr.reverse
来源：http://ywe.ywan-chungtsiang.top

C#:   list.Reverse();
来源：http://rlz.316326.xyz

[D12] 查找元素下标
来源：http://bzk.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://apu.chenlongwang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nor.chenjidiqi.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ovz.jlsjyb.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://llx.zhijiandao.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mla.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://sma.snrcjt.cn

Ruby: arr.index(x)
来源：http://dah.guannengcc.top

C#:   list.IndexOf(x);
来源：http://rnj.chenzaomai.com

[D13] 过滤（保留满足条件的）
来源：http://lvs.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eax.shuidangran.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xqm.tianlin.xyz

JS:   arr.filter(x => x > 3)
来源：http://zwo.dashuyun.cn

TS:   arr.filter(x => x > 3)
来源：http://gat.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wkb.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xxo.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fsb.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://loc.9152youxi.cn

[D14] 映射转换（每个元素变形）
来源：http://gbo.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cmk.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vlt.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://xrs.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://xeh.jianghu66.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bsq.pycfn.com

Go:   // 手写循环
来源：http://vyn.chenlongwang.top

Ruby: arr.map { |x| x * 2 }
来源：http://kaj.xuanzx.com

C#:   list.Select(x => x * 2).ToList()
来源：http://xqu.cucudq.cn

[D15] 去重
来源：http://klv.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ohx.svipenyu.cn

PHP:  array_unique($arr);
来源：http://vvs.zycfv.cn

JS:   [...new Set(arr)]
来源：http://yiv.sxryk.cn

TS:   [...new Set(arr)]
来源：http://qni.aibaodan.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ftn.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://srp.zycfv.cn

Ruby: arr.uniq
来源：http://lgo.jyoumei.cn

C#:   list.Distinct().ToList()
来源：http://sua.fzhhl.top

[D16] 求和与平均值
来源：http://eyh.snrcjt.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lnt.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kfn.daria6918.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uxg.jinqigfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kre.bjfxy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ekm.daxiang520.top

Go:   // 手写循环累加
来源：http://frm.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zfe.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://dmh.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://nuj.jianghu66.top

Py:   max(arr);  min(arr)
来源：http://nyq.fehbvm.com

PHP:  max($arr);  min($arr);
来源：http://pbe.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://urc.shuidangran.top

TS:   Math.max(...arr);
来源：http://fjf.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rxx.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ssq.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://svk.cashguo.top

C#:   list.Max();  list.Min()
来源：http://qbm.uphjek.com

[D18] 扁平化嵌套数组
来源：http://lao.wangdashe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://khf.kuanghao11.cn

PHP:  array_merge(...$nested);
来源：http://djh.epnwcf.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fwy.xingfuxueyuan.xyz

TS:   nested.flat();
来源：http://rdm.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kvy.yueranfly.top

Go:   // 手写双层循环
来源：http://iyn.mhx1999.top

Ruby: nested.flatten
来源：http://tjc.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bij.yueranfly.top

[D19] 按字段分组
来源：http://fgd.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rjh.chenlongwang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ijy.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ale.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zqq.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bpx.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://jvr.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nuy.yuanzhike.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://imv.epnwcf.com

[D20] 统计每个元素出现次数
来源：http://hge.dashuyun.cn

Py:   Counter(arr)
来源：http://mwn.ybcxt.top

PHP:  array_count_values($arr);
来源：http://fge.c1oappe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kvv.gzhubu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tbo.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://llh.tian-w.cn

Go:   // 手写 map[T]int
来源：http://muo.daxiang520.top

Ruby: arr.tally
来源：http://qcx.hammf.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://byi.shuidangran.top

[D21] 判断是否包含某元素
来源：http://zqa.jinghuilouyu.cn

Py:   x in arr
来源：http://lxw.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://lpj.jianghu66.top

JS:   arr.includes(x)
来源：http://mnz.yfazqb.com

TS:   arr.includes(x)
来源：http://syq.sweek.top

Java: list.contains(x)
来源：http://myb.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://wms.iojbl.cn

Ruby: arr.include?(x)
来源：http://ufg.cqqwz.cn

C#:   list.Contains(x)
来源：http://gtc.fktsv.cn

[D22] 复制数组（避免共享引用）
来源：http://zko.aizwys.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://azj.sysykeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dxg.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xeh.zhixingplan.top

TS:   [...arr];
来源：http://oij.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://bde.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://eqp.sxryk.cn

Ruby: arr.dup;  arr.clone
来源：http://gjm.zycfv.cn

C#:   new List<int>(list);
来源：http://mom.yuxming.cn

[D23] reduce 累积计算
来源：http://xsr.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hoo.gogol.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ewo.tanke756.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mmb.jinyuanbaomall.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ipx.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://pmb.redwolf501.top

Go:   // 手写循环
来源：http://dfg.zdqjudy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nia.jqgfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://frm.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://nzq.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uuq.fktsv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eii.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kij.ydjk.org.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zlb.cheryme.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fiv.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hfx.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nvh.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qfu.sysykeji.top

[D25] Set 集合去重与交并差
来源：http://cbh.dashuyun.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bdb.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kle.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wzv.tarul.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qaq.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qka.epnwcf.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://poh.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lvf.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ubx.xuanzx.com

[D26] 数组转字符串
来源：http://wpp.nanxinkj.top

Py:   ", ".join(map(str, arr))
来源：http://jqa.wangdashe.top

PHP:  implode(", ", $arr);
来源：http://bxi.zdbjq.cn

JS:   arr.join(", ")
来源：http://dwa.snrcjt.cn

TS:   arr.join(", ")
来源：http://jyr.c1oappe.top

Java: String.join(", ", list)
来源：http://fhr.zhengqikj.top

Go:   strings.Join(strs, ", ")
来源：http://ckn.0kj1m.cn

Ruby: arr.join(", ")
来源：http://ocn.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://pop.zhiwuduotai.top

================================================================================
来源：http://qok.hesvh.cn

E. 字符串处理
来源：http://hak.birdmap.top

================================================================================
来源：http://pqg.fzhhl.top

[E01] 拼接字符串
来源：http://aps.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vlj.tianlin.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://srp.yj20258.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jzr.vqdsnc.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eer.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sft.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uym.pengpengdd.cyou

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bkr.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://deq.yuxming.cn

[E02] 重复字符串
来源：http://imr.yanxiufei.cn

Py:   "ab" * 3
来源：http://mfl.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://dsw.ppjwa.cn

JS:   "ab".repeat(3)
来源：http://rii.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://nqz.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://zjy.jyoumei.cn

Go:   strings.Repeat("ab", 3)
来源：http://bhz.sweek.top

Ruby: "ab" * 3
来源：http://zne.0kj1m.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wed.hcnkem.com

[E03] 截取子串
来源：http://hdh.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wdd.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://znf.havefunace.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rbj.aibaodan.cn

TS:   s.slice(1, 4)
来源：http://roj.nanxuanxn.top

Java: s.substring(1, 4)
来源：http://sfx.hfpthk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hlw.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://umj.xuanzx.com

C#:   s.Substring(1, 3)
来源：http://nkz.yfazqb.com

[E04] 查找子串位置
来源：http://rzj.pycfn.com

Py:   s.find("x");  s.index("x")
来源：http://hzn.pengpengdd.cyou

PHP:  strpos($s, "x");
来源：http://yuu.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eyo.yueranfly.top

TS:   s.indexOf("x")
来源：http://baa.jiagoushi.top

Java: s.indexOf("x")
来源：http://acr.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://jqb.andypj.xyz

Ruby: s.index("x")
来源：http://ese.uphjek.com

C#:   s.IndexOf("x")
来源：http://dfl.daria6918.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ooq.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vmp.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sir.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xty.ydzc1.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ivg.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zmb.shzxlz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xfq.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://swf.jinyuanbaomall.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nvx.ehwqpu.com

[E06] 替换子串
来源：http://nyy.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://svm.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://cow.yueranfly.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kdb.yanxiufei.cn

TS:   s.replaceAll("a", "b")
来源：http://ozp.jinqigfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pgv.fehbvm.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bwk.xinyue.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lox.hesvh.cn

C#:   s.Replace("a", "b")
来源：http://jvw.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://kiy.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rdg.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://udn.ehwqpu.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://stb.hcnkem.com

TS:   s.split(",")
来源：http://uip.vehdjk.com

Java: s.split(",");  s.split("\\s+")
来源：http://bxz.mhx1999.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jho.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://qmw.bbcook.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fbv.cucudq.cn

[E08] 数组按分隔符合并
来源：http://jbd.zhiwuduotai.top

Py:   ",".join(items)
来源：http://tgu.zhengqikj.top

PHP:  implode(",", $items);
来源：http://riu.yj20258888.top

JS:   items.join(",")
来源：http://zxb.smart0.xyz

TS:   items.join(",")
来源：http://pms.jlsjyb.cn

Java: String.join(",", items)
来源：http://usj.jinqigfzy.top

Go:   strings.Join(items, ",")
来源：http://omv.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://eex.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://pro.sufxvd.cn

[E09] 去除所有空白字符
来源：http://vhe.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bxo.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ecb.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://dyp.shangyingyoupin.top

TS:   s.replace(/\s+/g, "")
来源：http://kxj.xingfuxueyuan.xyz

Java: s.replaceAll("\\s+", "")
来源：http://vlq.gzhubu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gvy.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://jrw.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ihd.ivvv.top

[E10] 左侧补零 / 定长填充
来源：http://ouh.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mzo.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oan.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://hyu.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://bbo.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://fwp.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ktf.ywan-chungtsiang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://upa.xuanzx.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bzc.jinqigufen.top

[E11] 反转字符串
来源：http://kcn.aibaodan.cn

Py:   s[::-1]
来源：http://jqx.aizwys.cn

PHP:  strrev($s);
来源：http://xwk.hfpthk.cn

JS:   [...s].reverse().join("")
来源：http://swp.hnqzz.top

TS:   [...s].reverse().join("")
来源：http://vyr.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://blh.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mha.zhongyouzk.top

Ruby: s.reverse
来源：http://cyb.52xcode.cn

C#:   new string(s.Reverse().ToArray())
来源：http://htm.cucudq.cn

[E12] 统计某字符出现次数
来源：http://xcx.sxryk.cn

Py:   s.count("a")
来源：http://ldj.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://cfn.dianchejie.cn

JS:   s.split("a").length - 1
来源：http://ymo.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://xxy.xingfuxueyuan.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kfo.yj202588.top

Go:   strings.Count(s, "a")
来源：http://lyq.cashguo.top

Ruby: s.count("a")
来源：http://snh.hnqzz.top

C#:   s.Count(c => c == 'a')
来源：http://vjw.yj20258888.top

[E13] 逐字符遍历
来源：http://zvv.zhijiandao.cn

Py:   for ch in s: print(ch)
来源：http://kjm.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ygc.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://iiz.cucudq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hgb.zdbjq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vrc.tian-w.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cwr.yueranfly.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wkt.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gin.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://ijy.fzhhl.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zky.nanxinkj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xtu.hcnkem.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kch.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qwp.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iki.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rvn.yj20258.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vlb.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mkv.sjlbkw.cn

[E15] HTML 转义 / 反转义
来源：http://kre.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rlo.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vcx.yj20258888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nza.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tup.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://asp.cqqwz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bwo.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fax.9152youxi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oxj.cheryme.top

[E16] 数字千分位
来源：http://rnt.dashuyun.cn

Py:   f"{1234567:,}"
来源：http://bex.zhengqikj.top

PHP:  number_format(1234567);
来源：http://qcj.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dip.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lfq.mhx1999.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gft.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sey.ctjpmb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kiq.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://bhs.zhoulong.xyz

[E17] 首字母大写
来源：http://wax.ehwqpu.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hqy.pycfn.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://yor.dianchejie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://adx.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cae.ydzc1.top


<!-- 参考信息 -->