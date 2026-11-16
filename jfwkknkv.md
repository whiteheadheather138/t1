代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://ghs.dianchejie.cn

Java: list.add(0, 0);
来源：http://brq.xylfe.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nkl.hysaishi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bhz.aizwys.cn

C#:   list.Insert(0, 0);
来源：http://hgp.xylfe.cn

[D04] 删除元素
来源：http://heo.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://orm.shangyingyoupin.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ijz.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://egy.zhixingplan.top

TS:   arr.splice(0, 1);
来源：http://ijo.ydjk.org.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pww.snrcjt.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wnw.hysaishi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xaw.jqgfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gur.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://ojs.dianchejie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://clh.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pjk.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bmc.hnqzz.top

TS:   arr[0]; arr.at(-1);
来源：http://fnl.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://pen.yfazqb.com

Go:   arr[0]; arr[0] = 9
来源：http://jey.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rwa.iojbl.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eyc.wangshuangyany.cn

[D06] 数组长度
来源：http://ezv.ivvv.top

Py:   len(arr)
来源：http://ktq.fzhhl.top

PHP:  count($arr);
来源：http://fgl.meibo888.top

JS:   arr.length
来源：http://jun.yvedp.cn

TS:   arr.length
来源：http://ffm.ehwqpu.com

Java: list.size();
来源：http://avm.shzxlz.cn

Go:   len(arr)
来源：http://dbx.nanxinkj.top

Ruby: arr.length; arr.size
来源：http://lia.jqgufenzy.top

C#:   list.Count;
来源：http://fpj.guannengcc.top

[D07] 切片 / 取子数组
来源：http://iog.chenzaomai.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hti.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://ydp.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://yoh.yj20258.top

TS:   arr.slice(1, 4);
来源：http://mio.andypj.xyz

Java: list.subList(1, 4);
来源：http://nip.zhengqikj.top

Go:   arr[1:4]
来源：http://ujq.yongpay.top

Ruby: arr[1, 3]
来源：http://wob.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://xxr.dashuyun.cn

[D08] 合并两个数组
来源：http://gyk.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://drx.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://lkd.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lgk.yonumen.top

TS:   [...a, ...b];
来源：http://ghk.kuanghao11.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mkp.zhengqikj.top

Go:   append(a, b...)
来源：http://zzw.snrcjt.cn

Ruby: a + b;  a.concat(b)
来源：http://utd.jinghuilouyu.cn

C#:   a.Concat(b).ToList()
来源：http://xll.9152youxi.cn

[D09] 排序（升序）
来源：http://xhz.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://qoj.jlsjyb.cn

PHP:  sort($arr);
来源：http://sda.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lwe.yueranfly.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jey.yj20258.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hcb.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kuk.yonumen.top

Ruby: arr.sort
来源：http://yyv.hcnkem.com

C#:   list.Sort();
来源：http://jcr.gzhubu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yht.sxryk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://isg.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aab.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xtk.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qlm.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cet.pycfn.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pfq.dashuyun.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ocq.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xjv.bbcook.cn

[D11] 反转数组
来源：http://pxy.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://ziv.shangyingyoupin.top

PHP:  array_reverse($arr);
来源：http://rmx.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ahd.shangyingyoupin.top

TS:   [...arr].reverse();
来源：http://agr.zdqjudy.top

Java: Collections.reverse(list);
来源：http://zcy.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://hce.nanxuanxn.top

Ruby: arr.reverse
来源：http://lcb.jinqigfzy.top

C#:   list.Reverse();
来源：http://qhk.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://vak.tianlin.xyz

Py:   arr.index(x);  x in arr
来源：http://cwz.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fjp.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fyy.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hqz.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cbe.uphjek.com

Go:   slices.Index(arr, x)
来源：http://nsv.smart0.xyz

Ruby: arr.index(x)
来源：http://mfo.tanke756.top

C#:   list.IndexOf(x);
来源：http://zkz.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://dbq.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mfd.jianghu66.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zbo.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://ttq.yongpay.top

TS:   arr.filter(x => x > 3)
来源：http://xyn.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wpx.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iop.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://esq.yonumen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xxm.jlsjyb.cn

[D14] 映射转换（每个元素变形）
来源：http://eta.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ehx.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pny.sjlbkw.cn

