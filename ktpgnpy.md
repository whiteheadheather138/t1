代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.bbcook.cn/Article/details/grxmffnoj.sHtML

Go:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gcuetucfi.sHtML

Ruby: return a, b
来源：http://m.share.yfazqb.com/Article/details/gdcsrrrox.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.bbcook.cn/Article/details/giuzndecx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.yfazqb.com/Article/details/gytdqluuv.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fktsv.cn/Article/details/gmgbbljkt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/godnmmqke.sHtML

JS:   const square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/gjgyricis.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gkqvstgxj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.tarul.cn/Article/details/gbgbybhtw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.bbcook.cn/Article/details/goytknggr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.vehdjk.com/Article/details/gjxgkcyqb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fktsv.cn/Article/details/gxlrdaosw.sHtML

[C07] 把函数作为参数传入
来源：http://blog.yfazqb.com/Article/details/glxautokb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.yfazqb.com/Article/details/gbccyuacj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.vehdjk.com/Article/details/ggfigrrtf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.yfazqb.com/Article/details/gmkhnaohy.sHtML

TS:   arr.map(String)
来源：http://www.m.share.sjlbkw.cn/Article/details/gejqbzzut.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.yfazqb.com/Article/details/gisfaguhw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fktsv.cn/Article/details/gizxucflf.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.tarul.cn/Article/details/gvhqubhbi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.epnwcf.com/Article/details/ggqfenswl.sHtML

[C08] 闭包
来源：http://www.share.fktsv.cn/Article/details/gjeqvfvpk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fktsv.cn/Article/details/gnjxplpdg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.epnwcf.com/Article/details/gygzwituq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gyxymatlt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gwacmhcjo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.sjlbkw.cn/Article/details/gyerujojj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.epnwcf.com/Article/details/gaxxoreoe.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.vehdjk.com/Article/details/gphdyfoft.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gbckzutox.sHtML

[C09] 递归
来源：http://mobile.bbcook.cn/Article/details/gatfhyngi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gpblnaafx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.vehdjk.com/Article/details/gqrnviaur.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/getsrkgfv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gebxnoicj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.sjlbkw.cn/Article/details/gyxkauisy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/gtujfmhgt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gyfplpbum.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.vehdjk.com/Article/details/gtrzkiazp.sHtML

[C10] 变量作用域
来源：http://wap.yfazqb.com/Article/details/gycwnsaou.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.yfazqb.com/Article/details/giyjglkvv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.tarul.cn/Article/details/gznejgwbs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.bbcook.cn/Article/details/gnbxsqtpc.sHtML

TS:   同 JS
来源：http://m.share.vehdjk.com/Article/details/ganpjfwmx.sHtML

Java: 方法内为块级作用域
来源：http://www.share.vehdjk.com/Article/details/gbctnknmi.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gpubgzadr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.epnwcf.com/Article/details/gpksgidkg.sHtML

C#:   块级作用域
来源：http://m.share.yfazqb.com/Article/details/gehhqcast.sHtML

[C11] 模块导入与导出
来源：http://read.share.sjlbkw.cn/Article/details/gpdrpougm.sHtML

Py:   from module import func
来源：http://wap.sjlbkw.cn/Article/details/grvtxfgxc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.tarul.cn/Article/details/ggpeboduw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.tarul.cn/Article/details/gqtrafwam.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.tarul.cn/Article/details/gpulibwmk.sHtML

Java: import java.util.List;
来源：http://mobile.tarul.cn/Article/details/gvwhydsch.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.sjlbkw.cn/Article/details/gckpdrfgm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.yfazqb.com/Article/details/gmviwzhod.sHtML

C#:   using System.Text;
来源：http://3g.tarul.cn/Article/details/gnrqvvrga.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.bbcook.cn/Article/details/ghxqqibkz.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.vehdjk.com/Article/details/ghntyhsna.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.tarul.cn/Article/details/gcgciyqqe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gkvhpgwbm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gmysoikyb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.yfazqb.com/Article/details/gclhyiafn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.sjlbkw.cn/Article/details/gndnzfddm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.vehdjk.com/Article/details/gonibnpij.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.epnwcf.com/Article/details/ghlzgjurm.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.vehdjk.com/Article/details/glaxxaato.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.vehdjk.com/Article/details/gynmbyhan.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gdlkxhdbh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.sjlbkw.cn/Article/details/gtwovtann.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/giyakifxe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gttebjhds.sHtML

Go:   func add(a, b int) int
来源：http://wap.yfazqb.com/Article/details/gsugoxvew.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.bbcook.cn/Article/details/gipnuysdn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fktsv.cn/Article/details/gdvrdtfdb.sHtML

