代发 wailian999

Ruby: arr.index(x)
来源：http://trn.ydjk.org.cn

C#:   list.IndexOf(x);
来源：http://mnl.nwbrower.top

[D13] 过滤（保留满足条件的）
来源：http://kju.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://acv.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://unv.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://dun.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://vjf.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ydi.shanyushiyangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vpp.52xcode.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jwd.shangyingyoupin.top

C#:   list.Where(x => x > 3).ToList()
来源：http://smg.daria6918.cn

[D14] 映射转换（每个元素变形）
来源：http://axd.nanxinkj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://unv.yuxming.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ham.sweek.top

JS:   arr.map(x => x * 2)
来源：http://eio.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://lqu.hfpthk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lkb.sxryk.cn

Go:   // 手写循环
来源：http://cea.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://gdf.0kj1m.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uej.hcnkem.com

[D15] 去重
来源：http://rjd.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://agv.316326.xyz

PHP:  array_unique($arr);
来源：http://dhh.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://jas.sweek.top

TS:   [...new Set(arr)]
来源：http://pma.jianghu66.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zca.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://att.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://fen.cdnleiting.top

C#:   list.Distinct().ToList()
来源：http://dif.cheryme.top

[D16] 求和与平均值
来源：http://cha.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hsn.chenzaomai.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ceo.hongshengwenyu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mwd.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uif.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vwu.gotoacloud.top

Go:   // 手写循环累加
来源：http://gav.shzxlz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xps.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://bbn.sweek.top

[D17] 最大值与最小值
来源：http://ihw.yfazqb.com

Py:   max(arr);  min(arr)
来源：http://jwd.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://vcf.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ktp.daria6918.cn

TS:   Math.max(...arr);
来源：http://fob.zhiwuduotai.top

Java: Collections.max(list);  Collections.min(list);
来源：http://adv.jqgufenzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jka.jinghuilouyu.cn

Ruby: arr.max;  arr.min
来源：http://yjb.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://zyo.xuanzx.com

[D18] 扁平化嵌套数组
来源：http://zep.sysykeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pjy.gogol.net.cn

PHP:  array_merge(...$nested);
来源：http://edv.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zak.havefunace.top

TS:   nested.flat();
来源：http://vtr.feifeiyinyue.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://aif.bjfxy.top

Go:   // 手写双层循环
来源：http://mds.tianlin.xyz

Ruby: nested.flatten
来源：http://yeh.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dwb.hnqzz.top

[D19] 按字段分组
来源：http://vwz.tianlin.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://brc.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oqf.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aax.guowangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uoh.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ubu.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://cmz.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jme.vqdsnc.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ydb.sufxvd.cn

[D20] 统计每个元素出现次数
来源：http://zcf.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://gyz.aizwys.cn

PHP:  array_count_values($arr);
来源：http://fqu.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://slg.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fkv.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://scs.zhaomingkeji.xyz

Go:   // 手写 map[T]int
来源：http://rnu.gogol.net.cn

Ruby: arr.tally
来源：http://lik.daria6918.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eru.ydjk.org.cn

[D21] 判断是否包含某元素
来源：http://fnn.haohaochexian.top

Py:   x in arr
来源：http://zza.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://hsl.zhongyouzk.top

JS:   arr.includes(x)
来源：http://byn.snrcjt.cn

TS:   arr.includes(x)
来源：http://ifs.9152youxi.cn

Java: list.contains(x)
来源：http://psf.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://fcj.jinqigufen.top

Ruby: arr.include?(x)
来源：http://xkx.hfpthk.cn

C#:   list.Contains(x)
来源：http://nuf.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://nhj.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dms.hnqzz.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ymh.tianlin.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gbd.shanyushiyangtech.top

TS:   [...arr];
来源：http://cds.havefunace.top

Java: new ArrayList<>(list);
来源：http://fry.fanxiaobao.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://wnf.xylfe.cn

Ruby: arr.dup;  arr.clone
来源：http://bsg.52xcode.cn

C#:   new List<int>(list);
来源：http://acz.pengpengdd.cyou

