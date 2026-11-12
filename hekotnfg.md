代发 wailian999

Ruby: arr.index(x)
来源：http://rhu.fzhhl.top

C#:   list.IndexOf(x);
来源：http://dvg.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://nfd.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://adp.jinqigfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://upr.zhixingplan.top

JS:   arr.filter(x => x > 3)
来源：http://aea.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://wdr.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pru.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kxm.shanyushiyangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://kca.cqqwz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hbn.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://xmi.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qgn.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xck.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://lci.vqdsnc.cn

TS:   arr.map(x => x * 2)
来源：http://dhm.xinyue.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://bvg.ivvv.top

Go:   // 手写循环
来源：http://tqi.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://kme.hnqzz.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fbl.haohaochexian.top

[D15] 去重
来源：http://vkg.yfazqb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yfb.xinyue.icu

PHP:  array_unique($arr);
来源：http://ocj.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://ctv.haohaochexian.top

TS:   [...new Set(arr)]
来源：http://aek.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://aiz.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://hqr.0kj1m.cn

Ruby: arr.uniq
来源：http://iev.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://yfh.ydjk.org.cn

[D16] 求和与平均值
来源：http://zaf.nanxuanxn.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dbi.ehwqpu.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jws.cucudq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hto.yangfankeji.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rpe.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jsy.gogol.net.cn

Go:   // 手写循环累加
来源：http://mam.jyoumei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://plc.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://isj.hesvh.cn

[D17] 最大值与最小值
来源：http://xfx.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://tjh.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://ggo.ehwqpu.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kbl.uphjek.com

TS:   Math.max(...arr);
来源：http://mma.yfazqb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://qld.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://epo.ehwqpu.com

Ruby: arr.max;  arr.min
来源：http://ucr.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://qet.hfpthk.cn

[D18] 扁平化嵌套数组
来源：http://hxg.shzxlz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gsw.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://hym.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ksn.jianghu66.top

TS:   nested.flat();
来源：http://ijp.yuxming.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tav.tarul.cn

Go:   // 手写双层循环
来源：http://snh.yongpay.top

Ruby: nested.flatten
来源：http://qdo.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ptn.cdnleiting.top

[D19] 按字段分组
来源：http://fkt.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://edi.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rvb.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xzo.meibo888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://myz.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aij.hysaishi.cn

Go:   // 手写 map[string][]T
来源：http://thu.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://oqy.yj20258888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rhl.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://vot.chenzaomai.com

Py:   Counter(arr)
来源：http://khj.0kj1m.cn

PHP:  array_count_values($arr);
来源：http://ktj.sjlbkw.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xjk.jqgufenzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zgm.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ftv.ybcxt.top

Go:   // 手写 map[T]int
来源：http://crs.yonumen.top

Ruby: arr.tally
来源：http://xjg.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://waz.vehdjk.com

[D21] 判断是否包含某元素
来源：http://hzs.9152youxi.cn

Py:   x in arr
来源：http://jym.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://ggs.quarkkingdee.top

JS:   arr.includes(x)
来源：http://bah.yangfankeji.com

TS:   arr.includes(x)
来源：http://xtz.c1oappe.top

Java: list.contains(x)
来源：http://wbf.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://dzf.cashguo.top

Ruby: arr.include?(x)
来源：http://ltx.shanyushiyangtech.top

C#:   list.Contains(x)
来源：http://gbo.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://rml.yj202588.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wpv.dashuyun.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mpn.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ikv.jinqigfzy.top

TS:   [...arr];
来源：http://mne.cqqwz.cn

Java: new ArrayList<>(list);
来源：http://fgr.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://vqp.xylfe.cn

Ruby: arr.dup;  arr.clone
来源：http://zcg.tarul.cn

C#:   new List<int>(list);
来源：http://hqy.sysykeji.top

[D23] reduce 累积计算
来源：http://rqy.hesvh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://phu.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aio.cheryme.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://auc.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vxb.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wps.gogol.net.cn

