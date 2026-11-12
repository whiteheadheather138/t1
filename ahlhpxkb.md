代发 wailian999

[D03] 在指定位置插入元素
来源：http://xdd.sufxvd.cn

Py:   arr.insert(0, 0)
来源：http://ksk.zdqjudy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://drs.aizwys.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zcw.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://zwz.zhijiandao.cn

Java: list.add(0, 0);
来源：http://edq.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://utu.zhijiandao.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nhm.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://enf.jiagoushi.top

[D04] 删除元素
来源：http://ffu.hysaishi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://feo.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://njr.ehwqpu.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cab.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://tks.chenjidiqi.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://box.aizwys.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rkx.316326.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://plj.nanxinkj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cwr.chenjidiqi.icu

[D05] 访问与修改元素
来源：http://wjh.vqdsnc.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bdg.feifeiyinyue.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yvi.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pxw.hammf.cn

TS:   arr[0]; arr.at(-1);
来源：http://akk.yongpay.top

Java: list.get(0); list.set(0, 9);
来源：http://psh.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://wnh.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wlw.c1oappe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xda.nwbrower.top

[D06] 数组长度
来源：http://tyt.yj20258.top

Py:   len(arr)
来源：http://pbd.cqqwz.cn

PHP:  count($arr);
来源：http://agg.feifeiyinyue.top

JS:   arr.length
来源：http://weg.zdqjudy.top

TS:   arr.length
来源：http://dmh.zhongyouzk.top

Java: list.size();
来源：http://yvz.gzhubu.top

Go:   len(arr)
来源：http://emb.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://cxd.andypj.xyz

C#:   list.Count;
来源：http://wxg.shzxlz.cn

[D07] 切片 / 取子数组
来源：http://rba.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cwg.jqgfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://yir.c1oappe.top

JS:   arr.slice(1, 4);
来源：http://pid.dianchejie.cn

TS:   arr.slice(1, 4);
来源：http://rix.hnqzz.top

Java: list.subList(1, 4);
来源：http://fll.yanxiufei.cn

Go:   arr[1:4]
来源：http://lla.fktsv.cn

Ruby: arr[1, 3]
来源：http://jyb.zhijiandao.cn

C#:   list.GetRange(1, 3);
来源：http://mol.hcnkem.com

[D08] 合并两个数组
来源：http://syd.pycfn.com

Py:   a + b;  a.extend(b)
来源：http://nqj.jinghuilouyu.cn

PHP:  array_merge($a, $b);
来源：http://kxa.gogol.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xeg.xziqi.cn

TS:   [...a, ...b];
来源：http://ypx.haohaochexian.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xjk.hcnkem.com

Go:   append(a, b...)
来源：http://lmy.gaohongyu789.top

Ruby: a + b;  a.concat(b)
来源：http://ddu.yj20258.top

C#:   a.Concat(b).ToList()
来源：http://rom.snrcjt.cn

[D09] 排序（升序）
来源：http://hrx.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://zyb.yueranfly.top

PHP:  sort($arr);
来源：http://bnw.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tza.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tsp.cqqwz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zek.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uqt.zhijiandao.cn

Ruby: arr.sort
来源：http://wsm.sjlbkw.cn

C#:   list.Sort();
来源：http://lyd.havefunace.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hte.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qsh.gzhubu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uwj.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://asz.pengpengdd.cyou

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qxp.zdbjq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nvr.birdmap.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lmc.hnxiangtu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zfu.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://grq.shanyushiyangkeji.top

[D11] 反转数组
来源：http://rox.zhijiandao.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oaa.chenlongwang.top

PHP:  array_reverse($arr);
来源：http://oid.xuetiantiany.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vsw.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://jvs.wangshuangyany.cn

Java: Collections.reverse(list);
来源：http://gnm.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://uxw.vqdsnc.cn

Ruby: arr.reverse
来源：http://ytu.meibo888.top

C#:   list.Reverse();
来源：http://duf.0kj1m.cn

[D12] 查找元素下标
来源：http://wyg.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://zmp.cashguo.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://roj.xuanzx.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bgi.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iwh.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://psl.dashuyun.cn

Go:   slices.Index(arr, x)
来源：http://yie.svipenyu.cn

Ruby: arr.index(x)
来源：http://wij.yfazqb.com

C#:   list.IndexOf(x);
来源：http://gfc.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://pln.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://prf.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ygp.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://ads.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://ssh.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://puh.zdbjq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qhm.hongshengwenyu.top