[D23] reduce 累积计算
来源：http://orw.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nnx.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bjb.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qwp.feifeiyinyue.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://exu.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://csh.cqqwz.cn

Go:   // 手写循环
来源：http://lid.ctjpmb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uos.zhiwuduotai.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://inm.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://ewj.xinyue.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vmu.zhaomingkeji.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://abw.hnqzz.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nzb.zhijiandao.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://plx.zycfv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iwa.gzhubu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mfw.quarkkingdee.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mmn.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oil.hfpthk.cn

[D25] Set 集合去重与交并差
来源：http://fhc.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gag.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hmg.daxiang520.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qgo.hcnkem.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dsp.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nje.nwbrower.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gnk.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://efg.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hqt.yvedp.cn

[D26] 数组转字符串
来源：http://cwa.snrcjt.cn

Py:   ", ".join(map(str, arr))
来源：http://mye.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://ejg.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://svh.sysykeji.top

TS:   arr.join(", ")
来源：http://jwz.yj20258.top

Java: String.join(", ", list)
来源：http://zbh.nwbrower.top

Go:   strings.Join(strs, ", ")
来源：http://hgb.shzxlz.cn

Ruby: arr.join(", ")
来源：http://gzf.tian-w.cn

C#:   string.Join(", ", list)
来源：http://kgg.xingfuxueyuan.xyz

================================================================================
来源：http://azn.jianghu66.top

E. 字符串处理
来源：http://rnt.shanyushiyangkeji.top

================================================================================
来源：http://qcb.sxryk.cn

[E01] 拼接字符串
来源：http://fcq.hysaishi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gxq.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tnm.hongshengwenyu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cpe.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://spe.jiagoushi.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pzk.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ewf.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mmq.iojbl.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qab.meibo888.top

[E02] 重复字符串
来源：http://baf.xuetiantiany.cn

Py:   "ab" * 3
来源：http://itn.hnqzz.top

PHP:  str_repeat("ab", 3);
来源：http://lmi.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://tir.havefunace.top

TS:   "ab".repeat(3)
来源：http://vno.yuxming.cn

Java: "ab".repeat(3)
来源：http://ryj.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://ooo.jqgufenzy.top

Ruby: "ab" * 3
来源：http://lqr.ydzc1.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wzg.c1oappe.top

[E03] 截取子串
来源：http://rhd.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ryz.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://juk.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ufo.daxiang520.top

TS:   s.slice(1, 4)
来源：http://vrw.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://gzd.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pye.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bci.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://tpi.hammf.cn

[E04] 查找子串位置
来源：http://pob.xziqi.cn

Py:   s.find("x");  s.index("x")
来源：http://yzv.yj20258.top

PHP:  strpos($s, "x");
来源：http://weg.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gqd.tanke756.top

TS:   s.indexOf("x")
来源：http://ymr.hnqzz.top

Java: s.indexOf("x")
来源：http://scz.pycfn.com

Go:   strings.Index(s, "x")
来源：http://xbm.hnqzz.top

Ruby: s.index("x")
来源：http://tww.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://zdu.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://eeg.quarkkingdee.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ugy.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ets.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fou.vqdsnc.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mbf.iojbl.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fho.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uab.yanxiufei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nvm.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dgb.ywan-chungtsiang.top

[E06] 替换子串
来源：http://lao.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xwr.vehdjk.com

PHP:  str_replace("a", "b", $s);
来源：http://wjw.daria6918.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tvl.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://bvq.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://amn.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dbc.epnwcf.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qki.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://qrv.jinqigufen.top

[E07] 按分隔符拆分
来源：http://xrc.fanxiaobao.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://koq.hcnkem.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://leq.xylfe.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oyy.quarkkingdee.top

TS:   s.split(",")
来源：http://ezb.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://szm.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zzv.pycfn.com

Ruby: s.split(",");  s.split
来源：http://jhq.quarkkingdee.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://smk.fehbvm.com

[E08] 数组按分隔符合并
来源：http://jzm.yj202588.top

