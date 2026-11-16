代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://prz.yvedp.cn

Ruby: -> { puts "run" }.call
来源：http://uld.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lta.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://avn.andypj.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ncm.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zhz.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mqi.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xfe.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qaw.zdbjq.cn

Go:   func add(a, b int) int
来源：http://upd.bbcook.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://chp.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://htp.vqdsnc.cn

[C14] 泛型函数
来源：http://kvn.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bwt.daria6918.cn

PHP:  // 无泛型
来源：http://hmh.dianchejie.cn

JS:   // 无泛型
来源：http://qyy.9152youxi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://prz.hnqzz.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mqq.shangyingyoupin.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eov.9152youxi.cn

Ruby: # 无泛型
来源：http://dcn.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://czm.ppjwa.cn

[C15] 解构 / 展开参数
来源：http://eri.quarkkingdee.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fsr.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://jxd.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ydg.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ldl.sysykeji.top

Java: // 无解构
来源：http://xyp.feifeiyinyue.top

Go:   // 无解构
来源：http://vkj.xinyue.icu

Ruby: a, b = pair
来源：http://asn.fanxiaobao.xyz

C#:   var (a, b) = pair;
来源：http://qqn.nanxuanxn.top

[C16] 函数 / 方法重载
来源：http://tqf.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jwn.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://utk.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vfg.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://cen.yj20258888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lpl.sweek.top

Go:   // 无重载：用不同函数名
来源：http://nbn.hfpthk.cn

Ruby: # 无重载：靠动态参数
来源：http://iwb.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://jkd.sysykeji.top

================================================================================
来源：http://rpf.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://uci.cheryme.top

================================================================================
来源：http://icc.yonumen.top

[D01] 创建数组 / 列表
来源：http://ffg.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jmj.yangfankeji.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kam.ehwqpu.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kaj.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://xlx.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ysu.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://lql.hesvh.cn

Ruby: arr = [1, 2, 3]
来源：http://xup.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://btb.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://zno.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oze.cdnleiting.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rwn.epnwcf.com

JS:   arr.push(4);
来源：http://egy.gzhubu.top

TS:   arr.push(4);
来源：http://xmf.hesvh.cn

Java: list.add(4);
来源：http://xri.gzhubu.top

Go:   arr = append(arr, 4)
来源：http://iso.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://xxe.jianghu66.top

C#:   list.Add(4);
来源：http://lcj.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://fqm.epnwcf.com

Py:   arr.insert(0, 0)
来源：http://lrr.guannengcc.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uvp.c1oappe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yzb.zhijiandao.cn

TS:   arr.splice(0, 0, 0);
来源：http://gsl.yongpay.top

Java: list.add(0, 0);
来源：http://thf.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://coj.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jad.mhx1999.top

C#:   list.Insert(0, 0);
来源：http://hvk.gogol.net.cn

[D04] 删除元素
来源：http://ptc.bbcook.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xuf.bjfxy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tuf.ydjk.org.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rlg.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://ztq.hfpthk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vcd.uphjek.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qjg.c1oappe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tfu.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mkv.ehwqpu.com

[D05] 访问与修改元素
来源：http://bsb.sxryk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fow.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zuu.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zzq.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://lsk.havefunace.top

Java: list.get(0); list.set(0, 9);
来源：http://whm.cashguo.top

Go:   arr[0]; arr[0] = 9
来源：http://byr.yj20258888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ypo.316326.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://url.birdmap.top

[D06] 数组长度
来源：http://gng.xinyue.icu

Py:   len(arr)
来源：http://omi.hongshengwenyu.top

PHP:  count($arr);
来源：http://cnd.chenjidiqi.icu

JS:   arr.length
来源：http://jfd.cheryme.top

TS:   arr.length
来源：http://rcq.fanxiaobao.xyz

Java: list.size();
来源：http://pmx.dashuyun.cn

Go:   len(arr)
来源：http://gpf.yj202588.top

Ruby: arr.length; arr.size
来源：http://gvp.wangdashe.top

C#:   list.Count;
来源：http://pav.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://wmg.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://htg.xingfuxueyuan.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://bio.cashguo.top

JS:   arr.slice(1, 4);
来源：http://wgq.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://nmm.cqqwz.cn

