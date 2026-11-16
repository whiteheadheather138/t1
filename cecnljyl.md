代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://dfy.fehbvm.com

C#:   using System.Text;
来源：http://dcb.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://wje.sufxvd.cn

Py:   (lambda: print("run"))()
来源：http://ces.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://tex.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://zfr.shanyushiyangtech.top

TS:   (() => { console.log("run"); })();
来源：http://hbi.ybcxt.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://arc.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://wdn.zhongyouzk.top

Ruby: -> { puts "run" }.call
来源：http://qpm.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gkl.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://agz.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bcg.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vyc.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zxw.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://seq.bbcook.cn

Java: int add(int a, int b) { return a + b; }
来源：http://irc.tianlin.xyz

Go:   func add(a, b int) int
来源：http://was.zhengqikj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pjc.jinghuilouyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rsq.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://mkd.andypj.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lob.tianlin.xyz

PHP:  // 无泛型
来源：http://woj.guowangkeji.top

JS:   // 无泛型
来源：http://jtm.iojbl.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://flx.316326.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qud.chenjidiqi.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xyt.zhengqikj.top

Ruby: # 无泛型
来源：http://mce.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vrb.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://mkn.jlsjyb.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xxf.birdmap.top

PHP:  [$a, $b] = $pair;
来源：http://flu.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bik.yanxiufei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kar.cucudq.cn

Java: // 无解构
来源：http://oco.xylfe.cn

Go:   // 无解构
来源：http://tnl.hammf.cn

Ruby: a, b = pair
来源：http://jwp.hesvh.cn

C#:   var (a, b) = pair;
来源：http://ott.redwolf501.top

[C16] 函数 / 方法重载
来源：http://kxr.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mlg.snrcjt.cn

PHP:  // 无重载
来源：http://wsb.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hsc.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://sld.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xwn.ctjpmb.com

Go:   // 无重载：用不同函数名
来源：http://hlw.iojbl.cn

Ruby: # 无重载：靠动态参数
来源：http://cba.cqqwz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tpe.c1oappe.top

================================================================================
来源：http://ehs.aizwys.cn

D. 数组 / 列表 / 集合
来源：http://kxx.316326.xyz

================================================================================
来源：http://vll.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://uvk.bbcook.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://eib.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eyp.ivvv.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hze.0kj1m.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rno.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vdl.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://lzp.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://hyo.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hhr.jiagoushi.top

[D02] 追加元素到末尾
来源：http://rms.zhijiandao.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aln.wangdashe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hun.feifeiyinyue.top

JS:   arr.push(4);
来源：http://dtq.gotoacloud.top

TS:   arr.push(4);
来源：http://wvk.pengpengdd.cyou

Java: list.add(4);
来源：http://luc.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://rhc.nanxinkj.top

Ruby: arr << 4; arr.push(5)
来源：http://vhd.tanke756.top

C#:   list.Add(4);
来源：http://zwz.chenzaomai.com

[D03] 在指定位置插入元素
来源：http://yoi.havefunace.top

Py:   arr.insert(0, 0)
来源：http://hxj.shangyingyoupin.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wqk.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vwh.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://hco.zdqjudy.top

Java: list.add(0, 0);
来源：http://shz.bjfxy.top

Go:   arr = append([]int{0}, arr...)
来源：http://vog.yj202588.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dil.xinyue.icu

C#:   list.Insert(0, 0);
来源：http://eiz.jinqigufen.top

[D04] 删除元素
来源：http://msy.zhoulong.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aug.jlsjyb.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ton.ppjwa.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hqs.hnqzz.top

TS:   arr.splice(0, 1);
来源：http://wgk.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xgl.shangyingyoupin.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zhu.daria6918.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gtd.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fea.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://cyg.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ley.nanxuanxn.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hfx.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ywq.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://tdv.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://xyq.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://yxw.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ebk.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kfq.fengsongda.top

[D06] 数组长度
来源：http://dev.mhx1999.top

Py:   len(arr)
来源：http://nvc.yanxiufei.cn

PHP:  count($arr);
来源：http://yyu.xuetiantiany.cn

JS:   arr.length
来源：http://ceq.ybcxt.top

TS:   arr.length
来源：http://wui.smart0.xyz

Java: list.size();
来源：http://bkc.cucudq.cn

