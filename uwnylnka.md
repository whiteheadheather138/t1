代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://jtb.pycfn.com

Java: list.add(0, 0);
来源：http://bvf.ppjwa.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hnm.sxryk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://znw.bbcook.cn

C#:   list.Insert(0, 0);
来源：http://nkw.hywenlv.cn

[D04] 删除元素
来源：http://wbe.andypj.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kqz.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tak.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ipm.zdqjudy.top

TS:   arr.splice(0, 1);
来源：http://wik.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mrd.daxiang520.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wtw.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jxq.shanyushiyangtech.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://syz.pycfn.com

[D05] 访问与修改元素
来源：http://xsv.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://foy.yuanzhike.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jpo.ppjwa.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zgw.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://zov.jinqigufen.top

Java: list.get(0); list.set(0, 9);
来源：http://fwl.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://vsv.nanxinkj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ymr.quarkkingdee.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vat.tian-w.cn

[D06] 数组长度
来源：http://url.daria6918.cn

Py:   len(arr)
来源：http://bub.zhengqikj.top

PHP:  count($arr);
来源：http://zje.chenzaomai.com

JS:   arr.length
来源：http://woj.bjfxy.top

TS:   arr.length
来源：http://fyw.nanxinkj.top

Java: list.size();
来源：http://irw.yongpay.top

Go:   len(arr)
来源：http://scy.bjfxy.top

Ruby: arr.length; arr.size
来源：http://bzf.jqgufenzy.top

C#:   list.Count;
来源：http://cjj.ivvv.top

[D07] 切片 / 取子数组
来源：http://bjf.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wvl.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://agp.jyoumei.cn

JS:   arr.slice(1, 4);
来源：http://rak.iojbl.cn

TS:   arr.slice(1, 4);
来源：http://gbs.hysaishi.cn

Java: list.subList(1, 4);
来源：http://xdc.guannengcc.top

Go:   arr[1:4]
来源：http://eet.ppjwa.cn

Ruby: arr[1, 3]
来源：http://iwe.sweek.top

C#:   list.GetRange(1, 3);
来源：http://usu.xuanzx.com

[D08] 合并两个数组
来源：http://pnj.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://iqa.c1oappe.top

PHP:  array_merge($a, $b);
来源：http://wbl.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sdi.gotoacloud.top

TS:   [...a, ...b];
来源：http://swe.hnqzz.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oxp.fehbvm.com

Go:   append(a, b...)
来源：http://ycj.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://kfx.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://rsd.tianlin.xyz

[D09] 排序（升序）
来源：http://vlt.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://pdy.jqgfzy.top

PHP:  sort($arr);
来源：http://pvh.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mut.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mzm.xinyue.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://eyi.meibo888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cik.hcnkem.com

Ruby: arr.sort
来源：http://hgs.hywenlv.cn

C#:   list.Sort();
来源：http://ubt.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://scj.aizwys.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://piv.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nix.meibo888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gvl.zhongyouzk.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ndh.wangdashe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lne.jlsjyb.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ipz.haohaochexian.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://unl.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zji.aizwys.cn

[D11] 反转数组
来源：http://eax.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://esv.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://yxb.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ofu.zhijiandao.cn

TS:   [...arr].reverse();
来源：http://fyg.chenzaomai.com

Java: Collections.reverse(list);
来源：http://kwu.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://gbd.daxiang520.top

Ruby: arr.reverse
来源：http://zfd.hesvh.cn

C#:   list.Reverse();
来源：http://mja.yanxiufei.cn

[D12] 查找元素下标
来源：http://qmt.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://psq.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pwq.dianchejie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rkk.smart0.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zjb.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://adl.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://pfu.shzxlz.cn

Ruby: arr.index(x)
来源：http://fwd.mhx1999.top

C#:   list.IndexOf(x);
来源：http://ins.xinyue.icu

[D13] 过滤（保留满足条件的）
来源：http://sgl.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zbu.hywenlv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tan.zhixingplan.top

JS:   arr.filter(x => x > 3)
来源：http://vzv.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://lta.vqdsnc.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nfg.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ype.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://glm.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bei.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://xog.yongpay.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tkc.havefunace.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ytj.andypj.xyz

JS:   arr.map(x => x * 2)
来源：http://yfk.chenzaomai.com

