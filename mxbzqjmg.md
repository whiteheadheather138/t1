代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://zxo.shzxlz.cn

C#:   using System.Text;
来源：http://llm.gotoacloud.top

[C12] 立即执行函数 IIFE
来源：http://kxj.pycfn.com

Py:   (lambda: print("run"))()
来源：http://ema.yj20258.top

PHP:  (function () { echo "run"; })();
来源：http://ofb.jinqigufen.top

JS:   (() => { console.log("run"); })();
来源：http://zrj.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://ixg.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://prm.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://kwk.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://vrl.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qgr.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://wby.yangfankeji.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oqi.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rmh.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://afo.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oin.cqqwz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kgy.havefunace.top

Go:   func add(a, b int) int
来源：http://bph.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fia.fktsv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qnf.ydjk.org.cn

[C14] 泛型函数
来源：http://yzr.dianchejie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xdc.birdmap.top

PHP:  // 无泛型
来源：http://wfh.hnqzz.top

JS:   // 无泛型
来源：http://izi.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hgj.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ckm.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xgg.hnxiangtu.top

Ruby: # 无泛型
来源：http://nsz.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pjk.yj202588.top

[C15] 解构 / 展开参数
来源：http://quo.ybcxt.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iwv.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://vhd.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iee.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eka.ywan-chungtsiang.top

Java: // 无解构
来源：http://bbt.kuanghao11.cn

Go:   // 无解构
来源：http://xap.xinyue.icu

Ruby: a, b = pair
来源：http://nvj.chenjidiqi.icu

C#:   var (a, b) = pair;
来源：http://ueg.hcnkem.com

[C16] 函数 / 方法重载
来源：http://dqd.wangdashe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://utj.52xcode.cn

PHP:  // 无重载
来源：http://oqd.shangyingyoupin.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xoq.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://ams.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://vqd.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://pdq.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://hou.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zsf.ydjk.org.cn

================================================================================
来源：http://ebv.snrcjt.cn

D. 数组 / 列表 / 集合
来源：http://skf.birdmap.top

================================================================================
来源：http://yjb.hesvh.cn

[D01] 创建数组 / 列表
来源：http://bkb.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://dkk.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fow.hywenlv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://isn.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pcr.fktsv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jzd.nanxuanxn.top

Go:   arr := []int{1, 2, 3}
来源：http://jea.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://udh.gogol.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://odq.zhoulong.xyz

[D02] 追加元素到末尾
来源：http://uao.epnwcf.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nhb.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sad.yj20258888.top

JS:   arr.push(4);
来源：http://pdu.hcnkem.com

TS:   arr.push(4);
来源：http://ctr.aizwys.cn

Java: list.add(4);
来源：http://hqv.316326.xyz

Go:   arr = append(arr, 4)
来源：http://ojn.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://uqc.birdmap.top

C#:   list.Add(4);
来源：http://qfb.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://faa.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://oxu.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uor.pycfn.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rdq.wangdashe.top

TS:   arr.splice(0, 0, 0);
来源：http://sog.dianchejie.cn

Java: list.add(0, 0);
来源：http://snr.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xwk.birdmap.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dlz.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://aiu.chenlongwang.top

[D04] 删除元素
来源：http://buo.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xej.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gwl.xinyue.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tir.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://mrp.ydzc1.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yxj.guannengcc.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nkv.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vwj.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dsa.xinyue.icu

[D05] 访问与修改元素
来源：http://puu.yanxiufei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hsq.hfpthk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yxa.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hpm.tian-w.cn

TS:   arr[0]; arr.at(-1);
来源：http://qtd.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://kfy.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://jyp.daxiang520.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wfe.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://acb.tianlin.xyz

[D06] 数组长度
来源：http://nca.guowangkeji.top

Py:   len(arr)
来源：http://uiw.vqdsnc.cn

PHP:  count($arr);
来源：http://ean.yueranfly.top

JS:   arr.length
来源：http://kie.tarul.cn

TS:   arr.length
来源：http://rgk.yongpay.top

Java: list.size();
来源：http://opt.jyoumei.cn

