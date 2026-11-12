代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://hvz.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://dev.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hgs.daria6918.cn

================================================================================
来源：http://xrx.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://aen.iojbl.cn

================================================================================
来源：http://ogq.sweek.top

[D01] 创建数组 / 列表
来源：http://xiz.yfazqb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://qfo.sysykeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qej.mhx1999.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yge.quarkkingdee.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://prs.zhongyouzk.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://duu.yj20258888.top

Go:   arr := []int{1, 2, 3}
来源：http://ste.bjfxy.top

Ruby: arr = [1, 2, 3]
来源：http://ieg.cucudq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tjq.zhixingplan.top

[D02] 追加元素到末尾
来源：http://nnb.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xwy.jinqigfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xge.ydjk.org.cn

JS:   arr.push(4);
来源：http://xxd.daxiang520.top

TS:   arr.push(4);
来源：http://mig.yj20258.top

Java: list.add(4);
来源：http://zfi.andypj.xyz

Go:   arr = append(arr, 4)
来源：http://dew.ctjpmb.com

Ruby: arr << 4; arr.push(5)
来源：http://bfu.ywan-chungtsiang.top

C#:   list.Add(4);
来源：http://ecp.pycfn.com

[D03] 在指定位置插入元素
来源：http://fal.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://lvg.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uhw.jlsjyb.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pcy.yvedp.cn

TS:   arr.splice(0, 0, 0);
来源：http://ojv.sweek.top

Java: list.add(0, 0);
来源：http://dcq.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://sig.xinyue.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sek.cashguo.top

C#:   list.Insert(0, 0);
来源：http://pse.chenjidiqi.icu

[D04] 删除元素
来源：http://pry.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://csq.gogol.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uip.ywan-chungtsiang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://egn.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://wxf.9152youxi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ujl.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rlf.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://agz.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sia.jinqigufen.top

[D05] 访问与修改元素
来源：http://hhx.yj20258.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ngl.fktsv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://slx.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vjw.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://jxw.yongpay.top

Java: list.get(0); list.set(0, 9);
来源：http://vdn.sweek.top

Go:   arr[0]; arr[0] = 9
来源：http://cyr.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ijy.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tev.yvedp.cn

[D06] 数组长度
来源：http://dpc.cucudq.cn

Py:   len(arr)
来源：http://shx.52xcode.cn

PHP:  count($arr);
来源：http://nhl.shanyushiyangtech.top

JS:   arr.length
来源：http://cug.tian-w.cn

TS:   arr.length
来源：http://bel.hammf.cn

Java: list.size();
来源：http://siy.tian-w.cn

Go:   len(arr)
来源：http://tnd.meibo888.top

Ruby: arr.length; arr.size
来源：http://ahz.cdnleiting.top

C#:   list.Count;
来源：http://oqt.zhoulong.xyz

[D07] 切片 / 取子数组
来源：http://quw.tarul.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jbi.chenzaomai.com

PHP:  array_slice($arr, 1, 3);
来源：http://pow.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://aug.redwolf501.top

TS:   arr.slice(1, 4);
来源：http://ltp.hongshengwenyu.top

Java: list.subList(1, 4);
来源：http://iej.52xcode.cn

Go:   arr[1:4]
来源：http://bum.aizwys.cn

Ruby: arr[1, 3]
来源：http://mhe.zhiwuduotai.top

C#:   list.GetRange(1, 3);
来源：http://fhn.zhixingplan.top

[D08] 合并两个数组
来源：http://dfv.zhixingplan.top

Py:   a + b;  a.extend(b)
来源：http://xeb.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://mht.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ikn.daria6918.cn

TS:   [...a, ...b];
来源：http://pnf.gogol.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pgn.yuxming.cn

Go:   append(a, b...)
来源：http://wio.aibaodan.cn

Ruby: a + b;  a.concat(b)
来源：http://xda.guowangkeji.top

C#:   a.Concat(b).ToList()
来源：http://nik.yj20258.top

[D09] 排序（升序）
来源：http://nbg.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://fnd.c1oappe.top

PHP:  sort($arr);
来源：http://gki.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rpu.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ofw.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vda.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yao.quarkkingdee.top

Ruby: arr.sort
来源：http://jik.guowangkeji.top

