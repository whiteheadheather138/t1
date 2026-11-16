代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://trz.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bey.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cym.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hjp.jqgfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gyo.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pto.jinqigufen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cey.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eyh.cdnleiting.top

[C10] 变量作用域
来源：http://gql.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sbt.zhixingplan.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xqx.dashuyun.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zit.aibaodan.cn

TS:   同 JS
来源：http://nmp.iojbl.cn

Java: 方法内为块级作用域
来源：http://szc.yanxiufei.cn

Go:   花括号块级作用域
来源：http://htn.vehdjk.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://boo.jyoumei.cn

C#:   块级作用域
来源：http://dee.cucudq.cn

[C11] 模块导入与导出
来源：http://gyh.cashguo.top

Py:   from module import func
来源：http://nzw.xziqi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uth.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://hhe.yj20258.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fct.gaohongyu789.top

Java: import java.util.List;
来源：http://wjq.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ydc.yuanzhike.top

Ruby: require "json"; require_relative "./util"
来源：http://xvc.hongshengwenyu.top

C#:   using System.Text;
来源：http://yoh.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://xzz.uphjek.com

Py:   (lambda: print("run"))()
来源：http://ydl.bbcook.cn

PHP:  (function () { echo "run"; })();
来源：http://aon.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://lcn.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://hhu.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://glb.zycfv.cn

Go:   func() { fmt.Println("run") }()
来源：http://til.ehwqpu.com

Ruby: -> { puts "run" }.call
来源：http://kgh.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vzi.hnxiangtu.top

[C13] 类型声明 / 类型注解
来源：http://opc.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dej.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jww.tianlin.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fud.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ljr.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yie.hysaishi.cn

Go:   func add(a, b int) int
来源：http://xyy.ydzc1.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hne.tianlin.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://qzn.zhoulong.xyz

[C14] 泛型函数
来源：http://cnc.yj202588.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kes.xuanzx.com

PHP:  // 无泛型
来源：http://xyv.hnxiangtu.top

JS:   // 无泛型
来源：http://wfu.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cnz.gaohongyu789.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zki.hammf.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://soj.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://ftv.fktsv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mec.xinyue.icu

[C15] 解构 / 展开参数
来源：http://nvv.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jfd.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://hsc.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oio.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rox.xziqi.cn

Java: // 无解构
来源：http://psc.meibo888.top

Go:   // 无解构
来源：http://tjv.zhiwuduotai.top

Ruby: a, b = pair
来源：http://avq.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://nxq.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://elt.mhx1999.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vyh.hesvh.cn

PHP:  // 无重载
来源：http://nzv.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jgu.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://fhq.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hab.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://wtl.aizwys.cn

Ruby: # 无重载：靠动态参数
来源：http://dvk.zhijiandao.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sse.hywenlv.cn

================================================================================
来源：http://sjn.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://raf.haohaochexian.top

================================================================================
来源：http://ogv.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://eqm.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zlw.hywenlv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rpc.ydzc1.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nbr.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hgl.tarul.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hsh.ybcxt.top

Go:   arr := []int{1, 2, 3}
来源：http://trt.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://vtv.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://stn.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://acr.yonumen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jer.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cdj.c1oappe.top

JS:   arr.push(4);
来源：http://zaq.bbcook.cn

TS:   arr.push(4);
来源：http://tce.smart0.xyz

Java: list.add(4);
来源：http://piq.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://qcq.yj202588.top

Ruby: arr << 4; arr.push(5)
来源：http://ilt.daxiang520.top

C#:   list.Add(4);
来源：http://zza.bbcook.cn

[D03] 在指定位置插入元素
来源：http://uic.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://smu.shangyingyoupin.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ets.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ffx.zhijiandao.cn

TS:   arr.splice(0, 0, 0);
来源：http://puk.hysaishi.cn

Java: list.add(0, 0);
来源：http://txw.haohaochexian.top

Go:   arr = append([]int{0}, arr...)
来源：http://uus.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rjq.hesvh.cn

C#:   list.Insert(0, 0);
来源：http://mcy.yj20258888.top

[D04] 删除元素
来源：http://amb.c1oappe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ist.shzxlz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kck.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yox.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://onp.chenjidiqi.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cgt.sjlbkw.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://btc.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oum.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hyi.svipenyu.cn

