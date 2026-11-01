代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.yfazqb.com/Article/details/gnrvfqavc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.epnwcf.com/Article/details/geklwassm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gikqdykvc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gokesjvnf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.sjlbkw.cn/Article/details/gcaqosibs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.epnwcf.com/Article/details/gerxxiyxz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.epnwcf.com/Article/details/ggwsknfqk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.yfazqb.com/Article/details/gogqqujbp.sHtML

[M04] 获取当前工作目录
来源：http://blog.fktsv.cn/Article/details/grzmsbqca.sHtML

Py:   os.getcwd()
来源：http://mobile.fktsv.cn/Article/details/gupdzzrkq.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gfajmbuhv.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gjpwdlcdl.sHtML

TS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/galzrtvwp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.bbcook.cn/Article/details/gdihzanqy.sHtML

Go:   os.Getwd()
来源：http://www.blog.fktsv.cn/Article/details/gggpyqjta.sHtML

Ruby: Dir.pwd
来源：http://mobile.sjlbkw.cn/Article/details/gwiyyprov.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.yfazqb.com/Article/details/gxcujiezt.sHtML

[M05] 设置退出码
来源：http://blog.tarul.cn/Article/details/gknudrzit.sHtML

Py:   sys.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gqxftzlnv.sHtML

PHP:  exit(1);
来源：http://blog.tarul.cn/Article/details/gbjxxqink.sHtML

JS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gancvuoka.sHtML

TS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gfouvzjtb.sHtML

Java: System.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gxuzlzfbz.sHtML

Go:   os.Exit(1)
来源：http://baike.epnwcf.com/Article/details/gcqyidtiz.sHtML

Ruby: exit 1
来源：http://www.share.vehdjk.com/Article/details/gebpkputk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.tarul.cn/Article/details/gxarpptbz.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gchqjceqs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.sjlbkw.cn/Article/details/gpsrceige.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.bbcook.cn/Article/details/gbuzciope.sHtML

JS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gwnewctyt.sHtML

TS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/gmjdwhjik.sHtML

Java: System.err.println("err")
来源：http://mobile.yfazqb.com/Article/details/gcwjaajra.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.epnwcf.com/Article/details/guxrzvdai.sHtML

Ruby: warn "err"
来源：http://www.share.yfazqb.com/Article/details/guylxtbye.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.vehdjk.com/Article/details/giohgyosh.sHtML

[M07] 判断是否为主入口
来源：http://www.share.vehdjk.com/Article/details/gsldryoqc.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fktsv.cn/Article/details/gdqxcwbbg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.vehdjk.com/Article/details/gklcomegg.sHtML

JS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/guhwzfhyt.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gxvhheegw.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gfybkpvkw.sHtML

Go:   func main()
来源：http://wap.sjlbkw.cn/Article/details/guvbuyjob.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.yfazqb.com/Article/details/gpzgdlthh.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/gpsnkybtd.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.bbcook.cn/Article/details/gkaoavpyx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.vehdjk.com/Article/details/guofniswo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.yfazqb.com/Article/details/gionpoish.sHtML

JS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gmargmnkr.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gmzmescdk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.yfazqb.com/Article/details/gkycsupdl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.yfazqb.com/Article/details/gidgvplnc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/ghbgkokst.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.vehdjk.com/Article/details/gukmhhrbl.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkbolbemw.sHtML

