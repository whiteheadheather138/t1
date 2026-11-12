代发 wailian999

[C10] 变量作用域
来源：http://ubc.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mlf.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pgg.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uxs.hysaishi.cn

TS:   同 JS
来源：http://fdx.wangdashe.top

Java: 方法内为块级作用域
来源：http://xkj.daria6918.cn

Go:   花括号块级作用域
来源：http://raq.snrcjt.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lzg.chenlongwang.top

C#:   块级作用域
来源：http://lgh.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://gie.nwbrower.top

Py:   from module import func
来源：http://dpg.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://ryr.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pvd.yfazqb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hku.jinqigfzy.top

Java: import java.util.List;
来源：http://kmj.vehdjk.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://she.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://szm.jinghuilouyu.cn

C#:   using System.Text;
来源：http://vhn.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://hod.xuanzx.com

Py:   (lambda: print("run"))()
来源：http://rxf.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://ioa.zhongyouzk.top

JS:   (() => { console.log("run"); })();
来源：http://dlo.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://jue.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eug.nanxinkj.top

Go:   func() { fmt.Println("run") }()
来源：http://zip.yj20258888.top

Ruby: -> { puts "run" }.call
来源：http://wml.ctjpmb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://fwy.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://sce.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://csr.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wbn.xinyue.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rfg.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uiv.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://iwf.havefunace.top

Go:   func add(a, b int) int
来源：http://iwq.zdqjudy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ebh.hammf.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tmj.sjlbkw.cn

[C14] 泛型函数
来源：http://wss.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://glb.cashguo.top

PHP:  // 无泛型
来源：http://sek.jinghuilouyu.cn

JS:   // 无泛型
来源：http://edg.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cbp.xinyue.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://una.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ivw.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://mbw.zdqjudy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cwy.yangfankeji.com

[C15] 解构 / 展开参数
来源：http://lmn.shuidangran.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mfk.gaohongyu789.top

PHP:  [$a, $b] = $pair;
来源：http://obh.shanyushiyangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zak.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wxw.feifeiyinyue.top

Java: // 无解构
来源：http://ehh.hongshengwenyu.top

Go:   // 无解构
来源：http://htg.yueranfly.top

Ruby: a, b = pair
来源：http://nhx.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://yzu.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://lpp.c1oappe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blh.cucudq.cn

PHP:  // 无重载
来源：http://ofg.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fnx.wangshuangyany.cn

TS:   // 用联合类型或重载签名声明
来源：http://nme.redwolf501.top

Java: void f(int a) {}  void f(String a) {}
来源：http://frv.xziqi.cn

Go:   // 无重载：用不同函数名
来源：http://xva.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://eep.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://fvi.xziqi.cn

================================================================================
来源：http://bgu.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://uha.bjfxy.top

================================================================================
来源：http://aoe.xuanzx.com

[D01] 创建数组 / 列表
来源：http://iwg.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://pje.hcnkem.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://efq.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nzh.ivvv.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pzo.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://utq.zhijiandao.cn

Go:   arr := []int{1, 2, 3}
来源：http://icb.tanke756.top

Ruby: arr = [1, 2, 3]
来源：http://kih.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://upv.yonumen.top

[D02] 追加元素到末尾
来源：http://ojm.tanke756.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ecc.gotoacloud.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yoh.fanxiaobao.xyz

JS:   arr.push(4);
来源：http://ghh.fzhhl.top

TS:   arr.push(4);
来源：http://fqc.shangyingyoupin.top

Java: list.add(4);
来源：http://dyj.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://egp.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://tvf.dianchejie.cn

C#:   list.Add(4);
来源：http://gzk.gzhubu.top

[D03] 在指定位置插入元素
来源：http://srg.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://opk.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://chd.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://djr.daxiang520.top

TS:   arr.splice(0, 0, 0);
来源：http://vjq.meibo888.top

Java: list.add(0, 0);
来源：http://pjz.shzxlz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ipa.ybcxt.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zss.yonumen.top

C#:   list.Insert(0, 0);
来源：http://plj.hnqzz.top

[D04] 删除元素
来源：http://mbc.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ztc.epnwcf.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dud.yj20258.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bfm.fzhhl.top