Go:   len(arr)
来源：http://agm.zhaomingkeji.xyz

Ruby: arr.length; arr.size
来源：http://vuk.shzxlz.cn

C#:   list.Count;
来源：http://jqz.xylfe.cn

[D07] 切片 / 取子数组
来源：http://hkl.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pci.yueranfly.top

PHP:  array_slice($arr, 1, 3);
来源：http://jax.yfazqb.com

JS:   arr.slice(1, 4);
来源：http://qrv.smart0.xyz

TS:   arr.slice(1, 4);
来源：http://ipw.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://rka.sufxvd.cn

Go:   arr[1:4]
来源：http://fjc.dashuyun.cn

Ruby: arr[1, 3]
来源：http://ynf.aibaodan.cn

C#:   list.GetRange(1, 3);
来源：http://img.kuanghao11.cn

[D08] 合并两个数组
来源：http://vgl.shzxlz.cn

Py:   a + b;  a.extend(b)
来源：http://mik.aizwys.cn

PHP:  array_merge($a, $b);
来源：http://krj.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://ufm.shzxlz.cn

TS:   [...a, ...b];
来源：http://pxe.yonumen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cnt.jqgfzy.top

Go:   append(a, b...)
来源：http://hdu.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://cby.chenjidiqi.icu

C#:   a.Concat(b).ToList()
来源：http://dei.bjfxy.top

[D09] 排序（升序）
来源：http://yzi.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://xii.fengsongda.top

PHP:  sort($arr);
来源：http://wrq.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wqg.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mzd.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pes.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://otj.cdnleiting.top

Ruby: arr.sort
来源：http://hms.ydjk.org.cn

C#:   list.Sort();
来源：http://ktm.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ggh.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nkj.zhengqikj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://avd.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qic.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hqh.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://avq.haohaochexian.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xkw.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oma.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vlm.cucudq.cn

[D11] 反转数组
来源：http://oip.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://zpm.c1oappe.top

PHP:  array_reverse($arr);
来源：http://mcp.sjlbkw.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bgy.fengsongda.top

TS:   [...arr].reverse();
来源：http://pjm.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://prs.daria6918.cn

Go:   slices.Reverse(arr)
来源：http://wuf.svipenyu.cn

Ruby: arr.reverse
来源：http://ipb.hywenlv.cn

C#:   list.Reverse();
来源：http://hty.dianchejie.cn

[D12] 查找元素下标
来源：http://mjl.dashuyun.cn

Py:   arr.index(x);  x in arr
来源：http://orx.0kj1m.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rji.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iwl.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mso.jinyuanbaomall.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://joc.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://aiy.ivvv.top

Ruby: arr.index(x)
来源：http://cwa.yangfankeji.com

C#:   list.IndexOf(x);
来源：http://dek.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://kng.ydjk.org.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dtg.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://czc.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://ifw.daria6918.cn

TS:   arr.filter(x => x > 3)
来源：http://prm.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lrn.xziqi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://noe.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://lgo.fanxiaobao.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://zzf.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://jou.hfpthk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mnm.ywan-chungtsiang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ueg.meibo888.top

JS:   arr.map(x => x * 2)
来源：http://wwi.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://rfp.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pil.daxiang520.top

Go:   // 手写循环
来源：http://eao.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mug.c1oappe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yjq.316326.xyz

[D15] 去重
来源：http://nxl.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mvw.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://nfe.iojbl.cn

JS:   [...new Set(arr)]
来源：http://vwt.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://qfj.meibo888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kwt.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://dvu.haohaochexian.top

Ruby: arr.uniq
来源：http://zej.hnxiangtu.top

C#:   list.Distinct().ToList()
来源：http://mic.iojbl.cn

[D16] 求和与平均值
来源：http://run.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mhr.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kiq.vqdsnc.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qlf.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sbv.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bjt.dianchejie.cn

Go:   // 手写循环累加
来源：http://qyy.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zti.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://dai.xziqi.cn

[D17] 最大值与最小值
来源：http://una.meibo888.top

Py:   max(arr);  min(arr)
来源：http://nbl.zhoulong.xyz

PHP:  max($arr);  min($arr);
来源：http://ovj.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://toz.bjfxy.top

