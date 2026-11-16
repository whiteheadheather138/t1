代发 wailian999

Java: list.size();
来源：http://kwt.sxryk.cn

Go:   len(arr)
来源：http://wvx.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://xlb.sweek.top

C#:   list.Count;
来源：http://kzp.jinqigufen.top

[D07] 切片 / 取子数组
来源：http://jdy.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xxn.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uuv.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://qjc.hywenlv.cn

TS:   arr.slice(1, 4);
来源：http://lcx.nanxinkj.top

Java: list.subList(1, 4);
来源：http://utx.meibo888.top

Go:   arr[1:4]
来源：http://adj.tianlin.xyz

Ruby: arr[1, 3]
来源：http://goc.jiagoushi.top

C#:   list.GetRange(1, 3);
来源：http://deo.chenzaomai.com

[D08] 合并两个数组
来源：http://hgo.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://bui.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://kis.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pqb.yonumen.top

TS:   [...a, ...b];
来源：http://upf.hnqzz.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yiq.hammf.cn

Go:   append(a, b...)
来源：http://tzu.hesvh.cn

Ruby: a + b;  a.concat(b)
来源：http://fvy.aizwys.cn

C#:   a.Concat(b).ToList()
来源：http://oho.hnxiangtu.top

[D09] 排序（升序）
来源：http://afh.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://urq.iojbl.cn

PHP:  sort($arr);
来源：http://agp.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cmp.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wng.ctjpmb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://ata.hammf.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://afg.jqgufenzy.top

Ruby: arr.sort
来源：http://cpu.shangyingyoupin.top

C#:   list.Sort();
来源：http://zxi.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zvk.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://euj.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pkv.tianlin.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ndr.xylfe.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mxd.aizwys.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://smx.fzhhl.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cbw.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xii.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bgt.shanyushiyangkeji.top

[D11] 反转数组
来源：http://yqo.hfpthk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://opu.haohaochexian.top

PHP:  array_reverse($arr);
来源：http://cis.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zix.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://xmg.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://djl.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://abj.yongpay.top

Ruby: arr.reverse
来源：http://hbb.yonumen.top

C#:   list.Reverse();
来源：http://szi.daxiang520.top

[D12] 查找元素下标
来源：http://ntc.quarkkingdee.top

Py:   arr.index(x);  x in arr
来源：http://eev.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ovq.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tse.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qyz.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rac.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://pjl.aizwys.cn

Ruby: arr.index(x)
来源：http://jyr.sysykeji.top

C#:   list.IndexOf(x);
来源：http://tzi.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://qlc.yj202588.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://whg.hammf.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qhi.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://vfq.cheryme.top

TS:   arr.filter(x => x > 3)
来源：http://npa.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://upb.zhixingplan.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mnq.cqqwz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uoq.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zar.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://wab.fktsv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pem.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cum.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://xos.gzhubu.top

TS:   arr.map(x => x * 2)
来源：http://kvq.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xuj.fengsongda.top

Go:   // 手写循环
来源：http://ydz.redwolf501.top

Ruby: arr.map { |x| x * 2 }
来源：http://yuh.snrcjt.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://all.dashuyun.cn

[D15] 去重
来源：http://aaw.chenzaomai.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://utr.redwolf501.top

PHP:  array_unique($arr);
来源：http://qns.cqqwz.cn

JS:   [...new Set(arr)]
来源：http://asb.0kj1m.cn

TS:   [...new Set(arr)]
来源：http://fim.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rxh.ydjk.org.cn

Go:   // 用 map[T]struct{} 手写
来源：http://spl.smart0.xyz

Ruby: arr.uniq
来源：http://krj.fengsongda.top

C#:   list.Distinct().ToList()
来源：http://llx.gotoacloud.top

[D16] 求和与平均值
来源：http://xih.cashguo.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://axg.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kwn.yongpay.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hck.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://krw.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://asm.xuetiantiany.cn

Go:   // 手写循环累加
来源：http://mxj.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nlk.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://qks.cashguo.top

[D17] 最大值与最小值
来源：http://tkw.sjlbkw.cn

Py:   max(arr);  min(arr)
来源：http://lob.yfazqb.com

