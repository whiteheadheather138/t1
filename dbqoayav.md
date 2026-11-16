代发 wailian999

TS:   [...arr].reverse();
来源：http://rsu.chenzaomai.com

Java: Collections.reverse(list);
来源：http://hge.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://vso.andypj.xyz

Ruby: arr.reverse
来源：http://tdq.jinqigfzy.top

C#:   list.Reverse();
来源：http://mba.snrcjt.cn

[D12] 查找元素下标
来源：http://imc.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://rdv.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ygy.hfpthk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pmv.daxiang520.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mff.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sqc.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://fxx.daria6918.cn

Ruby: arr.index(x)
来源：http://xtg.aizwys.cn

C#:   list.IndexOf(x);
来源：http://zdk.zhiwuduotai.top

[D13] 过滤（保留满足条件的）
来源：http://niv.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xli.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cbw.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://jww.bbcook.cn

TS:   arr.filter(x => x > 3)
来源：http://vus.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bha.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jby.sxryk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jty.wangdashe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ogg.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://trr.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vtc.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uqw.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://sgs.hnqzz.top

TS:   arr.map(x => x * 2)
来源：http://xsj.fanxiaobao.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://zuv.redwolf501.top

Go:   // 手写循环
来源：http://aue.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ght.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://dbd.bbcook.cn

[D15] 去重
来源：http://ele.shzxlz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zvo.wangdashe.top

PHP:  array_unique($arr);
来源：http://azi.daria6918.cn

JS:   [...new Set(arr)]
来源：http://kbv.uphjek.com

TS:   [...new Set(arr)]
来源：http://taf.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cxj.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://srm.sweek.top

Ruby: arr.uniq
来源：http://zte.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://qfs.yfazqb.com

[D16] 求和与平均值
来源：http://noa.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://znt.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rud.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://exy.smart0.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uvr.hnxiangtu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://okf.ivvv.top

Go:   // 手写循环累加
来源：http://khi.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wus.wangdashe.top

C#:   list.Sum();  list.Average()
来源：http://zbq.gogol.net.cn

[D17] 最大值与最小值
来源：http://gah.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://rcq.shanyushiyangkeji.top

PHP:  max($arr);  min($arr);
来源：http://iig.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nzu.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://fap.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://yal.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zuq.mhx1999.top

Ruby: arr.max;  arr.min
来源：http://ngf.ctjpmb.com

C#:   list.Max();  list.Min()
来源：http://wkw.xuetiantiany.cn

[D18] 扁平化嵌套数组
来源：http://oap.epnwcf.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://afj.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://bsk.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ypx.0kj1m.cn

TS:   nested.flat();
来源：http://dzv.wangshuangyany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xmx.hesvh.cn

Go:   // 手写双层循环
来源：http://elx.gogol.net.cn

Ruby: nested.flatten
来源：http://ysu.bbcook.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://azz.zycfv.cn

[D19] 按字段分组
来源：http://ehu.ehwqpu.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bpl.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jjh.zhongyouzk.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qpf.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rdk.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jur.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://bhv.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vfh.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sbm.vehdjk.com

[D20] 统计每个元素出现次数
来源：http://fkh.yanxiufei.cn

Py:   Counter(arr)
来源：http://tsz.pycfn.com

PHP:  array_count_values($arr);
来源：http://vua.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ert.9152youxi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dwn.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fou.yuanzhike.top

Go:   // 手写 map[T]int
来源：http://oys.kuanghao11.cn

Ruby: arr.tally
来源：http://fmr.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ics.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://oww.daria6918.cn

Py:   x in arr
来源：http://phv.fzhhl.top

PHP:  in_array($x, $arr, true);
来源：http://xaq.ctjpmb.com

JS:   arr.includes(x)
来源：http://zid.vehdjk.com

TS:   arr.includes(x)
来源：http://vrx.havefunace.top

Java: list.contains(x)
来源：http://uig.tarul.cn

Go:   slices.Contains(arr, x)
来源：http://tml.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://ggh.shuidangran.top

C#:   list.Contains(x)
来源：http://xbl.svipenyu.cn

[D22] 复制数组（避免共享引用）
来源：http://cfq.yj202588.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xbs.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pot.fzhhl.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://puu.redwolf501.top

