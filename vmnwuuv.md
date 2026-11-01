代发 wailian999

[M04] 获取当前工作目录
来源：http://www.share.yfazqb.com/Article/details/grpowyvap.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/gvyfkxxfm.sHtML

PHP:  getcwd();
来源：http://baike.fktsv.cn/Article/details/gfaevhgxh.sHtML

JS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gyhluqtid.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/ghyqnbsgq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.sjlbkw.cn/Article/details/gvqptzwzx.sHtML

Go:   os.Getwd()
来源：http://www.blog.epnwcf.com/Article/details/geiqcsgnp.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.tarul.cn/Article/details/gmreympsc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.tarul.cn/Article/details/gckemedli.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gtnerfsxf.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gsrbtcpgp.sHtML

PHP:  exit(1);
来源：http://m.share.vehdjk.com/Article/details/gtmnwsroj.sHtML

JS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/guncudypl.sHtML

TS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/glzpewgkz.sHtML

Java: System.exit(1)
来源：http://3g.yfazqb.com/Article/details/gpxkarvyx.sHtML

Go:   os.Exit(1)
来源：http://baike.epnwcf.com/Article/details/gxwjymamc.sHtML

Ruby: exit 1
来源：http://blog.epnwcf.com/Article/details/gxlpzzqbs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.epnwcf.com/Article/details/gywefyupd.sHtML

[M06] 向标准错误输出
来源：http://www.share.tarul.cn/Article/details/gfvhpddto.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/gbuqeddin.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfmwiwji.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gcumezutr.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gadxjbmxt.sHtML

Java: System.err.println("err")
来源：http://mobile.tarul.cn/Article/details/gtcbnamvz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.vehdjk.com/Article/details/gddyjkwbz.sHtML

Ruby: warn "err"
来源：http://read.share.fktsv.cn/Article/details/gykniqamt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.yfazqb.com/Article/details/gydffbkcj.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/gfnjfofey.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.epnwcf.com/Article/details/gpjrqngfd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.vehdjk.com/Article/details/gwvulhoyf.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gsbobvzge.sHtML

TS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gdhpsqpki.sHtML

Java: public static void main(String[] args)
来源：http://baike.bbcook.cn/Article/details/gdmjwccwx.sHtML

Go:   func main()
来源：http://baike.fktsv.cn/Article/details/gjhggulyc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.vehdjk.com/Article/details/gwrnudsnd.sHtML

C#:   static void Main(string[] args)
来源：http://blog.sjlbkw.cn/Article/details/gwjqlmxsp.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.epnwcf.com/Article/details/ggisnrmgx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.tarul.cn/Article/details/ggglrqeeo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/gliwgotzy.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gzjvccvgu.sHtML

TS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gbfooqfqe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.tarul.cn/Article/details/gskjunknc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/goyicckdg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.bbcook.cn/Article/details/gfjaoxmpy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.tarul.cn/Article/details/gjqeaqtgz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gagurkbmg.sHtML

N. 数据结构与算法
来源：http://wap.yfazqb.com/Article/details/gysjxrhyo.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/godhlmxdu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.yfazqb.com/Article/details/gqrwejwic.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.vehdjk.com/Article/details/gijpgdkro.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.vehdjk.com/Article/details/gqrrjinjz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gwfiomgqe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/garrdfwcy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gbzowvcln.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gqhfyhczo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.vehdjk.com/Article/details/gtmmnimaz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/ggpmhqgzj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.yfazqb.com/Article/details/gbeeisntu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gzcxryedg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.bbcook.cn/Article/details/gxotumdpk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gzujjkpez.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gyzzgnlxb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.tarul.cn/Article/details/gsnkioajh.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gmxncxswi.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gyctxkcqe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.yfazqb.com/Article/details/gpmbnsmjd.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/gqejyfnwv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.tarul.cn/Article/details/gnftzjulz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.yfazqb.com/Article/details/gzmmzutig.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/ggdknvvsx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/gsrxrfzbi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.bbcook.cn/Article/details/gvwoamzfi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.tarul.cn/Article/details/giksgfzay.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.tarul.cn/Article/details/gshckeojv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/gqwevqjef.sHtML

