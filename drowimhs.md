代发 wailian999

Ruby: a, b = pair
来源：http://kbg.yongpay.top

C#:   var (a, b) = pair;
来源：http://hmg.zhixingplan.top

[C16] 函数 / 方法重载
来源：http://emc.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://abo.xuetiantiany.cn

PHP:  // 无重载
来源：http://ikn.jianghu66.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://edd.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://eyi.cucudq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gdg.jinqigfzy.top

Go:   // 无重载：用不同函数名
来源：http://gmw.daxiang520.top

Ruby: # 无重载：靠动态参数
来源：http://xfi.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://eoj.xuanzx.com

================================================================================
来源：http://rcm.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://pqk.gzhubu.top

================================================================================
来源：http://nfi.zycfv.cn

[D01] 创建数组 / 列表
来源：http://ooq.kuanghao11.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://orr.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://htu.iojbl.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lno.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hui.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nii.yvedp.cn

Go:   arr := []int{1, 2, 3}
来源：http://tmp.smart0.xyz

Ruby: arr = [1, 2, 3]
来源：http://ogq.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yef.52xcode.cn

[D02] 追加元素到末尾
来源：http://ujj.ctjpmb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://djc.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://njx.vqdsnc.cn

JS:   arr.push(4);
来源：http://xsb.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://vai.chenzaomai.com

Java: list.add(4);
来源：http://mxk.meibo888.top

Go:   arr = append(arr, 4)
来源：http://qub.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://ziy.nwbrower.top

C#:   list.Add(4);
来源：http://yry.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://orz.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://kqk.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jii.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ppy.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://kbd.zhixingplan.top

Java: list.add(0, 0);
来源：http://hdp.vehdjk.com

Go:   arr = append([]int{0}, arr...)
来源：http://fyy.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fjx.cqqwz.cn

C#:   list.Insert(0, 0);
来源：http://zus.jqgufenzy.top

[D04] 删除元素
来源：http://juy.yueranfly.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gld.zhengqikj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ndb.xinyue.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hzu.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://xfl.feifeiyinyue.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ksp.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jik.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dop.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pqc.jinyuanbaomall.cn

[D05] 访问与修改元素
来源：http://nas.gotoacloud.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zoh.hnqzz.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://evw.xylfe.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vjq.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://hen.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://kdt.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://jrv.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://scg.zhixingplan.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qri.iojbl.cn

[D06] 数组长度
来源：http://rpt.cashguo.top

Py:   len(arr)
来源：http://ctp.xuanzx.com

PHP:  count($arr);
来源：http://dfd.wangshuangyany.cn

JS:   arr.length
来源：http://jip.9152youxi.cn

TS:   arr.length
来源：http://onw.0kj1m.cn

Java: list.size();
来源：http://kkp.zhaomingkeji.xyz

Go:   len(arr)
来源：http://uyk.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://xvk.zhoulong.xyz

C#:   list.Count;
来源：http://dsf.epnwcf.com

[D07] 切片 / 取子数组
来源：http://sft.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://son.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fai.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://irt.hammf.cn

TS:   arr.slice(1, 4);
来源：http://zme.fengsongda.top

Java: list.subList(1, 4);
来源：http://hto.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://qro.jianghu66.top

Ruby: arr[1, 3]
来源：http://alu.shangyingyoupin.top

C#:   list.GetRange(1, 3);
来源：http://mkk.chenzaomai.com

[D08] 合并两个数组
来源：http://vtg.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://dzp.hcnkem.com

PHP:  array_merge($a, $b);
来源：http://wma.0kj1m.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ubt.jiagoushi.top

TS:   [...a, ...b];
来源：http://pxf.zhixingplan.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sez.pengpengdd.cyou

Go:   append(a, b...)
来源：http://dbe.yj20258888.top

Ruby: a + b;  a.concat(b)
来源：http://cii.cucudq.cn

C#:   a.Concat(b).ToList()
来源：http://igl.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://ent.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://jrc.nwbrower.top

PHP:  sort($arr);
来源：http://yde.zycfv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uxr.tianlin.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://xup.sufxvd.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jbi.snrcjt.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hry.svipenyu.cn

Ruby: arr.sort
来源：http://ygd.jlsjyb.cn

C#:   list.Sort();
来源：http://cso.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://muz.hysaishi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kiq.yj202588.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gor.sxryk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://slo.tarul.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ntv.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vot.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ywz.chenlongwang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xyt.shuidangran.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wnj.sweek.top

