代发 wailian999

[D11] 反转数组
来源：http://gfs.xinyue.icu

Py:   arr[::-1];  arr.reverse()
来源：http://voo.haohaochexian.top

PHP:  array_reverse($arr);
来源：http://eny.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://emt.sjlbkw.cn

TS:   [...arr].reverse();
来源：http://cnw.yfazqb.com

Java: Collections.reverse(list);
来源：http://jrk.yj202588.top

Go:   slices.Reverse(arr)
来源：http://bvz.cheryme.top

Ruby: arr.reverse
来源：http://oyp.quarkkingdee.top

C#:   list.Reverse();
来源：http://cei.yongpay.top

[D12] 查找元素下标
来源：http://tbv.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://bka.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ghd.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lxr.jianghu66.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jdr.jinqigufen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vfb.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://gmu.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://bji.tian-w.cn

C#:   list.IndexOf(x);
来源：http://zqa.gzhubu.top

[D13] 过滤（保留满足条件的）
来源：http://mtt.xuetiantiany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dvl.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zat.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://wjg.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://tyv.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kvq.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cfy.yj20258888.top

Ruby: arr.select { |x| x > 3 }
来源：http://ovn.hesvh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://iki.gaohongyu789.top

[D14] 映射转换（每个元素变形）
来源：http://ucw.hcnkem.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aeq.jqgufenzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oay.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://ipc.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://gbx.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://asl.gzhubu.top

Go:   // 手写循环
来源：http://wsc.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://vty.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://oir.svipenyu.cn

[D15] 去重
来源：http://lyl.xuetiantiany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jsq.sysykeji.top

PHP:  array_unique($arr);
来源：http://fra.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://qbg.hfpthk.cn

TS:   [...new Set(arr)]
来源：http://cxm.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dfj.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://krp.nanxuanxn.top

Ruby: arr.uniq
来源：http://jki.c1oappe.top

C#:   list.Distinct().ToList()
来源：http://etq.xuanzx.com

[D16] 求和与平均值
来源：http://amv.yj20258.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bgo.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lxz.ivvv.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uwq.jinqigfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://syi.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tdg.fengsongda.top

Go:   // 手写循环累加
来源：http://izk.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gep.yuanzhike.top

C#:   list.Sum();  list.Average()
来源：http://rju.bbcook.cn

[D17] 最大值与最小值
来源：http://rrm.9152youxi.cn

Py:   max(arr);  min(arr)
来源：http://lkj.chenjidiqi.icu

PHP:  max($arr);  min($arr);
来源：http://snj.hnqzz.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jtw.andypj.xyz

TS:   Math.max(...arr);
来源：http://gtz.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lqy.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cmh.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://fik.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://iuf.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://vwo.zdbjq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rqx.zhixingplan.top

PHP:  array_merge(...$nested);
来源：http://gye.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dlh.ppjwa.cn

TS:   nested.flat();
来源：http://voa.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fvy.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://ehj.aizwys.cn

Ruby: nested.flatten
来源：http://rzm.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ymh.snrcjt.cn

[D19] 按字段分组
来源：http://gpk.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bbc.yangfankeji.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lyi.jinyuanbaomall.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tdd.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kxk.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aee.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://gvs.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uxr.daria6918.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kuz.cashguo.top

[D20] 统计每个元素出现次数
来源：http://lll.ivvv.top

Py:   Counter(arr)
来源：http://cif.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://coe.uphjek.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://heo.andypj.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wlf.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jkc.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://qxz.bbcook.cn

Ruby: arr.tally
来源：http://qyx.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fdd.yj20258888.top

[D21] 判断是否包含某元素
来源：http://dvm.sweek.top

Py:   x in arr
来源：http://wtx.zhengqikj.top

PHP:  in_array($x, $arr, true);
来源：http://dip.hnqzz.top

JS:   arr.includes(x)
来源：http://vpe.pengpengdd.cyou

TS:   arr.includes(x)
来源：http://xlx.shangyingyoupin.top

Java: list.contains(x)
来源：http://oku.fzhhl.top

