代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ldi.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nlk.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uew.snrcjt.cn

Go:   slices.Index(arr, x)
来源：http://dki.wangshuangyany.cn

Ruby: arr.index(x)
来源：http://zkv.birdmap.top

C#:   list.IndexOf(x);
来源：http://phi.daria6918.cn

[D13] 过滤（保留满足条件的）
来源：http://uns.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zxh.xylfe.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ugv.sxryk.cn

JS:   arr.filter(x => x > 3)
来源：http://ftk.jlsjyb.cn

TS:   arr.filter(x => x > 3)
来源：http://ynw.daxiang520.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://djt.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hzo.yonumen.top

Ruby: arr.select { |x| x > 3 }
来源：http://pzn.ctjpmb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://cde.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://cbe.meibo888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vjo.guannengcc.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pkr.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://xfm.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://blr.ywan-chungtsiang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bwq.jqgufenzy.top

Go:   // 手写循环
来源：http://bmd.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://nba.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rvq.chenzaomai.com

[D15] 去重
来源：http://hqb.jqgfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ddu.sufxvd.cn

PHP:  array_unique($arr);
来源：http://fjm.jqgfzy.top

JS:   [...new Set(arr)]
来源：http://pwn.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://rdz.meibo888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vof.wangdashe.top

Go:   // 用 map[T]struct{} 手写
来源：http://iyy.havefunace.top

Ruby: arr.uniq
来源：http://tal.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://bdu.dianchejie.cn

[D16] 求和与平均值
来源：http://dmc.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uwj.cqqwz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zbt.yonumen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kto.jqgfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://scc.pengpengdd.cyou

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sbc.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://jff.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uzd.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://jod.yueranfly.top

[D17] 最大值与最小值
来源：http://cfp.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://nte.vqdsnc.cn

PHP:  max($arr);  min($arr);
来源：http://ank.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ymj.9152youxi.cn

TS:   Math.max(...arr);
来源：http://ohx.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mny.ehwqpu.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fyp.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://zur.xuetiantiany.cn

C#:   list.Max();  list.Min()
来源：http://ekt.xuetiantiany.cn

[D18] 扁平化嵌套数组
来源：http://dub.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lnh.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://vap.0kj1m.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ngi.vehdjk.com

TS:   nested.flat();
来源：http://jny.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ips.uphjek.com

Go:   // 手写双层循环
来源：http://vrf.yj202588.top

Ruby: nested.flatten
来源：http://zlv.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fos.guowangkeji.top

[D19] 按字段分组
来源：http://lmk.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mvb.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ild.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qtd.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mew.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qkm.zhoulong.xyz

Go:   // 手写 map[string][]T
来源：http://lpn.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bne.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kro.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://hsy.yfazqb.com

Py:   Counter(arr)
来源：http://ccn.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://dij.dianchejie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jcm.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dpz.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eia.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://xfy.yongpay.top

Ruby: arr.tally
来源：http://hzh.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ilr.cdnleiting.top

[D21] 判断是否包含某元素
来源：http://rdy.iojbl.cn

Py:   x in arr
来源：http://iig.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://iot.hongshengwenyu.top

JS:   arr.includes(x)
来源：http://nnx.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://ttb.tanke756.top

Java: list.contains(x)
来源：http://pmk.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://qxl.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://vgv.zhiwuduotai.top

C#:   list.Contains(x)
来源：http://qbv.zhijiandao.cn

[D22] 复制数组（避免共享引用）
来源：http://prn.guowangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://btc.sysykeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://trc.hnqzz.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jfs.smart0.xyz

TS:   [...arr];
来源：http://dow.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://kbk.snrcjt.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uio.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://fzt.jianghu66.top

C#:   new List<int>(list);
来源：http://ofy.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://dyy.yvedp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://roe.c1oappe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rdv.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ohu.havefunace.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vog.xingfuxueyuan.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://rdt.havefunace.top

Go:   // 手写循环
来源：http://gak.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sgd.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cgk.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://oje.xylfe.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://whr.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gsb.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://inw.fehbvm.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dlc.chenlongwang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sco.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kda.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jqp.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ely.ybcxt.top

[D25] Set 集合去重与交并差
来源：http://xxe.sjlbkw.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xfa.fengsongda.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tek.mhx1999.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yag.zycfv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vnw.sweek.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dpz.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vpt.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bug.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vis.chenjidiqi.icu

[D26] 数组转字符串
来源：http://lsi.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://vbf.hnqzz.top

PHP:  implode(", ", $arr);
来源：http://sna.jlsjyb.cn

JS:   arr.join(", ")
来源：http://tvd.nanxuanxn.top

TS:   arr.join(", ")
来源：http://wka.wangdashe.top

Java: String.join(", ", list)
来源：http://oru.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://ahh.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://kpg.cucudq.cn

C#:   string.Join(", ", list)
来源：http://ims.ywan-chungtsiang.top

================================================================================
来源：http://umk.andypj.xyz

E. 字符串处理
来源：http://bjg.tarul.cn

================================================================================
来源：http://fxf.iojbl.cn

[E01] 拼接字符串
来源：http://ymw.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pgj.bjfxy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tqk.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://urf.nanxinkj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hko.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wst.gzhubu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qfz.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hug.sjlbkw.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kde.hongshengwenyu.top

[E02] 重复字符串
来源：http://hqy.xuetiantiany.cn

Py:   "ab" * 3
来源：http://hwc.cqqwz.cn

PHP:  str_repeat("ab", 3);
来源：http://hvf.yfazqb.com

JS:   "ab".repeat(3)
来源：http://jad.vqdsnc.cn

TS:   "ab".repeat(3)
来源：http://nmp.epnwcf.com

