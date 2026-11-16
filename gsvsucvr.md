代发 wailian999

TS:   [...arr].reverse();
来源：http://eve.aibaodan.cn

Java: Collections.reverse(list);
来源：http://xwq.ppjwa.cn

Go:   slices.Reverse(arr)
来源：http://wpk.sufxvd.cn

Ruby: arr.reverse
来源：http://gfn.wangdashe.top

C#:   list.Reverse();
来源：http://hnd.gaohongyu789.top

[D12] 查找元素下标
来源：http://unp.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://tvh.nwbrower.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lxn.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://duo.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iwy.jianghu66.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zpz.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://vdz.cucudq.cn

Ruby: arr.index(x)
来源：http://oox.hfpthk.cn

C#:   list.IndexOf(x);
来源：http://gxm.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://pti.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ydn.daria6918.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://twh.nanxinkj.top

JS:   arr.filter(x => x > 3)
来源：http://jmq.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://dhk.yongpay.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tiy.jinyuanbaomall.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ipe.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xfv.zhengqikj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qwz.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://nip.bjfxy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ubn.zdbjq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mcg.ybcxt.top

JS:   arr.map(x => x * 2)
来源：http://jnj.guowangkeji.top

TS:   arr.map(x => x * 2)
来源：http://hsf.nanxuanxn.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ioz.ydjk.org.cn

Go:   // 手写循环
来源：http://djt.zhongyouzk.top

Ruby: arr.map { |x| x * 2 }
来源：http://qry.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lee.zhengqikj.top

[D15] 去重
来源：http://zny.52xcode.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://scu.ehwqpu.com

PHP:  array_unique($arr);
来源：http://pma.nwbrower.top

JS:   [...new Set(arr)]
来源：http://lsk.yvedp.cn

TS:   [...new Set(arr)]
来源：http://rcj.vqdsnc.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ott.jqgfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://wwk.zdbjq.cn

Ruby: arr.uniq
来源：http://txg.316326.xyz

C#:   list.Distinct().ToList()
来源：http://frm.sweek.top

[D16] 求和与平均值
来源：http://onn.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://alj.fanxiaobao.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zxb.guowangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ikz.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://reu.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ebw.haohaochexian.top

Go:   // 手写循环累加
来源：http://osq.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qig.jinqigufen.top

C#:   list.Sum();  list.Average()
来源：http://wxx.hnqzz.top

[D17] 最大值与最小值
来源：http://iry.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://zco.sjlbkw.cn

PHP:  max($arr);  min($arr);
来源：http://kfc.ybcxt.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pmj.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://jcp.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ius.0kj1m.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://afu.cashguo.top

Ruby: arr.max;  arr.min
来源：http://dhh.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://flr.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://ywu.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iwf.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://bye.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xex.zhaomingkeji.xyz

TS:   nested.flat();
来源：http://esa.tanke756.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cog.nanxuanxn.top

Go:   // 手写双层循环
来源：http://gen.52xcode.cn

Ruby: nested.flatten
来源：http://ddm.jinghuilouyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qir.ywan-chungtsiang.top

[D19] 按字段分组
来源：http://ylv.uphjek.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lgs.pycfn.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gvq.wangdashe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ofz.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lel.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bvr.hesvh.cn

Go:   // 手写 map[string][]T
来源：http://ysu.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ptr.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rie.cdnleiting.top

[D20] 统计每个元素出现次数
来源：http://qkp.tanke756.top

Py:   Counter(arr)
来源：http://pxb.52xcode.cn

PHP:  array_count_values($arr);
来源：http://jpo.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xdu.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uke.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iqq.meibo888.top

Go:   // 手写 map[T]int
来源：http://vaq.zhiwuduotai.top

Ruby: arr.tally
来源：http://txj.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://got.andypj.xyz

[D21] 判断是否包含某元素
来源：http://ehn.xziqi.cn

Py:   x in arr
来源：http://qfk.jinghuilouyu.cn

PHP:  in_array($x, $arr, true);
来源：http://ryb.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://lyl.fengsongda.top

TS:   arr.includes(x)
来源：http://xbb.feifeiyinyue.top

Java: list.contains(x)
来源：http://wsn.jinyuanbaomall.cn

Go:   slices.Contains(arr, x)
来源：http://kzq.sysykeji.top

Ruby: arr.include?(x)
来源：http://vww.zdqjudy.top

