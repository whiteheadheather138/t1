代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://vmk.ppjwa.cn

Ruby: -> { puts "run" }.call
来源：http://wdu.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zmd.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://zar.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xem.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jlg.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bzp.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jfa.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wub.epnwcf.com

Go:   func add(a, b int) int
来源：http://fpv.hammf.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aea.sysykeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://uky.xingfuxueyuan.xyz

[C14] 泛型函数
来源：http://ria.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vnt.guannengcc.top

PHP:  // 无泛型
来源：http://oma.vqdsnc.cn

JS:   // 无泛型
来源：http://vvh.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sjc.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fqb.yuxming.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lrm.yonumen.top

Ruby: # 无泛型
来源：http://hbm.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hze.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://hyz.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sgr.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://mxk.zdbjq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yrt.pengpengdd.cyou

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nla.yj202588.top

Java: // 无解构
来源：http://kla.pycfn.com

Go:   // 无解构
来源：http://mdu.yuanzhike.top

Ruby: a, b = pair
来源：http://ept.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://tll.shzxlz.cn

[C16] 函数 / 方法重载
来源：http://uae.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tip.yongpay.top

PHP:  // 无重载
来源：http://vpc.andypj.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://roh.hywenlv.cn

TS:   // 用联合类型或重载签名声明
来源：http://xdr.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lwj.wangshuangyany.cn

Go:   // 无重载：用不同函数名
来源：http://mjv.tanke756.top

Ruby: # 无重载：靠动态参数
来源：http://wqk.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://muu.hcnkem.com

================================================================================
来源：http://aan.cashguo.top

D. 数组 / 列表 / 集合
来源：http://eie.svipenyu.cn

================================================================================
来源：http://yhg.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://qvj.wangshuangyany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nsn.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hmw.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xyy.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wbz.daxiang520.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bbc.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://axq.hfpthk.cn

Ruby: arr = [1, 2, 3]
来源：http://vlq.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zfu.cheryme.top

[D02] 追加元素到末尾
来源：http://xqc.xinyue.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rzc.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hhx.jqgfzy.top

JS:   arr.push(4);
来源：http://gsa.feifeiyinyue.top

TS:   arr.push(4);
来源：http://vbs.svipenyu.cn

Java: list.add(4);
来源：http://jgh.yonumen.top

Go:   arr = append(arr, 4)
来源：http://lig.havefunace.top

Ruby: arr << 4; arr.push(5)
来源：http://uuq.chenlongwang.top

C#:   list.Add(4);
来源：http://krm.fehbvm.com

[D03] 在指定位置插入元素
来源：http://nzi.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://dlp.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uue.zhoulong.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rbc.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://kzw.yuxming.cn

Java: list.add(0, 0);
来源：http://wfg.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sdy.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://auj.sxryk.cn

C#:   list.Insert(0, 0);
来源：http://fbb.dianchejie.cn

[D04] 删除元素
来源：http://mqx.jyoumei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://awx.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vbg.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xah.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://rbx.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jtp.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jae.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sbw.sxryk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yhy.tanke756.top

[D05] 访问与修改元素
来源：http://ooc.yj20258888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://djj.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wmw.yuanzhike.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pta.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://xuu.fengsongda.top

Java: list.get(0); list.set(0, 9);
来源：http://fkb.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://gaf.yanxiufei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fmx.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://doy.xuanzx.com

[D06] 数组长度
来源：http://sog.c1oappe.top

Py:   len(arr)
来源：http://wnl.nanxuanxn.top

PHP:  count($arr);
来源：http://sml.zhoulong.xyz

JS:   arr.length
来源：http://jla.zhengqikj.top

TS:   arr.length
来源：http://zys.gotoacloud.top

Java: list.size();
来源：http://byk.tianlin.xyz

Go:   len(arr)
来源：http://nlj.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://nul.xuanzx.com

C#:   list.Count;
来源：http://hbv.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://gmq.nanxinkj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ccc.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xnt.zhijiandao.cn

JS:   arr.slice(1, 4);
来源：http://vnl.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://qtu.yuanzhike.top

Java: list.subList(1, 4);
来源：http://nkd.pengpengdd.cyou