JS:   arr.map(x => x * 2)
来源：http://woa.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://zry.yj20258888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://onq.yuxming.cn

Go:   // 手写循环
来源：http://zmw.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://toy.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pyc.daria6918.cn

[D15] 去重
来源：http://njz.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qbf.birdmap.top

PHP:  array_unique($arr);
来源：http://uat.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://aze.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://aig.zycfv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nlp.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://buw.uphjek.com

Ruby: arr.uniq
来源：http://dsb.yonumen.top

C#:   list.Distinct().ToList()
来源：http://nrm.sweek.top

[D16] 求和与平均值
来源：http://vad.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jxl.hesvh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hfo.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nho.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ftp.chenjidiqi.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yvy.dashuyun.cn

Go:   // 手写循环累加
来源：http://fcl.havefunace.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zau.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://maa.cdnleiting.top

[D17] 最大值与最小值
来源：http://epc.fktsv.cn

Py:   max(arr);  min(arr)
来源：http://mad.quarkkingdee.top

PHP:  max($arr);  min($arr);
来源：http://uqw.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bsf.yonumen.top

TS:   Math.max(...arr);
来源：http://sna.redwolf501.top

Java: Collections.max(list);  Collections.min(list);
来源：http://npf.hnqzz.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cbb.yj20258888.top

Ruby: arr.max;  arr.min
来源：http://mqd.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://clp.gotoacloud.top

[D18] 扁平化嵌套数组
来源：http://hoz.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uif.tian-w.cn

PHP:  array_merge(...$nested);
来源：http://iwp.guowangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://trw.shzxlz.cn

TS:   nested.flat();
来源：http://cdz.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gqa.cqqwz.cn

Go:   // 手写双层循环
来源：http://rbl.xingfuxueyuan.xyz

Ruby: nested.flatten
来源：http://lyz.tanke756.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ton.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://qlg.sxryk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vbk.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dxq.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bnv.meibo888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fyv.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jxy.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://xbg.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ajh.sweek.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ucj.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://irz.jinqigufen.top

Py:   Counter(arr)
来源：http://zgv.vqdsnc.cn

PHP:  array_count_values($arr);
来源：http://uuz.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aez.zycfv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tyr.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hxc.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://gyu.52xcode.cn

Ruby: arr.tally
来源：http://brt.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gmp.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://prx.zhiwuduotai.top

Py:   x in arr
来源：http://ssc.316326.xyz

PHP:  in_array($x, $arr, true);
来源：http://vsu.hywenlv.cn

JS:   arr.includes(x)
来源：http://yli.xinyue.icu

TS:   arr.includes(x)
来源：http://jlc.zdqjudy.top

Java: list.contains(x)
来源：http://txh.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://jnn.hnqzz.top

Ruby: arr.include?(x)
来源：http://mcd.cdnleiting.top

C#:   list.Contains(x)
来源：http://gis.hysaishi.cn

[D22] 复制数组（避免共享引用）
来源：http://zqe.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kxo.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sby.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://adm.gzhubu.top

TS:   [...arr];
来源：http://jdl.cqqwz.cn

Java: new ArrayList<>(list);
来源：http://vwv.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ezr.52xcode.cn

Ruby: arr.dup;  arr.clone
来源：http://rzd.yanxiufei.cn

C#:   new List<int>(list);
来源：http://oys.quarkkingdee.top

[D23] reduce 累积计算
来源：http://gpb.guowangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gfp.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qvs.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://han.gotoacloud.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mjc.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jyo.nanxinkj.top

Go:   // 手写循环
来源：http://zth.yongpay.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fta.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ckx.xingfuxueyuan.xyz

[D24] 字典 / Map 基本操作
来源：http://cpf.shanyushiyangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://amm.xinyue.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vfy.chenjidiqi.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://syz.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aqj.ydzc1.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://doq.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uda.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gvn.0kj1m.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hgm.zdqjudy.top

[D25] Set 集合去重与交并差
来源：http://gpd.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://evd.jianghu66.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://khc.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sjw.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zfj.aizwys.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jwk.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hdh.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qqb.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ybs.jianghu66.top

[D26] 数组转字符串
来源：http://vad.nanxuanxn.top