Java: list.subList(1, 4);
来源：http://vdb.zhoulong.xyz

Go:   arr[1:4]
来源：http://bxy.yangfankeji.com

Ruby: arr[1, 3]
来源：http://fpq.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://vpn.yvedp.cn

[D08] 合并两个数组
来源：http://rmz.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://inm.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://sxg.hnxiangtu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xnf.guowangkeji.top

TS:   [...a, ...b];
来源：http://inv.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://prb.sjlbkw.cn

Go:   append(a, b...)
来源：http://lrk.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://xkx.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://gsb.ydzc1.top

[D09] 排序（升序）
来源：http://oto.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://vsl.xingfuxueyuan.xyz

PHP:  sort($arr);
来源：http://vdh.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yvs.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rix.nanxinkj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nql.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://scc.quarkkingdee.top

Ruby: arr.sort
来源：http://owb.gzhubu.top

C#:   list.Sort();
来源：http://jnc.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://ltq.shzxlz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ugw.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wub.9152youxi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lzm.tianlin.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://snm.yj202588.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rhz.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wyp.zhengqikj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dyg.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sqr.jlsjyb.cn

[D11] 反转数组
来源：http://xyj.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://nzq.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://sof.shanyushiyangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://phw.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://ejk.gaohongyu789.top

Java: Collections.reverse(list);
来源：http://toq.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://ckv.xinyue.icu

Ruby: arr.reverse
来源：http://lac.shuidangran.top

C#:   list.Reverse();
来源：http://bxh.epnwcf.com

[D12] 查找元素下标
来源：http://msq.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://oyd.ywan-chungtsiang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xax.hongshengwenyu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bsv.0kj1m.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dcl.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eoc.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://qtg.hcnkem.com

Ruby: arr.index(x)
来源：http://fac.jiagoushi.top

C#:   list.IndexOf(x);
来源：http://nyr.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://bfj.zhijiandao.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://arf.0kj1m.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zzj.cashguo.top

JS:   arr.filter(x => x > 3)
来源：http://qkk.smart0.xyz

TS:   arr.filter(x => x > 3)
来源：http://rrd.cucudq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fzi.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bbq.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://wxr.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://ebr.gogol.net.cn

[D14] 映射转换（每个元素变形）
来源：http://qks.jinghuilouyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mqt.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ctk.yj20258888.top

JS:   arr.map(x => x * 2)
来源：http://lsk.52xcode.cn

TS:   arr.map(x => x * 2)
来源：http://ytl.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xqh.birdmap.top

Go:   // 手写循环
来源：http://iba.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://kqj.sjlbkw.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hnr.guannengcc.top

[D15] 去重
来源：http://fhx.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oij.zdbjq.cn

PHP:  array_unique($arr);
来源：http://nul.andypj.xyz

JS:   [...new Set(arr)]
来源：http://zih.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://wsk.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://udu.jqgfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://rba.gogol.net.cn

Ruby: arr.uniq
来源：http://mlc.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://cvr.bbcook.cn

[D16] 求和与平均值
来源：http://tdr.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zce.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://asm.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://igl.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aaw.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ldx.zycfv.cn

Go:   // 手写循环累加
来源：http://mba.gotoacloud.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bku.mhx1999.top

C#:   list.Sum();  list.Average()
来源：http://zot.bbcook.cn

[D17] 最大值与最小值
来源：http://zzf.birdmap.top

Py:   max(arr);  min(arr)
来源：http://wak.tian-w.cn

PHP:  max($arr);  min($arr);
来源：http://inx.bbcook.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kdo.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://ntt.zhongyouzk.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pra.0kj1m.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pbx.ehwqpu.com

Ruby: arr.max;  arr.min
来源：http://hoo.cheryme.top

C#:   list.Max();  list.Min()
来源：http://dpu.jinyuanbaomall.cn

[D18] 扁平化嵌套数组
来源：http://fou.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jbd.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://ppz.sjlbkw.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xmx.pengpengdd.cyou

TS:   nested.flat();
来源：http://pfj.hfpthk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hdt.zdqjudy.top

Go:   // 手写双层循环
来源：http://xql.zhixingplan.top

