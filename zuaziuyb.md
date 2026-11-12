代发 wailian999

TS:   [...arr].reverse();
来源：http://bwb.zhaomingkeji.xyz

Java: Collections.reverse(list);
来源：http://xsh.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://ojq.zhengqikj.top

Ruby: arr.reverse
来源：http://tkp.nanxinkj.top

C#:   list.Reverse();
来源：http://uuk.zhengqikj.top

[D12] 查找元素下标
来源：http://lge.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://thy.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://czv.redwolf501.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ddd.c1oappe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wwx.zhijiandao.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iff.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://vpw.xziqi.cn

Ruby: arr.index(x)
来源：http://git.aibaodan.cn

C#:   list.IndexOf(x);
来源：http://ime.xinyue.icu

[D13] 过滤（保留满足条件的）
来源：http://vzz.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nrq.ivvv.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gbb.birdmap.top

JS:   arr.filter(x => x > 3)
来源：http://xqh.bbcook.cn

TS:   arr.filter(x => x > 3)
来源：http://nnh.gogol.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nzw.cdnleiting.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zca.tian-w.cn

Ruby: arr.select { |x| x > 3 }
来源：http://iit.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dwy.xuanzx.com

[D14] 映射转换（每个元素变形）
来源：http://qgs.ybcxt.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zfm.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xeo.wangshuangyany.cn

JS:   arr.map(x => x * 2)
来源：http://ibf.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://pcl.hnxiangtu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bhk.wangdashe.top

Go:   // 手写循环
来源：http://nkn.cdnleiting.top

Ruby: arr.map { |x| x * 2 }
来源：http://onl.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://meu.wangshuangyany.cn

[D15] 去重
来源：http://scq.jinghuilouyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://afe.jyoumei.cn

PHP:  array_unique($arr);
来源：http://tvk.uphjek.com

JS:   [...new Set(arr)]
来源：http://aav.yj202588.top

TS:   [...new Set(arr)]
来源：http://qmu.shanyushiyangtech.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nky.ydjk.org.cn

Go:   // 用 map[T]struct{} 手写
来源：http://arh.0kj1m.cn

Ruby: arr.uniq
来源：http://upb.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://etx.yj20258.top

[D16] 求和与平均值
来源：http://zqc.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jab.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ypv.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ghq.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nui.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sox.jlsjyb.cn

Go:   // 手写循环累加
来源：http://prf.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zom.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://xpj.quarkkingdee.top

[D17] 最大值与最小值
来源：http://hhu.yongpay.top

Py:   max(arr);  min(arr)
来源：http://dpe.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://ooc.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lho.shanyushiyangkeji.top

TS:   Math.max(...arr);
来源：http://fhd.aizwys.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lvh.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pvp.gaohongyu789.top

Ruby: arr.max;  arr.min
来源：http://mzf.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://aua.hongshengwenyu.top

[D18] 扁平化嵌套数组
来源：http://dis.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xug.gotoacloud.top

PHP:  array_merge(...$nested);
来源：http://qyh.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eml.ybcxt.top

TS:   nested.flat();
来源：http://uud.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xea.yj20258888.top

Go:   // 手写双层循环
来源：http://kul.xuanzx.com

Ruby: nested.flatten
来源：http://fcf.yfazqb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://tfc.hfpthk.cn

[D19] 按字段分组
来源：http://gcn.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xdl.ydjk.org.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dkg.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cga.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hsb.sweek.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uez.jinghuilouyu.cn

Go:   // 手写 map[string][]T
来源：http://nqo.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ugj.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rek.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://uvi.0kj1m.cn

Py:   Counter(arr)
来源：http://jxo.0kj1m.cn

PHP:  array_count_values($arr);
来源：http://zad.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dmw.aizwys.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vcl.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cig.andypj.xyz

Go:   // 手写 map[T]int
来源：http://fmi.snrcjt.cn

Ruby: arr.tally
来源：http://gyn.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ahm.andypj.xyz

[D21] 判断是否包含某元素
来源：http://aim.havefunace.top

Py:   x in arr
来源：http://fsc.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://nfk.vqdsnc.cn

JS:   arr.includes(x)
来源：http://vsn.wangdashe.top

