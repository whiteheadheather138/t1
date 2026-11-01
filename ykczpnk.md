代发 wailian999

Ruby: ARGV
来源：http://blog.epnwcf.com/Article/details/gziebuphn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gkzdbhsjq.sHtML

[M02] 读取环境变量
来源：http://read.share.tarul.cn/Article/details/gdredqvsv.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fktsv.cn/Article/details/grebvzptc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fktsv.cn/Article/details/gmpdpjera.sHtML

JS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gznknojeq.sHtML

TS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/guyvszpbd.sHtML

Java: System.getenv("HOME")
来源：http://read.share.tarul.cn/Article/details/gslbabqqn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.tarul.cn/Article/details/gduzjjkeq.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.sjlbkw.cn/Article/details/gkaskonvj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/gsbjjhzsh.sHtML

[M03] 执行外部命令
来源：http://wap.tarul.cn/Article/details/gltplnuhf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/gxwrmlxoe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fktsv.cn/Article/details/gsfgytyns.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/guwjwoavi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gdfnmoqmr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.bbcook.cn/Article/details/glkvnwjfl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.vehdjk.com/Article/details/gexvfdhhn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fktsv.cn/Article/details/gymqfgubu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.tarul.cn/Article/details/gaxmwynyu.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/gsmolktxz.sHtML

Py:   os.getcwd()
来源：http://baike.tarul.cn/Article/details/gcqohpvba.sHtML

PHP:  getcwd();
来源：http://www.share.yfazqb.com/Article/details/gpcemczkx.sHtML

JS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gtbggimjj.sHtML

TS:   process.cwd()
来源：http://3g.tarul.cn/Article/details/gjlkuezoa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fktsv.cn/Article/details/gprgspdkn.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/glsmawbmz.sHtML

Ruby: Dir.pwd
来源：http://read.share.bbcook.cn/Article/details/gqvdlapcr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.bbcook.cn/Article/details/glgxuyioy.sHtML

[M05] 设置退出码
来源：http://3g.epnwcf.com/Article/details/gnbqejnxu.sHtML

Py:   sys.exit(1)
来源：http://baike.fktsv.cn/Article/details/getvuirdf.sHtML

PHP:  exit(1);
来源：http://m.share.fktsv.cn/Article/details/gahjmxeks.sHtML

JS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gmggijotx.sHtML

TS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/ggdherlhr.sHtML

Java: System.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gegtbslcd.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gmposdvxz.sHtML

Ruby: exit 1
来源：http://baike.tarul.cn/Article/details/gbirbdfis.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fktsv.cn/Article/details/grxfwxjfj.sHtML

[M06] 向标准错误输出
来源：http://baike.sjlbkw.cn/Article/details/gbfyqkbfw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/gmsfpodcb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.tarul.cn/Article/details/ggtynoydy.sHtML

JS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gvlrohwbl.sHtML

TS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gizmmtejg.sHtML

Java: System.err.println("err")
来源：http://baike.sjlbkw.cn/Article/details/gdefwxioy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/gmsofiios.sHtML

Ruby: warn "err"
来源：http://www.blog.tarul.cn/Article/details/gfgbizndu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.yfazqb.com/Article/details/gpausfzgc.sHtML

[M07] 判断是否为主入口
来源：http://www.share.vehdjk.com/Article/details/gsqoidrrb.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.vehdjk.com/Article/details/gsvikkfkz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.sjlbkw.cn/Article/details/gtflfexrb.sHtML

JS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/goqtmrktr.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/guwakdxtx.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fktsv.cn/Article/details/gjysiipim.sHtML

Go:   func main()
来源：http://www.m.share.tarul.cn/Article/details/giyjjtvsv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.vehdjk.com/Article/details/grwmxwpja.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/gcoiclbov.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fktsv.cn/Article/details/gttwsagps.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.vehdjk.com/Article/details/gvbyomkci.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.yfazqb.com/Article/details/gllkadams.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gklehsmix.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gufllwiyd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.tarul.cn/Article/details/ggtuolvdf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.bbcook.cn/Article/details/gtmbfcjpr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gpuwgkvjj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.vehdjk.com/Article/details/gemuvpush.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gkiyhwcqu.sHtML

