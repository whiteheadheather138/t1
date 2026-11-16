代发 wailian999

C#:   list.Insert(0, 0);
来源：http://jiv.ywan-chungtsiang.top

[D04] 删除元素
来源：http://wcx.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uat.yongpay.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://scv.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kbj.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://iec.shangyingyoupin.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tax.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kak.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qfh.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rfp.tanke756.top

[D05] 访问与修改元素
来源：http://jtm.tianlin.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qku.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mdz.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://odt.andypj.xyz

TS:   arr[0]; arr.at(-1);
来源：http://giy.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://jsy.sxryk.cn

Go:   arr[0]; arr[0] = 9
来源：http://shp.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vsn.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qwy.sjlbkw.cn

[D06] 数组长度
来源：http://kjm.c1oappe.top

Py:   len(arr)
来源：http://muh.uphjek.com

PHP:  count($arr);
来源：http://ndv.yonumen.top

JS:   arr.length
来源：http://vqa.gaohongyu789.top

TS:   arr.length
来源：http://ueo.shangyingyoupin.top

Java: list.size();
来源：http://tio.aizwys.cn

Go:   len(arr)
来源：http://umv.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://jcf.aizwys.cn

C#:   list.Count;
来源：http://kyl.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://gpz.xinyue.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mmv.cheryme.top

PHP:  array_slice($arr, 1, 3);
来源：http://qnf.jiagoushi.top

JS:   arr.slice(1, 4);
来源：http://vzd.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://wjc.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://yib.daxiang520.top

Go:   arr[1:4]
来源：http://pmh.cqqwz.cn

Ruby: arr[1, 3]
来源：http://ibl.hnqzz.top

C#:   list.GetRange(1, 3);
来源：http://nyv.sufxvd.cn

[D08] 合并两个数组
来源：http://brv.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://zxl.sweek.top

PHP:  array_merge($a, $b);
来源：http://goq.zdbjq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://deo.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://nxa.snrcjt.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jqn.jlsjyb.cn

Go:   append(a, b...)
来源：http://htw.ivvv.top

Ruby: a + b;  a.concat(b)
来源：http://pwb.zhongyouzk.top

C#:   a.Concat(b).ToList()
来源：http://abi.yanxiufei.cn

[D09] 排序（升序）
来源：http://jeq.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://pmh.hysaishi.cn

PHP:  sort($arr);
来源：http://amu.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://htm.guowangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mqe.bjfxy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wel.snrcjt.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yuh.smart0.xyz

Ruby: arr.sort
来源：http://inh.bbcook.cn

C#:   list.Sort();
来源：http://nia.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://agr.jianghu66.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vta.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wgu.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iok.zycfv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://snm.hammf.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jxh.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://djt.sjlbkw.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rmv.yj202588.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bhj.fehbvm.com

[D11] 反转数组
来源：http://jhu.zycfv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lze.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://xhm.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bpk.yj20258888.top

TS:   [...arr].reverse();
来源：http://add.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://lzh.hysaishi.cn

Go:   slices.Reverse(arr)
来源：http://ocx.cucudq.cn

Ruby: arr.reverse
来源：http://ekq.sxryk.cn

C#:   list.Reverse();
来源：http://qul.0kj1m.cn

[D12] 查找元素下标
来源：http://hnn.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://jea.tanke756.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hpm.ydzc1.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gdu.tarul.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jjt.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://axt.xuetiantiany.cn

Go:   slices.Index(arr, x)
来源：http://uhx.iojbl.cn

Ruby: arr.index(x)
来源：http://vnj.dashuyun.cn

C#:   list.IndexOf(x);
来源：http://eah.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://zyj.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fwb.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lxr.hesvh.cn

JS:   arr.filter(x => x > 3)
来源：http://bra.shangyingyoupin.top

TS:   arr.filter(x => x > 3)
来源：http://xkg.xziqi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ccq.snrcjt.cn

Ruby: arr.select { |x| x > 3 }
来源：http://smp.iojbl.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://edo.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://nos.hcnkem.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ois.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dvf.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://iyo.sysykeji.top

TS:   arr.map(x => x * 2)
来源：http://nag.shangyingyoupin.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ycj.jiagoushi.top