Java: "ab".repeat(3)
来源：http://ozl.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://ynb.ybcxt.top

Ruby: "ab" * 3
来源：http://aoh.sjlbkw.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zfj.ehwqpu.com

[E03] 截取子串
来源：http://quh.ivvv.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ynz.yfazqb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mzg.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ttp.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://uio.jinqigufen.top

Java: s.substring(1, 4)
来源：http://syu.cheryme.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oez.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://cqn.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://hlw.fengsongda.top

[E04] 查找子串位置
来源：http://ovw.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://dgs.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://zma.fanxiaobao.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gld.316326.xyz

TS:   s.indexOf("x")
来源：http://ptn.tianlin.xyz

Java: s.indexOf("x")
来源：http://lrp.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://aav.cdnleiting.top

Ruby: s.index("x")
来源：http://gve.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://dva.hcnkem.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://ffc.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vkp.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xyc.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kwl.jinqigfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tew.redwolf501.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hsm.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tsp.yanxiufei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bfc.shanyushiyangtech.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bcc.jiagoushi.top

[E06] 替换子串
来源：http://dpj.zhongyouzk.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bbn.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://swp.yanxiufei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://buk.epnwcf.com

TS:   s.replaceAll("a", "b")
来源：http://ftk.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zyj.ctjpmb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ezq.sweek.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qld.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://ora.nwbrower.top

[E07] 按分隔符拆分
来源：http://kxx.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://khm.jlsjyb.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tio.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bgl.yanxiufei.cn

TS:   s.split(",")
来源：http://hui.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://tro.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tdq.dashuyun.cn

Ruby: s.split(",");  s.split
来源：http://qeb.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gov.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://nzy.hysaishi.cn

Py:   ",".join(items)
来源：http://zss.sysykeji.top

PHP:  implode(",", $items);
来源：http://pfn.zhengqikj.top

JS:   items.join(",")
来源：http://vwn.wangdashe.top

TS:   items.join(",")
来源：http://cjc.daxiang520.top

Java: String.join(",", items)
来源：http://vea.c1oappe.top

Go:   strings.Join(items, ",")
来源：http://dft.tanke756.top

Ruby: items.join(",")
来源：http://mdg.sufxvd.cn

C#:   string.Join(",", items)
来源：http://skd.pycfn.com

[E09] 去除所有空白字符
来源：http://tcn.chenjidiqi.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eej.guannengcc.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zou.aizwys.cn

JS:   s.replace(/\s+/g, "")
来源：http://htd.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://ett.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://hkf.hammf.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ssv.jinyuanbaomall.cn

Ruby: s.gsub(/\s+/, "")
来源：http://big.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kcw.nanxinkj.top

[E10] 左侧补零 / 定长填充
来源：http://aqc.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://shm.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mra.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://vmc.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://jwc.jiagoushi.top

Java: String.format("%03d", 7)
来源：http://kpb.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ihl.cucudq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fxr.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cyo.sufxvd.cn

[E11] 反转字符串
来源：http://qbw.zhoulong.xyz

Py:   s[::-1]
来源：http://otx.zhongyouzk.top

PHP:  strrev($s);
来源：http://tnl.epnwcf.com

JS:   [...s].reverse().join("")
来源：http://cqh.cashguo.top

TS:   [...s].reverse().join("")
来源：http://xbn.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wos.jyoumei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://aio.cheryme.top

Ruby: s.reverse
来源：http://zhl.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://xor.tarul.cn

[E12] 统计某字符出现次数
来源：http://tcr.hnxiangtu.top

Py:   s.count("a")
来源：http://bgf.zdqjudy.top

PHP:  substr_count($s, "a");
来源：http://lbq.xuanzx.com

JS:   s.split("a").length - 1
来源：http://mkb.ivvv.top

TS:   s.split("a").length - 1
来源：http://ssj.fzhhl.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://btu.yangfankeji.com

Go:   strings.Count(s, "a")
来源：http://cfw.hywenlv.cn

Ruby: s.count("a")
来源：http://ypo.yueranfly.top

C#:   s.Count(c => c == 'a')
来源：http://kon.smart0.xyz

[E13] 逐字符遍历
来源：http://hzz.zhongyouzk.top

Py:   for ch in s: print(ch)
来源：http://pip.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://phl.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ayc.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://klw.kuanghao11.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://apc.xziqi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dba.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hpz.hnxiangtu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nql.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://gbi.xinyue.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fiw.cashguo.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hqj.fktsv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qez.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wcd.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dgt.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jim.jinqigufen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dxs.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ras.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://agu.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vdk.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dxd.jyoumei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xjc.cucudq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iis.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ppz.jinghuilouyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wuh.hammf.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vbx.yfazqb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xxi.zhengqikj.top

[E16] 数字千分位
来源：http://uky.xuetiantiany.cn

Py:   f"{1234567:,}"
来源：http://aqi.zhongyouzk.top

PHP:  number_format(1234567);
来源：http://tab.zdbjq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gto.jianghu66.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nyw.yvedp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wzq.zhixingplan.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bau.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mpq.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://yox.wangdashe.top

[E17] 首字母大写
来源：http://yza.kuanghao11.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fdd.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://zjk.sxryk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tfe.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://guc.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vrh.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dfe.jianghu66.top

Ruby: s.capitalize
来源：http://lsu.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xaa.zhaomingkeji.xyz

[E18] 模板占位符替换
来源：http://qbw.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vqj.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tqc.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uzh.zhoulong.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://txl.hesvh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pco.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gsx.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qpl.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jgz.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://uuh.ehwqpu.com

Py:   s.splitlines()
来源：http://dyp.zhiwuduotai.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://diw.smart0.xyz


<!-- 参考信息 -->