N. 数据结构与算法
来源：http://read.share.vehdjk.com/Article/details/girhzibdb.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gzuxvqkdz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.tarul.cn/Article/details/gbfwpnjdh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/giwzqfggu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.tarul.cn/Article/details/geintrjdy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gpzqthlde.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gphgpfuxx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gkurtpvyo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gbhmfztgs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.yfazqb.com/Article/details/gewjmsurx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gqfcexkqz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.yfazqb.com/Article/details/gkozpircw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gxqymifcm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.bbcook.cn/Article/details/glawygbjj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gldazjzlo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gqlototcd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fktsv.cn/Article/details/gatwpjtfy.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.vehdjk.com/Article/details/gefpnofti.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gtikkuute.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fktsv.cn/Article/details/gcysrygfj.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fktsv.cn/Article/details/gblmwmods.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.epnwcf.com/Article/details/gxyjepner.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.yfazqb.com/Article/details/gsyhzlrdz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gkrmcjohz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gwsrimptg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fktsv.cn/Article/details/gnpaonynu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.vehdjk.com/Article/details/gxqaffxzl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbwlavad.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.yfazqb.com/Article/details/gpztwyhrk.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/gdoxehhyd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gzgfcgpva.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gksuecpwb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gwxvkwwvo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gjdvfliga.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.tarul.cn/Article/details/gkibnrlny.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.bbcook.cn/Article/details/goxaskywz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gqdftebap.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gxciihnco.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/gvmeoyjxy.sHtML

Py:   math.gcd(a, b)
来源：http://3g.tarul.cn/Article/details/geugdmpdj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.bbcook.cn/Article/details/gjzxznkfi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/ghdijzoaw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gyuaookev.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.vehdjk.com/Article/details/gslenwwiu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.tarul.cn/Article/details/glvrqapck.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.bbcook.cn/Article/details/gvgjkjdfm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.epnwcf.com/Article/details/ghozswunj.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/gzuhcapvk.sHtML

Py:   s == s[::-1]
来源：http://wap.tarul.cn/Article/details/grtcyzhwx.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gslbpwsxj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/giumzsccr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/goqkpmnfg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/gieyatblp.sHtML

Go:   // 双指针从两端比较
来源：http://blog.epnwcf.com/Article/details/gsfmzjbji.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gscwwhppk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gkcyjpbvr.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.yfazqb.com/Article/details/gcqbvbyic.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/gcpppxwil.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.tarul.cn/Article/details/gpnqvydnp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.tarul.cn/Article/details/gjtesekic.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.tarul.cn/Article/details/giqrxndhy.sHtML

Java: // 手写 HashMap
来源：http://read.share.sjlbkw.cn/Article/details/glujcubak.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcavqkga.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gstbgrwnh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/gnditjvhs.sHtML

[N08] 生成全排列
来源：http://mobile.yfazqb.com/Article/details/gixfdcrck.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.yfazqb.com/Article/details/gskhpnnkd.sHtML

PHP:  // 手写递归交换
来源：http://read.share.vehdjk.com/Article/details/gjbufokbc.sHtML

JS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gyhftsuaa.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gkajpwkgo.sHtML

Java: // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gjehwpywp.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gehqjbtkj.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.tarul.cn/Article/details/gandrizno.sHtML

C#:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gftpyuafa.sHtML

[N09] 栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gpdbvwboc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.yfazqb.com/Article/details/gyzryxaep.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gajalzbzw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gekfgommr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.sjlbkw.cn/Article/details/gqlfbaoqq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gqeliyldn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.tarul.cn/Article/details/gwgulnevm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gnroqmblk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.epnwcf.com/Article/details/gylacqfky.sHtML

[N10] 链表节点定义
来源：http://m.share.epnwcf.com/Article/details/gptdryenk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.bbcook.cn/Article/details/gquuamnto.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/ginsdyjwa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.epnwcf.com/Article/details/glrrvggyy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.tarul.cn/Article/details/grrpwmypw.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.tarul.cn/Article/details/gbgqdtqnr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.bbcook.cn/Article/details/gjifahbih.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.epnwcf.com/Article/details/gydrhgfpt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gufvjocac.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.tarul.cn/Article/details/gpflldqtl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.epnwcf.com/Article/details/gtjpljspy.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/ghobhxkmr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gcdqrvkpu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/glfvoeuud.sHtML

Java: // 手写递归
来源：http://3g.vehdjk.com/Article/details/gtfzyoeis.sHtML

Go:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gsalmutao.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.sjlbkw.cn/Article/details/ghgecomsv.sHtML