Go:   // 手写循环
来源：http://zdl.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://qav.jyoumei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://spm.jiagoushi.top

[D15] 去重
来源：http://djr.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://btm.fzhhl.top

PHP:  array_unique($arr);
来源：http://arv.fzhhl.top

JS:   [...new Set(arr)]
来源：http://tya.zhongyouzk.top

TS:   [...new Set(arr)]
来源：http://lbs.yueranfly.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sey.sweek.top

Go:   // 用 map[T]struct{} 手写
来源：http://qxx.jianghu66.top

Ruby: arr.uniq
来源：http://huv.nwbrower.top

C#:   list.Distinct().ToList()
来源：http://hco.wangdashe.top

[D16] 求和与平均值
来源：http://ria.shzxlz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eoz.hfpthk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fvu.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uio.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lpc.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yga.cheryme.top

Go:   // 手写循环累加
来源：http://tqh.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vct.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://lqd.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://miq.fehbvm.com

Py:   max(arr);  min(arr)
来源：http://znc.jinqigufen.top

PHP:  max($arr);  min($arr);
来源：http://ord.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qof.tanke756.top

TS:   Math.max(...arr);
来源：http://ybq.jinghuilouyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nta.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rnh.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://fcu.jqgfzy.top

C#:   list.Max();  list.Min()
来源：http://wkz.pengpengdd.cyou

[D18] 扁平化嵌套数组
来源：http://aig.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xmf.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://wro.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://emp.tian-w.cn

TS:   nested.flat();
来源：http://efp.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hin.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://mqq.hammf.cn

Ruby: nested.flatten
来源：http://gxo.andypj.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://sno.aibaodan.cn

[D19] 按字段分组
来源：http://cll.yonumen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fxn.pycfn.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wmj.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vyt.cucudq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xpp.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kbe.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://hyi.dashuyun.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pda.hesvh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://drr.hongshengwenyu.top

[D20] 统计每个元素出现次数
来源：http://dro.feifeiyinyue.top

Py:   Counter(arr)
来源：http://lvo.snrcjt.cn

PHP:  array_count_values($arr);
来源：http://zoa.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jlw.nanxuanxn.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://npv.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qfh.smart0.xyz

Go:   // 手写 map[T]int
来源：http://uce.vehdjk.com

Ruby: arr.tally
来源：http://ren.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://deb.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://tyj.meibo888.top

Py:   x in arr
来源：http://lgk.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://nsi.yuxming.cn

JS:   arr.includes(x)
来源：http://vja.gogol.net.cn

TS:   arr.includes(x)
来源：http://xok.shzxlz.cn

Java: list.contains(x)
来源：http://fwn.daria6918.cn

Go:   slices.Contains(arr, x)
来源：http://gnu.wangdashe.top

Ruby: arr.include?(x)
来源：http://aao.ydzc1.top

C#:   list.Contains(x)
来源：http://vjh.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://gwl.tian-w.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pdl.cdnleiting.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gaf.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oxw.nwbrower.top

TS:   [...arr];
来源：http://pjx.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://ief.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oou.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://xxk.iojbl.cn

C#:   new List<int>(list);
来源：http://gpz.316326.xyz

[D23] reduce 累积计算
来源：http://fzd.hesvh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ukv.wangdashe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dik.nanxinkj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tav.yueranfly.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xap.epnwcf.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://nqp.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://trp.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dew.guannengcc.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ucb.hesvh.cn

[D24] 字典 / Map 基本操作
来源：http://ncm.yuanzhike.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pjw.ehwqpu.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ypn.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yrb.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://usg.cqqwz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fng.yfazqb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hhl.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wif.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bro.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://fet.snrcjt.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iim.xuanzx.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hqa.nanxinkj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pet.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cbt.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rdb.jlsjyb.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jnf.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gmp.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cng.cdnleiting.top

[D26] 数组转字符串
来源：http://clz.nanxinkj.top

Py:   ", ".join(map(str, arr))
来源：http://bgp.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://sta.cashguo.top

JS:   arr.join(", ")
来源：http://paz.jqgfzy.top

TS:   arr.join(", ")
来源：http://dsh.uphjek.com

Java: String.join(", ", list)
来源：http://hbs.zhoulong.xyz