[N04] 斐波那契数列
来源：http://read.share.bbcook.cn/Article/details/gfzthzrkg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/grexzwjkz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gymefrmdk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gmlluiwzz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/glvdapxul.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.vehdjk.com/Article/details/gzcmtcdof.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.tarul.cn/Article/details/gjxaxepnn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gpnonsoaw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gjedctmgv.sHtML

[N05] 最大公约数
来源：http://blog.epnwcf.com/Article/details/gwcuesyhg.sHtML

Py:   math.gcd(a, b)
来源：http://baike.epnwcf.com/Article/details/gilgckrzn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fktsv.cn/Article/details/gsycwqzad.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gqqiubqya.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gbpnrsqkr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.epnwcf.com/Article/details/genvxdzbf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.vehdjk.com/Article/details/gzxywgmos.sHtML

Ruby: a.gcd(b)
来源：http://read.share.bbcook.cn/Article/details/gjdrkjuat.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.vehdjk.com/Article/details/gmuvwhqna.sHtML

[N06] 判断回文字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gogszwphq.sHtML

Py:   s == s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gntpaefch.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/gdvxrijns.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gvdfjvhmt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gujkvbmjq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/geszeekhk.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/gglenitfq.sHtML

Ruby: s == s.reverse
来源：http://m.share.vehdjk.com/Article/details/gwphdwbob.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/gaomwzjji.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.vehdjk.com/Article/details/ggfaxfnwy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fktsv.cn/Article/details/gealtfcix.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.bbcook.cn/Article/details/gunsfncqh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.sjlbkw.cn/Article/details/gnohphzbx.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/gridqdsdo.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/grzfxalij.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gegqdvzxk.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fktsv.cn/Article/details/grbssofys.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.bbcook.cn/Article/details/glwkqwgcv.sHtML

[N08] 生成全排列
来源：http://baike.bbcook.cn/Article/details/gbrrkzdep.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gynddnyzl.sHtML

PHP:  // 手写递归交换
来源：http://m.share.epnwcf.com/Article/details/gncgoggnw.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gmhhctnkn.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gyfuouwjf.sHtML

Java: // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gswaymlpm.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gfgxqrmdj.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.epnwcf.com/Article/details/guhakucgs.sHtML

C#:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gcolitdpu.sHtML

[N09] 栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gceowoovu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.vehdjk.com/Article/details/gcxywifhi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gmkscdyeh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gaamlxiwb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.tarul.cn/Article/details/gizdddcmc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gpvtowzyy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/gcnzvseva.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/grhbbmezl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.yfazqb.com/Article/details/gmgxatjac.sHtML

[N10] 链表节点定义
来源：http://wap.bbcook.cn/Article/details/gyognadfq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.tarul.cn/Article/details/gntesjqig.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/glycezvuq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/gygdxwlov.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.bbcook.cn/Article/details/gcjdnxnbk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gvpzppggd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.sjlbkw.cn/Article/details/ggqobufxv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fktsv.cn/Article/details/gwlesovyv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.yfazqb.com/Article/details/geqiydhhn.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/guealgqrb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.epnwcf.com/Article/details/gixeejlpb.sHtML

PHP:  // 手写递归函数
来源：http://m.share.vehdjk.com/Article/details/gjeuvlahx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/guoartxcd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gxbxlthox.sHtML

Java: // 手写递归
来源：http://blog.yfazqb.com/Article/details/gnqszuqgm.sHtML

Go:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gtcgarhyy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/gndteqdwr.sHtML

C#:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gemsyvuyx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.vehdjk.com/Article/details/gotakkxha.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.epnwcf.com/Article/details/gnvgxyshi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.sjlbkw.cn/Article/details/gzpqcjvuv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gvrcdibnx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/giwwyqwud.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gsmoaqntp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.bbcook.cn/Article/details/gzqufjexz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.yfazqb.com/Article/details/ggjfwapit.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gnpsaygww.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqvkhshfo.sHtML