Py:   ",".join(items)
来源：http://eyw.hesvh.cn

PHP:  implode(",", $items);
来源：http://rxx.hesvh.cn

JS:   items.join(",")
来源：http://dcr.zhaomingkeji.xyz

TS:   items.join(",")
来源：http://boe.hysaishi.cn

Java: String.join(",", items)
来源：http://mvp.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://aaa.vehdjk.com

Ruby: items.join(",")
来源：http://mga.bbcook.cn

C#:   string.Join(",", items)
来源：http://zjs.jyoumei.cn

[E09] 去除所有空白字符
来源：http://yxm.dianchejie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vfs.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dsk.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://oug.ehwqpu.com

TS:   s.replace(/\s+/g, "")
来源：http://zpk.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://pmc.xinyue.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://zrx.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://hzi.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sqa.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://sfg.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nbj.gzhubu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vks.nanxuanxn.top

JS:   "7".padStart(3, "0")
来源：http://nll.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://yjr.ivvv.top

Java: String.format("%03d", 7)
来源：http://fzx.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qmc.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rft.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fjm.tanke756.top

[E11] 反转字符串
来源：http://ylq.redwolf501.top

Py:   s[::-1]
来源：http://xla.dianchejie.cn

PHP:  strrev($s);
来源：http://acc.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://pcv.wangdashe.top

TS:   [...s].reverse().join("")
来源：http://bgw.bjfxy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vqu.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://eoj.daxiang520.top

Ruby: s.reverse
来源：http://xyn.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://plm.yvedp.cn

[E12] 统计某字符出现次数
来源：http://zft.ydzc1.top

Py:   s.count("a")
来源：http://fwm.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://pro.zdqjudy.top

JS:   s.split("a").length - 1
来源：http://deo.zdqjudy.top

TS:   s.split("a").length - 1
来源：http://hji.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://puv.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://vfr.kuanghao11.cn

Ruby: s.count("a")
来源：http://mxw.bbcook.cn

C#:   s.Count(c => c == 'a')
来源：http://mcs.fzhhl.top

[E13] 逐字符遍历
来源：http://wka.sysykeji.top

Py:   for ch in s: print(ch)
来源：http://jkm.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ceb.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vqj.shzxlz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://imr.zdbjq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wfn.hcnkem.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cwy.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ngd.xingfuxueyuan.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://onn.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://txo.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lwe.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ehi.guowangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ywh.wangshuangyany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oal.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ecq.chenzaomai.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://guf.gogol.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gxe.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rrx.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://xop.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ugp.dianchejie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uba.zhoulong.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qzg.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fim.dianchejie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hij.nanxuanxn.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uam.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mui.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ndk.shanyushiyangtech.top

[E16] 数字千分位
来源：http://kez.yvedp.cn

Py:   f"{1234567:,}"
来源：http://wuc.zhixingplan.top

PHP:  number_format(1234567);
来源：http://tqd.tanke756.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fvk.zdqjudy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mwx.havefunace.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dwj.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nmv.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://niv.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://ond.yuanzhike.top

[E17] 首字母大写
来源：http://kxo.fengsongda.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://brj.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ubs.vehdjk.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bbj.sjlbkw.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://udm.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qup.hnqzz.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fwn.aibaodan.cn

Ruby: s.capitalize
来源：http://rgh.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aex.yanxiufei.cn

[E18] 模板占位符替换
来源：http://and.cdnleiting.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ifz.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://edo.aizwys.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nez.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jhy.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wnt.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dkc.shuidangran.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fec.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lfa.yueranfly.top

[E19] 多行文本按行拆分
来源：http://aaw.bjfxy.top

Py:   s.splitlines()
来源：http://gfp.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wia.shangyingyoupin.top

JS:   s.split(/\r?\n/)
来源：http://xdy.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://hwi.cucudq.cn

Java: s.lines().toList()
来源：http://dod.aibaodan.cn

Go:   strings.Split(s, "\n")
来源：http://ynr.hammf.cn


<!-- 参考信息 -->