PHP:  max($arr);  min($arr);
来源：http://obt.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ygd.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://gjc.tianlin.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://udv.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fyy.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://wyx.jinghuilouyu.cn

C#:   list.Max();  list.Min()
来源：http://afp.hfpthk.cn

[D18] 扁平化嵌套数组
来源：http://hvw.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dem.tanke756.top

PHP:  array_merge(...$nested);
来源：http://din.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iwf.aibaodan.cn

TS:   nested.flat();
来源：http://yix.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xbj.ydzc1.top

Go:   // 手写双层循环
来源：http://mem.epnwcf.com

Ruby: nested.flatten
来源：http://imo.ivvv.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mvj.ywan-chungtsiang.top

[D19] 按字段分组
来源：http://pjl.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hey.vqdsnc.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aik.yvedp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wae.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://elp.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vbo.pengpengdd.cyou

Go:   // 手写 map[string][]T
来源：http://wro.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://rvg.yanxiufei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eax.tian-w.cn

[D20] 统计每个元素出现次数
来源：http://lah.uphjek.com

Py:   Counter(arr)
来源：http://alf.xuanzx.com

PHP:  array_count_values($arr);
来源：http://nea.fanxiaobao.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rvc.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hqr.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://auj.hammf.cn

Go:   // 手写 map[T]int
来源：http://lxr.c1oappe.top

Ruby: arr.tally
来源：http://gpu.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wnm.shangyingyoupin.top

[D21] 判断是否包含某元素
来源：http://cji.xingfuxueyuan.xyz

Py:   x in arr
来源：http://utx.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://jqf.jinghuilouyu.cn

JS:   arr.includes(x)
来源：http://rjg.havefunace.top

TS:   arr.includes(x)
来源：http://tev.hammf.cn

Java: list.contains(x)
来源：http://oid.hysaishi.cn

Go:   slices.Contains(arr, x)
来源：http://kdi.meibo888.top

Ruby: arr.include?(x)
来源：http://dmk.nanxinkj.top

C#:   list.Contains(x)
来源：http://djk.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://ccb.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://umy.fzhhl.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hmm.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://quy.cashguo.top

TS:   [...arr];
来源：http://fxs.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://mqc.sxryk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xzd.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://bjc.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://nvf.snrcjt.cn

[D23] reduce 累积计算
来源：http://hzy.quarkkingdee.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qvf.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xnz.jiagoushi.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mmk.hcnkem.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lvj.cashguo.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xbs.yonumen.top

Go:   // 手写循环
来源：http://uwx.nanxuanxn.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rvp.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kfc.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://ldi.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ovu.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hpj.yj20258.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://avo.xingfuxueyuan.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dnm.fzhhl.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gut.sweek.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ujm.daria6918.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mej.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vuo.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://nyn.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lpb.epnwcf.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pdn.yj20258888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://izm.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ssr.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cqs.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nlz.nanxinkj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://umj.dianchejie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hky.0kj1m.cn

[D26] 数组转字符串
来源：http://dph.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://oxm.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://xio.snrcjt.cn

JS:   arr.join(", ")
来源：http://kdr.zycfv.cn

TS:   arr.join(", ")
来源：http://rch.sxryk.cn

Java: String.join(", ", list)
来源：http://fyd.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://mov.yfazqb.com

Ruby: arr.join(", ")
来源：http://rul.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://cfx.sufxvd.cn

================================================================================
来源：http://mec.fengsongda.top

E. 字符串处理
来源：http://khd.gotoacloud.top

================================================================================
来源：http://fme.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://fqv.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://efh.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://thh.bjfxy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qls.zycfv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://upk.zdbjq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dwz.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zud.zhoulong.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gve.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iwa.smart0.xyz

[E02] 重复字符串
来源：http://jic.jinqigfzy.top

Py:   "ab" * 3
来源：http://jja.cqqwz.cn

PHP:  str_repeat("ab", 3);
来源：http://htl.quarkkingdee.top

JS:   "ab".repeat(3)
来源：http://tbj.hcnkem.com

TS:   "ab".repeat(3)
来源：http://tgk.guannengcc.top

Java: "ab".repeat(3)
来源：http://hos.jinyuanbaomall.cn

Go:   strings.Repeat("ab", 3)
来源：http://bgz.hammf.cn