[C14] 泛型函数
来源：http://wap.tarul.cn/Article/details/gsluxhrfe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/gmeurtooh.sHtML

PHP:  // 无泛型
来源：http://wap.vehdjk.com/Article/details/gdpxxnjwn.sHtML

JS:   // 无泛型
来源：http://wap.yfazqb.com/Article/details/gymcwwylq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.yfazqb.com/Article/details/gcesmadgx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.epnwcf.com/Article/details/gdbmedcej.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fktsv.cn/Article/details/gaqkmvefy.sHtML

Ruby: # 无泛型
来源：http://www.share.tarul.cn/Article/details/gnpaswzpy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.tarul.cn/Article/details/gcvmyafqk.sHtML

[C15] 解构 / 展开参数
来源：http://3g.tarul.cn/Article/details/glnhcoclk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fktsv.cn/Article/details/gadmxnpnd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.bbcook.cn/Article/details/gemfxlbzb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gbayzlbcu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.bbcook.cn/Article/details/ghcojhtqb.sHtML

Java: // 无解构
来源：http://baike.bbcook.cn/Article/details/gvpuolqaw.sHtML

Go:   // 无解构
来源：http://mobile.bbcook.cn/Article/details/gtyuxguph.sHtML

Ruby: a, b = pair
来源：http://mobile.yfazqb.com/Article/details/gtcdrwcau.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/gpydnlwqc.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.epnwcf.com/Article/details/grrwzofla.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fktsv.cn/Article/details/geyyjzdas.sHtML

PHP:  // 无重载
来源：http://3g.epnwcf.com/Article/details/gyectqalm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fktsv.cn/Article/details/ggrorfprv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.tarul.cn/Article/details/gtqbgqkrm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.yfazqb.com/Article/details/gdlfjhqdr.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.yfazqb.com/Article/details/gizchvovg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.vehdjk.com/Article/details/gprbfcjqs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.bbcook.cn/Article/details/glwejvhts.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwfupwfdi.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.sjlbkw.cn/Article/details/gljsiwgeg.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdtvpcpn.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/gqevvxvzd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.vehdjk.com/Article/details/gscrqlfqv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fktsv.cn/Article/details/gtxwuxfxe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/gthsdmpwp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.sjlbkw.cn/Article/details/grpvqfljz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.tarul.cn/Article/details/gnnqfumpo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/gnbarnbro.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.vehdjk.com/Article/details/gyhynyhgn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.bbcook.cn/Article/details/gttaexflq.sHtML

[D02] 追加元素到末尾
来源：http://read.share.yfazqb.com/Article/details/gisnpifxu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.yfazqb.com/Article/details/gjphznfty.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.epnwcf.com/Article/details/ghmpthdth.sHtML

JS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gstrvqezd.sHtML

TS:   arr.push(4);
来源：http://read.share.bbcook.cn/Article/details/gtcxkdjox.sHtML

Java: list.add(4);
来源：http://mobile.epnwcf.com/Article/details/gawrpzptj.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.bbcook.cn/Article/details/gtxwyiemb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.sjlbkw.cn/Article/details/gmpqhtabq.sHtML

C#:   list.Add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gwnpofavf.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fktsv.cn/Article/details/gzzyerlcw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gbqhiswhb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.yfazqb.com/Article/details/gzicypaxy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.vehdjk.com/Article/details/gqvpctaey.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fktsv.cn/Article/details/gbbafeida.sHtML

