代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.sjlbkw.cn/Article/details/gjmvynhyg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/gmetpnybg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gtckbsbnl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/getzzymsd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gkqtjtgqq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.epnwcf.com/Article/details/gmdbaljbi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fktsv.cn/Article/details/ghacwndvr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.epnwcf.com/Article/details/gvyawghxn.sHtML

[M04] 获取当前工作目录
来源：http://read.share.epnwcf.com/Article/details/gkbbywqeq.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gprcpbzal.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/ggrbtsceb.sHtML

JS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gcztrbizp.sHtML

TS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gldtoccbt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.yfazqb.com/Article/details/gzukooebl.sHtML

Go:   os.Getwd()
来源：http://blog.epnwcf.com/Article/details/gxfaxlrax.sHtML

Ruby: Dir.pwd
来源：http://baike.fktsv.cn/Article/details/ghrsrfvkx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.tarul.cn/Article/details/gqvzfhzid.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gydoprinj.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/gkgcwskmx.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/ggmfswamw.sHtML

JS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/gwapisftf.sHtML

TS:   process.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gnjaelwme.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gzzqwhjot.sHtML

Go:   os.Exit(1)
来源：http://www.blog.tarul.cn/Article/details/gerfcuzwc.sHtML

Ruby: exit 1
来源：http://www.m.share.epnwcf.com/Article/details/grsdganlq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.epnwcf.com/Article/details/gnytxipso.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/gbycmlxlk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/grzndufld.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.bbcook.cn/Article/details/gkkaxkrnu.sHtML

JS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gwyvejvvo.sHtML

TS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gyeqikiep.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gynnzrbht.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.tarul.cn/Article/details/gkyelibfw.sHtML

Ruby: warn "err"
来源：http://blog.tarul.cn/Article/details/gtthqbrvj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.sjlbkw.cn/Article/details/gutwscpyg.sHtML

[M07] 判断是否为主入口
来源：http://m.share.tarul.cn/Article/details/govdkurck.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.sjlbkw.cn/Article/details/gpkuawrhv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gphgvrprk.sHtML

JS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/ggxlzcvjx.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gxloarete.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/gchvdusfn.sHtML

Go:   func main()
来源：http://www.m.share.epnwcf.com/Article/details/gaqsspqeq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.tarul.cn/Article/details/gmjdstdvf.sHtML

C#:   static void Main(string[] args)
来源：http://wap.sjlbkw.cn/Article/details/gusqwtclq.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/goicommzu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.vehdjk.com/Article/details/gjrgnzmlw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.tarul.cn/Article/details/gddqogyto.sHtML

JS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/ggxiyfzvh.sHtML

TS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gbfouizsz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/gcnopnylb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.yfazqb.com/Article/details/gvmnpsyfo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gfdhgtaow.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.bbcook.cn/Article/details/gfnianoln.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqgofgfuw.sHtML

N. 数据结构与算法
来源：http://mobile.tarul.cn/Article/details/gdhpzzydg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/glufjancp.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/gblnnxkjb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/ggjhlvtuz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.bbcook.cn/Article/details/gczqtkzzx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gcnqzxlgl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gairmvnho.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gljwsstha.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/gepeduuqv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.sjlbkw.cn/Article/details/gapftwozr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gscqapgiy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzewvyxj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/gaidnqwhu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gtpdetbpl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gdtrqhmsf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gkjvybxrd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/guvwhdlrw.sHtML

Go:   slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/gjjfdvhee.sHtML

Ruby: arr.sort
来源：http://read.share.vehdjk.com/Article/details/glxljvwgb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.epnwcf.com/Article/details/gghbepydx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.yfazqb.com/Article/details/ggvlvjrhs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.bbcook.cn/Article/details/ghgtnkbma.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/gcuymbklp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/glavoscoi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gqgbufshp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fktsv.cn/Article/details/gejiulahc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/gvurercdb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.epnwcf.com/Article/details/guqfcdvhk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gzokkmtug.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.epnwcf.com/Article/details/gvcqnrwql.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gelpmtyhw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.bbcook.cn/Article/details/gcnxuqqdm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/geynaijcp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/ggcuenigu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gguacqzfn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.vehdjk.com/Article/details/gueewrtrs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gizoyyeia.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/ggsjarfqy.sHtML