Ruby: "ab" * 3
来源：http://khn.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://idx.jqgufenzy.top

[E03] 截取子串
来源：http://hfq.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://imf.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xfs.dashuyun.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yaq.nwbrower.top

TS:   s.slice(1, 4)
来源：http://vsp.xingfuxueyuan.xyz

Java: s.substring(1, 4)
来源：http://kat.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://opc.yvedp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://auu.pycfn.com

C#:   s.Substring(1, 3)
来源：http://ezf.pycfn.com

[E04] 查找子串位置
来源：http://ekp.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://xtl.xziqi.cn

PHP:  strpos($s, "x");
来源：http://rzk.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://odu.ppjwa.cn

TS:   s.indexOf("x")
来源：http://ecs.fktsv.cn

Java: s.indexOf("x")
来源：http://fqe.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://xgs.xylfe.cn

Ruby: s.index("x")
来源：http://kvx.bjfxy.top

C#:   s.IndexOf("x")
来源：http://obm.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kvq.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lcu.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cyt.cucudq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jfz.kuanghao11.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eqb.jlsjyb.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kao.ctjpmb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fch.xziqi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pav.ppjwa.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fnk.epnwcf.com

[E06] 替换子串
来源：http://kah.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rmb.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://ldt.wangshuangyany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wxr.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://tur.0kj1m.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kge.yanxiufei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kjw.aizwys.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://azg.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://hio.bbcook.cn

[E07] 按分隔符拆分
来源：http://xvw.mhx1999.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vkb.chenzaomai.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xxv.zycfv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cbz.zhixingplan.top

TS:   s.split(",")
来源：http://moe.yj20258.top

Java: s.split(",");  s.split("\\s+")
来源：http://yzu.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fvz.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://dxh.cqqwz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vjl.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://guq.gogol.net.cn

Py:   ",".join(items)
来源：http://bjr.cucudq.cn

PHP:  implode(",", $items);
来源：http://muq.hnxiangtu.top

JS:   items.join(",")
来源：http://emk.yfazqb.com

TS:   items.join(",")
来源：http://ltd.vehdjk.com

Java: String.join(",", items)
来源：http://nad.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://wel.fktsv.cn

Ruby: items.join(",")
来源：http://pse.c1oappe.top

C#:   string.Join(",", items)
来源：http://fwr.chenjidiqi.icu

[E09] 去除所有空白字符
来源：http://csc.zycfv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dtw.hywenlv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jsp.aizwys.cn

JS:   s.replace(/\s+/g, "")
来源：http://cel.zhijiandao.cn

TS:   s.replace(/\s+/g, "")
来源：http://khq.andypj.xyz

Java: s.replaceAll("\\s+", "")
来源：http://igh.jqgfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vli.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uax.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uct.yongpay.top

[E10] 左侧补零 / 定长填充
来源：http://lyp.jiagoushi.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cci.jinyuanbaomall.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eqd.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://rmj.xuanzx.com

TS:   "7".padStart(3, "0")
来源：http://vzg.hammf.cn

Java: String.format("%03d", 7)
来源：http://cfp.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://bnp.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://exo.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mjk.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://iig.aibaodan.cn

Py:   s[::-1]
来源：http://eyl.pengpengdd.cyou

PHP:  strrev($s);
来源：http://ukf.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://lcl.nanxinkj.top

TS:   [...s].reverse().join("")
来源：http://zrq.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rcg.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ugp.yj202588.top

Ruby: s.reverse
来源：http://azt.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nln.havefunace.top

[E12] 统计某字符出现次数
来源：http://hmg.yuanzhike.top

Py:   s.count("a")
来源：http://pxq.xziqi.cn

PHP:  substr_count($s, "a");
来源：http://vug.xylfe.cn

JS:   s.split("a").length - 1
来源：http://abn.hfpthk.cn

TS:   s.split("a").length - 1
来源：http://jlp.xuanzx.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://spg.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://wnj.9152youxi.cn

Ruby: s.count("a")
来源：http://vvq.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://cyg.yuanzhike.top

[E13] 逐字符遍历
来源：http://bmv.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://qvi.gogol.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wvh.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://axx.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://mtk.hnqzz.top


<!-- 参考信息 -->