Go:   arr[1:4]
来源：http://png.yuanzhike.top

Ruby: arr[1, 3]
来源：http://jql.jiagoushi.top

C#:   list.GetRange(1, 3);
来源：http://dao.xuetiantiany.cn

[D08] 合并两个数组
来源：http://jgb.guowangkeji.top

Py:   a + b;  a.extend(b)
来源：http://wjv.fanxiaobao.xyz

PHP:  array_merge($a, $b);
来源：http://bbq.chenzaomai.com

JS:   [...a, ...b];  a.concat(b);
来源：http://qri.vqdsnc.cn

TS:   [...a, ...b];
来源：http://aiy.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xjz.wangshuangyany.cn

Go:   append(a, b...)
来源：http://uyr.gzhubu.top

Ruby: a + b;  a.concat(b)
来源：http://ejh.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://dzf.bbcook.cn

[D09] 排序（升序）
来源：http://ivg.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://cam.svipenyu.cn

PHP:  sort($arr);
来源：http://yep.jinghuilouyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hym.52xcode.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yoj.meibo888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jvl.aizwys.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ivd.pengpengdd.cyou

Ruby: arr.sort
来源：http://jty.birdmap.top

C#:   list.Sort();
来源：http://sut.gzhubu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fbw.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://otb.tanke756.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cmw.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kka.jqgfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://npp.svipenyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aoj.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wzu.guannengcc.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://roq.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lls.hfpthk.cn

[D11] 反转数组
来源：http://nux.zhijiandao.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rto.aizwys.cn

PHP:  array_reverse($arr);
来源：http://ejv.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lpf.uphjek.com

TS:   [...arr].reverse();
来源：http://qfc.ehwqpu.com

Java: Collections.reverse(list);
来源：http://tiz.ivvv.top

Go:   slices.Reverse(arr)
来源：http://tls.jqgufenzy.top

Ruby: arr.reverse
来源：http://nba.guowangkeji.top

C#:   list.Reverse();
来源：http://wol.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://puv.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://njy.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hvv.sweek.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hak.9152youxi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mfp.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qcz.aibaodan.cn

Go:   slices.Index(arr, x)
来源：http://cdq.bjfxy.top

Ruby: arr.index(x)
来源：http://njz.xuanzx.com

C#:   list.IndexOf(x);
来源：http://vin.vqdsnc.cn

[D13] 过滤（保留满足条件的）
来源：http://fho.ehwqpu.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yjr.xuanzx.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xaq.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://ddh.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://pgj.havefunace.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bhk.xylfe.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ubl.xingfuxueyuan.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://upw.zhaomingkeji.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://bnr.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://wtr.svipenyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yuf.52xcode.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://auj.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://aod.ivvv.top

TS:   arr.map(x => x * 2)
来源：http://xpi.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://efk.hongshengwenyu.top

Go:   // 手写循环
来源：http://sis.shuidangran.top

Ruby: arr.map { |x| x * 2 }
来源：http://xrj.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ljj.svipenyu.cn

[D15] 去重
来源：http://tsv.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pge.quarkkingdee.top

PHP:  array_unique($arr);
来源：http://rbh.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://bzf.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://qwf.sufxvd.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://olk.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://kmi.jiagoushi.top

Ruby: arr.uniq
来源：http://tdv.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://sfd.zhengqikj.top

[D16] 求和与平均值
来源：http://vkd.snrcjt.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gnz.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nmg.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bbt.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oap.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fsc.svipenyu.cn

Go:   // 手写循环累加
来源：http://hrc.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://exo.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://qyg.tian-w.cn

[D17] 最大值与最小值
来源：http://bij.vqdsnc.cn

Py:   max(arr);  min(arr)
来源：http://pgb.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://jxy.xylfe.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://egf.cashguo.top

TS:   Math.max(...arr);
来源：http://gym.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://mmc.zdqjudy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rmx.cheryme.top

Ruby: arr.max;  arr.min
来源：http://vcb.meibo888.top

C#:   list.Max();  list.Min()
来源：http://aon.hongshengwenyu.top

[D18] 扁平化嵌套数组
来源：http://xge.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hgl.redwolf501.top