O. 并发与异步
来源：http://blog.tarul.cn/Article/details/grctusnmz.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gvtskepvn.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gtdhscscv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/gthrimzjj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fktsv.cn/Article/details/gelzyjiqh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.vehdjk.com/Article/details/gpjpsktbz.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/grciusbro.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.epnwcf.com/Article/details/gwzpelrho.sHtML

Go:   go f()
来源：http://blog.yfazqb.com/Article/details/gpvqtccmk.sHtML

Ruby: Thread.new { f }
来源：http://blog.bbcook.cn/Article/details/gyrqbmkih.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.yfazqb.com/Article/details/gpwfcomcr.sHtML

[O02] 使用线程池
来源：http://blog.fktsv.cn/Article/details/gnarkipkg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/gpxboludu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.vehdjk.com/Article/details/ggxkoolgr.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gsokigkil.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gcvmyxucp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/gduqaqmqh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/gurrdquhc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/gxipuvmtz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.vehdjk.com/Article/details/ghhgzsuqy.sHtML

[O03] 加锁保护共享数据
来源：http://baike.sjlbkw.cn/Article/details/gvujkehnn.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fktsv.cn/Article/details/gqmfdorzd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/ggqvbsqtp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.tarul.cn/Article/details/gpdnjwfoy.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gxnhfzmph.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gbytpgdux.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.epnwcf.com/Article/details/gkknocmmg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.tarul.cn/Article/details/gzighdwzc.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gizmoovpv.sHtML

[O04] 定义异步函数并等待
来源：http://wap.tarul.cn/Article/details/gorwfwroa.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.yfazqb.com/Article/details/gcrmupvhz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.bbcook.cn/Article/details/glgkvpgrv.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gkhsivejk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/gwqgpppjf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.bbcook.cn/Article/details/gvumwuwhs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/gndxuiogk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.bbcook.cn/Article/details/gydwzhdki.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.tarul.cn/Article/details/gtvdirddg.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.tarul.cn/Article/details/gmbdodaod.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.vehdjk.com/Article/details/glsbtmhla.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/gntieznlz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gylaiasnb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gpuokiycm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.yfazqb.com/Article/details/glcjiowzu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.yfazqb.com/Article/details/gugawciva.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.yfazqb.com/Article/details/ghtinkanu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.epnwcf.com/Article/details/gwdxvecks.sHtML

[O06] 使用进程池
来源：http://blog.fktsv.cn/Article/details/gwnevyewx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.bbcook.cn/Article/details/gouhsrxqx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.bbcook.cn/Article/details/gxvhuvodr.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gzweanmke.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gfsdgucmr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fktsv.cn/Article/details/gojtiipnv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.vehdjk.com/Article/details/gljdpnkvs.sHtML

Ruby: // fork 块
来源：http://m.share.sjlbkw.cn/Article/details/gykmomzml.sHtML

C#:   Parallel.For
来源：http://read.share.yfazqb.com/Article/details/ggrdifnfz.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gjczpqcwb.sHtML

P. 常用工具函数
来源：http://www.m.share.fktsv.cn/Article/details/gvfxgtpde.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gswrdfmbs.sHtML

[P01] 生成 UUID
来源：http://www.share.epnwcf.com/Article/details/ggloqwxtt.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.sjlbkw.cn/Article/details/gjazcpkjd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fktsv.cn/Article/details/gpjajoowm.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gbfhzetyg.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gpwxpdnww.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fktsv.cn/Article/details/gnuehkxhr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.epnwcf.com/Article/details/gdjcyndqi.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.bbcook.cn/Article/details/gkdvlaixp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fktsv.cn/Article/details/gazvmnuzb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fktsv.cn/Article/details/gdbyfkfbj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.vehdjk.com/Article/details/gagzdkeyx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.epnwcf.com/Article/details/gqqdckbrd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.sjlbkw.cn/Article/details/gyrbyywji.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.sjlbkw.cn/Article/details/gonsagabg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gpqfqryzr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.bbcook.cn/Article/details/gfivbjayx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/gtjcmwdam.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.tarul.cn/Article/details/gaaxsiykc.sHtML

