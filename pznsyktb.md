代发 wailian999

[D11] 反转数组
来源：http://nlf.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rrq.aizwys.cn

PHP:  array_reverse($arr);
来源：http://ozd.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yvw.birdmap.top

TS:   [...arr].reverse();
来源：http://zqm.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://bmz.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://gpz.jinyuanbaomall.cn

Ruby: arr.reverse
来源：http://xim.feifeiyinyue.top

C#:   list.Reverse();
来源：http://cfj.fanxiaobao.xyz

[D12] 查找元素下标
来源：http://drw.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://dlh.0kj1m.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eby.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iuk.hywenlv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zjs.ivvv.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uba.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://ibf.ybcxt.top

Ruby: arr.index(x)
来源：http://hod.yueranfly.top

C#:   list.IndexOf(x);
来源：http://ket.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://yvk.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eff.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qwk.tianlin.xyz

JS:   arr.filter(x => x > 3)
来源：http://wuo.jyoumei.cn

TS:   arr.filter(x => x > 3)
来源：http://fin.bjfxy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mva.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gdo.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://xrn.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://yji.sysykeji.top

[D14] 映射转换（每个元素变形）
来源：http://btq.uphjek.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rpc.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lyd.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://oeu.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://fvp.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://wyj.jiagoushi.top

Go:   // 手写循环
来源：http://niv.chenlongwang.top

Ruby: arr.map { |x| x * 2 }
来源：http://qee.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ueh.yuxming.cn

[D15] 去重
来源：http://ozv.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hro.guannengcc.top

PHP:  array_unique($arr);
来源：http://wto.jianghu66.top

JS:   [...new Set(arr)]
来源：http://hvx.vehdjk.com

TS:   [...new Set(arr)]
来源：http://jpq.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bqa.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cln.iojbl.cn

Ruby: arr.uniq
来源：http://bli.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://ojl.sxryk.cn

[D16] 求和与平均值
来源：http://rlb.ydjk.org.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wsc.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sft.316326.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ear.zdbjq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ebu.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pfk.yueranfly.top

Go:   // 手写循环累加
来源：http://qom.zhiwuduotai.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dsf.zhiwuduotai.top

C#:   list.Sum();  list.Average()
来源：http://jru.jqgufenzy.top

[D17] 最大值与最小值
来源：http://ofi.hysaishi.cn

Py:   max(arr);  min(arr)
来源：http://ewh.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://hqy.yvedp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://diu.yvedp.cn

TS:   Math.max(...arr);
来源：http://nuc.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://nxi.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ivp.fengsongda.top

Ruby: arr.max;  arr.min
来源：http://fjp.jinghuilouyu.cn

C#:   list.Max();  list.Min()
来源：http://qen.smart0.xyz

[D18] 扁平化嵌套数组
来源：http://hwf.uphjek.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lhc.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://ilf.jqgfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://haa.gzhubu.top

TS:   nested.flat();
来源：http://whs.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jsf.nanxinkj.top

Go:   // 手写双层循环
来源：http://bgi.hnqzz.top

Ruby: nested.flatten
来源：http://xbf.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://smu.52xcode.cn

[D19] 按字段分组
来源：http://asf.xuanzx.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://als.tanke756.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://igt.dianchejie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oex.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://evo.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fev.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://vxz.zhongyouzk.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jbf.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gyq.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://eir.guowangkeji.top

Py:   Counter(arr)
来源：http://aef.mhx1999.top

PHP:  array_count_values($arr);
来源：http://lbo.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://flq.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yek.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eer.gzhubu.top

Go:   // 手写 map[T]int
来源：http://rgp.ppjwa.cn

Ruby: arr.tally
来源：http://xzy.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://puo.epnwcf.com

[D21] 判断是否包含某元素
来源：http://ajn.cucudq.cn

Py:   x in arr
来源：http://urh.jqgufenzy.top

PHP:  in_array($x, $arr, true);
来源：http://ppx.nwbrower.top