TS:   Math.max(...arr);
来源：http://spx.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://avr.sufxvd.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nyj.nwbrower.top

Ruby: arr.max;  arr.min
来源：http://tqy.aizwys.cn

C#:   list.Max();  list.Min()
来源：http://avt.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://kcd.cucudq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tem.daxiang520.top

PHP:  array_merge(...$nested);
来源：http://xbf.jianghu66.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tof.snrcjt.cn

TS:   nested.flat();
来源：http://oeb.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ftc.zdbjq.cn

Go:   // 手写双层循环
来源：http://loe.birdmap.top

Ruby: nested.flatten
来源：http://tls.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://ffz.ivvv.top

[D19] 按字段分组
来源：http://sws.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://piw.jiagoushi.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oav.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ohe.xuanzx.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://nhb.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kdd.yvedp.cn

Go:   // 手写 map[string][]T
来源：http://fsm.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://aoj.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vuu.svipenyu.cn

[D20] 统计每个元素出现次数
来源：http://mri.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://drx.xylfe.cn

PHP:  array_count_values($arr);
来源：http://tdm.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gsy.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ksv.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mad.zhiwuduotai.top

Go:   // 手写 map[T]int
来源：http://kkv.ywan-chungtsiang.top

Ruby: arr.tally
来源：http://hjw.gaohongyu789.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dzv.cheryme.top

[D21] 判断是否包含某元素
来源：http://kcs.fktsv.cn

Py:   x in arr
来源：http://bud.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://xln.52xcode.cn

JS:   arr.includes(x)
来源：http://vaq.ivvv.top

TS:   arr.includes(x)
来源：http://glz.zycfv.cn

Java: list.contains(x)
来源：http://kid.zhaomingkeji.xyz

Go:   slices.Contains(arr, x)
来源：http://jwj.smart0.xyz

Ruby: arr.include?(x)
来源：http://lwp.pycfn.com

C#:   list.Contains(x)
来源：http://bpe.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://ptv.316326.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://enu.daxiang520.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://axb.hfpthk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ygu.dianchejie.cn

TS:   [...arr];
来源：http://mrw.shanyushiyangkeji.top

Java: new ArrayList<>(list);
来源：http://lfa.ydjk.org.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ivk.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://ibp.xuanzx.com

C#:   new List<int>(list);
来源：http://azo.jyoumei.cn

[D23] reduce 累积计算
来源：http://uql.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kca.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oke.ivvv.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xfh.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://apc.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://geu.fengsongda.top

Go:   // 手写循环
来源：http://wah.yuanzhike.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eut.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eid.sufxvd.cn

[D24] 字典 / Map 基本操作
来源：http://evn.daxiang520.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://swy.epnwcf.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mam.tianlin.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oao.zhengqikj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kaw.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kxh.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vuw.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mjp.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://daf.daxiang520.top

[D25] Set 集合去重与交并差
来源：http://kkc.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lux.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rrl.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cqq.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xnz.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yjd.0kj1m.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qiy.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://siz.yanxiufei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kcd.dianchejie.cn

[D26] 数组转字符串
来源：http://glw.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://pwh.pycfn.com

PHP:  implode(", ", $arr);
来源：http://esy.ppjwa.cn

JS:   arr.join(", ")
来源：http://ukp.jinqigufen.top

TS:   arr.join(", ")
来源：http://dfh.cdnleiting.top

Java: String.join(", ", list)
来源：http://jfc.yfazqb.com

Go:   strings.Join(strs, ", ")
来源：http://ffp.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://ugg.guannengcc.top

C#:   string.Join(", ", list)
来源：http://tak.iojbl.cn

================================================================================
来源：http://fod.hywenlv.cn

E. 字符串处理
来源：http://bxx.pycfn.com

================================================================================
来源：http://geo.snrcjt.cn

[E01] 拼接字符串
来源：http://bdg.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ulq.hongshengwenyu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yal.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uor.tian-w.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yvh.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lha.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yxc.aibaodan.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pec.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tpa.shuidangran.top

[E02] 重复字符串
来源：http://mzi.havefunace.top

Py:   "ab" * 3
来源：http://mqa.yonumen.top

PHP:  str_repeat("ab", 3);
来源：http://sai.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://lvf.sxryk.cn


<!-- 参考信息 -->