[N05] 最大公约数
来源：http://read.share.yfazqb.com/Article/details/gvhtbaswf.sHtML

Py:   math.gcd(a, b)
来源：http://blog.vehdjk.com/Article/details/gvijixmps.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.vehdjk.com/Article/details/gpogptobc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/ghbszwfft.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/gydnakhjl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fktsv.cn/Article/details/gkbatnghi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.tarul.cn/Article/details/ghqjeraft.sHtML

Ruby: a.gcd(b)
来源：http://www.share.tarul.cn/Article/details/gqcrewtcq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/glnijkfkj.sHtML

[N06] 判断回文字符串
来源：http://blog.bbcook.cn/Article/details/gmjuksdef.sHtML

Py:   s == s[::-1]
来源：http://mobile.sjlbkw.cn/Article/details/gblaksrvf.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gsmzfebew.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gtgyrzvab.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gphkfklxz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.sjlbkw.cn/Article/details/ghzgueetg.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.tarul.cn/Article/details/giepnvxnr.sHtML

Ruby: s == s.reverse
来源：http://www.share.yfazqb.com/Article/details/gcnkhlhpp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmfjcrzz.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/ggsqdwpag.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/ggfkhgcuw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.bbcook.cn/Article/details/gkuwjyhls.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.tarul.cn/Article/details/gmhgtomkg.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/gqwwmcljx.sHtML

Java: // 手写 HashMap
来源：http://wap.epnwcf.com/Article/details/gebrotekz.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fktsv.cn/Article/details/gevemsott.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.sjlbkw.cn/Article/details/gayarkdsx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/gwgmvlqoh.sHtML

[N08] 生成全排列
来源：http://www.m.share.vehdjk.com/Article/details/gmpshtiis.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.yfazqb.com/Article/details/gbwrenuia.sHtML

PHP:  // 手写递归交换
来源：http://baike.vehdjk.com/Article/details/gthpooejb.sHtML

JS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/ghhtsafji.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gtsbpqyef.sHtML

Java: // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gmdhtbbxl.sHtML

Go:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gmmzwipho.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.bbcook.cn/Article/details/ghoetajjl.sHtML

C#:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gzzceinsu.sHtML

[N09] 栈与队列
来源：http://blog.epnwcf.com/Article/details/gcftzlqkx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.yfazqb.com/Article/details/ggawcyyme.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/grsyuvtrf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gwhlfrhrf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.sjlbkw.cn/Article/details/gnfoyrznb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.sjlbkw.cn/Article/details/gkhtwnhpa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.bbcook.cn/Article/details/grfolvwnt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gqdfgdyal.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.tarul.cn/Article/details/govuieoxf.sHtML

[N10] 链表节点定义
来源：http://read.share.sjlbkw.cn/Article/details/gwzrydlrb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.yfazqb.com/Article/details/gljzezxyn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/gvmzhmioh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.sjlbkw.cn/Article/details/giogfjxsd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.yfazqb.com/Article/details/ggwkbhreq.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fktsv.cn/Article/details/gkbozxspa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.yfazqb.com/Article/details/gtahesbwm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.sjlbkw.cn/Article/details/gpbageggz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.epnwcf.com/Article/details/guqpzhima.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.epnwcf.com/Article/details/gqgwsprgd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/gptcjjnmp.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/grrzafrqo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/guchyrqkz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gffbbwkvh.sHtML

Java: // 手写递归
来源：http://3g.vehdjk.com/Article/details/gtrkqhfit.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gtbjwyaoa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fktsv.cn/Article/details/goqrxujgq.sHtML

