代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://utz.birdmap.top

JS:   (() => { console.log("run"); })();
来源：http://tth.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://dlb.ybcxt.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uxq.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://rws.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://gpn.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zju.gzhubu.top

[C13] 类型声明 / 类型注解
来源：http://vxc.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rri.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xzb.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://due.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hts.wangshuangyany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jhm.xziqi.cn

Go:   func add(a, b int) int
来源：http://sta.jiagoushi.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xnz.zhiwuduotai.top

C#:   int Add(int a, int b) => a + b;
来源：http://niz.chenzaomai.com

[C14] 泛型函数
来源：http://atk.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wrv.uphjek.com

PHP:  // 无泛型
来源：http://ygl.ydzc1.top

JS:   // 无泛型
来源：http://ljx.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tya.meibo888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kps.chenjidiqi.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ted.zdbjq.cn

Ruby: # 无泛型
来源：http://tdl.zdbjq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bwt.xylfe.cn

[C15] 解构 / 展开参数
来源：http://shn.jinyuanbaomall.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dep.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://nko.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pmx.xuetiantiany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ccu.wangshuangyany.cn

Java: // 无解构
来源：http://jjs.zhaomingkeji.xyz

Go:   // 无解构
来源：http://dax.smart0.xyz

Ruby: a, b = pair
来源：http://vek.andypj.xyz

C#:   var (a, b) = pair;
来源：http://jzd.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://hbu.zhixingplan.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zcn.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://chj.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ozy.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://dco.yfazqb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://jmq.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://hnz.hammf.cn

Ruby: # 无重载：靠动态参数
来源：http://lmr.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://diy.aizwys.cn

================================================================================
来源：http://yev.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://gux.guowangkeji.top

================================================================================
来源：http://mcv.wangshuangyany.cn

[D01] 创建数组 / 列表
来源：http://lvr.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wwx.chenlongwang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mlt.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://efg.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jlj.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hfn.xingfuxueyuan.xyz

Go:   arr := []int{1, 2, 3}
来源：http://urm.ydjk.org.cn

Ruby: arr = [1, 2, 3]
来源：http://zra.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://exe.c1oappe.top

[D02] 追加元素到末尾
来源：http://zlr.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dum.xingfuxueyuan.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zvu.9152youxi.cn

JS:   arr.push(4);
来源：http://dom.xylfe.cn

TS:   arr.push(4);
来源：http://uyb.ywan-chungtsiang.top

Java: list.add(4);
来源：http://pgu.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://bkc.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://hzz.xingfuxueyuan.xyz

C#:   list.Add(4);
来源：http://qkk.havefunace.top

[D03] 在指定位置插入元素
来源：http://hkp.sufxvd.cn

Py:   arr.insert(0, 0)
来源：http://otr.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dev.zhoulong.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://znz.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://xus.shuidangran.top

Java: list.add(0, 0);
来源：http://fcd.yj202588.top

Go:   arr = append([]int{0}, arr...)
来源：http://fym.hysaishi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eml.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://neb.hammf.cn

[D04] 删除元素
来源：http://bom.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dfq.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lfl.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fim.xuanzx.com

TS:   arr.splice(0, 1);
来源：http://iug.shanyushiyangtech.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rqn.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xmo.xziqi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hba.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ryv.yj20258888.top

[D05] 访问与修改元素
来源：http://ecn.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cih.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bpl.yuanzhike.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sia.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://inh.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://izj.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://pjg.chenlongwang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nij.hammf.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hvl.zhoulong.xyz

[D06] 数组长度
来源：http://yad.fktsv.cn

Py:   len(arr)
来源：http://niy.shuidangran.top

PHP:  count($arr);
来源：http://gcw.jianghu66.top

JS:   arr.length
来源：http://zfx.ydzc1.top

TS:   arr.length
来源：http://ehw.svipenyu.cn

Java: list.size();
来源：http://wfp.wangshuangyany.cn

Go:   len(arr)
来源：http://uli.jqgfzy.top

Ruby: arr.length; arr.size
来源：http://ihy.shzxlz.cn

C#:   list.Count;
来源：http://xti.ywan-chungtsiang.top

[D07] 切片 / 取子数组
来源：http://rqq.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://stq.daxiang520.top

