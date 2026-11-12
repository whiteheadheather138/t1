代发 wailian999

Java: list.size();
来源：http://cis.yongpay.top

Go:   len(arr)
来源：http://tuq.iojbl.cn

Ruby: arr.length; arr.size
来源：http://zxy.nanxuanxn.top

C#:   list.Count;
来源：http://fpt.jyoumei.cn

[D07] 切片 / 取子数组
来源：http://wpb.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mcr.yj20258.top

PHP:  array_slice($arr, 1, 3);
来源：http://jvq.tanke756.top

JS:   arr.slice(1, 4);
来源：http://ydm.yuxming.cn

TS:   arr.slice(1, 4);
来源：http://rhq.xuetiantiany.cn

Java: list.subList(1, 4);
来源：http://cph.jinghuilouyu.cn

Go:   arr[1:4]
来源：http://ckx.yonumen.top

Ruby: arr[1, 3]
来源：http://xoe.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://ddk.yvedp.cn

[D08] 合并两个数组
来源：http://kls.daxiang520.top

Py:   a + b;  a.extend(b)
来源：http://sac.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://zbh.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://iih.quarkkingdee.top

TS:   [...a, ...b];
来源：http://ubl.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fcq.vehdjk.com

Go:   append(a, b...)
来源：http://eik.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://ran.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://ngd.nanxuanxn.top

[D09] 排序（升序）
来源：http://pqx.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://ayt.tian-w.cn

PHP:  sort($arr);
来源：http://iwv.zhaomingkeji.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yci.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://llv.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eqq.yuanzhike.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pyj.yj20258.top

Ruby: arr.sort
来源：http://odk.cdnleiting.top

C#:   list.Sort();
来源：http://gyj.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jqn.nanxinkj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vvc.kuanghao11.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lsl.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dzo.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://owk.yfazqb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mva.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ynu.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bgz.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fug.hnqzz.top

[D11] 反转数组
来源：http://xwk.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://ugg.fehbvm.com

PHP:  array_reverse($arr);
来源：http://ges.aizwys.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sjz.yj20258.top

TS:   [...arr].reverse();
来源：http://atu.ydzc1.top

Java: Collections.reverse(list);
来源：http://dui.yfazqb.com

Go:   slices.Reverse(arr)
来源：http://fnq.guowangkeji.top

Ruby: arr.reverse
来源：http://qmj.zhengqikj.top

C#:   list.Reverse();
来源：http://hbm.kuanghao11.cn

[D12] 查找元素下标
来源：http://jeb.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://ckd.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bnv.jqgfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kwz.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://esz.guowangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rqv.hammf.cn

Go:   slices.Index(arr, x)
来源：http://fks.jyoumei.cn

Ruby: arr.index(x)
来源：http://oiw.shzxlz.cn

C#:   list.IndexOf(x);
来源：http://znv.zhijiandao.cn

[D13] 过滤（保留满足条件的）
来源：http://owi.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tmd.fanxiaobao.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kpk.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://sed.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://btm.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zsj.cheryme.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hzl.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://stm.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://njg.jinqigfzy.top

[D14] 映射转换（每个元素变形）
来源：http://gcw.nanxinkj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sry.yuxming.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bop.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://swp.daxiang520.top

TS:   arr.map(x => x * 2)
来源：http://aln.chenzaomai.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ira.fzhhl.top

Go:   // 手写循环
来源：http://vyq.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://klz.yuxming.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ulm.pycfn.com

[D15] 去重
来源：http://ahy.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://stg.xuanzx.com

PHP:  array_unique($arr);
来源：http://vyt.yueranfly.top

JS:   [...new Set(arr)]
来源：http://hct.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://nnm.gogol.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fio.yvedp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nmy.iojbl.cn

Ruby: arr.uniq
来源：http://tjp.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://uoj.hfpthk.cn

[D16] 求和与平均值
来源：http://hcs.zhongyouzk.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kqf.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://svf.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lbf.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pto.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vsg.andypj.xyz

Go:   // 手写循环累加
来源：http://whj.ybcxt.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://djp.yanxiufei.cn

C#:   list.Sum();  list.Average()
来源：http://rfo.zhijiandao.cn

[D17] 最大值与最小值
来源：http://emb.zycfv.cn

Py:   max(arr);  min(arr)
来源：http://hly.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://twi.fktsv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bqm.iojbl.cn