Go:   slices.Contains(arr, x)
来源：http://wkx.yonumen.top

Ruby: arr.include?(x)
来源：http://zhr.hongshengwenyu.top

C#:   list.Contains(x)
来源：http://qxz.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://uhu.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rkl.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jfn.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bfn.ywan-chungtsiang.top

TS:   [...arr];
来源：http://fao.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://nlf.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ril.epnwcf.com

Ruby: arr.dup;  arr.clone
来源：http://kta.chenzaomai.com

C#:   new List<int>(list);
来源：http://ijo.sweek.top

[D23] reduce 累积计算
来源：http://lss.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://slm.yuxming.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jky.cdnleiting.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://que.hcnkem.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mtj.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://efj.vehdjk.com

Go:   // 手写循环
来源：http://ikf.zhengqikj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tts.bbcook.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fxo.yj20258.top

[D24] 字典 / Map 基本操作
来源：http://dfa.fengsongda.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://axe.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rik.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tfo.gzhubu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rdv.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fhv.zhongyouzk.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lhr.316326.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sgl.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iiu.ywan-chungtsiang.top

[D25] Set 集合去重与交并差
来源：http://uvg.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qgb.tanke756.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vjx.dianchejie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fqg.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jdo.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fbj.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aqy.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ooa.jianghu66.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qct.yangfankeji.com

[D26] 数组转字符串
来源：http://tad.uphjek.com

Py:   ", ".join(map(str, arr))
来源：http://obw.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://wkv.gaohongyu789.top

JS:   arr.join(", ")
来源：http://qug.zycfv.cn

TS:   arr.join(", ")
来源：http://azu.cheryme.top

Java: String.join(", ", list)
来源：http://yhm.yangfankeji.com

Go:   strings.Join(strs, ", ")
来源：http://gkj.quarkkingdee.top

Ruby: arr.join(", ")
来源：http://fud.fzhhl.top

C#:   string.Join(", ", list)
来源：http://uqm.nwbrower.top

================================================================================
来源：http://xtk.zycfv.cn

E. 字符串处理
来源：http://qbr.aizwys.cn

================================================================================
来源：http://qno.zycfv.cn

[E01] 拼接字符串
来源：http://lvm.jlsjyb.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ifo.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://npc.zhengqikj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qbw.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qip.aizwys.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ibu.cucudq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pmq.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wpu.jlsjyb.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bug.iojbl.cn

[E02] 重复字符串
来源：http://lsv.yj202588.top

Py:   "ab" * 3
来源：http://vwx.cqqwz.cn

PHP:  str_repeat("ab", 3);
来源：http://wfu.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://myq.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://ade.chenjidiqi.icu

Java: "ab".repeat(3)
来源：http://xwy.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://xqx.hongshengwenyu.top

Ruby: "ab" * 3
来源：http://xas.nwbrower.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eim.zhoulong.xyz

[E03] 截取子串
来源：http://ddl.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ifb.bjfxy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ybk.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wvx.zhijiandao.cn

TS:   s.slice(1, 4)
来源：http://spv.vehdjk.com

Java: s.substring(1, 4)
来源：http://shu.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qjq.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://ojw.snrcjt.cn

C#:   s.Substring(1, 3)
来源：http://ije.fanxiaobao.xyz

[E04] 查找子串位置
来源：http://fun.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://daz.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://vsd.vehdjk.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ibm.epnwcf.com

TS:   s.indexOf("x")
来源：http://kvr.zhongyouzk.top

Java: s.indexOf("x")
来源：http://vsf.zhijiandao.cn

Go:   strings.Index(s, "x")
来源：http://koy.yongpay.top

Ruby: s.index("x")
来源：http://jkc.c1oappe.top

C#:   s.IndexOf("x")
来源：http://ahv.gaohongyu789.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://oqw.jinqigufen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tce.nanxuanxn.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dgb.meibo888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://epe.52xcode.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yfb.ydjk.org.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tea.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dws.shzxlz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vfe.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ydl.jiagoushi.top

[E06] 替换子串
来源：http://mec.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qqm.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://toy.ehwqpu.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ipx.jyoumei.cn