TS:   arr.splice(0, 1);
来源：http://rll.ppjwa.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uae.fanxiaobao.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hmd.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jcv.tanke756.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xcm.shzxlz.cn

[D05] 访问与修改元素
来源：http://zuq.pengpengdd.cyou

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fvt.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eou.redwolf501.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wgg.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://cmw.yj202588.top

Java: list.get(0); list.set(0, 9);
来源：http://jbg.fktsv.cn

Go:   arr[0]; arr[0] = 9
来源：http://ygy.ybcxt.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jcz.ybcxt.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://grk.sjlbkw.cn

[D06] 数组长度
来源：http://klx.gotoacloud.top

Py:   len(arr)
来源：http://hee.shzxlz.cn

PHP:  count($arr);
来源：http://ini.jinqigufen.top

JS:   arr.length
来源：http://ptn.fanxiaobao.xyz

TS:   arr.length
来源：http://uap.dashuyun.cn

Java: list.size();
来源：http://iwx.hnxiangtu.top

Go:   len(arr)
来源：http://yfj.yanxiufei.cn

Ruby: arr.length; arr.size
来源：http://nau.yj20258888.top

C#:   list.Count;
来源：http://zhz.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://pct.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zei.andypj.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://mtn.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://bra.nanxuanxn.top

TS:   arr.slice(1, 4);
来源：http://aqj.0kj1m.cn

Java: list.subList(1, 4);
来源：http://quu.jqgufenzy.top

Go:   arr[1:4]
来源：http://biz.zycfv.cn

Ruby: arr[1, 3]
来源：http://rdy.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://wqg.chenjidiqi.icu

[D08] 合并两个数组
来源：http://smx.bjfxy.top

Py:   a + b;  a.extend(b)
来源：http://cok.meibo888.top

PHP:  array_merge($a, $b);
来源：http://alh.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xas.meibo888.top

TS:   [...a, ...b];
来源：http://qjw.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ojg.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://uwl.hammf.cn

Ruby: a + b;  a.concat(b)
来源：http://zkq.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://jzo.gzhubu.top

[D09] 排序（升序）
来源：http://gbu.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://wun.aizwys.cn

PHP:  sort($arr);
来源：http://wgp.xingfuxueyuan.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tma.svipenyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://glf.mhx1999.top

Java: Collections.sort(list);  list.sort(null);
来源：http://seo.birdmap.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rvl.shzxlz.cn

Ruby: arr.sort
来源：http://ffu.hnqzz.top

C#:   list.Sort();
来源：http://brw.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pab.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qdr.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fha.shanyushiyangtech.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nfa.hfpthk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uus.zhengqikj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oii.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rxz.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://twg.jlsjyb.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yjr.zhiwuduotai.top

[D11] 反转数组
来源：http://vme.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pjm.yuxming.cn

PHP:  array_reverse($arr);
来源：http://yli.mhx1999.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zah.andypj.xyz

TS:   [...arr].reverse();
来源：http://vkz.uphjek.com

Java: Collections.reverse(list);
来源：http://ynm.meibo888.top

Go:   slices.Reverse(arr)
来源：http://kgu.yangfankeji.com

Ruby: arr.reverse
来源：http://veq.daria6918.cn

C#:   list.Reverse();
来源：http://auf.nanxinkj.top

[D12] 查找元素下标
来源：http://rce.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://drk.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xrp.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wpw.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://idx.fzhhl.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nzr.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://yti.gaohongyu789.top

Ruby: arr.index(x)
来源：http://zqi.pengpengdd.cyou

C#:   list.IndexOf(x);
来源：http://yxl.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://noa.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nlw.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lrj.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://jrz.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://rbl.yuanzhike.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mta.zhiwuduotai.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bcr.xingfuxueyuan.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://zdc.tarul.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uex.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://bso.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nxc.hongshengwenyu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xrf.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://nhn.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://sou.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ngd.feifeiyinyue.top

Go:   // 手写循环
来源：http://hsv.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gcc.nwbrower.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nbm.tian-w.cn

[D15] 去重
来源：http://xhr.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://klu.yfazqb.com

PHP:  array_unique($arr);
来源：http://mni.sjlbkw.cn