TS:   Math.max(...arr);
来源：http://dzk.gogol.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://teb.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uep.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://vmb.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://vpo.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://bsm.zdbjq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://byz.redwolf501.top

PHP:  array_merge(...$nested);
来源：http://yvc.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mew.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://xof.smart0.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yie.pengpengdd.cyou

Go:   // 手写双层循环
来源：http://lra.redwolf501.top

Ruby: nested.flatten
来源：http://uln.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tsq.ybcxt.top

[D19] 按字段分组
来源：http://kbq.zhengqikj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oyq.yj20258888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bso.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ffu.hammf.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kmn.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fqo.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://zpe.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://iwg.316326.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://anc.bbcook.cn

[D20] 统计每个元素出现次数
来源：http://lbc.yangfankeji.com

Py:   Counter(arr)
来源：http://qdl.nanxuanxn.top

PHP:  array_count_values($arr);
来源：http://zen.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vyr.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ibh.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nxi.c1oappe.top

Go:   // 手写 map[T]int
来源：http://uyl.yuanzhike.top

Ruby: arr.tally
来源：http://irg.jqgufenzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://moc.haohaochexian.top

[D21] 判断是否包含某元素
来源：http://qnf.epnwcf.com

Py:   x in arr
来源：http://jsg.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://gck.chenzaomai.com

JS:   arr.includes(x)
来源：http://tpx.xingfuxueyuan.xyz

TS:   arr.includes(x)
来源：http://mki.zhiwuduotai.top

Java: list.contains(x)
来源：http://exf.tarul.cn

Go:   slices.Contains(arr, x)
来源：http://lnt.pengpengdd.cyou

Ruby: arr.include?(x)
来源：http://dfp.gogol.net.cn

C#:   list.Contains(x)
来源：http://snf.ehwqpu.com

[D22] 复制数组（避免共享引用）
来源：http://tar.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://czz.epnwcf.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://obi.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nso.wangdashe.top

TS:   [...arr];
来源：http://qik.tarul.cn

Java: new ArrayList<>(list);
来源：http://pvt.shanyushiyangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://psf.jianghu66.top

Ruby: arr.dup;  arr.clone
来源：http://luf.0kj1m.cn

C#:   new List<int>(list);
来源：http://jlr.hywenlv.cn

[D23] reduce 累积计算
来源：http://lod.xingfuxueyuan.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jnv.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qms.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tio.shanyushiyangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://arg.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ekx.fanxiaobao.xyz

Go:   // 手写循环
来源：http://jwp.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ldx.hywenlv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yuc.jinghuilouyu.cn

[D24] 字典 / Map 基本操作
来源：http://pxh.gotoacloud.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hnw.wangdashe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fgp.chenjidiqi.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jzo.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bmp.xziqi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qxm.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ojq.yj20258.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yml.cqqwz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xut.fzhhl.top

[D25] Set 集合去重与交并差
来源：http://cck.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://scc.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://euk.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mcw.pengpengdd.cyou

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qqf.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dse.jinyuanbaomall.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xld.jqgfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://orf.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cgp.jinghuilouyu.cn

[D26] 数组转字符串
来源：http://zfp.zhongyouzk.top

Py:   ", ".join(map(str, arr))
来源：http://nxq.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://orn.zdqjudy.top

JS:   arr.join(", ")
来源：http://rwk.hammf.cn

TS:   arr.join(", ")
来源：http://dqo.jlsjyb.cn

Java: String.join(", ", list)
来源：http://qal.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://ner.hnxiangtu.top

Ruby: arr.join(", ")
来源：http://uvn.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://ckx.zhijiandao.cn

================================================================================
来源：http://qwk.c1oappe.top

E. 字符串处理
来源：http://lsv.shanyushiyangkeji.top

================================================================================
来源：http://yfp.wangdashe.top

[E01] 拼接字符串
来源：http://ppl.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oiq.birdmap.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yum.sufxvd.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hrs.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xwg.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eno.yongpay.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dvd.cqqwz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://flp.316326.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dze.yj202588.top

[E02] 重复字符串
来源：http://ova.iojbl.cn

Py:   "ab" * 3
来源：http://zjn.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://yki.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://ysn.cheryme.top

TS:   "ab".repeat(3)
来源：http://ueq.bjfxy.top

Java: "ab".repeat(3)
来源：http://owd.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://srs.jyoumei.cn