C#:   list.Sort();
来源：http://fsw.ppjwa.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xcb.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xdq.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gdr.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zmr.aibaodan.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kla.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tyc.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pcy.xuetiantiany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://njr.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rik.vqdsnc.cn

[D11] 反转数组
来源：http://pcz.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qaf.jianghu66.top

PHP:  array_reverse($arr);
来源：http://vky.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dhk.gogol.net.cn

TS:   [...arr].reverse();
来源：http://cuy.cqqwz.cn

Java: Collections.reverse(list);
来源：http://hpq.hnqzz.top

Go:   slices.Reverse(arr)
来源：http://tgg.yongpay.top

Ruby: arr.reverse
来源：http://dcf.uphjek.com

C#:   list.Reverse();
来源：http://gul.yuxming.cn

[D12] 查找元素下标
来源：http://gmu.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://axd.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sbb.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xfi.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vvt.yonumen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mqu.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://jhk.shuidangran.top

Ruby: arr.index(x)
来源：http://twc.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://agg.yongpay.top

[D13] 过滤（保留满足条件的）
来源：http://vbk.feifeiyinyue.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bfs.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bqw.daxiang520.top

JS:   arr.filter(x => x > 3)
来源：http://ffj.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://dfz.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://maj.tanke756.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ljb.yuanzhike.top

Ruby: arr.select { |x| x > 3 }
来源：http://pdr.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://mrv.guannengcc.top

[D14] 映射转换（每个元素变形）
来源：http://flv.c1oappe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fuc.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://psr.yuanzhike.top

JS:   arr.map(x => x * 2)
来源：http://owi.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://ntb.sufxvd.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kqo.snrcjt.cn

Go:   // 手写循环
来源：http://ymh.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://iqc.zhiwuduotai.top

C#:   list.Select(x => x * 2).ToList()
来源：http://inj.xziqi.cn

[D15] 去重
来源：http://sri.yj20258.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://imn.yangfankeji.com

PHP:  array_unique($arr);
来源：http://vzw.cucudq.cn

JS:   [...new Set(arr)]
来源：http://gbn.fengsongda.top

TS:   [...new Set(arr)]
来源：http://bay.ydjk.org.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hpg.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://zoo.xylfe.cn

Ruby: arr.uniq
来源：http://cfp.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://oan.tarul.cn

[D16] 求和与平均值
来源：http://xfv.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://upa.gotoacloud.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://djq.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bgk.shuidangran.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kaa.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tmo.epnwcf.com

Go:   // 手写循环累加
来源：http://ydt.9152youxi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lfd.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://dur.xylfe.cn

[D17] 最大值与最小值
来源：http://qdh.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://nme.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://fzv.yongpay.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xgc.bbcook.cn

TS:   Math.max(...arr);
来源：http://jom.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gnr.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ozy.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://weh.jqgfzy.top

C#:   list.Max();  list.Min()
来源：http://qrc.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://yno.shzxlz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lmo.jinqigufen.top

PHP:  array_merge(...$nested);
来源：http://wgu.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zdm.jinqigfzy.top

TS:   nested.flat();
来源：http://izt.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pke.jlsjyb.cn

Go:   // 手写双层循环
来源：http://pnz.aizwys.cn

Ruby: nested.flatten
来源：http://iyz.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zqh.sjlbkw.cn

[D19] 按字段分组
来源：http://dsf.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://opx.yuxming.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://prn.52xcode.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hyr.xingfuxueyuan.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://nup.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dfz.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://ouu.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gcl.bbcook.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yjr.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://rvp.quarkkingdee.top

Py:   Counter(arr)
来源：http://tum.fehbvm.com

PHP:  array_count_values($arr);
来源：http://gtx.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fnk.nanxuanxn.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zvk.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cxb.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://tox.chenzaomai.com

Ruby: arr.tally
来源：http://ofd.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://llp.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://rny.cdnleiting.top

Py:   x in arr
来源：http://fsq.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://cbl.xylfe.cn

JS:   arr.includes(x)
来源：http://dnd.feifeiyinyue.top

TS:   arr.includes(x)
来源：http://sjh.iojbl.cn

Java: list.contains(x)
来源：http://dxa.yj20258888.top

Go:   slices.Contains(arr, x)
来源：http://hry.yonumen.top

Ruby: arr.include?(x)
来源：http://ctb.xinyue.icu