[P03] 生成短随机字符串
来源：http://mobile.epnwcf.com/Article/details/glkhbyunw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.yfazqb.com/Article/details/gaquoznhi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.epnwcf.com/Article/details/gznfhuaww.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/grfrklgpv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/ghsngqohx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fktsv.cn/Article/details/gmjhfkbjm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.tarul.cn/Article/details/gefpyzuyb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.bbcook.cn/Article/details/gfeplhrih.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fktsv.cn/Article/details/gyhzgflvl.sHtML

[P04] 求长度
来源：http://3g.bbcook.cn/Article/details/gkmpwbpbt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.sjlbkw.cn/Article/details/gvgisqoch.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/ggbcltrvg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/guonfikqo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/grxinzblq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.yfazqb.com/Article/details/gvrbiegkv.sHtML

Go:   len(arr);  len(m)
来源：http://3g.yfazqb.com/Article/details/gnjqsieim.sHtML

Ruby: x.length;  x.size
来源：http://3g.sjlbkw.cn/Article/details/gqquxeccr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fktsv.cn/Article/details/gfhhqkidg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.sjlbkw.cn/Article/details/gmlcwdfku.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.tarul.cn/Article/details/gxrgivoey.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fktsv.cn/Article/details/gapkjpmmp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.bbcook.cn/Article/details/gaavmhkcp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.bbcook.cn/Article/details/gczsshhvo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.yfazqb.com/Article/details/gfjzhngfc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gmeiktkjj.sHtML

Ruby: a == b
来源：http://www.m.share.fktsv.cn/Article/details/gwozkojaq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fktsv.cn/Article/details/glulkixzn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.yfazqb.com/Article/details/gbthsliqj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.bbcook.cn/Article/details/gwibqabpe.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fktsv.cn/Article/details/ghkrhmswq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.sjlbkw.cn/Article/details/gqstmskfx.sHtML

TS:   if (x == null) {}
来源：http://www.blog.tarul.cn/Article/details/gjeehokeh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/gpidpdmyy.sHtML

Go:   if x == nil {}
来源：http://www.share.yfazqb.com/Article/details/gjmmcpxmx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.epnwcf.com/Article/details/gfockkqcs.sHtML

C#:   if (x is null) {}
来源：http://baike.epnwcf.com/Article/details/gbqnmcpce.sHtML

[P07] 防抖与节流
来源：http://www.blog.yfazqb.com/Article/details/geniisbbd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/gegvxsnii.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.sjlbkw.cn/Article/details/gruverzpf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/ghynkwhnd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkysjdnf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.vehdjk.com/Article/details/gtvdcrjfi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.epnwcf.com/Article/details/goapdbuck.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fktsv.cn/Article/details/goflggqpu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.tarul.cn/Article/details/gnujoykty.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.yfazqb.com/Article/details/guiekepxc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.bbcook.cn/Article/details/gqeesaxjd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.yfazqb.com/Article/details/gxrsubarb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/gwxvtlxjc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gnoehpoxw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.vehdjk.com/Article/details/gokyarfbm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.epnwcf.com/Article/details/gzskntbbd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.epnwcf.com/Article/details/gkgghyhqu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.bbcook.cn/Article/details/garsvanoq.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwawwolkz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fktsv.cn/Article/details/gwuisvknw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gpcxaiyxx.sHtML

[Q01] 创建表
来源：http://read.share.vehdjk.com/Article/details/glfacvfop.sHtML

CREATE TABLE users (
来源：http://blog.fktsv.cn/Article/details/gdppqspzw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/gruxrvwmj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gnugdcbxj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fktsv.cn/Article/details/gkxgftcmz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.vehdjk.com/Article/details/goielbglw.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gyrbcupxf.sHtML

[Q02] 创建带外键的表
来源：http://mobile.yfazqb.com/Article/details/gxjkawtte.sHtML

CREATE TABLE orders (
来源：http://www.blog.tarul.cn/Article/details/gyikrculs.sHtML


<!-- 参考信息 -->