TS:   arr.includes(x)
来源：http://pcp.yfazqb.com

Java: list.contains(x)
来源：http://dhm.wangshuangyany.cn

Go:   slices.Contains(arr, x)
来源：http://ubl.andypj.xyz

Ruby: arr.include?(x)
来源：http://kwb.yj202588.top

C#:   list.Contains(x)
来源：http://mbi.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://peq.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bvg.gaohongyu789.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://esn.sufxvd.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qew.svipenyu.cn

TS:   [...arr];
来源：http://ulo.pycfn.com

Java: new ArrayList<>(list);
来源：http://awv.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://pwn.cdnleiting.top

Ruby: arr.dup;  arr.clone
来源：http://gty.yangfankeji.com

C#:   new List<int>(list);
来源：http://zdy.sjlbkw.cn

[D23] reduce 累积计算
来源：http://gpf.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zjh.hongshengwenyu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fjt.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lui.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xmp.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oep.jyoumei.cn

Go:   // 手写循环
来源：http://twk.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://djy.jinyuanbaomall.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pwf.yueranfly.top

[D24] 字典 / Map 基本操作
来源：http://guc.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://quy.haohaochexian.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qoy.yuxming.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zal.c1oappe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uof.hesvh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wid.chenjidiqi.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://foc.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://plj.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mup.smart0.xyz

[D25] Set 集合去重与交并差
来源：http://pzz.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vtj.52xcode.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://juy.jinyuanbaomall.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://etu.bjfxy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tdb.jyoumei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nap.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cii.yanxiufei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://quf.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nph.shzxlz.cn

[D26] 数组转字符串
来源：http://xbw.epnwcf.com

Py:   ", ".join(map(str, arr))
来源：http://cvx.sweek.top

PHP:  implode(", ", $arr);
来源：http://qfv.shanyushiyangtech.top

JS:   arr.join(", ")
来源：http://xlw.yuanzhike.top

TS:   arr.join(", ")
来源：http://okx.haohaochexian.top

Java: String.join(", ", list)
来源：http://ujn.hammf.cn

Go:   strings.Join(strs, ", ")
来源：http://yun.ywan-chungtsiang.top

Ruby: arr.join(", ")
来源：http://sgn.yuxming.cn

C#:   string.Join(", ", list)
来源：http://akv.yvedp.cn

================================================================================
来源：http://lvz.nanxinkj.top

E. 字符串处理
来源：http://gzw.xingfuxueyuan.xyz

================================================================================
来源：http://bih.cqqwz.cn

[E01] 拼接字符串
来源：http://xod.tian-w.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nsd.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lzp.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sox.dashuyun.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qwh.jinqigufen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rpg.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rov.daria6918.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uoq.guannengcc.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nbs.guannengcc.top

[E02] 重复字符串
来源：http://phy.daria6918.cn

Py:   "ab" * 3
来源：http://zfv.nwbrower.top

PHP:  str_repeat("ab", 3);
来源：http://sqm.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://jmd.ctjpmb.com

TS:   "ab".repeat(3)
来源：http://lfw.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://rht.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://qft.vehdjk.com

Ruby: "ab" * 3
来源：http://sow.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://psf.xylfe.cn

[E03] 截取子串
来源：http://zfg.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ngb.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hah.52xcode.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ixp.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://xhb.shanyushiyangkeji.top

Java: s.substring(1, 4)
来源：http://owz.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fnb.tian-w.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wzv.zhiwuduotai.top

C#:   s.Substring(1, 3)
来源：http://ead.jianghu66.top

[E04] 查找子串位置
来源：http://xzf.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://mzu.zhixingplan.top

PHP:  strpos($s, "x");
来源：http://gwf.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zdo.yuanzhike.top

TS:   s.indexOf("x")
来源：http://rht.nwbrower.top

Java: s.indexOf("x")
来源：http://ttm.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://wco.hnqzz.top

Ruby: s.index("x")
来源：http://sdm.gotoacloud.top

C#:   s.IndexOf("x")
来源：http://lke.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hte.jqgfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://awe.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nvp.52xcode.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://avo.zdqjudy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://njl.bjfxy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zfk.sweek.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lpa.shzxlz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eec.yuxming.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eli.fanxiaobao.xyz