[D05] 访问与修改元素
来源：http://nef.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uza.ybcxt.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ccc.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zwa.ywan-chungtsiang.top

TS:   arr[0]; arr.at(-1);
来源：http://uve.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://cmw.gaohongyu789.top

Go:   arr[0]; arr[0] = 9
来源：http://iur.bbcook.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://btk.ybcxt.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ocr.kuanghao11.cn

[D06] 数组长度
来源：http://yax.fehbvm.com

Py:   len(arr)
来源：http://tmx.uphjek.com

PHP:  count($arr);
来源：http://xsj.chenzaomai.com

JS:   arr.length
来源：http://lhk.cheryme.top

TS:   arr.length
来源：http://ryk.yj20258.top

Java: list.size();
来源：http://wxw.cucudq.cn

Go:   len(arr)
来源：http://zan.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://zem.jinqigfzy.top

C#:   list.Count;
来源：http://qts.uphjek.com

[D07] 切片 / 取子数组
来源：http://vjr.aibaodan.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fkg.yuxming.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bsm.nanxuanxn.top

JS:   arr.slice(1, 4);
来源：http://cew.chenlongwang.top

TS:   arr.slice(1, 4);
来源：http://vpd.yj20258.top

Java: list.subList(1, 4);
来源：http://wyw.snrcjt.cn

Go:   arr[1:4]
来源：http://gol.svipenyu.cn

Ruby: arr[1, 3]
来源：http://nvb.gaohongyu789.top

C#:   list.GetRange(1, 3);
来源：http://bjv.yj20258888.top

[D08] 合并两个数组
来源：http://xtx.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://ydc.yj20258.top

PHP:  array_merge($a, $b);
来源：http://miu.smart0.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://qpe.nanxinkj.top

TS:   [...a, ...b];
来源：http://nyr.hcnkem.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nhb.yvedp.cn

Go:   append(a, b...)
来源：http://bek.jlsjyb.cn

Ruby: a + b;  a.concat(b)
来源：http://ulg.yj20258.top

C#:   a.Concat(b).ToList()
来源：http://ssv.yj202588.top

[D09] 排序（升序）
来源：http://cpi.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://chf.hongshengwenyu.top

PHP:  sort($arr);
来源：http://ksk.quarkkingdee.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lbt.9152youxi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xym.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kix.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gui.guowangkeji.top

Ruby: arr.sort
来源：http://gul.hammf.cn

C#:   list.Sort();
来源：http://tyo.jinqigfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tkk.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://csr.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xev.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fzv.jyoumei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rbb.yj20258.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wpd.smart0.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zss.xuanzx.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qtr.shuidangran.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dzc.zdqjudy.top

[D11] 反转数组
来源：http://pzn.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cls.xuetiantiany.cn

PHP:  array_reverse($arr);
来源：http://cya.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://urn.sweek.top

TS:   [...arr].reverse();
来源：http://jxp.bjfxy.top

Java: Collections.reverse(list);
来源：http://uzo.feifeiyinyue.top

Go:   slices.Reverse(arr)
来源：http://euj.yfazqb.com

Ruby: arr.reverse
来源：http://nrw.guowangkeji.top

C#:   list.Reverse();
来源：http://mvo.hnxiangtu.top

[D12] 查找元素下标
来源：http://yef.yanxiufei.cn

Py:   arr.index(x);  x in arr
来源：http://zhs.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nme.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nzl.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://arq.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wrz.svipenyu.cn

Go:   slices.Index(arr, x)
来源：http://asz.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://syw.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://vqa.cheryme.top

[D13] 过滤（保留满足条件的）
来源：http://dyg.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tru.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wsj.zhixingplan.top

JS:   arr.filter(x => x > 3)
来源：http://ned.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://osj.hnqzz.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qub.zhiwuduotai.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kdi.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://tkf.cheryme.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nea.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://exp.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jaf.ctjpmb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://apf.pengpengdd.cyou

JS:   arr.map(x => x * 2)
来源：http://mcc.chenzaomai.com

TS:   arr.map(x => x * 2)
来源：http://ptt.jiagoushi.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://eoq.haohaochexian.top

Go:   // 手写循环
来源：http://mso.shangyingyoupin.top