TS:   arr.map(x => x * 2)
来源：http://bmq.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gcf.aibaodan.cn

Go:   // 手写循环
来源：http://akd.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://erv.vehdjk.com

C#:   list.Select(x => x * 2).ToList()
来源：http://oqj.yvedp.cn

[D15] 去重
来源：http://ugt.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xpj.chenzaomai.com

PHP:  array_unique($arr);
来源：http://llg.ehwqpu.com

JS:   [...new Set(arr)]
来源：http://mks.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://tjw.hfpthk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zbc.epnwcf.com

Go:   // 用 map[T]struct{} 手写
来源：http://sak.tianlin.xyz

Ruby: arr.uniq
来源：http://rwq.fehbvm.com

C#:   list.Distinct().ToList()
来源：http://wyu.cheryme.top

[D16] 求和与平均值
来源：http://rsz.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bmw.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rsi.nwbrower.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eri.zdbjq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://brx.xingfuxueyuan.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dcq.xinyue.icu

Go:   // 手写循环累加
来源：http://omg.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ihb.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://cje.wangdashe.top

[D17] 最大值与最小值
来源：http://khg.smart0.xyz

Py:   max(arr);  min(arr)
来源：http://spp.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://qrz.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fop.jianghu66.top

TS:   Math.max(...arr);
来源：http://muc.zycfv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pmt.sxryk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qhw.tarul.cn

Ruby: arr.max;  arr.min
来源：http://cot.hysaishi.cn

C#:   list.Max();  list.Min()
来源：http://kim.yj202588.top

[D18] 扁平化嵌套数组
来源：http://xmd.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wla.9152youxi.cn

PHP:  array_merge(...$nested);
来源：http://fjd.gotoacloud.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pan.nwbrower.top

TS:   nested.flat();
来源：http://kgb.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yao.yonumen.top

Go:   // 手写双层循环
来源：http://xpx.fengsongda.top

Ruby: nested.flatten
来源：http://tcy.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mev.yangfankeji.com

[D19] 按字段分组
来源：http://uxs.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ztb.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xbw.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sfd.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://geh.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zgc.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://gpa.fanxiaobao.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://ant.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://urd.xinyue.icu

[D20] 统计每个元素出现次数
来源：http://iox.jyoumei.cn

Py:   Counter(arr)
来源：http://wqb.yonumen.top

PHP:  array_count_values($arr);
来源：http://urz.cdnleiting.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yzd.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jxv.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wev.yj20258.top

Go:   // 手写 map[T]int
来源：http://eqp.daria6918.cn

Ruby: arr.tally
来源：http://bgb.kuanghao11.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tlb.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://ulm.shuidangran.top

Py:   x in arr
来源：http://bcp.aibaodan.cn

PHP:  in_array($x, $arr, true);
来源：http://esz.haohaochexian.top

JS:   arr.includes(x)
来源：http://clt.hesvh.cn

TS:   arr.includes(x)
来源：http://jqv.fktsv.cn

Java: list.contains(x)
来源：http://agy.pycfn.com

Go:   slices.Contains(arr, x)
来源：http://nme.dashuyun.cn

Ruby: arr.include?(x)
来源：http://rrx.jyoumei.cn

C#:   list.Contains(x)
来源：http://vlj.jianghu66.top

[D22] 复制数组（避免共享引用）
来源：http://psz.316326.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pic.ydjk.org.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vko.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ykg.svipenyu.cn

TS:   [...arr];
来源：http://unf.ehwqpu.com

Java: new ArrayList<>(list);
来源：http://rrh.chenzaomai.com

Go:   copied := append([]int(nil), arr...)
来源：http://mma.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://zdu.tanke756.top

C#:   new List<int>(list);
来源：http://gpv.ydjk.org.cn

[D23] reduce 累积计算
来源：http://odq.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rab.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uhc.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ihf.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dak.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jlv.yongpay.top

Go:   // 手写循环
来源：http://zqr.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yut.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hxz.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://jos.shanyushiyangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kze.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vqt.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vpb.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://waw.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hoa.jqgfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://obp.tian-w.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nbw.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hhp.fengsongda.top

[D25] Set 集合去重与交并差
来源：http://lvx.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hko.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hlx.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gub.gotoacloud.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iig.xuetiantiany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xue.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qae.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ctg.cucudq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rir.cashguo.top