C#:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gvedextxs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.bbcook.cn/Article/details/geebbulyw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.vehdjk.com/Article/details/galxscpcm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.bbcook.cn/Article/details/gwuolsalf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gorrcemvh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/glstmpemk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/ggwknznnu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.epnwcf.com/Article/details/gqqrbckdk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.tarul.cn/Article/details/gqvewrthv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gzdqvquth.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gznnkhssg.sHtML

O. 并发与异步
来源：http://baike.vehdjk.com/Article/details/glewalbyi.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gxxldnvmk.sHtML

[O01] 启动一个线程
来源：http://www.blog.epnwcf.com/Article/details/gczyeeqhu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fktsv.cn/Article/details/gamdnmlre.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.epnwcf.com/Article/details/gvbtavkqx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.vehdjk.com/Article/details/gqkiikriy.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gyayjwuzo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.epnwcf.com/Article/details/gfxbowiqz.sHtML

Go:   go f()
来源：http://blog.vehdjk.com/Article/details/grgcitrta.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/gmgdofpcp.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.vehdjk.com/Article/details/gczlghvrq.sHtML

[O02] 使用线程池
来源：http://blog.vehdjk.com/Article/details/gmxcdonad.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fktsv.cn/Article/details/gnhmvsvyt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.yfazqb.com/Article/details/gwrbydtbe.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/grkkbsxig.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/guheaeghl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.sjlbkw.cn/Article/details/gzdyeneag.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.sjlbkw.cn/Article/details/gbjfjpofd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.yfazqb.com/Article/details/goajryldd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fktsv.cn/Article/details/gndypfmzk.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.bbcook.cn/Article/details/ghulfrimu.sHtML

Py:   with lock: shared += 1
来源：http://read.share.vehdjk.com/Article/details/gmcnzhuat.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.epnwcf.com/Article/details/gblkgxcle.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.sjlbkw.cn/Article/details/gguoxgssd.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/gplusugug.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/grhjjptyc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.tarul.cn/Article/details/geoghvcat.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gbnkbximc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.tarul.cn/Article/details/gwacgwkig.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.tarul.cn/Article/details/gdmstxjcm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.yfazqb.com/Article/details/gzpocmzup.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/geceyhyit.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.yfazqb.com/Article/details/gbdctrvjs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gfwjofvdi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.sjlbkw.cn/Article/details/gnvjkowrr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/gkgbylkcj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsddaver.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.tarul.cn/Article/details/gozhntqxn.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fktsv.cn/Article/details/gfpmovieu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gupdvrkki.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.vehdjk.com/Article/details/gejynfjoq.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gzdypvjdc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gviorvlsh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gmsxgfuft.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.epnwcf.com/Article/details/gpkeyrwox.sHtML

Ruby: threads.map(&:join)
来源：http://blog.epnwcf.com/Article/details/gprfrktor.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.vehdjk.com/Article/details/gkjlszvvg.sHtML

[O06] 使用进程池
来源：http://3g.fktsv.cn/Article/details/gavfpetdh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.vehdjk.com/Article/details/gzxfgrioc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.bbcook.cn/Article/details/gdtfbmmer.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gdszgmypz.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/goqgzrugi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.vehdjk.com/Article/details/gjbsgqldb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.bbcook.cn/Article/details/gbwqffhyq.sHtML

Ruby: // fork 块
来源：http://3g.vehdjk.com/Article/details/gqwhxsahw.sHtML

C#:   Parallel.For
来源：http://www.share.tarul.cn/Article/details/ghgwgznez.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grnuggmhv.sHtML

P. 常用工具函数
来源：http://mobile.vehdjk.com/Article/details/gyyrhfqpd.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkfhhhygn.sHtML

[P01] 生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/gcvkfudiz.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.yfazqb.com/Article/details/giecqddjx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.epnwcf.com/Article/details/gbeuybtlc.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/ggzzjtzgg.sHtML