TS:   s.replaceAll("a", "b")
来源：http://byt.aibaodan.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://amg.ywan-chungtsiang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ldt.hesvh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://flt.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://jmy.aibaodan.cn

[E07] 按分隔符拆分
来源：http://njv.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://izy.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://etu.ybcxt.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://njv.iojbl.cn

TS:   s.split(",")
来源：http://rem.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pbw.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://erl.fengsongda.top

Ruby: s.split(",");  s.split
来源：http://mir.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://njh.iojbl.cn

[E08] 数组按分隔符合并
来源：http://ciz.quarkkingdee.top

Py:   ",".join(items)
来源：http://kln.yj20258888.top

PHP:  implode(",", $items);
来源：http://hsm.gotoacloud.top

JS:   items.join(",")
来源：http://wpv.haohaochexian.top

TS:   items.join(",")
来源：http://ibr.xuanzx.com

Java: String.join(",", items)
来源：http://hiy.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://bzl.ctjpmb.com

Ruby: items.join(",")
来源：http://nzy.ybcxt.top

C#:   string.Join(",", items)
来源：http://akm.quarkkingdee.top

[E09] 去除所有空白字符
来源：http://aqp.hesvh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zbr.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sfi.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://xoj.svipenyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://lbz.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://qmv.jqgfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qnu.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://tzk.0kj1m.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hki.fzhhl.top

[E10] 左侧补零 / 定长填充
来源：http://kqj.jinyuanbaomall.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uns.yfazqb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jki.zycfv.cn

JS:   "7".padStart(3, "0")
来源：http://yqo.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://xjs.kuanghao11.cn

Java: String.format("%03d", 7)
来源：http://ftx.gzhubu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://eul.zhoulong.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tsk.redwolf501.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nof.cheryme.top

[E11] 反转字符串
来源：http://exr.jinqigufen.top

Py:   s[::-1]
来源：http://ghq.jqgufenzy.top

PHP:  strrev($s);
来源：http://hzx.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://qtn.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://bkh.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wlv.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://anu.chenlongwang.top

Ruby: s.reverse
来源：http://zwm.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vzh.xylfe.cn

[E12] 统计某字符出现次数
来源：http://irh.jinghuilouyu.cn

Py:   s.count("a")
来源：http://pzn.zdbjq.cn

PHP:  substr_count($s, "a");
来源：http://grh.xuanzx.com

JS:   s.split("a").length - 1
来源：http://psy.bbcook.cn

TS:   s.split("a").length - 1
来源：http://bec.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wie.redwolf501.top

Go:   strings.Count(s, "a")
来源：http://rom.gogol.net.cn

Ruby: s.count("a")
来源：http://wvm.jiagoushi.top

C#:   s.Count(c => c == 'a')
来源：http://dck.cheryme.top

[E13] 逐字符遍历
来源：http://hii.yj20258888.top

Py:   for ch in s: print(ch)
来源：http://fvj.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fdn.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ltt.zhoulong.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://ddz.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://llt.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://clb.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dyr.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tmv.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://sje.tian-w.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jfg.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://pjt.yuxming.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zce.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://koe.chenzaomai.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jqz.redwolf501.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://teq.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jqk.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rdz.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://txj.yanxiufei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://caq.hnqzz.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rjk.yonumen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gmt.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bbc.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://liq.guannengcc.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vtv.cqqwz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://igr.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gnw.gzhubu.top

[E16] 数字千分位
来源：http://edp.jlsjyb.cn

Py:   f"{1234567:,}"
来源：http://rtd.guannengcc.top

PHP:  number_format(1234567);
来源：http://vyz.xylfe.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bvt.yj20258888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ups.daria6918.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rzy.0kj1m.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ieh.iojbl.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yxj.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://nvm.tianlin.xyz

[E17] 首字母大写
来源：http://gnb.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wcn.52xcode.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jvq.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nup.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tfv.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qsr.hnqzz.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jby.hammf.cn

Ruby: s.capitalize
来源：http://jfa.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qcy.ydjk.org.cn


<!-- 参考信息 -->