Go:   len(arr)
来源：http://gkr.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://dkn.tianlin.xyz

C#:   list.Count;
来源：http://faq.pycfn.com

[D07] 切片 / 取子数组
来源：http://jib.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ebv.xingfuxueyuan.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://mke.hfpthk.cn

JS:   arr.slice(1, 4);
来源：http://ybm.jinqigfzy.top

TS:   arr.slice(1, 4);
来源：http://lon.xylfe.cn

Java: list.subList(1, 4);
来源：http://yoz.cashguo.top

Go:   arr[1:4]
来源：http://oov.yj20258888.top

Ruby: arr[1, 3]
来源：http://sfg.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://ver.gotoacloud.top

[D08] 合并两个数组
来源：http://foz.zhiwuduotai.top

Py:   a + b;  a.extend(b)
来源：http://ryv.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://esk.zhengqikj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://iof.daxiang520.top

TS:   [...a, ...b];
来源：http://qlm.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pmg.shanyushiyangkeji.top

Go:   append(a, b...)
来源：http://svq.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://poz.kuanghao11.cn

C#:   a.Concat(b).ToList()
来源：http://yvb.havefunace.top

[D09] 排序（升序）
来源：http://jdf.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://lon.bbcook.cn

PHP:  sort($arr);
来源：http://fbf.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kce.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vhm.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kst.vehdjk.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tup.bjfxy.top

Ruby: arr.sort
来源：http://qop.ppjwa.cn

C#:   list.Sort();
来源：http://hvd.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tfj.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ghm.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vza.wangdashe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://atr.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zxu.jiagoushi.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eok.zdqjudy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oma.daxiang520.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kmv.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nuj.redwolf501.top

[D11] 反转数组
来源：http://avy.ydjk.org.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qdy.hongshengwenyu.top

PHP:  array_reverse($arr);
来源：http://sui.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dce.daria6918.cn

TS:   [...arr].reverse();
来源：http://xrj.vehdjk.com

Java: Collections.reverse(list);
来源：http://sqt.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://nuu.yj202588.top

Ruby: arr.reverse
来源：http://tfd.zhixingplan.top

C#:   list.Reverse();
来源：http://zya.jiagoushi.top

[D12] 查找元素下标
来源：http://kjh.yj20258888.top

Py:   arr.index(x);  x in arr
来源：http://jvs.bjfxy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xqw.0kj1m.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vhj.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wnz.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lto.meibo888.top

Go:   slices.Index(arr, x)
来源：http://njp.jinqigufen.top

Ruby: arr.index(x)
来源：http://xcv.zycfv.cn

C#:   list.IndexOf(x);
来源：http://ecz.jinghuilouyu.cn

[D13] 过滤（保留满足条件的）
来源：http://fuf.fengsongda.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hio.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bgl.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://zux.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://fzg.yongpay.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://upz.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zat.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://dix.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kys.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://isv.yuanzhike.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jxn.hongshengwenyu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gow.gaohongyu789.top

JS:   arr.map(x => x * 2)
来源：http://bcs.yangfankeji.com

TS:   arr.map(x => x * 2)
来源：http://lym.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qve.zycfv.cn

Go:   // 手写循环
来源：http://wiy.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://xqm.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ftv.cqqwz.cn

[D15] 去重
来源：http://sgo.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bru.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://zgx.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://ohj.ydzc1.top

TS:   [...new Set(arr)]
来源：http://wsf.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://apz.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://xgm.meibo888.top

Ruby: arr.uniq
来源：http://awq.dianchejie.cn

C#:   list.Distinct().ToList()
来源：http://mcf.aizwys.cn

[D16] 求和与平均值
来源：http://qkd.daria6918.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jei.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mda.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://swz.andypj.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wcu.yuxming.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bix.pycfn.com

Go:   // 手写循环累加
来源：http://qmm.snrcjt.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mun.jinqigfzy.top

C#:   list.Sum();  list.Average()
来源：http://ptx.jiagoushi.top

[D17] 最大值与最小值
来源：http://aij.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://frz.xingfuxueyuan.xyz