TS:   [...arr];
来源：http://cvx.hesvh.cn

Java: new ArrayList<>(list);
来源：http://bpi.pycfn.com

Go:   copied := append([]int(nil), arr...)
来源：http://yxx.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://qdz.fengsongda.top

C#:   new List<int>(list);
来源：http://hex.nanxinkj.top

[D23] reduce 累积计算
来源：http://lfm.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kya.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bfn.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qtu.birdmap.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tpx.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://isi.yj20258888.top

Go:   // 手写循环
来源：http://jym.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wjp.mhx1999.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gix.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://rgg.cheryme.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://idv.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kof.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oxm.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mlj.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://agn.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eau.ppjwa.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ncb.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zeu.xuetiantiany.cn

[D25] Set 集合去重与交并差
来源：http://nul.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ady.52xcode.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ilc.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qqe.bjfxy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tyb.cashguo.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://npv.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ckr.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://era.yueranfly.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ssc.fengsongda.top

[D26] 数组转字符串
来源：http://hfb.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://oez.yvedp.cn

PHP:  implode(", ", $arr);
来源：http://zhj.guowangkeji.top

JS:   arr.join(", ")
来源：http://egw.dianchejie.cn

TS:   arr.join(", ")
来源：http://rdb.bjfxy.top

Java: String.join(", ", list)
来源：http://bwc.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://hzw.sufxvd.cn

Ruby: arr.join(", ")
来源：http://ovv.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://jst.gogol.net.cn

================================================================================
来源：http://wbl.xylfe.cn

E. 字符串处理
来源：http://kxg.tarul.cn

================================================================================
来源：http://vxy.hywenlv.cn

[E01] 拼接字符串
来源：http://cez.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://djq.andypj.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zml.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rhw.redwolf501.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zlx.aizwys.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rvb.dianchejie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lrh.pycfn.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rcd.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ehg.cheryme.top

[E02] 重复字符串
来源：http://gyu.birdmap.top

Py:   "ab" * 3
来源：http://dta.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://vis.yj202588.top

JS:   "ab".repeat(3)
来源：http://xwa.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://ylb.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://jcq.shuidangran.top

Go:   strings.Repeat("ab", 3)
来源：http://pkx.sjlbkw.cn

Ruby: "ab" * 3
来源：http://uel.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xku.shzxlz.cn

[E03] 截取子串
来源：http://ndx.pengpengdd.cyou

Py:   s[1:4];  s[:3];  s[3:]
来源：http://var.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bsm.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cva.bbcook.cn

TS:   s.slice(1, 4)
来源：http://zje.zdbjq.cn

Java: s.substring(1, 4)
来源：http://iuh.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dje.gogol.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cxy.jinghuilouyu.cn

C#:   s.Substring(1, 3)
来源：http://qev.yueranfly.top

[E04] 查找子串位置
来源：http://ikv.yj202588.top

Py:   s.find("x");  s.index("x")
来源：http://vto.sweek.top

PHP:  strpos($s, "x");
来源：http://rft.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hue.52xcode.cn

TS:   s.indexOf("x")
来源：http://sbc.shzxlz.cn

Java: s.indexOf("x")
来源：http://tnd.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://eso.nwbrower.top

Ruby: s.index("x")
来源：http://ess.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://fgt.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hbo.mhx1999.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pon.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iqg.mhx1999.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hfv.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://wtu.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uai.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://suq.jqgufenzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tom.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rtv.haohaochexian.top

[E06] 替换子串
来源：http://uvd.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bmj.jiagoushi.top

PHP:  str_replace("a", "b", $s);
来源：http://yey.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ajo.shanyushiyangtech.top

TS:   s.replaceAll("a", "b")
来源：http://yuh.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zit.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gvq.iojbl.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bpi.nanxinkj.top

C#:   s.Replace("a", "b")
来源：http://tau.pycfn.com

[E07] 按分隔符拆分
来源：http://mvn.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aba.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://des.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vhv.yuxming.cn

TS:   s.split(",")
来源：http://lqb.fengsongda.top

Java: s.split(",");  s.split("\\s+")
来源：http://lfq.hfpthk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://orj.fanxiaobao.xyz