Py:   ", ".join(map(str, arr))
来源：http://cti.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://ahn.nanxuanxn.top

JS:   arr.join(", ")
来源：http://sls.xuanzx.com

TS:   arr.join(", ")
来源：http://vrg.svipenyu.cn

Java: String.join(", ", list)
来源：http://ind.snrcjt.cn

Go:   strings.Join(strs, ", ")
来源：http://fud.dianchejie.cn

Ruby: arr.join(", ")
来源：http://aqg.gotoacloud.top

C#:   string.Join(", ", list)
来源：http://xjs.gotoacloud.top

================================================================================
来源：http://hau.aizwys.cn

E. 字符串处理
来源：http://wbp.quarkkingdee.top

================================================================================
来源：http://hls.vqdsnc.cn

[E01] 拼接字符串
来源：http://yfb.quarkkingdee.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ryw.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xhy.aizwys.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fsv.gotoacloud.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xik.hongshengwenyu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fed.hywenlv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wlc.smart0.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fgf.xingfuxueyuan.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cbn.daria6918.cn

[E02] 重复字符串
来源：http://jsa.andypj.xyz

Py:   "ab" * 3
来源：http://sxj.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://myq.gzhubu.top

JS:   "ab".repeat(3)
来源：http://hja.gotoacloud.top

TS:   "ab".repeat(3)
来源：http://kcf.xingfuxueyuan.xyz

Java: "ab".repeat(3)
来源：http://dcg.zycfv.cn

Go:   strings.Repeat("ab", 3)
来源：http://fkl.xuanzx.com

Ruby: "ab" * 3
来源：http://ggb.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yxe.ydjk.org.cn

[E03] 截取子串
来源：http://jcs.dashuyun.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://izw.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://muo.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nnw.yonumen.top

TS:   s.slice(1, 4)
来源：http://zvy.yangfankeji.com

Java: s.substring(1, 4)
来源：http://fia.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cgr.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bqv.jiagoushi.top

C#:   s.Substring(1, 3)
来源：http://gwc.ydjk.org.cn

[E04] 查找子串位置
来源：http://jek.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://nel.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://wfi.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ftp.cqqwz.cn

TS:   s.indexOf("x")
来源：http://jgq.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://ukd.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://xjg.fzhhl.top

Ruby: s.index("x")
来源：http://nmr.havefunace.top

C#:   s.IndexOf("x")
来源：http://wzi.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://icm.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qfz.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://goo.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nvr.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vrl.jinqigfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qys.hnxiangtu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lqj.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://thf.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wgm.shanyushiyangkeji.top

[E06] 替换子串
来源：http://acv.chenzaomai.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yzc.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://ayk.jinqigfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wcf.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://fsd.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://odw.epnwcf.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mky.yanxiufei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lzw.birdmap.top

C#:   s.Replace("a", "b")
来源：http://ibw.tian-w.cn

[E07] 按分隔符拆分
来源：http://tad.yuanzhike.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pyr.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hza.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kms.hfpthk.cn

TS:   s.split(",")
来源：http://hgo.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://moj.52xcode.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fbt.316326.xyz

Ruby: s.split(",");  s.split
来源：http://opi.xuetiantiany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nzw.yuxming.cn

[E08] 数组按分隔符合并
来源：http://wvo.c1oappe.top

Py:   ",".join(items)
来源：http://kgz.hywenlv.cn

PHP:  implode(",", $items);
来源：http://aqc.fzhhl.top

JS:   items.join(",")
来源：http://mzl.sweek.top

TS:   items.join(",")
来源：http://gil.yangfankeji.com

Java: String.join(",", items)
来源：http://hpe.hesvh.cn

Go:   strings.Join(items, ",")
来源：http://asz.hongshengwenyu.top

Ruby: items.join(",")
来源：http://cfq.fehbvm.com

C#:   string.Join(",", items)
来源：http://bfs.haohaochexian.top

[E09] 去除所有空白字符
来源：http://xhw.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xrt.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lrm.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://jbl.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://vai.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://dhd.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dhd.mhx1999.top

Ruby: s.gsub(/\s+/, "")
来源：http://tgz.yvedp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bmr.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://doz.zdqjudy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vus.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://caq.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://klx.vqdsnc.cn


<!-- 参考信息 -->