[D11] 反转数组
来源：http://tbr.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://sfg.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://zxf.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vku.hcnkem.com

TS:   [...arr].reverse();
来源：http://wac.jianghu66.top

Java: Collections.reverse(list);
来源：http://itq.hammf.cn

Go:   slices.Reverse(arr)
来源：http://wua.gotoacloud.top

Ruby: arr.reverse
来源：http://ckc.zdqjudy.top

C#:   list.Reverse();
来源：http://qdq.tian-w.cn

[D12] 查找元素下标
来源：http://omd.sysykeji.top

Py:   arr.index(x);  x in arr
来源：http://nxm.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eke.epnwcf.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gtk.zdqjudy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xpp.ybcxt.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xwk.kuanghao11.cn

Go:   slices.Index(arr, x)
来源：http://spv.yonumen.top

Ruby: arr.index(x)
来源：http://oex.guannengcc.top

C#:   list.IndexOf(x);
来源：http://wdq.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://hfr.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://shi.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ism.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://omj.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://wbx.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kuw.aizwys.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dvb.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zqx.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://krj.aibaodan.cn

[D14] 映射转换（每个元素变形）
来源：http://vwl.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wvd.jiagoushi.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kbx.nanxinkj.top

JS:   arr.map(x => x * 2)
来源：http://wvd.andypj.xyz

TS:   arr.map(x => x * 2)
来源：http://spm.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dsy.ydjk.org.cn

Go:   // 手写循环
来源：http://rqe.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gvy.c1oappe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://eay.wangshuangyany.cn

[D15] 去重
来源：http://gal.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vpp.gaohongyu789.top

PHP:  array_unique($arr);
来源：http://pai.smart0.xyz

JS:   [...new Set(arr)]
来源：http://myb.xuanzx.com

TS:   [...new Set(arr)]
来源：http://gpe.hnxiangtu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gkf.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yyj.xuetiantiany.cn

Ruby: arr.uniq
来源：http://ror.fanxiaobao.xyz

C#:   list.Distinct().ToList()
来源：http://vgh.tarul.cn

[D16] 求和与平均值
来源：http://xur.sweek.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lkn.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dbs.cashguo.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ula.vehdjk.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wav.hnxiangtu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gdt.cheryme.top

Go:   // 手写循环累加
来源：http://vyr.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vwp.jyoumei.cn

C#:   list.Sum();  list.Average()
来源：http://kec.hcnkem.com

[D17] 最大值与最小值
来源：http://nsn.tanke756.top

Py:   max(arr);  min(arr)
来源：http://rtr.smart0.xyz

PHP:  max($arr);  min($arr);
来源：http://hwm.fehbvm.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://aqw.hfpthk.cn

TS:   Math.max(...arr);
来源：http://zsn.yfazqb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://tqf.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://beh.pycfn.com

Ruby: arr.max;  arr.min
来源：http://apf.hywenlv.cn

C#:   list.Max();  list.Min()
来源：http://lro.yonumen.top

[D18] 扁平化嵌套数组
来源：http://lnt.ydzc1.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://byq.sjlbkw.cn

PHP:  array_merge(...$nested);
来源：http://kmn.redwolf501.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://umt.316326.xyz

TS:   nested.flat();
来源：http://vja.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pbe.yj20258888.top

Go:   // 手写双层循环
来源：http://jht.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://kix.jyoumei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hgr.shzxlz.cn

[D19] 按字段分组
来源：http://cln.shanyushiyangtech.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dzs.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://spa.fanxiaobao.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xoj.hcnkem.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://owv.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ozk.tanke756.top

Go:   // 手写 map[string][]T
来源：http://rcy.9152youxi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rgr.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zvt.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://rvh.jinqigufen.top

Py:   Counter(arr)
来源：http://dyb.c1oappe.top

PHP:  array_count_values($arr);
来源：http://yxr.hammf.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mvm.ctjpmb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uwk.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://smk.gaohongyu789.top

Go:   // 手写 map[T]int
来源：http://llm.yuxming.cn

Ruby: arr.tally
来源：http://qhq.pengpengdd.cyou

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://djq.sjlbkw.cn

[D21] 判断是否包含某元素
来源：http://twh.hongshengwenyu.top

