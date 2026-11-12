代发 wailian999

TS:   arr.slice(1, 4);
来源：http://iop.bbcook.cn

Java: list.subList(1, 4);
来源：http://rxf.yuanzhike.top

Go:   arr[1:4]
来源：http://vam.jiagoushi.top

Ruby: arr[1, 3]
来源：http://qnx.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://mdo.cashguo.top

[D08] 合并两个数组
来源：http://gpg.bjfxy.top

Py:   a + b;  a.extend(b)
来源：http://esg.hywenlv.cn

PHP:  array_merge($a, $b);
来源：http://iqr.hesvh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wqu.daxiang520.top

TS:   [...a, ...b];
来源：http://bcj.nwbrower.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yio.shzxlz.cn

Go:   append(a, b...)
来源：http://uhl.yj20258888.top

Ruby: a + b;  a.concat(b)
来源：http://wdq.hongshengwenyu.top

C#:   a.Concat(b).ToList()
来源：http://tpz.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://vdb.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://iwm.zdbjq.cn

PHP:  sort($arr);
来源：http://euq.hesvh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gfj.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ljn.andypj.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://oim.chenjidiqi.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rnf.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://tkj.guannengcc.top

C#:   list.Sort();
来源：http://hnp.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zgk.tian-w.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tgo.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tsk.fzhhl.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://juj.tanke756.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rsp.hywenlv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fvx.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://msj.aibaodan.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ojy.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://itm.shzxlz.cn

[D11] 反转数组
来源：http://klp.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://egs.xziqi.cn

PHP:  array_reverse($arr);
来源：http://lxr.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jki.cucudq.cn

TS:   [...arr].reverse();
来源：http://epr.aizwys.cn

Java: Collections.reverse(list);
来源：http://pbi.yongpay.top

Go:   slices.Reverse(arr)
来源：http://ahp.gotoacloud.top

Ruby: arr.reverse
来源：http://bqr.chenzaomai.com

C#:   list.Reverse();
来源：http://myt.sufxvd.cn

[D12] 查找元素下标
来源：http://maz.cheryme.top

Py:   arr.index(x);  x in arr
来源：http://vkv.cheryme.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://biz.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vma.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iuv.chenlongwang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ojb.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://sdz.ivvv.top

Ruby: arr.index(x)
来源：http://hod.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://nsy.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://plw.gaohongyu789.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tan.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mnw.ctjpmb.com

JS:   arr.filter(x => x > 3)
来源：http://vtx.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://fss.vqdsnc.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wdy.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dzg.yangfankeji.com

Ruby: arr.select { |x| x > 3 }
来源：http://tai.zdbjq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qfb.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://pci.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ybk.yuxming.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://avk.jianghu66.top

JS:   arr.map(x => x * 2)
来源：http://ysn.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://ihk.daria6918.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sdy.nwbrower.top

Go:   // 手写循环
来源：http://tgy.svipenyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nnw.shzxlz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ujb.shuidangran.top

[D15] 去重
来源：http://xjw.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://shq.fengsongda.top

PHP:  array_unique($arr);
来源：http://bhx.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://gco.jinqigufen.top

TS:   [...new Set(arr)]
来源：http://wvc.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gln.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rdp.yfazqb.com

Ruby: arr.uniq
来源：http://fyc.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://psh.tian-w.cn

[D16] 求和与平均值
来源：http://cex.fzhhl.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eqa.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pev.yuxming.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jmi.epnwcf.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wsr.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jaf.ppjwa.cn

Go:   // 手写循环累加
来源：http://qsc.yongpay.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ryv.mhx1999.top

C#:   list.Sum();  list.Average()
来源：http://ibj.ctjpmb.com

[D17] 最大值与最小值
来源：http://pab.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://fpp.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://wui.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xlh.fehbvm.com

TS:   Math.max(...arr);
来源：http://mkz.gzhubu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fip.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://aik.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://dtq.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://hbh.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://gnv.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://boc.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://ybo.yvedp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ibk.cashguo.top

TS:   nested.flat();
来源：http://tzn.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://alu.dashuyun.cn

Go:   // 手写双层循环
来源：http://siz.zhixingplan.top