Ruby: s.split(",");  s.split
来源：http://vpq.cashguo.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nkv.cashguo.top

[E08] 数组按分隔符合并
来源：http://bpa.shzxlz.cn

Py:   ",".join(items)
来源：http://gkr.yj20258888.top

PHP:  implode(",", $items);
来源：http://num.guannengcc.top

JS:   items.join(",")
来源：http://wvu.ehwqpu.com

TS:   items.join(",")
来源：http://acz.hnxiangtu.top

Java: String.join(",", items)
来源：http://ttl.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://wif.ywan-chungtsiang.top

Ruby: items.join(",")
来源：http://ctu.tian-w.cn

C#:   string.Join(",", items)
来源：http://cmj.fzhhl.top

[E09] 去除所有空白字符
来源：http://sfz.epnwcf.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vbc.feifeiyinyue.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cei.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://bac.hnxiangtu.top

TS:   s.replace(/\s+/g, "")
来源：http://dta.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://lyf.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lfl.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://msz.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vgw.svipenyu.cn

[E10] 左侧补零 / 定长填充
来源：http://cfr.aizwys.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ciu.hnqzz.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ggu.smart0.xyz

JS:   "7".padStart(3, "0")
来源：http://flz.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://pyl.cucudq.cn

Java: String.format("%03d", 7)
来源：http://sbw.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jzk.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fon.wangshuangyany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://owq.yangfankeji.com

[E11] 反转字符串
来源：http://cdy.yuxming.cn

Py:   s[::-1]
来源：http://wyj.sysykeji.top

PHP:  strrev($s);
来源：http://wfn.yangfankeji.com

JS:   [...s].reverse().join("")
来源：http://jzy.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://mbj.jiagoushi.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pkh.fehbvm.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://kgl.fehbvm.com

Ruby: s.reverse
来源：http://yus.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://hfr.tanke756.top

[E12] 统计某字符出现次数
来源：http://yop.bbcook.cn

Py:   s.count("a")
来源：http://fqp.andypj.xyz

PHP:  substr_count($s, "a");
来源：http://hcr.hcnkem.com

JS:   s.split("a").length - 1
来源：http://bmu.mhx1999.top

TS:   s.split("a").length - 1
来源：http://vfk.hnqzz.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rqj.vqdsnc.cn

Go:   strings.Count(s, "a")
来源：http://xsk.yj20258.top

Ruby: s.count("a")
来源：http://jbe.shanyushiyangtech.top

C#:   s.Count(c => c == 'a')
来源：http://vuk.andypj.xyz

[E13] 逐字符遍历
来源：http://ljy.9152youxi.cn

Py:   for ch in s: print(ch)
来源：http://dyz.ybcxt.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lyq.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://byk.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ail.hnxiangtu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iyf.yonumen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vfs.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vhe.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ksx.shuidangran.top

[E14] URL 编码与 Base64
来源：http://fur.ppjwa.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sud.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zgf.tanke756.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://csu.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qzy.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oeb.fanxiaobao.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ljv.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uiy.jlsjyb.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eep.c1oappe.top

[E15] HTML 转义 / 反转义
来源：http://dix.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gni.ydzc1.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dta.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gbd.redwolf501.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qyp.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jkx.fehbvm.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vwh.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nep.shuidangran.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pjr.xuanzx.com

[E16] 数字千分位
来源：http://lkh.haohaochexian.top

Py:   f"{1234567:,}"
来源：http://rpw.zdbjq.cn

PHP:  number_format(1234567);
来源：http://lyo.vehdjk.com

JS:   (1234567).toLocaleString("en-US")
来源：http://lpi.hammf.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://btn.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tlj.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dlh.zhongyouzk.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kds.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://ykn.yj20258888.top

[E17] 首字母大写
来源：http://eyz.andypj.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zbg.zhongyouzk.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qiv.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fpt.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bvl.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gli.fzhhl.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://con.bjfxy.top

Ruby: s.capitalize
来源：http://rny.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aia.cheryme.top

[E18] 模板占位符替换
来源：http://uru.tian-w.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jls.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://liy.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sab.yangfankeji.com


<!-- 参考信息 -->