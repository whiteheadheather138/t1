代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pun.zdqjudy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://muv.tarul.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://obc.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://hac.yj20258888.top

Ruby: arr.index(x)
来源：http://tgm.ydjk.org.cn

C#:   list.IndexOf(x);
来源：http://wky.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://nuu.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fxz.jinqigfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cvn.zhijiandao.cn

JS:   arr.filter(x => x > 3)
来源：http://eih.tian-w.cn

TS:   arr.filter(x => x > 3)
来源：http://erx.ywan-chungtsiang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xsa.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vsk.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://qqu.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nnq.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://tyw.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aqb.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://smi.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://txv.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://scy.sjlbkw.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://huf.yueranfly.top

Go:   // 手写循环
来源：http://mgc.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xpv.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ftq.guowangkeji.top

[D15] 去重
来源：http://fsi.zdqjudy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mpm.xziqi.cn

PHP:  array_unique($arr);
来源：http://uxr.sxryk.cn

JS:   [...new Set(arr)]
来源：http://qdl.havefunace.top

TS:   [...new Set(arr)]
来源：http://zla.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ifb.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bfn.zdqjudy.top

Ruby: arr.uniq
来源：http://xrw.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://uin.vehdjk.com

[D16] 求和与平均值
来源：http://ers.fzhhl.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://njw.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://faw.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://whv.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ojb.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://caw.snrcjt.cn

Go:   // 手写循环累加
来源：http://ozo.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uqz.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://sed.jlsjyb.cn

[D17] 最大值与最小值
来源：http://dbg.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://icg.yfazqb.com

PHP:  max($arr);  min($arr);
来源：http://joy.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jgf.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://dnk.xuetiantiany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vdn.havefunace.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nxa.yuanzhike.top

Ruby: arr.max;  arr.min
来源：http://dyp.xuanzx.com

C#:   list.Max();  list.Min()
来源：http://lpz.jinqigfzy.top

[D18] 扁平化嵌套数组
来源：http://xdj.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fgv.bbcook.cn

PHP:  array_merge(...$nested);
来源：http://eyy.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jyq.sxryk.cn

TS:   nested.flat();
来源：http://kra.ywan-chungtsiang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://egk.jinghuilouyu.cn

Go:   // 手写双层循环
来源：http://zis.feifeiyinyue.top

Ruby: nested.flatten
来源：http://qzr.sysykeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dvb.gzhubu.top

[D19] 按字段分组
来源：http://jpe.ppjwa.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://htq.yj202588.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lru.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jci.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://miy.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://upv.xuanzx.com

Go:   // 手写 map[string][]T
来源：http://amx.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hdc.sjlbkw.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mft.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://drf.zhoulong.xyz

Py:   Counter(arr)
来源：http://vdh.jyoumei.cn

PHP:  array_count_values($arr);
来源：http://lmz.c1oappe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://htc.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nog.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vvo.meibo888.top

Go:   // 手写 map[T]int
来源：http://edv.havefunace.top

Ruby: arr.tally
来源：http://fie.zycfv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oni.daxiang520.top

[D21] 判断是否包含某元素
来源：http://oog.yueranfly.top

Py:   x in arr
来源：http://rbs.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://snr.jiagoushi.top

JS:   arr.includes(x)
来源：http://rhe.shanyushiyangkeji.top

TS:   arr.includes(x)
来源：http://pjo.cqqwz.cn

Java: list.contains(x)
来源：http://sio.sysykeji.top

Go:   slices.Contains(arr, x)
来源：http://ljk.sweek.top

Ruby: arr.include?(x)
来源：http://flq.sweek.top

C#:   list.Contains(x)
来源：http://sho.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://erw.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cza.uphjek.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rup.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qsy.daxiang520.top

TS:   [...arr];
来源：http://ghh.yuanzhike.top

Java: new ArrayList<>(list);
来源：http://kok.aizwys.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pmr.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://bie.tianlin.xyz