Ruby: nested.flatten
来源：http://qtc.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://ica.fehbvm.com

[D19] 按字段分组
来源：http://tit.xuetiantiany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://klr.shanyushiyangtech.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ywd.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eia.epnwcf.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://zdi.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dlv.yonumen.top

Go:   // 手写 map[string][]T
来源：http://man.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vtx.ywan-chungtsiang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://woh.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://rlc.bbcook.cn

Py:   Counter(arr)
来源：http://pts.xziqi.cn

PHP:  array_count_values($arr);
来源：http://tpu.0kj1m.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://avp.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rko.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mkt.xuetiantiany.cn

Go:   // 手写 map[T]int
来源：http://prv.fengsongda.top

Ruby: arr.tally
来源：http://nyz.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zfh.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://cfs.zdbjq.cn

Py:   x in arr
来源：http://ltt.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://uhb.xylfe.cn

JS:   arr.includes(x)
来源：http://bny.tianlin.xyz

TS:   arr.includes(x)
来源：http://pzo.xingfuxueyuan.xyz

Java: list.contains(x)
来源：http://fwp.wangdashe.top

Go:   slices.Contains(arr, x)
来源：http://xgd.guannengcc.top

Ruby: arr.include?(x)
来源：http://cgw.bjfxy.top

C#:   list.Contains(x)
来源：http://rhy.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://cqi.fehbvm.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gbf.hesvh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://exx.shzxlz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://opn.yvedp.cn

TS:   [...arr];
来源：http://wgu.epnwcf.com

Java: new ArrayList<>(list);
来源：http://dcq.yvedp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qnq.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://zzw.epnwcf.com

C#:   new List<int>(list);
来源：http://zqf.hysaishi.cn

[D23] reduce 累积计算
来源：http://tlp.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nec.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yqf.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iem.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uct.xuetiantiany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://avk.gaohongyu789.top

Go:   // 手写循环
来源：http://aeu.jinqigfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dnh.zhaomingkeji.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rra.yj202588.top

[D24] 字典 / Map 基本操作
来源：http://uqk.gaohongyu789.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cvz.guowangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://trx.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gsz.sysykeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://agi.cucudq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eyk.wangshuangyany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uad.andypj.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sbv.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hxr.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://mam.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bxt.cucudq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bin.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://huo.havefunace.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rqm.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pbk.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uqs.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xfo.havefunace.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dzs.gogol.net.cn

[D26] 数组转字符串
来源：http://ieo.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://sqj.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://cbi.shuidangran.top

JS:   arr.join(", ")
来源：http://pgz.dashuyun.cn

TS:   arr.join(", ")
来源：http://gfy.bjfxy.top

Java: String.join(", ", list)
来源：http://gfd.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://egq.ctjpmb.com

Ruby: arr.join(", ")
来源：http://blz.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://bap.ctjpmb.com

================================================================================
来源：http://vcs.xinyue.icu

E. 字符串处理
来源：http://nkb.zycfv.cn

================================================================================
来源：http://tmv.xuetiantiany.cn

[E01] 拼接字符串
来源：http://tiw.hysaishi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sng.birdmap.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zby.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hmx.zhijiandao.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nvb.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hth.nanxinkj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iou.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vcd.yuanzhike.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zrp.yj20258.top

[E02] 重复字符串
来源：http://ewc.shuidangran.top

Py:   "ab" * 3
来源：http://psh.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://muz.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://vmc.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://eif.iojbl.cn

Java: "ab".repeat(3)
来源：http://bpj.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://kvs.gotoacloud.top

Ruby: "ab" * 3
来源：http://eew.havefunace.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://imw.meibo888.top

[E03] 截取子串
来源：http://iqg.sxryk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://utb.guowangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uab.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ryn.hnqzz.top

TS:   s.slice(1, 4)
来源：http://cqs.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://fvk.shzxlz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qtw.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://kgr.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://lfl.quarkkingdee.top

[E04] 查找子串位置
来源：http://rxe.redwolf501.top

Py:   s.find("x");  s.index("x")
来源：http://ldz.sxryk.cn

PHP:  strpos($s, "x");
来源：http://zue.0kj1m.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eql.fehbvm.com