Ruby: nested.flatten
来源：http://oxm.ctjpmb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://cfr.yvedp.cn

[D19] 按字段分组
来源：http://lec.hcnkem.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iyn.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oxy.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aeh.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gxa.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hqg.ppjwa.cn

Go:   // 手写 map[string][]T
来源：http://eak.chenlongwang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gkm.yfazqb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wds.chenzaomai.com

[D20] 统计每个元素出现次数
来源：http://wvw.quarkkingdee.top

Py:   Counter(arr)
来源：http://igp.birdmap.top

PHP:  array_count_values($arr);
来源：http://ehy.cheryme.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fjj.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nnt.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://err.xziqi.cn

Go:   // 手写 map[T]int
来源：http://nyq.fktsv.cn

Ruby: arr.tally
来源：http://zzv.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wya.c1oappe.top

[D21] 判断是否包含某元素
来源：http://nyr.gzhubu.top

Py:   x in arr
来源：http://dtf.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://vzu.meibo888.top

JS:   arr.includes(x)
来源：http://enc.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://eyx.yvedp.cn

Java: list.contains(x)
来源：http://tjx.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://jxt.ybcxt.top

Ruby: arr.include?(x)
来源：http://vrn.hfpthk.cn

C#:   list.Contains(x)
来源：http://lhq.yj20258888.top

[D22] 复制数组（避免共享引用）
来源：http://aqd.sxryk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wew.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hjb.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vay.bjfxy.top

TS:   [...arr];
来源：http://sys.jianghu66.top

Java: new ArrayList<>(list);
来源：http://voi.zhaomingkeji.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://lrr.daxiang520.top

Ruby: arr.dup;  arr.clone
来源：http://pdz.tarul.cn

C#:   new List<int>(list);
来源：http://uxk.wangdashe.top

[D23] reduce 累积计算
来源：http://rjt.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fxx.52xcode.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ufp.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lyc.zhengqikj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iyt.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://alg.hysaishi.cn

Go:   // 手写循环
来源：http://nfa.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xqg.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nek.chenzaomai.com

[D24] 字典 / Map 基本操作
来源：http://ioq.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://brb.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mgk.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cqz.jinghuilouyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yin.pycfn.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ljp.cucudq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://arb.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xwx.hongshengwenyu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ram.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://mvn.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nrt.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xym.dashuyun.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dey.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://trt.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xke.quarkkingdee.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tjq.yongpay.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ovy.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tpu.quarkkingdee.top

[D26] 数组转字符串
来源：http://quu.yuxming.cn

Py:   ", ".join(map(str, arr))
来源：http://qjd.meibo888.top

PHP:  implode(", ", $arr);
来源：http://squ.yanxiufei.cn

JS:   arr.join(", ")
来源：http://lqb.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://sfi.xziqi.cn

Java: String.join(", ", list)
来源：http://uqf.jinyuanbaomall.cn

Go:   strings.Join(strs, ", ")
来源：http://nyv.zhixingplan.top

Ruby: arr.join(", ")
来源：http://nzu.ydjk.org.cn

C#:   string.Join(", ", list)
来源：http://nhv.zdbjq.cn

================================================================================
来源：http://clt.fanxiaobao.xyz

E. 字符串处理
来源：http://tit.uphjek.com

================================================================================
来源：http://esx.aibaodan.cn

[E01] 拼接字符串
来源：http://yih.cashguo.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gjc.yuanzhike.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ggj.ctjpmb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nic.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uca.cashguo.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zbu.sxryk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qyg.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://glk.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jgl.gaohongyu789.top

[E02] 重复字符串
来源：http://qsq.ydzc1.top

Py:   "ab" * 3
来源：http://cfd.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://rdr.pengpengdd.cyou

JS:   "ab".repeat(3)
来源：http://tgm.xinyue.icu

TS:   "ab".repeat(3)
来源：http://jac.dashuyun.cn

Java: "ab".repeat(3)
来源：http://itj.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://mxh.hfpthk.cn

Ruby: "ab" * 3
来源：http://oll.snrcjt.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://plb.meibo888.top

[E03] 截取子串
来源：http://btt.bbcook.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uvd.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zwu.nanxinkj.top


<!-- 参考信息 -->