JS:   arr.includes(x)
来源：http://tvx.fengsongda.top

TS:   arr.includes(x)
来源：http://zrx.cdnleiting.top

Java: list.contains(x)
来源：http://rwn.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://qez.hesvh.cn

Ruby: arr.include?(x)
来源：http://ugd.yonumen.top

C#:   list.Contains(x)
来源：http://jnf.wangshuangyany.cn

[D22] 复制数组（避免共享引用）
来源：http://ejl.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gzy.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nka.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ckc.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://yle.tanke756.top

Java: new ArrayList<>(list);
来源：http://pnp.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://siu.sjlbkw.cn

Ruby: arr.dup;  arr.clone
来源：http://cws.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://fte.yueranfly.top

[D23] reduce 累积计算
来源：http://jlj.shzxlz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://azk.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ymo.chenlongwang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ifb.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pky.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://pjs.iojbl.cn

Go:   // 手写循环
来源：http://prp.yfazqb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hmf.ehwqpu.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tbp.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://zcs.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://szx.c1oappe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mri.xuetiantiany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zec.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cfs.gogol.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://irv.zdbjq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kxe.chenjidiqi.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pcr.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://olc.fzhhl.top

[D25] Set 集合去重与交并差
来源：http://kwr.yueranfly.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://idv.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tsc.hnqzz.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sik.yj20258.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://akq.zdqjudy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ltk.zhiwuduotai.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dvk.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lhn.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vst.snrcjt.cn

[D26] 数组转字符串
来源：http://rxu.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://qvj.wangshuangyany.cn

PHP:  implode(", ", $arr);
来源：http://lsg.guowangkeji.top

JS:   arr.join(", ")
来源：http://tlf.mhx1999.top

TS:   arr.join(", ")
来源：http://nhu.pycfn.com

Java: String.join(", ", list)
来源：http://jrf.xziqi.cn

Go:   strings.Join(strs, ", ")
来源：http://qsb.zhijiandao.cn

Ruby: arr.join(", ")
来源：http://yoy.ctjpmb.com

C#:   string.Join(", ", list)
来源：http://dby.uphjek.com

================================================================================
来源：http://ava.sxryk.cn

E. 字符串处理
来源：http://uuj.ydjk.org.cn

================================================================================
来源：http://wxx.0kj1m.cn

[E01] 拼接字符串
来源：http://xvu.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hui.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://btm.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://btd.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jwk.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tzc.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jmb.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iuf.52xcode.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ktx.chenlongwang.top

[E02] 重复字符串
来源：http://kyw.redwolf501.top

Py:   "ab" * 3
来源：http://caa.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://pna.yuxming.cn

JS:   "ab".repeat(3)
来源：http://hqi.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://vfb.bbcook.cn

Java: "ab".repeat(3)
来源：http://rvm.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://xki.sjlbkw.cn

Ruby: "ab" * 3
来源：http://vfb.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jlk.ydjk.org.cn

[E03] 截取子串
来源：http://xey.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dcu.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sgl.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aru.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://deh.hywenlv.cn

Java: s.substring(1, 4)
来源：http://yek.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wqz.bjfxy.top

Ruby: s[1, 3];  s[1..3]
来源：http://rio.ehwqpu.com

C#:   s.Substring(1, 3)
来源：http://yhn.iojbl.cn

[E04] 查找子串位置
来源：http://oro.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://axy.fktsv.cn

PHP:  strpos($s, "x");
来源：http://njy.cucudq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://emj.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://npn.zdqjudy.top

Java: s.indexOf("x")
来源：http://yfy.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://mwv.yonumen.top

Ruby: s.index("x")
来源：http://bwo.vehdjk.com

C#:   s.IndexOf("x")
来源：http://zrc.daxiang520.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nla.zhongyouzk.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dug.uphjek.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://apq.chenzaomai.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ama.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://cko.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uqv.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://arz.quarkkingdee.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tpm.jianghu66.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ccl.hnxiangtu.top