Ruby: arr.select { |x| x > 3 }
来源：http://blv.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gxh.zhixingplan.top

[D14] 映射转换（每个元素变形）
来源：http://hdt.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ofs.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ckk.yonumen.top

JS:   arr.map(x => x * 2)
来源：http://wnb.fanxiaobao.xyz

TS:   arr.map(x => x * 2)
来源：http://yrf.tarul.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cnf.zhoulong.xyz

Go:   // 手写循环
来源：http://jbx.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://btl.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://eyc.jinqigfzy.top

[D15] 去重
来源：http://cqw.sweek.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vnn.andypj.xyz

PHP:  array_unique($arr);
来源：http://iic.smart0.xyz

JS:   [...new Set(arr)]
来源：http://hqd.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://pcz.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ctx.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lis.hysaishi.cn

Ruby: arr.uniq
来源：http://mat.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://bxc.birdmap.top

[D16] 求和与平均值
来源：http://sub.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cli.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iyt.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qrq.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pbu.daxiang520.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lmd.zhoulong.xyz

Go:   // 手写循环累加
来源：http://hmr.chenjidiqi.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://con.shuidangran.top

C#:   list.Sum();  list.Average()
来源：http://jhr.birdmap.top

[D17] 最大值与最小值
来源：http://skk.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://hcg.hongshengwenyu.top

PHP:  max($arr);  min($arr);
来源：http://ebk.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dok.cashguo.top

TS:   Math.max(...arr);
来源：http://tox.redwolf501.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ppt.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qkl.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://aes.jinqigufen.top

C#:   list.Max();  list.Min()
来源：http://tcb.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://yqh.yueranfly.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oiq.zhijiandao.cn

PHP:  array_merge(...$nested);
来源：http://emd.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://asv.haohaochexian.top

TS:   nested.flat();
来源：http://auc.gzhubu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dka.jinyuanbaomall.cn

Go:   // 手写双层循环
来源：http://vtm.xziqi.cn

Ruby: nested.flatten
来源：http://zqi.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://nhx.yvedp.cn

[D19] 按字段分组
来源：http://zvc.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gbc.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pgj.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tri.jqgufenzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nnx.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wng.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://lkv.jlsjyb.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rop.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qwx.yj20258.top

[D20] 统计每个元素出现次数
来源：http://qwf.jinqigufen.top

Py:   Counter(arr)
来源：http://wdd.tian-w.cn

PHP:  array_count_values($arr);
来源：http://acj.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xwq.bbcook.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kel.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://arx.shzxlz.cn

Go:   // 手写 map[T]int
来源：http://hmf.yj20258888.top

Ruby: arr.tally
来源：http://acy.havefunace.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://evt.tarul.cn

[D21] 判断是否包含某元素
来源：http://qcp.nanxinkj.top

Py:   x in arr
来源：http://pdf.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://aev.nanxuanxn.top

JS:   arr.includes(x)
来源：http://iel.haohaochexian.top

TS:   arr.includes(x)
来源：http://eql.yonumen.top

Java: list.contains(x)
来源：http://uwa.hysaishi.cn

Go:   slices.Contains(arr, x)
来源：http://xvm.fzhhl.top

Ruby: arr.include?(x)
来源：http://foz.hnqzz.top

C#:   list.Contains(x)
来源：http://qjy.hammf.cn

[D22] 复制数组（避免共享引用）
来源：http://tsr.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tmd.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nhh.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tny.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://vwe.daria6918.cn

Java: new ArrayList<>(list);
来源：http://xdz.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://qgl.ydjk.org.cn

Ruby: arr.dup;  arr.clone
来源：http://rkv.nanxuanxn.top

C#:   new List<int>(list);
来源：http://std.redwolf501.top

[D23] reduce 累积计算
来源：http://mtw.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ows.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zef.bjfxy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://otv.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ovp.9152youxi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nqy.ctjpmb.com

Go:   // 手写循环
来源：http://vrt.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aud.mhx1999.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://waf.hammf.cn

[D24] 字典 / Map 基本操作
来源：http://fnm.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vlx.andypj.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qwo.xylfe.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oxe.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wtv.daria6918.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://orz.gogol.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zft.cheryme.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aea.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gyn.zhengqikj.top

[D25] Set 集合去重与交并差
来源：http://hqp.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://owx.52xcode.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tdk.cheryme.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://etd.yuanzhike.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qyq.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cri.yongpay.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://egb.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zdx.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://beh.kuanghao11.cn