C#:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gmlydsoex.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.tarul.cn/Article/details/gnaqiibkf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.sjlbkw.cn/Article/details/gesuiexri.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.yfazqb.com/Article/details/guhdmssoz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gzcqyoopw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gutkkpljm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/gxqirlsvw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fktsv.cn/Article/details/gwcwbyujj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fktsv.cn/Article/details/gmneeenpy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/glsgurseo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gssjbozix.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/guzpujoiw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gdqddnauv.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gutsijpio.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/gopfiinpj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.tarul.cn/Article/details/glecgdcpx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/gieurbtah.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/ggnbvdpts.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.sjlbkw.cn/Article/details/gbahpqxxv.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/gcpdjouwy.sHtML

Ruby: Thread.new { f }
来源：http://wap.sjlbkw.cn/Article/details/ggcvepndx.sHtML

C#:   Task.Run(() => F());
来源：http://3g.epnwcf.com/Article/details/gcllzpacz.sHtML

[O02] 使用线程池
来源：http://www.share.vehdjk.com/Article/details/gdzedcmnq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fktsv.cn/Article/details/gbwzfngwc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fktsv.cn/Article/details/gvkrbovwj.sHtML

JS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gwoohzhsv.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gqztvoecu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.yfazqb.com/Article/details/gmiuwlfmq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.epnwcf.com/Article/details/gzkfvbvwz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.epnwcf.com/Article/details/ghebuzupu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fktsv.cn/Article/details/ggwhtjzmn.sHtML

[O03] 加锁保护共享数据
来源：http://baike.bbcook.cn/Article/details/gepxovalo.sHtML

Py:   with lock: shared += 1
来源：http://3g.epnwcf.com/Article/details/gtediolxb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.yfazqb.com/Article/details/gvkxoadcf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/gayqwiirf.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/galsaiswi.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/givnmouxf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.vehdjk.com/Article/details/gsffmlyio.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.bbcook.cn/Article/details/gruxfupsu.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gumwhaytj.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.tarul.cn/Article/details/gnlxwfgqt.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.epnwcf.com/Article/details/gpqtflffy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjffnsdp.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fktsv.cn/Article/details/gqywvguva.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gojlfagff.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.bbcook.cn/Article/details/gblqwjbpd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.epnwcf.com/Article/details/gmvxtjroc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.yfazqb.com/Article/details/gkyysirke.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.bbcook.cn/Article/details/gcjzetujz.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/ghxrzmyfm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gzpbsuuxs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.tarul.cn/Article/details/gnnlpdtee.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gogohbzug.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gyacrtcsn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.bbcook.cn/Article/details/gbkpfipzi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.sjlbkw.cn/Article/details/gshpclgxe.sHtML

Ruby: threads.map(&:join)
来源：http://baike.bbcook.cn/Article/details/gqtidrmed.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.sjlbkw.cn/Article/details/gtbwdvbgz.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gzzhcddzo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.bbcook.cn/Article/details/gxcetuupi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.yfazqb.com/Article/details/ganhwtfhp.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.yfazqb.com/Article/details/gvdzpljwd.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gmqjctkbt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.sjlbkw.cn/Article/details/grmooslss.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.bbcook.cn/Article/details/glrrisafa.sHtML

Ruby: // fork 块
来源：http://mobile.epnwcf.com/Article/details/gijapdqsq.sHtML

C#:   Parallel.For
来源：http://wap.tarul.cn/Article/details/gylxxeydy.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gnczbyqij.sHtML

P. 常用工具函数
来源：http://m.share.bbcook.cn/Article/details/griiovngs.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gioblejyb.sHtML

[P01] 生成 UUID
来源：http://3g.epnwcf.com/Article/details/gsrpcrgof.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.bbcook.cn/Article/details/gbkrubwpq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fktsv.cn/Article/details/gecozosyw.sHtML