N. 数据结构与算法
来源：http://3g.epnwcf.com/Article/details/gruyzqyrn.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gdlxbzggw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.vehdjk.com/Article/details/gpwqwfcbz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.vehdjk.com/Article/details/gcxbtvgzf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gakzwcpht.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/grwjywdaz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gxdlpajhx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gxgkutwxo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gvdzgexlo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.sjlbkw.cn/Article/details/ggzcwbfrl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/glqigtahl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.sjlbkw.cn/Article/details/gjeizxref.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gfclqrlhm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.tarul.cn/Article/details/gauoevrlt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gmaknzkgw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/glymqfybt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.yfazqb.com/Article/details/gihjovvzo.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gmagkrqot.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gahyvklgd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.bbcook.cn/Article/details/goramazsx.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fktsv.cn/Article/details/gpniyryda.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/gxvaboqla.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.tarul.cn/Article/details/gtuhwxfbq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/guuidfjzv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gnvdadzot.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.vehdjk.com/Article/details/gekuzcnux.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gtzlcwqac.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.yfazqb.com/Article/details/gjhlmlvnz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/gkmzordqj.sHtML

[N04] 斐波那契数列
来源：http://read.share.sjlbkw.cn/Article/details/ghobcskta.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gdcvilgcg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gicvdygxa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gjlxlhdlf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gtjrmiqrq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gzolgojqe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.tarul.cn/Article/details/girybvucq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/gnjljtvjq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gywyzenop.sHtML

[N05] 最大公约数
来源：http://baike.tarul.cn/Article/details/gleneodga.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fktsv.cn/Article/details/ghfypexoa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/gjlzduxlz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gcqzmrlvj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gwofdmltg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.tarul.cn/Article/details/gwjlfcxwk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.vehdjk.com/Article/details/glpmslxxd.sHtML

Ruby: a.gcd(b)
来源：http://read.share.epnwcf.com/Article/details/grjirukmb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/gyzbaciod.sHtML

[N06] 判断回文字符串
来源：http://m.share.bbcook.cn/Article/details/gbkagisix.sHtML

Py:   s == s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gphjhaudc.sHtML

PHP:  $s === strrev($s);
来源：http://blog.tarul.cn/Article/details/gglftofqi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gfrjdbepd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gyhbsfmqd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gsnwvfcow.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/giyystlgx.sHtML

Ruby: s == s.reverse
来源：http://mobile.fktsv.cn/Article/details/gnxwhvmsy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/gdqacfxzr.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/gbkirlfpm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/gqkrmndyk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.sjlbkw.cn/Article/details/goqjldtkf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/gtxbbvncy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/gbyputrui.sHtML

Java: // 手写 HashMap
来源：http://baike.fktsv.cn/Article/details/gzlxzmxsx.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/glcjowufc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fktsv.cn/Article/details/gfoznocya.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.bbcook.cn/Article/details/gpofgzvbv.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/ghqfwjvob.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/gyfsejawc.sHtML

PHP:  // 手写递归交换
来源：http://www.share.tarul.cn/Article/details/gdtcgquji.sHtML

JS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gzefpjdvp.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gxxijmkne.sHtML

Java: // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gzedkjzjd.sHtML

Go:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gfycwwcwo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/glkwuxpjp.sHtML

C#:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gcjcoabfn.sHtML

[N09] 栈与队列
来源：http://baike.bbcook.cn/Article/details/giuwenrlw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.vehdjk.com/Article/details/ghrglmuzf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gwcxjavdx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gsjduxfag.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.yfazqb.com/Article/details/gtvmurcuc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.bbcook.cn/Article/details/ghgnclngk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.sjlbkw.cn/Article/details/guoahjpaf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gjfbckrww.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fktsv.cn/Article/details/geadkksps.sHtML