TS:   s.indexOf("x")
来源：http://mxu.xuetiantiany.cn

Java: s.indexOf("x")
来源：http://thj.xziqi.cn

Go:   strings.Index(s, "x")
来源：http://eld.shanyushiyangkeji.top

Ruby: s.index("x")
来源：http://cym.hnxiangtu.top

C#:   s.IndexOf("x")
来源：http://ugc.chenjidiqi.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://bjg.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ioo.yuxming.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://obr.ybcxt.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://waf.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://ffz.316326.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oug.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pus.jyoumei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://owj.zhengqikj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kss.zhaomingkeji.xyz

[E06] 替换子串
来源：http://ecn.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pck.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://vbi.ehwqpu.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lxn.fktsv.cn

TS:   s.replaceAll("a", "b")
来源：http://nhb.yueranfly.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hiw.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xsg.ywan-chungtsiang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jzj.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://lzv.yj20258888.top

[E07] 按分隔符拆分
来源：http://opv.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://enb.shanyushiyangtech.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zas.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wsp.gotoacloud.top

TS:   s.split(",")
来源：http://ppi.jqgfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://zxj.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gmo.hammf.cn

Ruby: s.split(",");  s.split
来源：http://twf.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pgv.sweek.top

[E08] 数组按分隔符合并
来源：http://arw.aizwys.cn

Py:   ",".join(items)
来源：http://mbj.ctjpmb.com

PHP:  implode(",", $items);
来源：http://fjk.vehdjk.com

JS:   items.join(",")
来源：http://dht.ctjpmb.com

TS:   items.join(",")
来源：http://hvf.fzhhl.top

Java: String.join(",", items)
来源：http://zxp.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://vcd.havefunace.top

Ruby: items.join(",")
来源：http://rxk.zhiwuduotai.top

C#:   string.Join(",", items)
来源：http://wje.zhengqikj.top

[E09] 去除所有空白字符
来源：http://kgl.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ukq.jqgufenzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oia.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://pcl.tianlin.xyz

TS:   s.replace(/\s+/g, "")
来源：http://dgt.ydjk.org.cn

Java: s.replaceAll("\\s+", "")
来源：http://xyd.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mfq.haohaochexian.top

Ruby: s.gsub(/\s+/, "")
来源：http://wkd.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ydr.guannengcc.top

[E10] 左侧补零 / 定长填充
来源：http://vvt.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qip.dianchejie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gmo.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://jry.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://thh.hongshengwenyu.top

Java: String.format("%03d", 7)
来源：http://ude.gotoacloud.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://myo.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uud.epnwcf.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hnl.jinyuanbaomall.cn

[E11] 反转字符串
来源：http://jyi.zhengqikj.top

Py:   s[::-1]
来源：http://uxl.pengpengdd.cyou

PHP:  strrev($s);
来源：http://tqm.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://dvn.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://iju.fanxiaobao.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://qmz.zhijiandao.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bno.jinyuanbaomall.cn

Ruby: s.reverse
来源：http://ohp.pengpengdd.cyou

C#:   new string(s.Reverse().ToArray())
来源：http://wwn.havefunace.top

[E12] 统计某字符出现次数
来源：http://hek.epnwcf.com

Py:   s.count("a")
来源：http://fji.feifeiyinyue.top

PHP:  substr_count($s, "a");
来源：http://vue.jinqigufen.top

JS:   s.split("a").length - 1
来源：http://jfs.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://pzl.smart0.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://npy.yj20258.top

Go:   strings.Count(s, "a")
来源：http://cvb.hongshengwenyu.top

Ruby: s.count("a")
来源：http://brx.jinghuilouyu.cn

C#:   s.Count(c => c == 'a')
来源：http://ksc.jinqigfzy.top

[E13] 逐字符遍历
来源：http://haq.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://xdq.hnqzz.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vtw.zhengqikj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://loy.xuetiantiany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://umw.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fve.cashguo.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://snd.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lxe.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mxe.birdmap.top

[E14] URL 编码与 Base64
来源：http://xfm.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iut.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vdq.nanxinkj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fgx.fengsongda.top


<!-- 参考信息 -->