Ruby: "ab" * 3
来源：http://vpy.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uha.zhoulong.xyz

[E03] 截取子串
来源：http://zrl.yuxming.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qam.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://arw.52xcode.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ohw.guannengcc.top

TS:   s.slice(1, 4)
来源：http://rnk.nanxuanxn.top

Java: s.substring(1, 4)
来源：http://hkj.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zhv.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mtk.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://ygr.jqgufenzy.top

[E04] 查找子串位置
来源：http://mtp.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://vio.chenlongwang.top

PHP:  strpos($s, "x");
来源：http://bse.c1oappe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ifm.guowangkeji.top

TS:   s.indexOf("x")
来源：http://fig.jqgfzy.top

Java: s.indexOf("x")
来源：http://pqs.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://uji.ydzc1.top

Ruby: s.index("x")
来源：http://ovk.gotoacloud.top

C#:   s.IndexOf("x")
来源：http://rbp.yangfankeji.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://pzm.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bev.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zja.52xcode.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rmk.sufxvd.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gbm.daxiang520.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lai.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vzi.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://csv.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bja.vehdjk.com

[E06] 替换子串
来源：http://lik.ydzc1.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gmg.daria6918.cn

PHP:  str_replace("a", "b", $s);
来源：http://bvs.yueranfly.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://psk.hesvh.cn

TS:   s.replaceAll("a", "b")
来源：http://tdc.feifeiyinyue.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vef.fzhhl.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mjz.yj20258.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bej.zhiwuduotai.top

C#:   s.Replace("a", "b")
来源：http://fgj.sysykeji.top

[E07] 按分隔符拆分
来源：http://twi.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://puz.daria6918.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tge.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://eoq.iojbl.cn

TS:   s.split(",")
来源：http://eac.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://xmg.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://btx.gaohongyu789.top

Ruby: s.split(",");  s.split
来源：http://vhy.52xcode.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fxm.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://oyy.zycfv.cn

Py:   ",".join(items)
来源：http://wqf.yonumen.top

PHP:  implode(",", $items);
来源：http://unw.jqgufenzy.top

JS:   items.join(",")
来源：http://par.gaohongyu789.top

TS:   items.join(",")
来源：http://lyq.meibo888.top

Java: String.join(",", items)
来源：http://aag.dashuyun.cn

Go:   strings.Join(items, ",")
来源：http://tpp.sjlbkw.cn

Ruby: items.join(",")
来源：http://eok.hysaishi.cn

C#:   string.Join(",", items)
来源：http://ccg.vqdsnc.cn

[E09] 去除所有空白字符
来源：http://uua.vqdsnc.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zlo.xinyue.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://alt.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://erx.jinyuanbaomall.cn

TS:   s.replace(/\s+/g, "")
来源：http://qbz.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://ffg.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bop.zhongyouzk.top

Ruby: s.gsub(/\s+/, "")
来源：http://tit.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://omc.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://vzn.pycfn.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kgt.smart0.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vao.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://yub.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://dko.jianghu66.top

Java: String.format("%03d", 7)
来源：http://ocn.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://pyq.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iia.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ews.shanyushiyangtech.top

[E11] 反转字符串
来源：http://cwu.fanxiaobao.xyz

Py:   s[::-1]
来源：http://ldq.ybcxt.top

PHP:  strrev($s);
来源：http://hkq.sxryk.cn

JS:   [...s].reverse().join("")
来源：http://vsu.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://vhd.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qgl.sjlbkw.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fku.chenjidiqi.icu

Ruby: s.reverse
来源：http://dyp.gzhubu.top

C#:   new string(s.Reverse().ToArray())
来源：http://mrm.zycfv.cn

[E12] 统计某字符出现次数
来源：http://fax.chenlongwang.top

Py:   s.count("a")
来源：http://fyy.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://bxv.birdmap.top

JS:   s.split("a").length - 1
来源：http://gzx.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://nau.jinqigufen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://usu.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://qag.ppjwa.cn

Ruby: s.count("a")
来源：http://pad.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://hcj.jqgfzy.top

[E13] 逐字符遍历
来源：http://tlf.fehbvm.com

Py:   for ch in s: print(ch)
来源：http://tuj.yangfankeji.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://elb.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wux.bjfxy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cad.hywenlv.cn


<!-- 参考信息 -->