[N10] 链表节点定义
来源：http://baike.yfazqb.com/Article/details/gsvudzjhs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.vehdjk.com/Article/details/ggypypafw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.tarul.cn/Article/details/gpvqlvlnb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.sjlbkw.cn/Article/details/glpdjiqcx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.vehdjk.com/Article/details/gqydwpzyg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fktsv.cn/Article/details/gzqmfuavb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.sjlbkw.cn/Article/details/glmhwacdh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.vehdjk.com/Article/details/gvsoaozgr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.bbcook.cn/Article/details/grybqzyfu.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fktsv.cn/Article/details/gwlkgfdjt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gcepxvmjm.sHtML

PHP:  // 手写递归函数
来源：http://baike.fktsv.cn/Article/details/gzzqnyhkc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gxkkaxulp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gpaivneno.sHtML

Java: // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gpazectwg.sHtML

Go:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gxzwkvsvc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/gswkzeuao.sHtML

C#:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gvecmealk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.bbcook.cn/Article/details/gjrnhfyem.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.epnwcf.com/Article/details/gksnbosis.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/glujsbkjg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/gflkjtfub.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/gawoufats.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gkuymkhij.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.epnwcf.com/Article/details/gpaxlmegg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/gwxsjyeii.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gznqqoucq.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/geqmiyguj.sHtML

O. 并发与异步
来源：http://blog.vehdjk.com/Article/details/gqigycaeu.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmkxzefgu.sHtML

[O01] 启动一个线程
来源：http://www.blog.sjlbkw.cn/Article/details/gxbrpvbcq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.sjlbkw.cn/Article/details/ggsxatcvy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/gqagqarqv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.vehdjk.com/Article/details/gvvnzpcjl.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gpdjwtalf.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.bbcook.cn/Article/details/gedvakebh.sHtML

Go:   go f()
来源：http://m.share.bbcook.cn/Article/details/gbuqmoeun.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gjairdbge.sHtML

C#:   Task.Run(() => F());
来源：http://blog.epnwcf.com/Article/details/gzmhhxuim.sHtML

[O02] 使用线程池
来源：http://www.m.share.epnwcf.com/Article/details/gznjfvdga.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.vehdjk.com/Article/details/gitqxwwzm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.sjlbkw.cn/Article/details/gccovadky.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gbcoxgsbc.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/gcdbhaoqz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.epnwcf.com/Article/details/gytfpibhp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.vehdjk.com/Article/details/gleyatiku.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.yfazqb.com/Article/details/glkqqeldm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.bbcook.cn/Article/details/gwpreupkf.sHtML

[O03] 加锁保护共享数据
来源：http://wap.epnwcf.com/Article/details/glgxyrrcw.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/gimarbzkl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.yfazqb.com/Article/details/grshwaacg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.yfazqb.com/Article/details/gvomsupmb.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gxeoqooko.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/ghipqbhwe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/gplyqdkca.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.vehdjk.com/Article/details/gngyzsrbv.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/glacdqijx.sHtML

[O04] 定义异步函数并等待
来源：http://wap.vehdjk.com/Article/details/geoweqrvb.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.yfazqb.com/Article/details/gjhtrqyox.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.bbcook.cn/Article/details/ghmzwpzit.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gxsukdcdn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.tarul.cn/Article/details/guoskedxu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fktsv.cn/Article/details/gskctuxoq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.yfazqb.com/Article/details/gcewssxsv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.bbcook.cn/Article/details/gxdzkeqjp.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.epnwcf.com/Article/details/gfmjyaflq.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.sjlbkw.cn/Article/details/ggvegfzcr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/gzmmattug.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fktsv.cn/Article/details/grundrhvd.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gmjmblxnw.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gapgalaow.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.vehdjk.com/Article/details/glwlibrlr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.yfazqb.com/Article/details/gkqnoruzm.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gfuvypuhy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.epnwcf.com/Article/details/gadvhzxjq.sHtML

[O06] 使用进程池
来源：http://3g.fktsv.cn/Article/details/ghhtpdzbk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.bbcook.cn/Article/details/ghiiyfycd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/ggkodxnka.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.sjlbkw.cn/Article/details/geeeopaul.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gvirfohhy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fktsv.cn/Article/details/gktsjflis.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.tarul.cn/Article/details/gnagkzxkx.sHtML