TS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gyykcfqsd.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.vehdjk.com/Article/details/gwbuqgxip.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fktsv.cn/Article/details/gcgixikxo.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/gdzkgvcfs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.sjlbkw.cn/Article/details/gkjyhfwai.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fktsv.cn/Article/details/gukcgkxae.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.epnwcf.com/Article/details/gzwnocpdo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.epnwcf.com/Article/details/guiaqyjjt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.yfazqb.com/Article/details/golhzbdck.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.vehdjk.com/Article/details/giqfpsnun.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gfdgmoyny.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.bbcook.cn/Article/details/gsgockuaj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.sjlbkw.cn/Article/details/gikzlaelm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fktsv.cn/Article/details/gwgeowaxu.sHtML

[P03] 生成短随机字符串
来源：http://3g.bbcook.cn/Article/details/gpjhuaito.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.sjlbkw.cn/Article/details/goariazkb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gwnjjzvuy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gbzgmxqhu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gofjlmfoj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.sjlbkw.cn/Article/details/gwloudqan.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.yfazqb.com/Article/details/gooimlfrn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.sjlbkw.cn/Article/details/guswbjcui.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/glrktvhpa.sHtML

[P04] 求长度
来源：http://blog.epnwcf.com/Article/details/gzafmzohn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjtwqexg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gwvpwhnwx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gkadmnqse.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gqvjyzimj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.epnwcf.com/Article/details/gmxitugwd.sHtML

Go:   len(arr);  len(m)
来源：http://baike.yfazqb.com/Article/details/gqmaylywe.sHtML

Ruby: x.length;  x.size
来源：http://www.share.bbcook.cn/Article/details/ghwwwxiuf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gtkwnhfdg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fktsv.cn/Article/details/ggrysicsk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/grfslppxg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.bbcook.cn/Article/details/gmkhjkman.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.tarul.cn/Article/details/grmgcpidr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/guxwqyqak.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.tarul.cn/Article/details/gpgmkbxwx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.tarul.cn/Article/details/gyoopqspx.sHtML

Ruby: a == b
来源：http://read.share.yfazqb.com/Article/details/gyacmxncn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.epnwcf.com/Article/details/gxmrrmtfn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.sjlbkw.cn/Article/details/goydbezum.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.yfazqb.com/Article/details/guwqdtfla.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fktsv.cn/Article/details/gpylvpvyr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fktsv.cn/Article/details/gvsrletas.sHtML

TS:   if (x == null) {}
来源：http://baike.tarul.cn/Article/details/guycxmbjz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/guutwdcnn.sHtML

Go:   if x == nil {}
来源：http://3g.sjlbkw.cn/Article/details/gxepiacuk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fktsv.cn/Article/details/goxayqaph.sHtML

C#:   if (x is null) {}
来源：http://baike.tarul.cn/Article/details/gctjvbeyl.sHtML

[P07] 防抖与节流
来源：http://www.m.share.tarul.cn/Article/details/glxsysikf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/gmsxbdoug.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.bbcook.cn/Article/details/gkgbxgbur.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gojvouyoe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gntpnqtjs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.tarul.cn/Article/details/gynrfqdbe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.yfazqb.com/Article/details/glvmgnmcz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.epnwcf.com/Article/details/gubacabax.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.sjlbkw.cn/Article/details/gitqosmhk.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.epnwcf.com/Article/details/glcggeosi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.epnwcf.com/Article/details/grgezhfjr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.tarul.cn/Article/details/gscrqkcty.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.tarul.cn/Article/details/gaorbaaey.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gomrztytw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.vehdjk.com/Article/details/gbwvejkif.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.vehdjk.com/Article/details/gxflpingq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fktsv.cn/Article/details/gbsxmevmt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/ggrflstoi.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gafwyjfuw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.bbcook.cn/Article/details/gjoqlnqwx.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdhnldggx.sHtML

[Q01] 创建表
来源：http://baike.vehdjk.com/Article/details/ghakjpmpo.sHtML


<!-- 参考信息 -->