PHP:  array_merge(...$nested);
来源：http://vya.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kei.jinghuilouyu.cn

TS:   nested.flat();
来源：http://kvb.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gux.iojbl.cn

Go:   // 手写双层循环
来源：http://jdl.9152youxi.cn

Ruby: nested.flatten
来源：http://ejw.guowangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ynd.birdmap.top

[D19] 按字段分组
来源：http://llq.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://amd.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lfs.sysykeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://veo.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://nmw.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ape.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://itm.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://bnv.mhx1999.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://alk.zdqjudy.top

[D20] 统计每个元素出现次数
来源：http://iik.jiagoushi.top

Py:   Counter(arr)
来源：http://oym.0kj1m.cn

PHP:  array_count_values($arr);
来源：http://gnr.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kve.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pze.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rhy.quarkkingdee.top

Go:   // 手写 map[T]int
来源：http://psu.shzxlz.cn

Ruby: arr.tally
来源：http://ymy.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://szm.yanxiufei.cn

[D21] 判断是否包含某元素
来源：http://bpi.zhiwuduotai.top

Py:   x in arr
来源：http://jpr.mhx1999.top

PHP:  in_array($x, $arr, true);
来源：http://xsa.52xcode.cn

JS:   arr.includes(x)
来源：http://aax.guowangkeji.top

TS:   arr.includes(x)
来源：http://tpa.feifeiyinyue.top

Java: list.contains(x)
来源：http://gpa.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://gfq.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://saz.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://xqf.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://quy.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eqt.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vyu.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jor.jinqigfzy.top

TS:   [...arr];
来源：http://hiq.jlsjyb.cn

Java: new ArrayList<>(list);
来源：http://vdk.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://okp.jqgfzy.top

Ruby: arr.dup;  arr.clone
来源：http://rxj.hfpthk.cn

C#:   new List<int>(list);
来源：http://cif.hnxiangtu.top

[D23] reduce 累积计算
来源：http://zka.pengpengdd.cyou

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qws.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fjm.cdnleiting.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kfa.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qqi.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jto.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://ytl.pengpengdd.cyou

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ibk.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wvn.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://dgu.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nut.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dct.cqqwz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ygi.cdnleiting.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://knv.redwolf501.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ijy.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aet.zhijiandao.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sxp.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jxv.ywan-chungtsiang.top

[D25] Set 集合去重与交并差
来源：http://bnv.aizwys.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tra.zdqjudy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gqj.gzhubu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kdr.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://clz.cashguo.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://arx.xziqi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://igt.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://stu.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nmu.yuanzhike.top

[D26] 数组转字符串
来源：http://pmm.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://all.daria6918.cn

PHP:  implode(", ", $arr);
来源：http://khz.yj202588.top

JS:   arr.join(", ")
来源：http://vxk.ybcxt.top

TS:   arr.join(", ")
来源：http://jfu.redwolf501.top

Java: String.join(", ", list)
来源：http://ctm.zhijiandao.cn

Go:   strings.Join(strs, ", ")
来源：http://wyf.yangfankeji.com

Ruby: arr.join(", ")
来源：http://ovj.jianghu66.top

C#:   string.Join(", ", list)
来源：http://yzx.havefunace.top

================================================================================
来源：http://tpe.zhengqikj.top

E. 字符串处理
来源：http://fak.guowangkeji.top

================================================================================
来源：http://rbr.hfpthk.cn

[E01] 拼接字符串
来源：http://uss.smart0.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mvq.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ccp.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cel.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vay.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jzd.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ycp.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jgk.yuanzhike.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bai.daria6918.cn

[E02] 重复字符串
来源：http://tmy.zhengqikj.top

Py:   "ab" * 3
来源：http://zql.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://edf.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://kyo.zycfv.cn

TS:   "ab".repeat(3)
来源：http://jrc.shzxlz.cn

Java: "ab".repeat(3)
来源：http://ppg.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://bpa.hesvh.cn

Ruby: "ab" * 3
来源：http://eeo.pengpengdd.cyou

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dfw.zdqjudy.top

[E03] 截取子串
来源：http://wzc.ehwqpu.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://juq.jianghu66.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eng.gaohongyu789.top


<!-- 参考信息 -->