PHP:  max($arr);  min($arr);
来源：http://wcf.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cnd.yonumen.top

TS:   Math.max(...arr);
来源：http://zgo.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://kue.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hfs.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://ozu.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://pnk.zdqjudy.top

[D18] 扁平化嵌套数组
来源：http://naq.ctjpmb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rjv.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://mvt.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qdg.hywenlv.cn

TS:   nested.flat();
来源：http://adj.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jui.hnxiangtu.top

Go:   // 手写双层循环
来源：http://ptb.hesvh.cn

Ruby: nested.flatten
来源：http://nvy.shzxlz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tov.zhengqikj.top

[D19] 按字段分组
来源：http://svk.feifeiyinyue.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fiq.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oud.yuanzhike.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yma.yueranfly.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cbi.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://chy.svipenyu.cn

Go:   // 手写 map[string][]T
来源：http://nsy.aizwys.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ptx.iojbl.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xbg.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://mgp.sweek.top

Py:   Counter(arr)
来源：http://yyo.zycfv.cn

PHP:  array_count_values($arr);
来源：http://phg.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qkm.hnxiangtu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://auy.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rko.yongpay.top

Go:   // 手写 map[T]int
来源：http://sca.aizwys.cn

Ruby: arr.tally
来源：http://vhw.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ihj.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://eng.andypj.xyz

Py:   x in arr
来源：http://mxj.zdbjq.cn

PHP:  in_array($x, $arr, true);
来源：http://jza.cdnleiting.top

JS:   arr.includes(x)
来源：http://xit.quarkkingdee.top

TS:   arr.includes(x)
来源：http://xyj.wangshuangyany.cn

Java: list.contains(x)
来源：http://ueh.havefunace.top

Go:   slices.Contains(arr, x)
来源：http://mca.ppjwa.cn

Ruby: arr.include?(x)
来源：http://luh.jinqigufen.top

C#:   list.Contains(x)
来源：http://hxn.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://rhb.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://soi.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qnf.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://omm.xylfe.cn

TS:   [...arr];
来源：http://jhf.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://lbp.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wpz.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://pyk.jyoumei.cn

C#:   new List<int>(list);
来源：http://gsz.sjlbkw.cn

[D23] reduce 累积计算
来源：http://lmg.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bgd.jinqigfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bwy.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gvl.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mir.0kj1m.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://skk.wangshuangyany.cn

Go:   // 手写循环
来源：http://det.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jdv.gaohongyu789.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rrt.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://mdr.yanxiufei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wev.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ijv.nanxinkj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hss.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eso.0kj1m.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uoi.birdmap.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fpw.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lie.52xcode.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://flf.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://tzs.smart0.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://utf.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xbr.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rnk.xziqi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rci.jiagoushi.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dod.dashuyun.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hsg.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iwj.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eaa.ydzc1.top

[D26] 数组转字符串
来源：http://gsy.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://kvv.tianlin.xyz

PHP:  implode(", ", $arr);
来源：http://ozg.fzhhl.top

JS:   arr.join(", ")
来源：http://tkq.shanyushiyangtech.top

TS:   arr.join(", ")
来源：http://iil.ydzc1.top

Java: String.join(", ", list)
来源：http://mlx.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://ouq.dianchejie.cn

Ruby: arr.join(", ")
来源：http://tcr.shangyingyoupin.top

C#:   string.Join(", ", list)
来源：http://xvu.gzhubu.top

================================================================================
来源：http://qsg.ywan-chungtsiang.top

E. 字符串处理
来源：http://fbn.guannengcc.top

================================================================================
来源：http://vjo.shzxlz.cn

[E01] 拼接字符串
来源：http://spd.vehdjk.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bzg.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dcu.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ppk.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://neh.birdmap.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vud.zhiwuduotai.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tmr.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://elq.yanxiufei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://psh.52xcode.cn

[E02] 重复字符串
来源：http://zdb.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://zwv.xziqi.cn

PHP:  str_repeat("ab", 3);
来源：http://bbl.yanxiufei.cn

JS:   "ab".repeat(3)
来源：http://cbw.fengsongda.top


<!-- 参考信息 -->