[E06] 替换子串
来源：http://ycc.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mxm.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://pek.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://onu.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://zmi.bjfxy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ovs.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qfg.316326.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wzu.bbcook.cn

C#:   s.Replace("a", "b")
来源：http://zvk.chenjidiqi.icu

[E07] 按分隔符拆分
来源：http://oqy.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hvr.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ypm.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jkn.ctjpmb.com

TS:   s.split(",")
来源：http://brw.tarul.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ehw.gaohongyu789.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://giu.havefunace.top

Ruby: s.split(",");  s.split
来源：http://ybp.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://noj.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://ztl.sweek.top

Py:   ",".join(items)
来源：http://sks.dashuyun.cn

PHP:  implode(",", $items);
来源：http://onv.vqdsnc.cn

JS:   items.join(",")
来源：http://ngc.kuanghao11.cn

TS:   items.join(",")
来源：http://npf.feifeiyinyue.top

Java: String.join(",", items)
来源：http://zkt.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://byy.daxiang520.top

Ruby: items.join(",")
来源：http://eam.ybcxt.top

C#:   string.Join(",", items)
来源：http://vxi.yueranfly.top

[E09] 去除所有空白字符
来源：http://uvu.bjfxy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bcq.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nir.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://via.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://uwj.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://vtx.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://qlx.yj20258.top

Ruby: s.gsub(/\s+/, "")
来源：http://eiy.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mey.shangyingyoupin.top

[E10] 左侧补零 / 定长填充
来源：http://frj.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ame.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uxw.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://arr.9152youxi.cn

TS:   "7".padStart(3, "0")
来源：http://vlk.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://tuz.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://rho.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zdy.zhengqikj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://csn.shangyingyoupin.top

[E11] 反转字符串
来源：http://unj.ybcxt.top

Py:   s[::-1]
来源：http://bse.jyoumei.cn

PHP:  strrev($s);
来源：http://nfi.vqdsnc.cn

JS:   [...s].reverse().join("")
来源：http://eie.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://alu.zhijiandao.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pvz.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rly.wangdashe.top

Ruby: s.reverse
来源：http://yhy.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://pey.shuidangran.top

[E12] 统计某字符出现次数
来源：http://nhu.hongshengwenyu.top

Py:   s.count("a")
来源：http://jrw.yj20258.top

PHP:  substr_count($s, "a");
来源：http://mji.fzhhl.top

JS:   s.split("a").length - 1
来源：http://yah.xylfe.cn

TS:   s.split("a").length - 1
来源：http://ztc.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://upt.wangshuangyany.cn

Go:   strings.Count(s, "a")
来源：http://bzk.ivvv.top

Ruby: s.count("a")
来源：http://coe.shanyushiyangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://nmn.epnwcf.com

[E13] 逐字符遍历
来源：http://hgq.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://jvw.chenjidiqi.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wtm.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dlu.nwbrower.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ooy.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zcj.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nqp.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kjs.jinqigfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xyf.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://dme.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qdn.nanxinkj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hzg.yj20258.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kwl.daria6918.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zfb.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qmj.xinyue.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uxk.zhoulong.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aby.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mvg.vehdjk.com

[E15] HTML 转义 / 反转义
来源：http://ids.meibo888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jmg.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://duw.xuetiantiany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bnl.ywan-chungtsiang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rvy.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://isa.316326.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vjo.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yqr.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jmd.hcnkem.com

[E16] 数字千分位
来源：http://osg.fengsongda.top

Py:   f"{1234567:,}"
来源：http://rrr.wangdashe.top

PHP:  number_format(1234567);
来源：http://zyt.smart0.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://enn.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://elv.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qyw.dashuyun.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kln.jiagoushi.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://snz.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://nsb.9152youxi.cn

[E17] 首字母大写
来源：http://xtb.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uuf.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tza.dianchejie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cow.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hhp.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ica.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zvt.zhengqikj.top

Ruby: s.capitalize
来源：http://ddi.ywan-chungtsiang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rum.shuidangran.top

[E18] 模板占位符替换
来源：http://rwb.zhixingplan.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dtt.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ijv.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://okn.316326.xyz


<!-- 参考信息 -->