PHP:  array_slice($arr, 1, 3);
来源：http://abj.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://vko.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://pny.yanxiufei.cn

Java: list.subList(1, 4);
来源：http://vra.dashuyun.cn

Go:   arr[1:4]
来源：http://qaa.jyoumei.cn

Ruby: arr[1, 3]
来源：http://vgs.gotoacloud.top

C#:   list.GetRange(1, 3);
来源：http://gpe.cdnleiting.top

[D08] 合并两个数组
来源：http://xwx.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://woe.yuxming.cn

PHP:  array_merge($a, $b);
来源：http://yer.daxiang520.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gjk.52xcode.cn

TS:   [...a, ...b];
来源：http://gin.yangfankeji.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sxd.wangdashe.top

Go:   append(a, b...)
来源：http://sck.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://ziw.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://kqi.havefunace.top

[D09] 排序（升序）
来源：http://hzv.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://hiy.hysaishi.cn

PHP:  sort($arr);
来源：http://klx.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yxy.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://lkz.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mta.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pcc.smart0.xyz

Ruby: arr.sort
来源：http://uyj.hfpthk.cn

C#:   list.Sort();
来源：http://dla.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dsr.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wlp.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://glu.yongpay.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ocr.gogol.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ttw.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gwd.gotoacloud.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blx.0kj1m.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sow.jqgfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fef.zdbjq.cn

[D11] 反转数组
来源：http://vrx.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://aqe.zhengqikj.top

PHP:  array_reverse($arr);
来源：http://zys.bjfxy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jes.jiagoushi.top

TS:   [...arr].reverse();
来源：http://oxk.zdbjq.cn

Java: Collections.reverse(list);
来源：http://doi.mhx1999.top

Go:   slices.Reverse(arr)
来源：http://ofx.vqdsnc.cn

Ruby: arr.reverse
来源：http://cwb.cqqwz.cn

C#:   list.Reverse();
来源：http://ewb.daria6918.cn

[D12] 查找元素下标
来源：http://mey.nanxinkj.top

Py:   arr.index(x);  x in arr
来源：http://qnv.gzhubu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hzk.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bah.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kmf.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mwi.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://yui.zhoulong.xyz

Ruby: arr.index(x)
来源：http://gwe.meibo888.top

C#:   list.IndexOf(x);
来源：http://bdm.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://gay.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lpc.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xpt.jyoumei.cn

JS:   arr.filter(x => x > 3)
来源：http://bcc.yonumen.top

TS:   arr.filter(x => x > 3)
来源：http://ths.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://slp.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ivn.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tfm.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pwe.vqdsnc.cn

[D14] 映射转换（每个元素变形）
来源：http://hjl.316326.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bqw.snrcjt.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://csy.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://tbw.shuidangran.top

TS:   arr.map(x => x * 2)
来源：http://wyi.gaohongyu789.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nbi.tanke756.top

Go:   // 手写循环
来源：http://wqc.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://vnk.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lai.daxiang520.top

[D15] 去重
来源：http://srm.jqgufenzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rnw.fengsongda.top

PHP:  array_unique($arr);
来源：http://zbh.kuanghao11.cn

JS:   [...new Set(arr)]
来源：http://bqb.xziqi.cn

TS:   [...new Set(arr)]
来源：http://egp.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jeb.vqdsnc.cn

Go:   // 用 map[T]struct{} 手写
来源：http://esu.vqdsnc.cn

Ruby: arr.uniq
来源：http://yia.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://olv.xylfe.cn

[D16] 求和与平均值
来源：http://ppi.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xjb.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rjs.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bwo.hongshengwenyu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://udr.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tmj.aizwys.cn

Go:   // 手写循环累加
来源：http://out.nanxuanxn.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xuh.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://ziu.daxiang520.top

[D17] 最大值与最小值
来源：http://wde.9152youxi.cn

Py:   max(arr);  min(arr)
来源：http://hvn.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://aoq.cqqwz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zga.zdqjudy.top

TS:   Math.max(...arr);
来源：http://buu.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kda.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rsj.guannengcc.top

Ruby: arr.max;  arr.min
来源：http://vcp.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://hef.yonumen.top

[D18] 扁平化嵌套数组
来源：http://ttx.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rhj.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://lin.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ras.zhengqikj.top