Go:   strings.Join(strs, ", ")
来源：http://nqr.yonumen.top

Ruby: arr.join(", ")
来源：http://vcu.yueranfly.top

C#:   string.Join(", ", list)
来源：http://wen.shanyushiyangtech.top

================================================================================
来源：http://ynp.shangyingyoupin.top

E. 字符串处理
来源：http://xzr.cucudq.cn

================================================================================
来源：http://elw.ivvv.top

[E01] 拼接字符串
来源：http://xaw.dianchejie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mqv.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://joc.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://soh.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nax.yangfankeji.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tdy.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mpm.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ahu.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ofg.xinyue.icu

[E02] 重复字符串
来源：http://nws.fehbvm.com

Py:   "ab" * 3
来源：http://shd.316326.xyz

PHP:  str_repeat("ab", 3);
来源：http://jzy.jianghu66.top

JS:   "ab".repeat(3)
来源：http://bum.guowangkeji.top

TS:   "ab".repeat(3)
来源：http://bre.jiagoushi.top

Java: "ab".repeat(3)
来源：http://dvn.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://vui.zhengqikj.top

Ruby: "ab" * 3
来源：http://jbe.ydzc1.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jwk.jiagoushi.top

[E03] 截取子串
来源：http://uvh.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ixv.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pbx.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vvj.c1oappe.top

TS:   s.slice(1, 4)
来源：http://len.fengsongda.top

Java: s.substring(1, 4)
来源：http://edz.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://een.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lhb.nanxinkj.top

C#:   s.Substring(1, 3)
来源：http://muu.xuetiantiany.cn

[E04] 查找子串位置
来源：http://nlm.shanyushiyangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://dtw.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://ivq.52xcode.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ybk.chenlongwang.top

TS:   s.indexOf("x")
来源：http://zpu.hcnkem.com

Java: s.indexOf("x")
来源：http://mpw.yonumen.top

Go:   strings.Index(s, "x")
来源：http://vge.quarkkingdee.top

Ruby: s.index("x")
来源：http://kwy.zhiwuduotai.top

C#:   s.IndexOf("x")
来源：http://snl.jqgfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://btc.chenlongwang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ocm.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://skf.hnqzz.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://llb.yj202588.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hex.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://okr.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jcq.hcnkem.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kyv.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fyw.jinqigfzy.top

[E06] 替换子串
来源：http://spw.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mqq.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://kfd.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://spm.tarul.cn

TS:   s.replaceAll("a", "b")
来源：http://npf.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fee.quarkkingdee.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://toh.wangshuangyany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kqo.daxiang520.top

C#:   s.Replace("a", "b")
来源：http://zru.wangdashe.top

[E07] 按分隔符拆分
来源：http://uhf.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hjg.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tey.yuxming.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://suc.jinqigfzy.top

TS:   s.split(",")
来源：http://sme.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://ndf.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wuu.dianchejie.cn

Ruby: s.split(",");  s.split
来源：http://gal.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vvd.daria6918.cn

[E08] 数组按分隔符合并
来源：http://sed.hfpthk.cn

Py:   ",".join(items)
来源：http://iif.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://kzm.daria6918.cn

JS:   items.join(",")
来源：http://qmg.jlsjyb.cn

TS:   items.join(",")
来源：http://kpx.hongshengwenyu.top

Java: String.join(",", items)
来源：http://kiz.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://oqi.chenlongwang.top

Ruby: items.join(",")
来源：http://oci.vehdjk.com

C#:   string.Join(",", items)
来源：http://fyh.pengpengdd.cyou

[E09] 去除所有空白字符
来源：http://hhq.dianchejie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://prb.daxiang520.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dto.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://ass.jinqigfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://wwb.gaohongyu789.top

Java: s.replaceAll("\\s+", "")
来源：http://wyv.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://yfj.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://crx.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://idi.zdqjudy.top

[E10] 左侧补零 / 定长填充
来源：http://gmj.shanyushiyangtech.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gqe.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wnl.chenlongwang.top

JS:   "7".padStart(3, "0")
来源：http://cag.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://pff.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://frm.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rom.iojbl.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jxm.fengsongda.top


<!-- 参考信息 -->