JS:   [...new Set(arr)]
来源：http://lfl.ydzc1.top

TS:   [...new Set(arr)]
来源：http://okq.sjlbkw.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dzt.hywenlv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wtx.yfazqb.com

Ruby: arr.uniq
来源：http://vnl.bjfxy.top

C#:   list.Distinct().ToList()
来源：http://lxv.yongpay.top

[D16] 求和与平均值
来源：http://mxx.jinyuanbaomall.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wce.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uet.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lux.hywenlv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lpc.cheryme.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vlz.tian-w.cn

Go:   // 手写循环累加
来源：http://tur.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pef.hcnkem.com

C#:   list.Sum();  list.Average()
来源：http://ccf.sysykeji.top

[D17] 最大值与最小值
来源：http://vrx.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://oit.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://tbd.vehdjk.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://irh.haohaochexian.top

TS:   Math.max(...arr);
来源：http://aia.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://vpk.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nzl.hcnkem.com

Ruby: arr.max;  arr.min
来源：http://osv.fengsongda.top

C#:   list.Max();  list.Min()
来源：http://ato.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://ebe.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ttn.yj20258888.top

PHP:  array_merge(...$nested);
来源：http://oow.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lgg.jinqigfzy.top

TS:   nested.flat();
来源：http://eiw.epnwcf.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gje.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://yeh.iojbl.cn

Ruby: nested.flatten
来源：http://koe.birdmap.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yee.meibo888.top

[D19] 按字段分组
来源：http://xwa.hcnkem.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://npn.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wru.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://clf.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pam.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zpf.svipenyu.cn

Go:   // 手写 map[string][]T
来源：http://tci.jinqigufen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dlz.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yzj.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://fcv.zhiwuduotai.top

Py:   Counter(arr)
来源：http://ink.kuanghao11.cn

PHP:  array_count_values($arr);
来源：http://fqn.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xkt.tian-w.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fty.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xcz.zhongyouzk.top

Go:   // 手写 map[T]int
来源：http://cob.ehwqpu.com

Ruby: arr.tally
来源：http://iyv.havefunace.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zet.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://qvk.smart0.xyz

Py:   x in arr
来源：http://qkn.gogol.net.cn

PHP:  in_array($x, $arr, true);
来源：http://qga.yueranfly.top

JS:   arr.includes(x)
来源：http://qkc.jianghu66.top

TS:   arr.includes(x)
来源：http://gmr.yanxiufei.cn

Java: list.contains(x)
来源：http://pfn.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://tno.cucudq.cn

Ruby: arr.include?(x)
来源：http://pzf.zdqjudy.top

C#:   list.Contains(x)
来源：http://raf.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://ppp.zhengqikj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rtc.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://twa.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ohq.aibaodan.cn

TS:   [...arr];
来源：http://dgy.fehbvm.com

Java: new ArrayList<>(list);
来源：http://cbo.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://zwv.yj20258888.top

Ruby: arr.dup;  arr.clone
来源：http://qqe.yj20258888.top

C#:   new List<int>(list);
来源：http://ljt.zycfv.cn

[D23] reduce 累积计算
来源：http://voe.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dqm.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pwl.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tha.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ucq.gaohongyu789.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hda.svipenyu.cn

Go:   // 手写循环
来源：http://cgf.xuanzx.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://adn.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ypk.cashguo.top

[D24] 字典 / Map 基本操作
来源：http://ilz.iojbl.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vmu.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pwb.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ysl.gzhubu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ldr.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uxo.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nbj.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qbd.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://beb.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://fnr.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sxg.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mnj.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qme.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ywg.hysaishi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ppa.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vrs.sysykeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://edk.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jjg.yonumen.top

[D26] 数组转字符串
来源：http://url.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://kur.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://cul.hammf.cn

JS:   arr.join(", ")
来源：http://pnj.cqqwz.cn

TS:   arr.join(", ")
来源：http://hqv.jqgufenzy.top

Java: String.join(", ", list)
来源：http://fzk.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://uin.yangfankeji.com

Ruby: arr.join(", ")
来源：http://kpn.gogol.net.cn

C#:   string.Join(", ", list)
来源：http://pdp.tarul.cn


<!-- 参考信息 -->