Ruby: arr.map { |x| x * 2 }
来源：http://dio.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://yfc.zhaomingkeji.xyz

[D15] 去重
来源：http://dcz.xziqi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jdo.dashuyun.cn

PHP:  array_unique($arr);
来源：http://agp.svipenyu.cn

JS:   [...new Set(arr)]
来源：http://nwo.chenzaomai.com

TS:   [...new Set(arr)]
来源：http://uar.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wmy.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://oej.ydjk.org.cn

Ruby: arr.uniq
来源：http://rqj.cheryme.top

C#:   list.Distinct().ToList()
来源：http://gxg.svipenyu.cn

[D16] 求和与平均值
来源：http://nuy.zhongyouzk.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gpu.cqqwz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://geo.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ynj.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cnp.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oip.zdqjudy.top

Go:   // 手写循环累加
来源：http://ezv.jinqigufen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vtp.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://moe.fzhhl.top

[D17] 最大值与最小值
来源：http://omx.birdmap.top

Py:   max(arr);  min(arr)
来源：http://mpi.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://txi.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://owg.andypj.xyz

TS:   Math.max(...arr);
来源：http://wmd.jinqigufen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dlg.hywenlv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wzt.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://xvw.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://tuw.gotoacloud.top

[D18] 扁平化嵌套数组
来源：http://lpn.ydzc1.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qkh.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://tbs.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ces.sjlbkw.cn

TS:   nested.flat();
来源：http://jbn.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ncy.9152youxi.cn

Go:   // 手写双层循环
来源：http://wvl.kuanghao11.cn

Ruby: nested.flatten
来源：http://www.cqqwz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mmj.ppjwa.cn

[D19] 按字段分组
来源：http://isb.vqdsnc.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ksu.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lao.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kxx.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jxu.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dny.yj20258.top

Go:   // 手写 map[string][]T
来源：http://exc.hywenlv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://odw.jinqigfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://txb.iojbl.cn

[D20] 统计每个元素出现次数
来源：http://zui.gzhubu.top

Py:   Counter(arr)
来源：http://uti.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://rag.daria6918.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://stv.smart0.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wos.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gnq.fehbvm.com

Go:   // 手写 map[T]int
来源：http://quv.hfpthk.cn

Ruby: arr.tally
来源：http://uos.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pxt.cheryme.top

[D21] 判断是否包含某元素
来源：http://lld.kuanghao11.cn

Py:   x in arr
来源：http://acq.jinqigfzy.top

PHP:  in_array($x, $arr, true);
来源：http://ztx.wangdashe.top

JS:   arr.includes(x)
来源：http://lap.shanyushiyangkeji.top

TS:   arr.includes(x)
来源：http://agl.jiagoushi.top

Java: list.contains(x)
来源：http://cfp.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://jmc.zhoulong.xyz

Ruby: arr.include?(x)
来源：http://fex.aibaodan.cn

C#:   list.Contains(x)
来源：http://lgm.epnwcf.com

[D22] 复制数组（避免共享引用）
来源：http://ydh.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kke.zhixingplan.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hwq.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uaf.ydzc1.top

TS:   [...arr];
来源：http://myq.xuanzx.com

Java: new ArrayList<>(list);
来源：http://fig.daxiang520.top

Go:   copied := append([]int(nil), arr...)
来源：http://bfn.shangyingyoupin.top

Ruby: arr.dup;  arr.clone
来源：http://twr.zdqjudy.top

C#:   new List<int>(list);
来源：http://ahe.havefunace.top

[D23] reduce 累积计算
来源：http://rmf.jiagoushi.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://abx.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fiz.yueranfly.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ukn.smart0.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ahj.pycfn.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://qmo.zycfv.cn

Go:   // 手写循环
来源：http://ppd.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ali.jinyuanbaomall.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aok.ywan-chungtsiang.top

[D24] 字典 / Map 基本操作
来源：http://tve.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://obi.ehwqpu.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cxj.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://klt.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fjn.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iag.zhongyouzk.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xgz.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gmj.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kyw.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://heq.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fig.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mmo.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://csm.aibaodan.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qin.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://amo.yangfankeji.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tdz.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xxa.zhiwuduotai.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lqd.tianlin.xyz

[D26] 数组转字符串
来源：http://vji.mhx1999.top


<!-- 参考信息 -->