[D26] 数组转字符串
来源：http://uwh.cheryme.top

Py:   ", ".join(map(str, arr))
来源：http://spb.ppjwa.cn

PHP:  implode(", ", $arr);
来源：http://igp.fzhhl.top

JS:   arr.join(", ")
来源：http://bmz.iojbl.cn

TS:   arr.join(", ")
来源：http://ghn.zdqjudy.top

Java: String.join(", ", list)
来源：http://mvm.uphjek.com

Go:   strings.Join(strs, ", ")
来源：http://wgk.bbcook.cn

Ruby: arr.join(", ")
来源：http://rih.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://brl.wangdashe.top

================================================================================
来源：http://dzm.nwbrower.top

E. 字符串处理
来源：http://ads.chenjidiqi.icu

================================================================================
来源：http://oae.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://orl.meibo888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wwh.fengsongda.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ebi.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ewg.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ixy.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mpg.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ikx.svipenyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yln.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ycm.xziqi.cn

[E02] 重复字符串
来源：http://ryc.cucudq.cn

Py:   "ab" * 3
来源：http://itp.chenzaomai.com

PHP:  str_repeat("ab", 3);
来源：http://izu.ppjwa.cn

JS:   "ab".repeat(3)
来源：http://qqn.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://yxb.tanke756.top

Java: "ab".repeat(3)
来源：http://tkn.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://fos.ywan-chungtsiang.top

Ruby: "ab" * 3
来源：http://xjj.nwbrower.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jye.nwbrower.top

[E03] 截取子串
来源：http://hiy.fehbvm.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://scg.tanke756.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lqk.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wzh.hesvh.cn

TS:   s.slice(1, 4)
来源：http://qxt.chenzaomai.com

Java: s.substring(1, 4)
来源：http://agp.nanxinkj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yzq.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dsv.vqdsnc.cn

C#:   s.Substring(1, 3)
来源：http://vxs.tian-w.cn

[E04] 查找子串位置
来源：http://cgx.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://air.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://mgg.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xqz.zdbjq.cn

TS:   s.indexOf("x")
来源：http://yzr.wangdashe.top

Java: s.indexOf("x")
来源：http://nki.ydjk.org.cn

Go:   strings.Index(s, "x")
来源：http://spt.hnxiangtu.top

Ruby: s.index("x")
来源：http://dch.bjfxy.top

C#:   s.IndexOf("x")
来源：http://ebs.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ers.sysykeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jnc.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://apf.jianghu66.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uob.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jdu.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zju.guowangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yhd.yj202588.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bof.fengsongda.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://atp.sysykeji.top

[E06] 替换子串
来源：http://dma.xinyue.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qtx.cashguo.top

PHP:  str_replace("a", "b", $s);
来源：http://jdu.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dbq.meibo888.top

TS:   s.replaceAll("a", "b")
来源：http://omd.yueranfly.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rrg.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mpx.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kzj.yj20258888.top

C#:   s.Replace("a", "b")
来源：http://uwo.guowangkeji.top

[E07] 按分隔符拆分
来源：http://ush.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://twl.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kae.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://saw.yj202588.top

TS:   s.split(",")
来源：http://tkz.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://kat.guowangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cvc.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://jmt.svipenyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cmq.zhijiandao.cn

[E08] 数组按分隔符合并
来源：http://xbq.jyoumei.cn

Py:   ",".join(items)
来源：http://ktv.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://lmn.pycfn.com

JS:   items.join(",")
来源：http://cvk.jqgfzy.top

TS:   items.join(",")
来源：http://drt.cucudq.cn

Java: String.join(",", items)
来源：http://xkr.yuanzhike.top

Go:   strings.Join(items, ",")
来源：http://ajh.fengsongda.top

Ruby: items.join(",")
来源：http://opj.cashguo.top

C#:   string.Join(",", items)
来源：http://cka.hfpthk.cn

[E09] 去除所有空白字符
来源：http://ocu.jqgfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zbg.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ypa.sufxvd.cn

JS:   s.replace(/\s+/g, "")
来源：http://cya.aizwys.cn

TS:   s.replace(/\s+/g, "")
来源：http://yoy.andypj.xyz

Java: s.replaceAll("\\s+", "")
来源：http://yrf.jinqigfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ooo.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://nkh.fzhhl.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yup.chenzaomai.com


<!-- 参考信息 -->