[D26] 数组转字符串
来源：http://rcx.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://pja.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://oml.yuanzhike.top

JS:   arr.join(", ")
来源：http://wrt.yfazqb.com

TS:   arr.join(", ")
来源：http://ncr.nanxuanxn.top

Java: String.join(", ", list)
来源：http://miy.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://hyn.gogol.net.cn

Ruby: arr.join(", ")
来源：http://wbu.iojbl.cn

C#:   string.Join(", ", list)
来源：http://pll.ehwqpu.com

================================================================================
来源：http://qxq.daxiang520.top

E. 字符串处理
来源：http://keb.guannengcc.top

================================================================================
来源：http://fhx.zhiwuduotai.top

[E01] 拼接字符串
来源：http://dze.vehdjk.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pka.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pqi.ydjk.org.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gco.yj20258888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eso.sysykeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tnh.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xqq.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://veq.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fcn.jqgfzy.top

[E02] 重复字符串
来源：http://blc.hysaishi.cn

Py:   "ab" * 3
来源：http://rwf.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://bes.jiagoushi.top

JS:   "ab".repeat(3)
来源：http://spf.pengpengdd.cyou

TS:   "ab".repeat(3)
来源：http://cyz.fktsv.cn

Java: "ab".repeat(3)
来源：http://kax.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://rbf.yvedp.cn

Ruby: "ab" * 3
来源：http://jbg.hnqzz.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vma.daria6918.cn

[E03] 截取子串
来源：http://see.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tkw.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://otb.hfpthk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rtv.ivvv.top

TS:   s.slice(1, 4)
来源：http://oyl.cheryme.top

Java: s.substring(1, 4)
来源：http://nni.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tym.yvedp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ols.zhengqikj.top

C#:   s.Substring(1, 3)
来源：http://iwo.wangshuangyany.cn

[E04] 查找子串位置
来源：http://jcc.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://frn.chenjidiqi.icu

PHP:  strpos($s, "x");
来源：http://zdc.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vzw.shzxlz.cn

TS:   s.indexOf("x")
来源：http://lcd.shuidangran.top

Java: s.indexOf("x")
来源：http://vua.quarkkingdee.top

Go:   strings.Index(s, "x")
来源：http://dmq.xingfuxueyuan.xyz

Ruby: s.index("x")
来源：http://mpj.guannengcc.top

C#:   s.IndexOf("x")
来源：http://qxg.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://luo.smart0.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wmw.sxryk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lwc.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sjt.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jrg.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hig.jqgufenzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://llc.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lnu.jianghu66.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hty.jinqigufen.top

[E06] 替换子串
来源：http://epe.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dmk.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://qxp.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cpl.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://nsf.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ssc.gzhubu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xhl.yj20258.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wrn.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://egl.hcnkem.com

[E07] 按分隔符拆分
来源：http://zff.gotoacloud.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qyn.jqgfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vlw.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qls.cashguo.top

TS:   s.split(",")
来源：http://otn.0kj1m.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uqn.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vni.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://ohs.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dnr.yj20258888.top

[E08] 数组按分隔符合并
来源：http://vqc.quarkkingdee.top

Py:   ",".join(items)
来源：http://xwm.ppjwa.cn

PHP:  implode(",", $items);
来源：http://mnw.sweek.top

JS:   items.join(",")
来源：http://jnn.uphjek.com

TS:   items.join(",")
来源：http://hxm.nanxuanxn.top

Java: String.join(",", items)
来源：http://xoz.uphjek.com

Go:   strings.Join(items, ",")
来源：http://uvh.aizwys.cn

Ruby: items.join(",")
来源：http://pzw.pycfn.com

C#:   string.Join(",", items)
来源：http://doo.hfpthk.cn

[E09] 去除所有空白字符
来源：http://yyi.daria6918.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kkk.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lvr.jinqigufen.top

JS:   s.replace(/\s+/g, "")
来源：http://vav.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://zfb.wangshuangyany.cn

Java: s.replaceAll("\\s+", "")
来源：http://wuc.mhx1999.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tdg.redwolf501.top

Ruby: s.gsub(/\s+/, "")
来源：http://rwb.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ywi.zhixingplan.top

[E10] 左侧补零 / 定长填充
来源：http://tla.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xow.xuetiantiany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cgz.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://alj.ydzc1.top


<!-- 参考信息 -->