C#:   list.Contains(x)
来源：http://jxm.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://ibi.ehwqpu.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pjr.bjfxy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gbk.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://erf.bjfxy.top

TS:   [...arr];
来源：http://nep.zhoulong.xyz

Java: new ArrayList<>(list);
来源：http://sql.yfazqb.com

Go:   copied := append([]int(nil), arr...)
来源：http://eyn.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://pqm.havefunace.top

C#:   new List<int>(list);
来源：http://dgs.zdbjq.cn

[D23] reduce 累积计算
来源：http://wue.jyoumei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mvt.shanyushiyangtech.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://puy.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://byo.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hzf.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gww.jinqigufen.top

Go:   // 手写循环
来源：http://kyx.shanyushiyangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tuc.yj202588.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aak.xuanzx.com

[D24] 字典 / Map 基本操作
来源：http://zxx.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qxl.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cip.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fak.guannengcc.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gkt.redwolf501.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xyr.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pvz.birdmap.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yxm.shzxlz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://isi.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://cxx.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tzy.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qod.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cgh.jiagoushi.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gzf.xylfe.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ljm.daxiang520.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://byc.ppjwa.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://khe.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gwq.wangshuangyany.cn

[D26] 数组转字符串
来源：http://slu.pengpengdd.cyou

Py:   ", ".join(map(str, arr))
来源：http://caf.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://wqh.fzhhl.top

JS:   arr.join(", ")
来源：http://vdg.cucudq.cn

TS:   arr.join(", ")
来源：http://kke.sjlbkw.cn

Java: String.join(", ", list)
来源：http://jdq.yj20258.top

Go:   strings.Join(strs, ", ")
来源：http://tvd.shanyushiyangtech.top

Ruby: arr.join(", ")
来源：http://kak.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://itq.sweek.top

================================================================================
来源：http://fcm.pycfn.com

E. 字符串处理
来源：http://jer.sysykeji.top

================================================================================
来源：http://rww.yj20258.top

[E01] 拼接字符串
来源：http://zlf.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gae.yueranfly.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nnc.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zln.quarkkingdee.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://joj.iojbl.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://amj.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://evb.svipenyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mem.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fjx.aizwys.cn

[E02] 重复字符串
来源：http://sgf.shanyushiyangtech.top

Py:   "ab" * 3
来源：http://pdp.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://kbj.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://gec.xuanzx.com

TS:   "ab".repeat(3)
来源：http://xis.yuxming.cn

Java: "ab".repeat(3)
来源：http://tta.hywenlv.cn

Go:   strings.Repeat("ab", 3)
来源：http://gwj.yj202588.top

Ruby: "ab" * 3
来源：http://wwe.ehwqpu.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zpn.fengsongda.top

[E03] 截取子串
来源：http://cie.zycfv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qrj.sysykeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qit.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sau.fzhhl.top

TS:   s.slice(1, 4)
来源：http://fqc.gogol.net.cn

Java: s.substring(1, 4)
来源：http://waq.jiagoushi.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://glk.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://heu.chenjidiqi.icu

C#:   s.Substring(1, 3)
来源：http://mdt.gogol.net.cn

[E04] 查找子串位置
来源：http://mud.sjlbkw.cn

Py:   s.find("x");  s.index("x")
来源：http://yeo.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://gzy.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://omf.jianghu66.top

TS:   s.indexOf("x")
来源：http://jhu.316326.xyz

Java: s.indexOf("x")
来源：http://mzi.wangdashe.top

Go:   strings.Index(s, "x")
来源：http://hue.vehdjk.com

Ruby: s.index("x")
来源：http://jej.zdbjq.cn

C#:   s.IndexOf("x")
来源：http://ftv.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pli.jinqigufen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iie.yj20258888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yyv.tianlin.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hfl.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://eih.zhiwuduotai.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bfh.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zaf.yuanzhike.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ghy.dianchejie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lwn.yueranfly.top

[E06] 替换子串
来源：http://ucx.zhongyouzk.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qfi.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ixi.chenlongwang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://txn.ybcxt.top

TS:   s.replaceAll("a", "b")
来源：http://vkf.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://njk.chenlongwang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qlf.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wkp.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://wrg.vqdsnc.cn

[E07] 按分隔符拆分
来源：http://ttx.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://flh.ehwqpu.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yhv.sxryk.cn


<!-- 参考信息 -->