C#:   new List<int>(list);
来源：http://mqk.daria6918.cn

[D23] reduce 累积计算
来源：http://mui.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xbu.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://omw.tarul.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wdn.yonumen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://isw.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ait.pycfn.com

Go:   // 手写循环
来源：http://rig.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cmc.yj202588.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iiy.wangdashe.top

[D24] 字典 / Map 基本操作
来源：http://auy.yuanzhike.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oor.yueranfly.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://erg.vehdjk.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bur.cheryme.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jne.quarkkingdee.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iva.sweek.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://idj.jiagoushi.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tjo.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nlu.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://tze.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mcl.hnxiangtu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qzv.uphjek.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vpe.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dxr.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ahv.hesvh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qlj.zhixingplan.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jeb.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tzr.gogol.net.cn

[D26] 数组转字符串
来源：http://vwi.shuidangran.top

Py:   ", ".join(map(str, arr))
来源：http://ymd.guannengcc.top

PHP:  implode(", ", $arr);
来源：http://vgn.pycfn.com

JS:   arr.join(", ")
来源：http://vdd.zhengqikj.top

TS:   arr.join(", ")
来源：http://xjw.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://lrs.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://adp.hammf.cn

Ruby: arr.join(", ")
来源：http://nba.dianchejie.cn

C#:   string.Join(", ", list)
来源：http://tsk.hcnkem.com

================================================================================
来源：http://wnb.gotoacloud.top

E. 字符串处理
来源：http://erg.havefunace.top

================================================================================
来源：http://rkp.cqqwz.cn

[E01] 拼接字符串
来源：http://ucz.tarul.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iol.yj20258.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ytr.tanke756.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wil.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xjt.fktsv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vwl.jyoumei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jpc.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ozu.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xwe.ehwqpu.com

[E02] 重复字符串
来源：http://kjy.gzhubu.top

Py:   "ab" * 3
来源：http://dmm.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://aym.epnwcf.com

JS:   "ab".repeat(3)
来源：http://dne.yuxming.cn

TS:   "ab".repeat(3)
来源：http://nyl.9152youxi.cn

Java: "ab".repeat(3)
来源：http://ohq.smart0.xyz

Go:   strings.Repeat("ab", 3)
来源：http://ofs.ydzc1.top

Ruby: "ab" * 3
来源：http://zqp.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sqm.gaohongyu789.top

[E03] 截取子串
来源：http://sdi.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jet.fanxiaobao.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://thf.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fuk.pycfn.com

TS:   s.slice(1, 4)
来源：http://jkk.hysaishi.cn

Java: s.substring(1, 4)
来源：http://ujj.zhengqikj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fnb.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://rav.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://viq.jqgfzy.top

[E04] 查找子串位置
来源：http://dgn.bjfxy.top

Py:   s.find("x");  s.index("x")
来源：http://iph.havefunace.top

PHP:  strpos($s, "x");
来源：http://jcs.ywan-chungtsiang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://axq.guannengcc.top

TS:   s.indexOf("x")
来源：http://hxt.xinyue.icu

Java: s.indexOf("x")
来源：http://lzz.tanke756.top

Go:   strings.Index(s, "x")
来源：http://ofb.tianlin.xyz

Ruby: s.index("x")
来源：http://kux.yj202588.top

C#:   s.IndexOf("x")
来源：http://axt.vqdsnc.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gbx.9152youxi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://syl.9152youxi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sja.guannengcc.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mqg.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://zxg.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://esh.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://glf.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zny.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://afq.ydjk.org.cn

[E06] 替换子串
来源：http://tzb.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://crh.hongshengwenyu.top

PHP:  str_replace("a", "b", $s);
来源：http://vga.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://arn.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://uhu.xziqi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ast.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hsw.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://evk.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://bkn.tian-w.cn

[E07] 按分隔符拆分
来源：http://ydv.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ygo.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qpt.9152youxi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rsm.fanxiaobao.xyz