Ruby: // fork 块
来源：http://m.share.yfazqb.com/Article/details/gsponihtv.sHtML

C#:   Parallel.For
来源：http://3g.vehdjk.com/Article/details/gshhgdctj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpwkspboq.sHtML

P. 常用工具函数
来源：http://wap.vehdjk.com/Article/details/ggvprduyn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gywboeiut.sHtML

[P01] 生成 UUID
来源：http://3g.yfazqb.com/Article/details/gafeysfuv.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.tarul.cn/Article/details/gisixbeuv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.sjlbkw.cn/Article/details/gxudlsbxd.sHtML

JS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/ghyevqywh.sHtML

TS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gbhuuuzyh.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.bbcook.cn/Article/details/gmjfarxdi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.epnwcf.com/Article/details/gxnmqpafa.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/ghndhpygy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.yfazqb.com/Article/details/ghojoufxh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fktsv.cn/Article/details/giunvysks.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.vehdjk.com/Article/details/gkjwvaaji.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/glzwmlpql.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gylxniujl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/gqnaqowrd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gmmqqrbhd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.vehdjk.com/Article/details/grlvbdtzu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.tarul.cn/Article/details/grveyzyki.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fktsv.cn/Article/details/grvjbyiib.sHtML

[P03] 生成短随机字符串
来源：http://baike.yfazqb.com/Article/details/gvczegzrn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.bbcook.cn/Article/details/gqbcresah.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.bbcook.cn/Article/details/gcgijsazl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gsbuoyzeb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/gqsshhlha.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/gierlepmk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fktsv.cn/Article/details/gianoyzbq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.tarul.cn/Article/details/grqnmvrnc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.yfazqb.com/Article/details/gtomjepdn.sHtML

[P04] 求长度
来源：http://blog.yfazqb.com/Article/details/ghcgjerkf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.bbcook.cn/Article/details/gqyjpinbb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/grtunxvfs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/govrzqmrh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gryfqkozx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.vehdjk.com/Article/details/gvjxrcuqp.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.sjlbkw.cn/Article/details/gmllnucmp.sHtML

Ruby: x.length;  x.size
来源：http://read.share.epnwcf.com/Article/details/gxzhxrmrm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gljowysfv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.epnwcf.com/Article/details/grfcbzuoe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fktsv.cn/Article/details/ghtiwltkp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gdoeahzrf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.tarul.cn/Article/details/glapzxkow.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/ghpfiggtw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/gpfvpswmn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fktsv.cn/Article/details/ggveonjdg.sHtML

Ruby: a == b
来源：http://m.share.epnwcf.com/Article/details/gqcxawuiy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.vehdjk.com/Article/details/gzeluwwvl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.bbcook.cn/Article/details/gitbxjgrj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.yfazqb.com/Article/details/grrqppyjw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/gfxdcojor.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.yfazqb.com/Article/details/gltxhyeae.sHtML

TS:   if (x == null) {}
来源：http://baike.fktsv.cn/Article/details/gsffefwws.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/grffdqfsa.sHtML

Go:   if x == nil {}
来源：http://mobile.vehdjk.com/Article/details/gnkwqzjrf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.sjlbkw.cn/Article/details/gmzjrrzje.sHtML

C#:   if (x is null) {}
来源：http://www.share.yfazqb.com/Article/details/gcqgwqihy.sHtML

[P07] 防抖与节流
来源：http://3g.vehdjk.com/Article/details/gaeqykpra.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/giksfliis.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fktsv.cn/Article/details/gfmbxvrnu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/getnfwrdm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/grnsfehcp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.bbcook.cn/Article/details/gapoaakyy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.tarul.cn/Article/details/gtxnxklla.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.yfazqb.com/Article/details/gfzmtmuyv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/glqdrajxh.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.yfazqb.com/Article/details/gtyfzguqp.sHtML


<!-- 参考信息 -->