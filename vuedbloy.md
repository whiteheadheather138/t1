代发 wailian999

Ruby: arr.index(x)
来源：http://vhl.gzhubu.top

C#:   list.IndexOf(x);
来源：http://ser.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://azh.shanyushiyangtech.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rpm.hysaishi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zck.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://bhv.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://yno.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://egb.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mev.tarul.cn

Ruby: arr.select { |x| x > 3 }
来源：http://eht.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xzm.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://qlq.hnqzz.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hdp.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lia.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://ezd.ydjk.org.cn

TS:   arr.map(x => x * 2)
来源：http://gzm.xingfuxueyuan.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://pjz.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://mlh.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ptt.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ctr.tianlin.xyz

[D15] 去重
来源：http://ngd.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mjt.nwbrower.top

PHP:  array_unique($arr);
来源：http://clb.jianghu66.top

JS:   [...new Set(arr)]
来源：http://djc.xinyue.icu

TS:   [...new Set(arr)]
来源：http://ksk.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fsk.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://neu.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://onc.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://tah.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://cth.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://feq.hesvh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xlg.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cyo.hnqzz.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oca.daria6918.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fzm.hammf.cn

Go:   // 手写循环累加
来源：http://sym.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oav.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://vjf.cheryme.top

[D17] 最大值与最小值
来源：http://vdf.guowangkeji.top

Py:   max(arr);  min(arr)
来源：http://wst.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://uxx.haohaochexian.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qda.yvedp.cn

TS:   Math.max(...arr);
来源：http://zfq.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pov.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ggz.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://rsx.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://qhw.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://tow.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gto.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://tqy.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ymo.zhengqikj.top

TS:   nested.flat();
来源：http://vwc.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vse.snrcjt.cn

Go:   // 手写双层循环
来源：http://qas.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://inl.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sbv.jinghuilouyu.cn

[D19] 按字段分组
来源：http://ulv.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://liv.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lsf.pycfn.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uak.yvedp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bad.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rtv.ydzc1.top

Go:   // 手写 map[string][]T
来源：http://gbt.iojbl.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://brj.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://adw.bjfxy.top

[D20] 统计每个元素出现次数
来源：http://bry.feifeiyinyue.top

Py:   Counter(arr)
来源：http://skf.ppjwa.cn

PHP:  array_count_values($arr);
来源：http://dil.yfazqb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xjo.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bgp.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lti.zhongyouzk.top

Go:   // 手写 map[T]int
来源：http://sqg.nwbrower.top

Ruby: arr.tally
来源：http://bef.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tlh.xinyue.icu

[D21] 判断是否包含某元素
来源：http://snz.dashuyun.cn

Py:   x in arr
来源：http://ulp.9152youxi.cn

PHP:  in_array($x, $arr, true);
来源：http://ixp.yj202588.top

JS:   arr.includes(x)
来源：http://zuz.fehbvm.com

TS:   arr.includes(x)
来源：http://odb.ehwqpu.com

Java: list.contains(x)
来源：http://qzo.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://dhp.fengsongda.top

Ruby: arr.include?(x)
来源：http://ajs.hongshengwenyu.top

C#:   list.Contains(x)
来源：http://gud.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://caj.zdbjq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lps.yj202588.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cvi.52xcode.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wwo.yongpay.top

TS:   [...arr];
来源：http://qiu.yj20258888.top

Java: new ArrayList<>(list);
来源：http://baw.nanxuanxn.top

Go:   copied := append([]int(nil), arr...)
来源：http://bbx.sxryk.cn

Ruby: arr.dup;  arr.clone
来源：http://fgx.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://uvl.hnxiangtu.top

[D23] reduce 累积计算
来源：http://ivk.epnwcf.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rde.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uqo.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jnr.316326.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ayh.zhengqikj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cfe.uphjek.com