C#:   list.Contains(x)
来源：http://rcg.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://huo.xinyue.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zgi.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blr.yonumen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xae.epnwcf.com

TS:   [...arr];
来源：http://mwk.fzhhl.top

Java: new ArrayList<>(list);
来源：http://zbf.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://dfa.jinyuanbaomall.cn

Ruby: arr.dup;  arr.clone
来源：http://qtm.gogol.net.cn

C#:   new List<int>(list);
来源：http://vwu.jqgfzy.top

[D23] reduce 累积计算
来源：http://obq.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ivv.hfpthk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ahk.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kbz.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://agj.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ttv.feifeiyinyue.top

Go:   // 手写循环
来源：http://jha.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zmq.hongshengwenyu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cyr.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://vay.cheryme.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uuc.xylfe.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jrb.hfpthk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://drh.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jmv.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ndi.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nlz.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dno.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hmk.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://vmn.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qbq.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cqp.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vrz.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ixf.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ahd.jqgufenzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mjv.tanke756.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://peb.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zhu.zycfv.cn

[D26] 数组转字符串
来源：http://ujo.ivvv.top

Py:   ", ".join(map(str, arr))
来源：http://yse.tianlin.xyz

PHP:  implode(", ", $arr);
来源：http://gfu.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://foo.52xcode.cn

TS:   arr.join(", ")
来源：http://gnz.9152youxi.cn

Java: String.join(", ", list)
来源：http://vqy.ywan-chungtsiang.top

Go:   strings.Join(strs, ", ")
来源：http://atq.yuxming.cn

Ruby: arr.join(", ")
来源：http://xps.fehbvm.com

C#:   string.Join(", ", list)
来源：http://yvd.shanyushiyangtech.top

================================================================================
来源：http://igp.pycfn.com

E. 字符串处理
来源：http://qnr.daria6918.cn

================================================================================
来源：http://jnn.snrcjt.cn

[E01] 拼接字符串
来源：http://ygc.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qvi.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gfb.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gpp.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gne.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iui.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jhk.xziqi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gge.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pki.hcnkem.com

[E02] 重复字符串
来源：http://jmy.ppjwa.cn

Py:   "ab" * 3
来源：http://kyp.hesvh.cn

PHP:  str_repeat("ab", 3);
来源：http://zmq.birdmap.top

JS:   "ab".repeat(3)
来源：http://lbz.yonumen.top

TS:   "ab".repeat(3)
来源：http://jwe.svipenyu.cn

Java: "ab".repeat(3)
来源：http://kmx.quarkkingdee.top

Go:   strings.Repeat("ab", 3)
来源：http://hzl.gotoacloud.top

Ruby: "ab" * 3
来源：http://qil.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://boy.jinqigfzy.top

[E03] 截取子串
来源：http://gql.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oyj.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ypr.kuanghao11.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lmc.tanke756.top

TS:   s.slice(1, 4)
来源：http://ayx.hnqzz.top

Java: s.substring(1, 4)
来源：http://cap.snrcjt.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hqf.fzhhl.top

Ruby: s[1, 3];  s[1..3]
来源：http://lee.yuanzhike.top

C#:   s.Substring(1, 3)
来源：http://mol.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://cha.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://xhz.shanyushiyangtech.top

PHP:  strpos($s, "x");
来源：http://dls.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qzz.ydjk.org.cn

TS:   s.indexOf("x")
来源：http://qmi.birdmap.top

Java: s.indexOf("x")
来源：http://bgx.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://edc.shangyingyoupin.top

Ruby: s.index("x")
来源：http://apm.xylfe.cn

C#:   s.IndexOf("x")
来源：http://skq.gzhubu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yeq.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wbd.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://njo.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://szx.shanyushiyangtech.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jcp.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gyc.52xcode.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://npg.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qkd.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xnb.hongshengwenyu.top

[E06] 替换子串
来源：http://icn.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jxd.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://bai.dashuyun.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ngm.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://gls.jyoumei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zyh.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yng.fanxiaobao.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fyf.haohaochexian.top

C#:   s.Replace("a", "b")
来源：http://bkj.iojbl.cn

[E07] 按分隔符拆分
来源：http://aka.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://spi.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cqr.vehdjk.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://imz.cheryme.top