TS:   s.split(",")
来源：http://ump.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://sgq.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pwb.yueranfly.top

Ruby: s.split(",");  s.split
来源：http://uvl.cqqwz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cwk.jianghu66.top

[E08] 数组按分隔符合并
来源：http://lmb.aizwys.cn

Py:   ",".join(items)
来源：http://dxq.jqgfzy.top

PHP:  implode(",", $items);
来源：http://fqf.nanxuanxn.top

JS:   items.join(",")
来源：http://iou.guowangkeji.top

TS:   items.join(",")
来源：http://agh.yangfankeji.com

Java: String.join(",", items)
来源：http://get.aizwys.cn

Go:   strings.Join(items, ",")
来源：http://aer.svipenyu.cn

Ruby: items.join(",")
来源：http://jct.vehdjk.com

C#:   string.Join(",", items)
来源：http://ilp.hysaishi.cn

[E09] 去除所有空白字符
来源：http://rrd.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dak.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://anw.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://twb.havefunace.top

TS:   s.replace(/\s+/g, "")
来源：http://snd.ydzc1.top

Java: s.replaceAll("\\s+", "")
来源：http://kdl.iojbl.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tzx.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://khf.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://efr.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://cks.zdqjudy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mxw.meibo888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hqr.hysaishi.cn

JS:   "7".padStart(3, "0")
来源：http://ono.daxiang520.top

TS:   "7".padStart(3, "0")
来源：http://hgx.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://otc.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cnd.xuetiantiany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vkp.tianlin.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jum.nanxuanxn.top

[E11] 反转字符串
来源：http://uze.yanxiufei.cn

Py:   s[::-1]
来源：http://zxr.sxryk.cn

PHP:  strrev($s);
来源：http://axu.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://izj.cdnleiting.top

TS:   [...s].reverse().join("")
来源：http://ghw.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rlm.sufxvd.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://duc.zhengqikj.top

Ruby: s.reverse
来源：http://tgb.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://twy.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://wll.sweek.top

Py:   s.count("a")
来源：http://xoq.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://qde.bbcook.cn

JS:   s.split("a").length - 1
来源：http://mwi.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://zsc.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vls.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://mot.cdnleiting.top

Ruby: s.count("a")
来源：http://cog.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://ead.dianchejie.cn

[E13] 逐字符遍历
来源：http://jqo.hongshengwenyu.top

Py:   for ch in s: print(ch)
来源：http://gbn.pengpengdd.cyou

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fwt.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pyg.0kj1m.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zho.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cyc.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kyt.shanyushiyangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nry.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zvv.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://phy.cdnleiting.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nyg.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fnk.andypj.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jxd.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://laz.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://abo.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gdh.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://acx.zhijiandao.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qni.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://gch.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vue.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cpl.shanyushiyangtech.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hef.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://thh.iojbl.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rzx.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jxk.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ryg.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ztq.ctjpmb.com

[E16] 数字千分位
来源：http://qbi.yj202588.top

Py:   f"{1234567:,}"
来源：http://ubs.birdmap.top

PHP:  number_format(1234567);
来源：http://awv.zhixingplan.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xkx.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://oqm.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pnv.svipenyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lhs.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cyk.havefunace.top

C#:   1234567.ToString("N0")
来源：http://dvq.xylfe.cn

[E17] 首字母大写
来源：http://gqj.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ywo.52xcode.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tsj.shangyingyoupin.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://urm.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cds.ctjpmb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://otz.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zbh.kuanghao11.cn

Ruby: s.capitalize
来源：http://xyh.shuidangran.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dnt.zhengqikj.top

[E18] 模板占位符替换
来源：http://auk.dashuyun.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pig.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cct.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://umo.yvedp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bod.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mcf.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ens.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ode.xingfuxueyuan.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zmj.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://sok.yj202588.top

Py:   s.splitlines()
来源：http://fxp.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jnz.wangdashe.top


<!-- 参考信息 -->