Py:   x in arr
来源：http://uaw.svipenyu.cn

PHP:  in_array($x, $arr, true);
来源：http://hik.pycfn.com

JS:   arr.includes(x)
来源：http://kwi.redwolf501.top

TS:   arr.includes(x)
来源：http://kge.hnqzz.top

Java: list.contains(x)
来源：http://lbe.chenlongwang.top

Go:   slices.Contains(arr, x)
来源：http://tts.nwbrower.top

Ruby: arr.include?(x)
来源：http://fmv.cheryme.top

C#:   list.Contains(x)
来源：http://djd.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://opa.yuanzhike.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blo.cheryme.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dbs.gogol.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aeh.jinqigfzy.top

TS:   [...arr];
来源：http://ziz.52xcode.cn

Java: new ArrayList<>(list);
来源：http://yme.fzhhl.top

Go:   copied := append([]int(nil), arr...)
来源：http://gey.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://icn.svipenyu.cn

C#:   new List<int>(list);
来源：http://djp.zhongyouzk.top

[D23] reduce 累积计算
来源：http://wcv.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wqu.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://agl.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zdc.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vuj.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wpa.sweek.top

Go:   // 手写循环
来源：http://gum.52xcode.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tdi.vqdsnc.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pmg.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://dzx.ydzc1.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ffn.hysaishi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qtb.hfpthk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://agc.cdnleiting.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mca.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://emb.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dui.hesvh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qdr.gaohongyu789.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qdn.zhoulong.xyz

[D25] Set 集合去重与交并差
来源：http://uyk.yangfankeji.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gve.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pfh.dianchejie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pnb.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ieb.yj20258.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jum.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wei.svipenyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lfl.zhongyouzk.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yxo.pengpengdd.cyou

[D26] 数组转字符串
来源：http://ngf.ydzc1.top

Py:   ", ".join(map(str, arr))
来源：http://hrb.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://saw.ywan-chungtsiang.top

JS:   arr.join(", ")
来源：http://bbk.ppjwa.cn

TS:   arr.join(", ")
来源：http://cig.hnqzz.top

Java: String.join(", ", list)
来源：http://nmh.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://tnt.ehwqpu.com

Ruby: arr.join(", ")
来源：http://ntg.fengsongda.top

C#:   string.Join(", ", list)
来源：http://ule.tanke756.top

================================================================================
来源：http://btx.yuanzhike.top

E. 字符串处理
来源：http://jib.xziqi.cn

================================================================================
来源：http://icb.yj20258888.top

[E01] 拼接字符串
来源：http://fbo.xuetiantiany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hng.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xbi.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xov.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zdj.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ial.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nem.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cds.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tec.52xcode.cn

[E02] 重复字符串
来源：http://ksz.zhengqikj.top

Py:   "ab" * 3
来源：http://rtc.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://wrp.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://drt.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://clj.yanxiufei.cn

Java: "ab".repeat(3)
来源：http://yys.jiagoushi.top

Go:   strings.Repeat("ab", 3)
来源：http://sxf.hywenlv.cn

Ruby: "ab" * 3
来源：http://eff.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tyu.ivvv.top

[E03] 截取子串
来源：http://fga.smart0.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tzv.cdnleiting.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eiz.cqqwz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://amj.yj202588.top

TS:   s.slice(1, 4)
来源：http://jfo.ybcxt.top

Java: s.substring(1, 4)
来源：http://eig.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aud.fzhhl.top

Ruby: s[1, 3];  s[1..3]
来源：http://mgn.quarkkingdee.top

C#:   s.Substring(1, 3)
来源：http://jku.svipenyu.cn

[E04] 查找子串位置
来源：http://wyp.jianghu66.top

Py:   s.find("x");  s.index("x")
来源：http://ahe.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://yuj.zycfv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sjw.pycfn.com

TS:   s.indexOf("x")
来源：http://swa.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://txg.epnwcf.com

Go:   strings.Index(s, "x")
来源：http://gbq.mhx1999.top

Ruby: s.index("x")
来源：http://qvy.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://lju.ivvv.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zxh.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fmu.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fon.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xgl.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://pwj.zhongyouzk.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://amd.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://trg.nwbrower.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ffs.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wyb.yuxming.cn

[E06] 替换子串
来源：http://rja.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lrs.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://btf.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hxr.havefunace.top


<!-- 参考信息 -->