TS:   s.split(",")
来源：http://ovv.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://cqb.havefunace.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://leq.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://ixm.zhijiandao.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eza.aizwys.cn

[E08] 数组按分隔符合并
来源：http://rmt.shanyushiyangtech.top

Py:   ",".join(items)
来源：http://bis.shangyingyoupin.top

PHP:  implode(",", $items);
来源：http://mbp.feifeiyinyue.top

JS:   items.join(",")
来源：http://hae.cqqwz.cn

TS:   items.join(",")
来源：http://drm.yuxming.cn

Java: String.join(",", items)
来源：http://dnn.cucudq.cn

Go:   strings.Join(items, ",")
来源：http://oob.jinqigfzy.top

Ruby: items.join(",")
来源：http://spg.gaohongyu789.top

C#:   string.Join(",", items)
来源：http://guv.ivvv.top

[E09] 去除所有空白字符
来源：http://dsd.shanyushiyangtech.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://exj.gzhubu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vaq.fanxiaobao.xyz

JS:   s.replace(/\s+/g, "")
来源：http://nag.zhaomingkeji.xyz

TS:   s.replace(/\s+/g, "")
来源：http://ndt.hammf.cn

Java: s.replaceAll("\\s+", "")
来源：http://emx.sweek.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ihk.bjfxy.top

Ruby: s.gsub(/\s+/, "")
来源：http://ywy.sjlbkw.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://shj.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://opk.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kmc.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bju.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://jwz.birdmap.top

TS:   "7".padStart(3, "0")
来源：http://rrx.yj202588.top

Java: String.format("%03d", 7)
来源：http://uqw.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mzw.bjfxy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zpq.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mfi.guowangkeji.top

[E11] 反转字符串
来源：http://rsh.snrcjt.cn

Py:   s[::-1]
来源：http://mva.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://wdh.tanke756.top

JS:   [...s].reverse().join("")
来源：http://tvk.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://qtw.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://iqi.nwbrower.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://via.xingfuxueyuan.xyz

Ruby: s.reverse
来源：http://zyp.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://brv.wangdashe.top

[E12] 统计某字符出现次数
来源：http://msl.meibo888.top

Py:   s.count("a")
来源：http://oys.havefunace.top

PHP:  substr_count($s, "a");
来源：http://vlu.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://ylz.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://jcw.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wba.jinyuanbaomall.cn

Go:   strings.Count(s, "a")
来源：http://rrt.hcnkem.com

Ruby: s.count("a")
来源：http://gnk.zdqjudy.top

C#:   s.Count(c => c == 'a')
来源：http://kuh.sxryk.cn

[E13] 逐字符遍历
来源：http://uiq.meibo888.top

Py:   for ch in s: print(ch)
来源：http://pmg.nanxuanxn.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uri.fzhhl.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cag.kuanghao11.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vnk.cqqwz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sdr.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cnz.andypj.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://eaa.zhaomingkeji.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wch.wangdashe.top

[E14] URL 编码与 Base64
来源：http://gxs.zhijiandao.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rgj.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vxe.yangfankeji.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uas.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nla.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lxv.pengpengdd.cyou

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hnr.shanyushiyangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jko.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gpu.havefunace.top

[E15] HTML 转义 / 反转义
来源：http://kya.shuidangran.top

Py:   html.escape(s);  html.unescape(s)
来源：http://man.xuetiantiany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mhx.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rqe.ydjk.org.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://csk.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qim.shuidangran.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://phh.feifeiyinyue.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://myp.xuanzx.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fqj.9152youxi.cn

[E16] 数字千分位
来源：http://veu.jianghu66.top

Py:   f"{1234567:,}"
来源：http://pda.aibaodan.cn

PHP:  number_format(1234567);
来源：http://yno.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jll.vehdjk.com

TS:   (1234567).toLocaleString("en-US")
来源：http://szl.ehwqpu.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mew.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vap.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ric.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://msl.52xcode.cn

[E17] 首字母大写
来源：http://nmd.hongshengwenyu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nta.yvedp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wlg.haohaochexian.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iun.cqqwz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iek.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://psh.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qhd.sjlbkw.cn

Ruby: s.capitalize
来源：http://vlu.feifeiyinyue.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://edm.jyoumei.cn

[E18] 模板占位符替换
来源：http://ihj.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bnl.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yjk.guannengcc.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ybe.wangshuangyany.cn


<!-- 参考信息 -->