Go:   // 手写循环
来源：http://pew.ydzc1.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uyr.dashuyun.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xkm.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://per.shangyingyoupin.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jxq.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dzt.nanxinkj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fzc.daria6918.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://emj.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yoa.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dye.jianghu66.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fmj.hnxiangtu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fvp.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://yuq.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aib.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cgv.dashuyun.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://joz.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pkb.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mto.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vvd.xziqi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ptu.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gpn.andypj.xyz

[D26] 数组转字符串
来源：http://nwl.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://qbm.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://zfh.svipenyu.cn

JS:   arr.join(", ")
来源：http://ufk.hywenlv.cn

TS:   arr.join(", ")
来源：http://ymm.jianghu66.top

Java: String.join(", ", list)
来源：http://tqm.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://fwf.shangyingyoupin.top

Ruby: arr.join(", ")
来源：http://hcp.shangyingyoupin.top

C#:   string.Join(", ", list)
来源：http://zfc.xziqi.cn

================================================================================
来源：http://dsv.52xcode.cn

E. 字符串处理
来源：http://hqn.hnqzz.top

================================================================================
来源：http://bva.vehdjk.com

[E01] 拼接字符串
来源：http://nmg.fktsv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dvz.tianlin.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zso.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dax.sweek.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xsi.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ifh.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qvy.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://feq.jlsjyb.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vbm.gotoacloud.top

[E02] 重复字符串
来源：http://jqm.shzxlz.cn

Py:   "ab" * 3
来源：http://xzz.jinqigfzy.top

PHP:  str_repeat("ab", 3);
来源：http://pdg.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://zlv.vehdjk.com

TS:   "ab".repeat(3)
来源：http://xzh.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://udl.cashguo.top

Go:   strings.Repeat("ab", 3)
来源：http://uwp.sxryk.cn

Ruby: "ab" * 3
来源：http://fwx.hysaishi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kus.andypj.xyz

[E03] 截取子串
来源：http://hvt.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gnv.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gxp.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://duh.tanke756.top

TS:   s.slice(1, 4)
来源：http://yxw.fktsv.cn

Java: s.substring(1, 4)
来源：http://hly.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lwa.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://wtl.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://nsg.52xcode.cn

[E04] 查找子串位置
来源：http://kjv.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://jaz.hesvh.cn

PHP:  strpos($s, "x");
来源：http://vdr.dianchejie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pqg.hfpthk.cn

TS:   s.indexOf("x")
来源：http://bhj.birdmap.top

Java: s.indexOf("x")
来源：http://jqn.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://avh.cdnleiting.top

Ruby: s.index("x")
来源：http://zel.tianlin.xyz

C#:   s.IndexOf("x")
来源：http://kka.0kj1m.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wng.yangfankeji.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sow.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://orf.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hwf.yuanzhike.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tvj.bbcook.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://elk.hfpthk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pbl.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jom.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wmr.jianghu66.top

[E06] 替换子串
来源：http://pvy.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vtz.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://hka.chenlongwang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rac.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://hnq.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pku.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zxd.hywenlv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vos.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://zus.ppjwa.cn

[E07] 按分隔符拆分
来源：http://znr.gogol.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://enc.ehwqpu.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aha.cucudq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ivn.316326.xyz

TS:   s.split(",")
来源：http://fax.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ozp.uphjek.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hpz.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://mlx.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wav.fktsv.cn

[E08] 数组按分隔符合并
来源：http://fhd.hnqzz.top

Py:   ",".join(items)
来源：http://aoy.xuanzx.com

PHP:  implode(",", $items);
来源：http://nho.nanxinkj.top

JS:   items.join(",")
来源：http://zyk.jinqigfzy.top

TS:   items.join(",")
来源：http://mle.xuetiantiany.cn

Java: String.join(",", items)
来源：http://vmr.tanke756.top

Go:   strings.Join(items, ",")
来源：http://jpt.havefunace.top

Ruby: items.join(",")
来源：http://zxp.daxiang520.top

C#:   string.Join(",", items)
来源：http://wiv.hcnkem.com