Java: list.add(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gpzjynrwx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.tarul.cn/Article/details/gditvlgus.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.tarul.cn/Article/details/gmugsrllp.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.epnwcf.com/Article/details/gvohcfiwo.sHtML

[D04] 删除元素
来源：http://3g.vehdjk.com/Article/details/goaujkqoj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fktsv.cn/Article/details/gzqlnbyek.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gzqdiwxik.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fktsv.cn/Article/details/gqoimgbnx.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.sjlbkw.cn/Article/details/gvmvkavms.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.tarul.cn/Article/details/gqmtabbeu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.sjlbkw.cn/Article/details/gzyjaecra.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.tarul.cn/Article/details/goohqfrba.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlxnvvne.sHtML

[D05] 访问与修改元素
来源：http://www.blog.tarul.cn/Article/details/gudwdgqxe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gkjpouifp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gywaxwxey.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gsrilmbgf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.epnwcf.com/Article/details/gyaodduib.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.sjlbkw.cn/Article/details/grmkvujxv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gwvskccub.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/ggsbazoca.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gkgldwdjd.sHtML

[D06] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/gezlcbgla.sHtML

Py:   len(arr)
来源：http://wap.bbcook.cn/Article/details/gnmnbsytk.sHtML

PHP:  count($arr);
来源：http://www.share.vehdjk.com/Article/details/goflszskz.sHtML

JS:   arr.length
来源：http://baike.yfazqb.com/Article/details/gfncfrpnr.sHtML

TS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/gywghidbg.sHtML

Java: list.size();
来源：http://www.blog.vehdjk.com/Article/details/gaaczifis.sHtML

Go:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gjdztfyid.sHtML

Ruby: arr.length; arr.size
来源：http://baike.vehdjk.com/Article/details/ggynrqytz.sHtML

C#:   list.Count;
来源：http://3g.yfazqb.com/Article/details/gbveszvfm.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.tarul.cn/Article/details/gfbmofbsr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fktsv.cn/Article/details/gdntbphwu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.epnwcf.com/Article/details/grocuhykq.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.epnwcf.com/Article/details/gsigxhaqd.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gahcnsqrg.sHtML

Java: list.subList(1, 4);
来源：http://blog.vehdjk.com/Article/details/gfyqtveeu.sHtML

Go:   arr[1:4]
来源：http://www.blog.fktsv.cn/Article/details/gutwwatme.sHtML

Ruby: arr[1, 3]
来源：http://mobile.tarul.cn/Article/details/gjbgcwzxc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/ghazapkbf.sHtML

[D08] 合并两个数组
来源：http://www.share.bbcook.cn/Article/details/goerdxfnm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.bbcook.cn/Article/details/gexrcvehm.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/gsbcagziu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/gzosbbpzs.sHtML

TS:   [...a, ...b];
来源：http://www.share.vehdjk.com/Article/details/gzfhvpdtx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.sjlbkw.cn/Article/details/gwxefjzpw.sHtML

Go:   append(a, b...)
来源：http://mobile.bbcook.cn/Article/details/gfebsufjz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.sjlbkw.cn/Article/details/gvdrdvotv.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.vehdjk.com/Article/details/grtwdtzfz.sHtML

[D09] 排序（升序）
来源：http://www.share.yfazqb.com/Article/details/gpzcjfkoa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/ghvlwhrzg.sHtML

PHP:  sort($arr);
来源：http://www.blog.epnwcf.com/Article/details/ggbdmzjxp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.tarul.cn/Article/details/gagsuhnwy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fktsv.cn/Article/details/gcoqxasmm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.yfazqb.com/Article/details/gxutaaeux.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/grqzecgqe.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gkhfykzqa.sHtML

C#:   list.Sort();
来源：http://mobile.tarul.cn/Article/details/glnphgics.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.bbcook.cn/Article/details/gjlgcghjd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.vehdjk.com/Article/details/gqgfvhhad.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/giqwhglev.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/grhkqbumi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fktsv.cn/Article/details/ggxnujajf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/guatrkgfq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.epnwcf.com/Article/details/gngjrbvpr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fktsv.cn/Article/details/guazgkyqz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.yfazqb.com/Article/details/gwjymuryi.sHtML

[D11] 反转数组
来源：http://www.share.bbcook.cn/Article/details/grdvdjtqn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.sjlbkw.cn/Article/details/gmdpmnnkd.sHtML

PHP:  array_reverse($arr);
来源：http://wap.yfazqb.com/Article/details/gctbbzapx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.vehdjk.com/Article/details/gtjlmgahr.sHtML

TS:   [...arr].reverse();
来源：http://baike.epnwcf.com/Article/details/gnpamtgim.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fktsv.cn/Article/details/gwolidljs.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fktsv.cn/Article/details/gyyqdevpj.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/gzhzhputq.sHtML

C#:   list.Reverse();
来源：http://m.share.tarul.cn/Article/details/gbeubusup.sHtML

[D12] 查找元素下标
来源：http://read.share.sjlbkw.cn/Article/details/gfbhiqyup.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.tarul.cn/Article/details/gczifvppg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.tarul.cn/Article/details/gnqgpysva.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gtjiygsvo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gnljkrpxa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.yfazqb.com/Article/details/gsjaonykv.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gdzixcszu.sHtML

Ruby: arr.index(x)
来源：http://baike.yfazqb.com/Article/details/gfudjhtkh.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.bbcook.cn/Article/details/gceeblpvv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.vehdjk.com/Article/details/gpirfyzeq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.bbcook.cn/Article/details/gvqdwmpaa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.vehdjk.com/Article/details/gmkeykyua.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gzmagjpvp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/glaqtdpjw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.tarul.cn/Article/details/gdbajyooh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/garkuffqy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.yfazqb.com/Article/details/gdpebmzxx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.yfazqb.com/Article/details/gfqudfksn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.vehdjk.com/Article/details/gcreyajbs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.sjlbkw.cn/Article/details/gsfskkcda.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.sjlbkw.cn/Article/details/gdgkbhkfr.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gbicbmqut.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/guwvmjjde.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.sjlbkw.cn/Article/details/gqzqstjad.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gwutkzxyz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gazucxmmc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gomdiqzft.sHtML

[D15] 去重
来源：http://3g.tarul.cn/Article/details/ghjphxwyy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/gnrwgaxxe.sHtML

PHP:  array_unique($arr);
来源：http://m.share.sjlbkw.cn/Article/details/grpgeprqv.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/govwquuks.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/gupqvhluo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.bbcook.cn/Article/details/gmrlewdvy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.tarul.cn/Article/details/ghbjrkjzg.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/guwjdxnjk.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.vehdjk.com/Article/details/gjnwvtzyn.sHtML

[D16] 求和与平均值
来源：http://3g.tarul.cn/Article/details/gxmermhje.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gzuinasqg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.yfazqb.com/Article/details/gbswreynu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gmyzvxolw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.bbcook.cn/Article/details/gyrylwzfe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.vehdjk.com/Article/details/gfvbwecem.sHtML

Go:   // 手写循环累加
来源：http://wap.tarul.cn/Article/details/gbqcxxxmw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.epnwcf.com/Article/details/gsjhictvr.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.yfazqb.com/Article/details/gtcoxxfvh.sHtML

[D17] 最大值与最小值
来源：http://blog.fktsv.cn/Article/details/gftoxiwao.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.bbcook.cn/Article/details/gzogfkecc.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fktsv.cn/Article/details/glwrspwkk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.bbcook.cn/Article/details/goljznkkw.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/ggqbefadu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.tarul.cn/Article/details/gmscaxepk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.bbcook.cn/Article/details/gnsmihwan.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.bbcook.cn/Article/details/gingroddl.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fktsv.cn/Article/details/gltkzjrpu.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.vehdjk.com/Article/details/gnihbbrrw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.yfazqb.com/Article/details/gukacfvlj.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.sjlbkw.cn/Article/details/glsnmdszf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.epnwcf.com/Article/details/gfhippewk.sHtML

TS:   nested.flat();
来源：http://3g.yfazqb.com/Article/details/gitcnedbz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.yfazqb.com/Article/details/gspwigwpt.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.tarul.cn/Article/details/gvyvvxbxg.sHtML

Ruby: nested.flatten
来源：http://www.share.sjlbkw.cn/Article/details/gglychumg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.vehdjk.com/Article/details/gfvmtrraf.sHtML

[D19] 按字段分组
来源：http://3g.fktsv.cn/Article/details/gisymcvpk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.epnwcf.com/Article/details/ghokayrlt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.tarul.cn/Article/details/gyiwrbfox.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.tarul.cn/Article/details/gkiksivaj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.tarul.cn/Article/details/giarydogw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.tarul.cn/Article/details/ggtytskww.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.epnwcf.com/Article/details/gtazmrghb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.vehdjk.com/Article/details/giwhslfns.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.bbcook.cn/Article/details/ghgzugzkw.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.vehdjk.com/Article/details/gljnefowc.sHtML

Py:   Counter(arr)
来源：http://wap.epnwcf.com/Article/details/gkdvqqewr.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.yfazqb.com/Article/details/grafkqufg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.sjlbkw.cn/Article/details/gajrgevxb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gjeaaliyb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.vehdjk.com/Article/details/gsrbszusc.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.epnwcf.com/Article/details/ggsulgebk.sHtML

Ruby: arr.tally
来源：http://read.share.sjlbkw.cn/Article/details/gxqsusxcp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.tarul.cn/Article/details/gdcdpdwxb.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fktsv.cn/Article/details/gdxyjvbav.sHtML

Py:   x in arr
来源：http://mobile.sjlbkw.cn/Article/details/gfxfqolgg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.yfazqb.com/Article/details/gonpsxkxt.sHtML

JS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/gvjutctjm.sHtML

TS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gsifgktjx.sHtML

Java: list.contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gnwsgbgqi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.bbcook.cn/Article/details/ghhtmklvn.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fktsv.cn/Article/details/guldagymq.sHtML

C#:   list.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/grhbyvqvz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.yfazqb.com/Article/details/gzlptpzsg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fktsv.cn/Article/details/gptbkuopa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.yfazqb.com/Article/details/gyjkcgawl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/gfpydlhae.sHtML

TS:   [...arr];
来源：http://baike.tarul.cn/Article/details/gdtnhkmxp.sHtML


<!-- 参考信息 -->