[E06] 替换子串
来源：http://ryr.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mag.meibo888.top

PHP:  str_replace("a", "b", $s);
来源：http://hea.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xlx.guowangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://bcf.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mng.xziqi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kpo.nanxuanxn.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://efp.yvedp.cn

C#:   s.Replace("a", "b")
来源：http://ffl.sxryk.cn

[E07] 按分隔符拆分
来源：http://gfs.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ldq.jqgufenzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rwp.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dgi.snrcjt.cn

TS:   s.split(",")
来源：http://oqd.ydjk.org.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kmr.hysaishi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tkh.jqgfzy.top

Ruby: s.split(",");  s.split
来源：http://uor.chenjidiqi.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ujn.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://jcz.zhixingplan.top

Py:   ",".join(items)
来源：http://cgd.redwolf501.top

PHP:  implode(",", $items);
来源：http://wep.nwbrower.top

JS:   items.join(",")
来源：http://rwz.hywenlv.cn

TS:   items.join(",")
来源：http://yua.nanxuanxn.top

Java: String.join(",", items)
来源：http://wxh.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://usr.vehdjk.com

Ruby: items.join(",")
来源：http://ivu.tarul.cn

C#:   string.Join(",", items)
来源：http://hzv.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://ett.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yba.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zvv.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://rkl.yongpay.top

TS:   s.replace(/\s+/g, "")
来源：http://ssu.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://xkf.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://wcm.hammf.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gxe.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wqx.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://zog.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lov.ivvv.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gne.sweek.top

JS:   "7".padStart(3, "0")
来源：http://uaq.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://gxg.shanyushiyangkeji.top

Java: String.format("%03d", 7)
来源：http://mgi.pengpengdd.cyou

Go:   fmt.Sprintf("%03d", 7)
来源：http://maa.zhijiandao.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ikl.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://poj.ppjwa.cn

[E11] 反转字符串
来源：http://wum.ehwqpu.com

Py:   s[::-1]
来源：http://iba.ctjpmb.com

PHP:  strrev($s);
来源：http://vjk.shuidangran.top

JS:   [...s].reverse().join("")
来源：http://rxh.52xcode.cn

TS:   [...s].reverse().join("")
来源：http://qnh.cashguo.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lry.nwbrower.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hle.nanxuanxn.top

Ruby: s.reverse
来源：http://plm.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lfs.kuanghao11.cn

[E12] 统计某字符出现次数
来源：http://sar.zhiwuduotai.top

Py:   s.count("a")
来源：http://jaf.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://rmb.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://lop.ywan-chungtsiang.top

TS:   s.split("a").length - 1
来源：http://onm.yfazqb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dwl.zycfv.cn

Go:   strings.Count(s, "a")
来源：http://vkx.xuetiantiany.cn

Ruby: s.count("a")
来源：http://ffp.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://men.jinyuanbaomall.cn

[E13] 逐字符遍历
来源：http://rsg.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://sqq.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zsv.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xov.jianghu66.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wfu.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dxg.gotoacloud.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wcp.gotoacloud.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dru.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bbn.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://scy.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://til.zdqjudy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mjx.tianlin.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://foq.yvedp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jdw.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cot.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wzx.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sgr.pycfn.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gin.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://aet.wangdashe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://iza.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hbz.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vfx.hammf.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kxm.bbcook.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zza.zhongyouzk.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://grg.jqgfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ssr.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cop.wangdashe.top

[E16] 数字千分位
来源：http://bib.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://svu.chenlongwang.top

PHP:  number_format(1234567);
来源：http://ovv.cucudq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://obf.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hbw.fktsv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vzu.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://prp.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fso.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://kxj.gzhubu.top

[E17] 首字母大写
来源：http://dmd.yongpay.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rxm.vqdsnc.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://aaq.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gvj.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lyg.chenzaomai.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bmf.bbcook.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bru.smart0.xyz

Ruby: s.capitalize
来源：http://fok.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cfj.sweek.top


<!-- 参考信息 -->