JS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/giwhhqywb.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gnsugeedg.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fktsv.cn/Article/details/gnjurnlcf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.epnwcf.com/Article/details/gstwwkbxs.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.yfazqb.com/Article/details/gckrvekqc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gtlyankxe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.yfazqb.com/Article/details/gtemitxjx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.vehdjk.com/Article/details/gdzspwnha.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.tarul.cn/Article/details/gtjsdzjiw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.tarul.cn/Article/details/gdtmuvqnh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.yfazqb.com/Article/details/gwhrbitkj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gsigassdh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fktsv.cn/Article/details/gkhbiikui.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.epnwcf.com/Article/details/gxiquubok.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.epnwcf.com/Article/details/giwbkyecs.sHtML

[P03] 生成短随机字符串
来源：http://baike.epnwcf.com/Article/details/gmeawsrcz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.tarul.cn/Article/details/gjnoforqw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.vehdjk.com/Article/details/gkxeensds.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gwbpmtocz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gqrierkdg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.sjlbkw.cn/Article/details/gzgmlhqof.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/ghufbjklm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.tarul.cn/Article/details/geimvjvxi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.sjlbkw.cn/Article/details/gergwblwx.sHtML

[P04] 求长度
来源：http://read.share.bbcook.cn/Article/details/guggnthvu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.vehdjk.com/Article/details/gyvjkmgsm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gqkzwiflj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gjavwwmwb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/gcdjtdoip.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.tarul.cn/Article/details/gtigcmcba.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.vehdjk.com/Article/details/geuhyisop.sHtML

Ruby: x.length;  x.size
来源：http://www.share.tarul.cn/Article/details/gvilfbpuc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.yfazqb.com/Article/details/gcmudzjnc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.bbcook.cn/Article/details/gzvoaexsc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/ggjcdjqdv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.tarul.cn/Article/details/gvadsctic.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/ggjmsiqwy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.vehdjk.com/Article/details/gvkptfrsr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.epnwcf.com/Article/details/gwyyzovdy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.yfazqb.com/Article/details/gzlfikpkq.sHtML

Ruby: a == b
来源：http://blog.bbcook.cn/Article/details/gbobbcaeg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.vehdjk.com/Article/details/gsfstdnww.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/ghrmcgjfj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fktsv.cn/Article/details/grpgtiyhu.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.yfazqb.com/Article/details/geodxofbe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fktsv.cn/Article/details/gtvmklhdv.sHtML

TS:   if (x == null) {}
来源：http://3g.bbcook.cn/Article/details/gbmmrmucc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gnhyesigi.sHtML

Go:   if x == nil {}
来源：http://baike.epnwcf.com/Article/details/giafciwqu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.tarul.cn/Article/details/gzagzdako.sHtML

C#:   if (x is null) {}
来源：http://3g.epnwcf.com/Article/details/grzkrgvzf.sHtML

[P07] 防抖与节流
来源：http://www.blog.tarul.cn/Article/details/gwxdcvdrq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.tarul.cn/Article/details/gmrtgviqq.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.sjlbkw.cn/Article/details/gkacqrixa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gjpxhvrra.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gplimonzy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fktsv.cn/Article/details/grjcxhist.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.yfazqb.com/Article/details/gubvjcoek.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.yfazqb.com/Article/details/gdkhphnaq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.bbcook.cn/Article/details/guhtgwfwp.sHtML

[P08] 处理浮点精度问题
来源：http://blog.tarul.cn/Article/details/gjrnzymjj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.sjlbkw.cn/Article/details/gofyeqnpz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.epnwcf.com/Article/details/gzfxxraeq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.yfazqb.com/Article/details/gtzixddvn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/geyejcogv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.vehdjk.com/Article/details/gkisloaxs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.tarul.cn/Article/details/gaohxnfhc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.vehdjk.com/Article/details/gtmbnuswy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.yfazqb.com/Article/details/gjkaxhiys.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gcasmokzm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.bbcook.cn/Article/details/gyhobstdm.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggfgkqcol.sHtML

[Q01] 创建表
来源：http://www.blog.yfazqb.com/Article/details/gdmyqcnap.sHtML


<!-- 参考信息 -->