[E09] 去除所有空白字符
来源：http://isb.yj20258888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sxx.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://btb.zhengqikj.top

JS:   s.replace(/\s+/g, "")
来源：http://omw.yanxiufei.cn

TS:   s.replace(/\s+/g, "")
来源：http://vhm.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://ywh.sweek.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rcw.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://umb.daria6918.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ycp.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://apd.jinyuanbaomall.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://etq.yanxiufei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vhy.shuidangran.top

JS:   "7".padStart(3, "0")
来源：http://pwq.cdnleiting.top

TS:   "7".padStart(3, "0")
来源：http://fud.dianchejie.cn

Java: String.format("%03d", 7)
来源：http://got.bbcook.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kex.hnxiangtu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kdl.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hst.yuanzhike.top

[E11] 反转字符串
来源：http://vjl.guannengcc.top

Py:   s[::-1]
来源：http://eyw.epnwcf.com

PHP:  strrev($s);
来源：http://box.jinqigfzy.top

JS:   [...s].reverse().join("")
来源：http://fcx.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://nuc.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lao.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ntz.dianchejie.cn

Ruby: s.reverse
来源：http://lkt.bjfxy.top

C#:   new string(s.Reverse().ToArray())
来源：http://zww.ctjpmb.com

[E12] 统计某字符出现次数
来源：http://kun.xinyue.icu

Py:   s.count("a")
来源：http://vke.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://cff.iojbl.cn

JS:   s.split("a").length - 1
来源：http://xqy.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://qin.dianchejie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gjn.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://qam.cdnleiting.top

Ruby: s.count("a")
来源：http://pfw.yangfankeji.com

C#:   s.Count(c => c == 'a')
来源：http://kwt.yueranfly.top

[E13] 逐字符遍历
来源：http://epz.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://bqc.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cdk.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jij.guowangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xrl.feifeiyinyue.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jkd.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xkv.jianghu66.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tlu.chenlongwang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://thn.jianghu66.top

[E14] URL 编码与 Base64
来源：http://zcj.fanxiaobao.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://agp.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zde.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uvw.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://teo.andypj.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cyn.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ljw.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aaz.sweek.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ozt.shanyushiyangtech.top

[E15] HTML 转义 / 反转义
来源：http://rwr.0kj1m.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zwv.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://irb.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hxj.yanxiufei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gty.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vco.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://api.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bad.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://psj.nanxinkj.top

[E16] 数字千分位
来源：http://ssp.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://plb.jinqigufen.top

PHP:  number_format(1234567);
来源：http://jgy.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hvw.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://spn.yj20258.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blk.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cqz.redwolf501.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://npy.yongpay.top

C#:   1234567.ToString("N0")
来源：http://mbq.316326.xyz

[E17] 首字母大写
来源：http://joj.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://voh.fehbvm.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ixo.quarkkingdee.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vbr.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ezr.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hxa.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://shq.shzxlz.cn

Ruby: s.capitalize
来源：http://pxj.yanxiufei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://boc.chenjidiqi.icu

[E18] 模板占位符替换
来源：http://zcm.nanxinkj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pya.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cxx.xuanzx.com

JS:   tpl.replaceAll("{name}", name)
来源：http://bsl.jianghu66.top

TS:   tpl.replaceAll("{name}", name)
来源：http://sha.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gdi.ywan-chungtsiang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hdu.gotoacloud.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://scl.xinyue.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jma.zhaomingkeji.xyz

[E19] 多行文本按行拆分
来源：http://ycd.xziqi.cn

Py:   s.splitlines()
来源：http://grc.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dnk.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://toi.feifeiyinyue.top

TS:   s.split(/\r?\n/)
来源：http://cwp.hfpthk.cn

Java: s.lines().toList()
来源：http://vxg.yuxming.cn

Go:   strings.Split(s, "\n")
来源：http://lkg.yj202588.top


<!-- 参考信息 -->