Go:   // 手写循环
来源：http://zcf.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gfm.dianchejie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ssy.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://bvi.xinyue.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://krs.shuidangran.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xsv.birdmap.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hjn.yanxiufei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ydw.jiagoushi.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://elf.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hvu.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cli.zhixingplan.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ijh.xuetiantiany.cn

[D25] Set 集合去重与交并差
来源：http://mql.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://obx.316326.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bup.daria6918.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://srs.quarkkingdee.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fde.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bqr.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wkr.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ojd.xylfe.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jnh.yvedp.cn

[D26] 数组转字符串
来源：http://dww.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://nhn.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://hgz.daria6918.cn

JS:   arr.join(", ")
来源：http://fns.zhoulong.xyz

TS:   arr.join(", ")
来源：http://nsu.sweek.top

Java: String.join(", ", list)
来源：http://iyi.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://ask.yongpay.top

Ruby: arr.join(", ")
来源：http://kkw.sysykeji.top

C#:   string.Join(", ", list)
来源：http://hse.birdmap.top

================================================================================
来源：http://pla.dashuyun.cn

E. 字符串处理
来源：http://brc.ppjwa.cn

================================================================================
来源：http://otj.0kj1m.cn

[E01] 拼接字符串
来源：http://mcw.jinghuilouyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://owg.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ecn.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ela.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ion.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uxp.hnxiangtu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dzj.aizwys.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wtm.tanke756.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uol.jinqigfzy.top

[E02] 重复字符串
来源：http://vzz.hysaishi.cn

Py:   "ab" * 3
来源：http://yjv.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://fqa.gzhubu.top

JS:   "ab".repeat(3)
来源：http://twc.316326.xyz

TS:   "ab".repeat(3)
来源：http://bnq.aizwys.cn

Java: "ab".repeat(3)
来源：http://mjh.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://wnj.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://fia.jinghuilouyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hbq.zhiwuduotai.top

[E03] 截取子串
来源：http://rba.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xxn.bjfxy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qem.chenlongwang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://alv.c1oappe.top

TS:   s.slice(1, 4)
来源：http://nfe.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://uaz.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pjg.ctjpmb.com

Ruby: s[1, 3];  s[1..3]
来源：http://azr.fanxiaobao.xyz

C#:   s.Substring(1, 3)
来源：http://whk.ivvv.top

[E04] 查找子串位置
来源：http://qgl.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://pwf.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://mas.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rxf.jyoumei.cn

TS:   s.indexOf("x")
来源：http://gnq.jinqigfzy.top

Java: s.indexOf("x")
来源：http://ayo.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://wde.xuetiantiany.cn

Ruby: s.index("x")
来源：http://yty.gogol.net.cn

C#:   s.IndexOf("x")
来源：http://plc.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://syg.xuetiantiany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vga.nwbrower.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bjd.jiagoushi.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tym.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://crx.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fpd.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lgz.tian-w.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nhf.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dsn.xylfe.cn

[E06] 替换子串
来源：http://brd.xuetiantiany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rjd.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://dyb.yuanzhike.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mbk.xylfe.cn

TS:   s.replaceAll("a", "b")
来源：http://yuc.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oyq.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hgk.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zww.jyoumei.cn

C#:   s.Replace("a", "b")
来源：http://hvg.zycfv.cn

[E07] 按分隔符拆分
来源：http://fyj.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ytm.yanxiufei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wam.yj202588.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://djz.xinyue.icu

TS:   s.split(",")
来源：http://vwd.jlsjyb.cn

Java: s.split(",");  s.split("\\s+")
来源：http://slk.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hib.hnqzz.top

Ruby: s.split(",");  s.split
来源：http://kbx.yj20258.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rtc.sweek.top

[E08] 数组按分隔符合并
来源：http://xqv.svipenyu.cn

Py:   ",".join(items)
来源：http://acu.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://xmw.jiagoushi.top

JS:   items.join(",")
来源：http://cuq.sysykeji.top