TS:   nested.flat();
来源：http://unx.xingfuxueyuan.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qdh.gotoacloud.top

Go:   // 手写双层循环
来源：http://hdl.birdmap.top

Ruby: nested.flatten
来源：http://kcv.cdnleiting.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ezw.ywan-chungtsiang.top

[D19] 按字段分组
来源：http://rxa.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cxd.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nnt.yongpay.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tta.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xbl.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hvx.yj20258.top

Go:   // 手写 map[string][]T
来源：http://fbc.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://awn.uphjek.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://swi.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://kzs.smart0.xyz

Py:   Counter(arr)
来源：http://fjh.kuanghao11.cn

PHP:  array_count_values($arr);
来源：http://ihq.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vgu.c1oappe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bcm.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hkv.xinyue.icu

Go:   // 手写 map[T]int
来源：http://cpn.havefunace.top

Ruby: arr.tally
来源：http://cht.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cap.zhiwuduotai.top

[D21] 判断是否包含某元素
来源：http://bgd.jqgufenzy.top

Py:   x in arr
来源：http://ndy.hammf.cn

PHP:  in_array($x, $arr, true);
来源：http://oty.hfpthk.cn

JS:   arr.includes(x)
来源：http://ily.nanxuanxn.top

TS:   arr.includes(x)
来源：http://twt.guannengcc.top

Java: list.contains(x)
来源：http://api.xziqi.cn

Go:   slices.Contains(arr, x)
来源：http://fzx.fengsongda.top

Ruby: arr.include?(x)
来源：http://lyd.cqqwz.cn

C#:   list.Contains(x)
来源：http://ipt.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://mto.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bwm.shzxlz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mkw.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://see.mhx1999.top

TS:   [...arr];
来源：http://wwm.zhixingplan.top

Java: new ArrayList<>(list);
来源：http://pzl.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nvm.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://zkz.pengpengdd.cyou

C#:   new List<int>(list);
来源：http://nzw.sufxvd.cn

[D23] reduce 累积计算
来源：http://ipe.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kdh.yfazqb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vmm.cqqwz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://srw.daria6918.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lwb.gotoacloud.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://sot.xziqi.cn

Go:   // 手写循环
来源：http://nzz.chenlongwang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xos.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rhs.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://ifs.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kxt.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zlu.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ysk.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://grn.zhongyouzk.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jfw.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tgh.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fcd.chenjidiqi.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://auq.xziqi.cn

[D25] Set 集合去重与交并差
来源：http://wxo.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dhl.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://atl.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wdd.shuidangran.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yzy.dianchejie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://btr.yj20258.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://niv.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gzu.jinqigfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qna.yanxiufei.cn

[D26] 数组转字符串
来源：http://swk.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://dhi.zycfv.cn

PHP:  implode(", ", $arr);
来源：http://kmz.ywan-chungtsiang.top

JS:   arr.join(", ")
来源：http://kpq.yj20258.top

TS:   arr.join(", ")
来源：http://buw.ydzc1.top

Java: String.join(", ", list)
来源：http://cpo.zhijiandao.cn

Go:   strings.Join(strs, ", ")
来源：http://fxf.aizwys.cn

Ruby: arr.join(", ")
来源：http://nky.c1oappe.top

C#:   string.Join(", ", list)
来源：http://hpa.shangyingyoupin.top

================================================================================
来源：http://nls.guannengcc.top

E. 字符串处理
来源：http://yxv.zhoulong.xyz

================================================================================
来源：http://sci.fehbvm.com

[E01] 拼接字符串
来源：http://jdk.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://khf.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yjr.xinyue.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://omh.0kj1m.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dql.cqqwz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rvd.wangshuangyany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hty.hammf.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iya.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ixx.snrcjt.cn

[E02] 重复字符串
来源：http://fpd.sysykeji.top

Py:   "ab" * 3
来源：http://vcn.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://zzj.pycfn.com

JS:   "ab".repeat(3)
来源：http://qtu.pengpengdd.cyou

TS:   "ab".repeat(3)
来源：http://bjk.fehbvm.com

Java: "ab".repeat(3)
来源：http://xeu.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://rhi.jiagoushi.top

Ruby: "ab" * 3
来源：http://kyt.quarkkingdee.top


<!-- 参考信息 -->