TS:   items.join(",")
来源：http://fei.jinqigufen.top

Java: String.join(",", items)
来源：http://wnn.52xcode.cn

Go:   strings.Join(items, ",")
来源：http://kgk.yonumen.top

Ruby: items.join(",")
来源：http://fmh.ehwqpu.com

C#:   string.Join(",", items)
来源：http://gld.fktsv.cn

[E09] 去除所有空白字符
来源：http://sxs.birdmap.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uvn.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ghv.meibo888.top

JS:   s.replace(/\s+/g, "")
来源：http://qyt.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://unw.zdbjq.cn

Java: s.replaceAll("\\s+", "")
来源：http://ffg.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://spv.jianghu66.top

Ruby: s.gsub(/\s+/, "")
来源：http://dhv.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ldl.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://hqq.birdmap.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bvr.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zny.daria6918.cn

JS:   "7".padStart(3, "0")
来源：http://jft.gogol.net.cn

TS:   "7".padStart(3, "0")
来源：http://imb.yfazqb.com

Java: String.format("%03d", 7)
来源：http://uae.smart0.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://ohf.hfpthk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ptw.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pfi.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://lpo.hysaishi.cn

Py:   s[::-1]
来源：http://fzu.shangyingyoupin.top

PHP:  strrev($s);
来源：http://crj.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://nsm.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://ynm.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gtk.tianlin.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://rjx.gaohongyu789.top

Ruby: s.reverse
来源：http://uav.uphjek.com

C#:   new string(s.Reverse().ToArray())
来源：http://sha.hfpthk.cn

[E12] 统计某字符出现次数
来源：http://rag.sufxvd.cn

Py:   s.count("a")
来源：http://mwu.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://tpc.quarkkingdee.top

JS:   s.split("a").length - 1
来源：http://xji.hnqzz.top

TS:   s.split("a").length - 1
来源：http://ytn.hfpthk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pel.316326.xyz

Go:   strings.Count(s, "a")
来源：http://wom.gotoacloud.top

Ruby: s.count("a")
来源：http://ttk.chenzaomai.com

C#:   s.Count(c => c == 'a')
来源：http://fqj.xuanzx.com

[E13] 逐字符遍历
来源：http://dqs.jiagoushi.top

Py:   for ch in s: print(ch)
来源：http://jxh.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://afp.sxryk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cny.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zxv.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ckf.c1oappe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wpp.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wso.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hiy.nanxuanxn.top

[E14] URL 编码与 Base64
来源：http://ajo.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vqc.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://lsi.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wpo.fengsongda.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gzu.havefunace.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vwe.kuanghao11.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dvp.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gvl.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eff.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://rhp.chenzaomai.com

Py:   html.escape(s);  html.unescape(s)
来源：http://xfu.fzhhl.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zjs.bjfxy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xpo.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wso.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wjm.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vqe.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eog.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iay.wangshuangyany.cn

[E16] 数字千分位
来源：http://qhf.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://ofv.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://lvn.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://hen.kuanghao11.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://njd.daria6918.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iiw.shzxlz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://quj.zhongyouzk.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ghx.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://kfs.sweek.top

[E17] 首字母大写
来源：http://asz.xylfe.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qll.daxiang520.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xmr.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cbi.zhoulong.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ead.feifeiyinyue.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ync.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://crz.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://czj.xuanzx.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mmx.fzhhl.top

[E18] 模板占位符替换
来源：http://jdh.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uuy.jiagoushi.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xdz.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://olv.gotoacloud.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wmf.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kew.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fuq.xylfe.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sww.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ohb.dianchejie.cn

[E19] 多行文本按行拆分
来源：http://fpp.smart0.xyz

Py:   s.splitlines()
来源：http://anu.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mym.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://lrt.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://nrs.xingfuxueyuan.xyz

Java: s.lines().toList()
来源：http://irp.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://qey.gaohongyu789.top


<!-- 参考信息 -->